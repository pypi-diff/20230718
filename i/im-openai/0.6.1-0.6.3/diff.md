# Comparing `tmp/im_openai-0.6.1.tar.gz` & `tmp/im_openai-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "im_openai-0.6.1.tar", last modified: Thu Jul 13 00:40:08 2023, max compression
+gzip compressed data, was "im_openai-0.6.3.tar", last modified: Tue Jul 18 19:49:59 2023, max compression
```

## Comparing `im_openai-0.6.1.tar` & `im_openai-0.6.3.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.472920 im_openai-0.6.1/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.6.1/AUTHORS.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.6.1/CONTRIBUTING.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.6.1/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.6.1/MANIFEST.in
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3254 2023-07-13 00:40:08.473461 im_openai-0.6.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.6.1/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.422836 im_openai-0.6.1/docs/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/Makefile
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/authors.rst
--rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/conf.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/contributing.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/history.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/index.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/installation.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/make.bat
--rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.6.1/docs/readme.rst
--rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.6.1/docs/usage.rst
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.438664 im_openai-0.6.1/im_openai/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-13 00:39:40.000000 im_openai-0.6.1/im_openai/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4792 2023-07-10 22:37:03.000000 im_openai-0.6.1/im_openai/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14978 2023-07-13 00:23:57.000000 im_openai-0.6.1/im_openai/langchain_util.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3353 2023-07-07 00:30:57.000000 im_openai-0.6.1/im_openai/patch.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.6.1/im_openai/template.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.462974 im_openai-0.6.1/im_openai.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3254 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/not-zip-safe
--rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-13 00:40:08.000000 im_openai-0.6.1/im_openai.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      426 2023-07-13 00:40:08.475266 im_openai-0.6.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-13 00:39:40.000000 im_openai-0.6.1/setup.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-13 00:40:08.470694 im_openai-0.6.1/tests/
--rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.6.1/tests/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      559 2023-06-20 23:30:14.000000 im_openai-0.6.1/tests/test_im_openai.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-18 19:49:59.280239 im_openai-0.6.3/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      150 2023-06-20 23:30:14.000000 im_openai-0.6.3/AUTHORS.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3560 2023-06-22 20:28:17.000000 im_openai-0.6.3/CONTRIBUTING.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1069 2023-06-20 23:30:14.000000 im_openai-0.6.3/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      261 2023-06-22 20:24:41.000000 im_openai-0.6.3/MANIFEST.in
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3501 2023-07-18 19:49:59.280952 im_openai-0.6.3/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1553 2023-06-24 00:40:31.000000 im_openai-0.6.3/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-18 19:49:59.218253 im_openai-0.6.3/docs/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/Makefile
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/authors.rst
+-rwxr-xr-x   0 vscode    (1000) vscode    (1000)     4874 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/conf.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       33 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/contributing.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       28 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/history.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      325 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/index.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1175 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/installation.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      807 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/make.bat
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       26 2023-06-22 20:24:52.000000 im_openai-0.6.3/docs/readme.rst
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       92 2023-06-20 23:30:14.000000 im_openai-0.6.3/docs/usage.rst
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-18 19:49:59.247431 im_openai-0.6.3/im_openai/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      255 2023-07-18 19:04:29.000000 im_openai-0.6.3/im_openai/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     5310 2023-07-17 23:13:21.000000 im_openai-0.6.3/im_openai/client.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)    20197 2023-07-18 00:50:43.000000 im_openai-0.6.3/im_openai/langchain_util.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3353 2023-07-07 00:30:57.000000 im_openai-0.6.3/im_openai/patch.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      423 2023-06-23 21:56:38.000000 im_openai-0.6.3/im_openai/template.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     8724 2023-07-18 00:39:04.000000 im_openai-0.6.3/im_openai/test_langchain_util.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-18 19:49:59.269464 im_openai-0.6.3/im_openai.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3501 2023-07-18 19:49:59.000000 im_openai-0.6.3/im_openai.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      592 2023-07-18 19:49:59.000000 im_openai-0.6.3/im_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-18 19:49:59.000000 im_openai-0.6.3/im_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-07-18 19:49:59.000000 im_openai-0.6.3/im_openai.egg-info/not-zip-safe
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       10 2023-07-18 19:49:59.000000 im_openai-0.6.3/im_openai.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      396 2023-07-18 19:49:59.283902 im_openai-0.6.3/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1350 2023-07-18 19:04:29.000000 im_openai-0.6.3/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-07-18 19:49:59.277631 im_openai-0.6.3/tests/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       39 2023-06-20 23:30:14.000000 im_openai-0.6.3/tests/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      544 2023-07-14 22:02:59.000000 im_openai-0.6.3/tests/test_im_openai.py
```

### Comparing `im_openai-0.6.1/CONTRIBUTING.rst` & `im_openai-0.6.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.6.1/LICENSE` & `im_openai-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `im_openai-0.6.1/PKG-INFO` & `im_openai-0.6.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im_openai
-Version: 0.6.1
+Version: 0.6.3
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -130,8 +130,18 @@
 
 - Handle duplicate callbacks, agents, etc
 
 ## 0.6.1 (2023-07-12)
 
 - Fix prompt retrieval in deep chains
 
+## 0.6.2 (2023-07-13)
+
+- Handle cases where input values are not strings
+
+## 0.6.3 (2023-07-18)
+
+- Better support for server-generated event ids 
+  (pre-llm sends event, post-llm re-uses the same id)
+- more tests for different kinds of templates
+
```

### Comparing `im_openai-0.6.1/README.md` & `im_openai-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `im_openai-0.6.1/docs/Makefile` & `im_openai-0.6.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `im_openai-0.6.1/docs/conf.py` & `im_openai-0.6.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.6.1/docs/installation.rst` & `im_openai-0.6.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `im_openai-0.6.1/docs/make.bat` & `im_openai-0.6.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `im_openai-0.6.1/im_openai/client.py` & `im_openai-0.6.3/im_openai/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,24 +8,27 @@
 
 import aiohttp
 
 
 async def send_event(
     session: aiohttp.ClientSession,
     project_key: str,
+    *,
     api_name: str | None,
     prompt_event_id: str | None,
     prompt_template_text: str | None,
     prompt_template_chat: List | None,
     prompt_params: Dict | None,
     chat_id: str | None,
     response: str | None = None,
     response_time: float | None = None,
     prompt: Any | None = None,
-):
+    parent_event_id: str | None = None,
+) -> str | None:
+    """Send an event to Imaginary Dev. Returns the id of the event that was added on the server."""
     PROMPT_REPORTING_URL = os.environ.get(
         "PROMPT_REPORTING_URL", "https://app.imaginary.dev/api/event"
     )
     event = {
         "projectKey": project_key,
         "apiName": api_name,
         "params": {},
@@ -63,27 +66,34 @@
         event["params"] = prompt_params
     if response is not None:
         event["response"] = response
     if response_time is not None:
         event["responseTime"] = response_time
     if chat_id is not None:
         event["chatId"] = chat_id
+    if parent_event_id is not None:
+        event["parentEventId"] = str(parent_event_id)
 
-    await session.post(PROMPT_REPORTING_URL, json=event)
+    result = await session.post(PROMPT_REPORTING_URL, json=event)
+    json = await result.json()
+    print("Got response", json)
+    if isinstance(json, dict):
+        return json.get("id")
 
 
 @asynccontextmanager
 async def event_session(
     project_key: str,
     api_name: str | None,
     prompt_template_text: str | None,
     prompt_template_chat: List | None,
     chat_id: str | None = None,
     prompt_template_params: dict | None = None,
     prompt_event_id: str | None = None,
+    parent_event_id: str | None = None,
 ):
     """Context manager for sending an event to Imaginary Dev.
 
     Usage::
 
         with event_session(project_key, api_name, prompt_text, prompt_event_id) as complete_event:
             # do something
@@ -101,14 +111,15 @@
             project_key=project_key,
             api_name=api_name,
             prompt_event_id=prompt_event_id,
             prompt_template_text=prompt_template_text,
             prompt_template_chat=prompt_template_chat,
             prompt_params=prompt_template_params,
             chat_id=chat_id,
+            parent_event_id=parent_event_id,
         )
         pending_events_sent.append(first_event_sent)
 
         async def complete_event(response):
             response_time = (time.time() - start) * 1000
             second_event_sent = send_event(
                 session=session,
@@ -117,14 +128,15 @@
                 prompt_event_id=prompt_event_id,
                 prompt_template_text=prompt_template_text,
                 prompt_template_chat=prompt_template_chat,
                 prompt_params=prompt_template_params,
                 chat_id=chat_id,
                 response=response,
                 response_time=response_time,
+                parent_event_id=parent_event_id,
             )
             pending_events_sent.append(second_event_sent)
 
         yield complete_event
         w = time.time()
         pending_events_results = await asyncio.gather(
             *pending_events_sent, return_exceptions=True
```

### Comparing `im_openai-0.6.1/im_openai/langchain_util.py` & `im_openai-0.6.3/im_openai/langchain_util.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import asyncio
 import json
 import logging
 import os
 import time
 import uuid
 from itertools import zip_longest
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, TypeVar, Union
 from uuid import UUID
 
 import aiohttp
 from langchain.callbacks.base import BaseCallbackHandler
-from langchain.load.load import load
+from langchain.load.load import loads
 from langchain.prompts import (
     BaseChatPromptTemplate,
-    StringPromptTemplate,
     BasePromptTemplate,
+    StringPromptTemplate,
 )
 from langchain.prompts.chat import (
     BaseChatPromptTemplate,
     BaseMessagePromptTemplate,
     MessagesPlaceholder,
 )
 from langchain.schema import (
@@ -30,31 +30,33 @@
     BaseMessage,
     ChatMessage,
     HumanMessage,
     LLMResult,
     SystemMessage,
 )
 
-from .client import send_event
+from im_openai import client
 
 logger = logging.getLogger(__name__)
 
 from functools import wraps
 
 
 def format_langchain_value(value: Any) -> Any:
     if isinstance(value, (str, bool, int, float)):
         return value
-    if isinstance(value, list):
+    if isinstance(value, (list, tuple)):
         return [format_langchain_value(v) for v in value]
     if isinstance(value, dict):
         return {k: format_langchain_value(v) for k, v in value.items()}
     if isinstance(value, StringPromptTemplate):
         inputs = {k: f"{{{k}}}" for k in value.input_variables}
         return value.format(**inputs)
+    if isinstance(value, BaseMessage):
+        return format_chat_template([value])[0]
     return format_chat_template(value)
 
 
 def format_chat_template(
     messages: List[
         Union[BaseMessagePromptTemplate, BaseChatPromptTemplate, BaseMessage, List[Any]]
     ]
@@ -98,29 +100,46 @@
     elif isinstance(message, dict):
         return [message]
     else:
         raise ValueError(f"Got unknown type {type(message)}: {message}")
 
 
 class PromptWatchCallbacks(BaseCallbackHandler):
-    runs: Dict[UUID, Dict[str, Any]] = {}
     project_key: str
     api_name: str
+
     template_chat: List[Dict] | None
+    template_text: str | None
+
+    runs: Dict[UUID, Dict[str, Any]] = {}
+    """A dictionary of information about a run, keyed by run_id"""
     parent_run_ids: Dict[UUID, UUID] = {}
+    """In case self.runs is missing a run, we can walk up the parent chain to find it"""
+
+    server_event_ids: Dict[UUID, str | None] = {}
+    """Mapping of run_id to server event id"""
 
     def __init__(
         self,
         project_key: str,
         api_name: str,
         *,
-        template_text: str | None = None,
-        template_chat: List[Union[BaseMessagePromptTemplate, BaseMessage]]
-        | None = None,
+        template_text: Optional[str] = None,
+        template_chat: Optional[
+            List[Union[BaseMessagePromptTemplate, BaseMessage]]
+        ] = None,
     ):
+        """Initialize the callback handler
+
+        Args:
+            project_key (str): The Imaginary Programming project key
+            api_name (str): The Imaginary Programming API name
+            template_text (Optional[str], optional): The template to use for completion events. Defaults to None.
+            template_chat (Optional[List[Union[BaseMessagePromptTemplate, BaseMessage]]], optional): The template to use for chat events. Defaults to None.
+        """
         self.project_key = project_key or os.environ.get("PROMPT_PROJECT_KEY", "")
         if not self.project_key:
             raise ValueError("project_key must be provided")
         self.runs = {}
         self.api_name = api_name
         if template_text is not None:
             self.template_text = template_text
@@ -133,60 +152,61 @@
     def _get_run(self, run_id: UUID):
         if run_id in self.runs:
             return self.runs[run_id]
         if run_id in self.parent_run_ids:
             return self._get_run(self.parent_run_ids[run_id])
         return None
 
-    def _get_run_metadata(self, run_id: UUID, metadata_key: str):
+    def _get_run_info(self, run_id: UUID, metadata_key: str):
         """Walk up the parent chain looking for the nearest run with the metadata_key defined"""
         if run_id in self.runs and metadata_key in self.runs[run_id]:
             return self.runs[run_id][metadata_key]
         if run_id in self.parent_run_ids:
-            return self._get_run_metadata(self.parent_run_ids[run_id], metadata_key)
+            return self._get_run_info(self.parent_run_ids[run_id], metadata_key)
         return None
 
+    def _get_server_event_id(self, run_id: UUID):
+        """Lazily insert a server event id if it doesn't exist. This will get filled in later when the initial event is sent"""
+        if run_id not in self.server_event_ids:
+            self.server_event_ids[run_id] = None
+        return self.server_event_ids[run_id]
+
     def on_chain_start(
         self,
-        serialized,
-        inputs,
-        *a,
-        run_id,
-        parent_run_id,
-        tags,
-        metadata=None,
-        **kwargs,
+        serialized: Dict[str, Any],
+        inputs: Dict[str, Any],
+        *,
+        run_id: UUID,
+        parent_run_id: Optional[UUID] = None,
+        tags: Optional[List[str]] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+        **kwargs: Any,
     ):
         if parent_run_id:
             self.parent_run_ids[run_id] = parent_run_id
         logger.info(
-            "on_chain_start      %s [%s]",
+            "on_chain_start      %s [%s] %s",
             self._format_run_id(run_id),
             ", ".join(inputs.keys()),
+            ".".join(serialized["id"]),
         )
-        # super hack to extract the prompt if it exists
-        prompt_template_chat = None
-        prompt_template_text = None
-        prompt_obj = serialized.get("kwargs", {}).get("prompt")
-        if prompt_obj:
-            prompt_template = load(prompt_obj)
-            variable_inputs = {k: f"{{{k}}}" for k in prompt_template.input_variables}
-            if isinstance(prompt_template, BasePromptTemplate):
-                prompt_template_value = prompt_template.format_prompt(**variable_inputs)
-                prompt_template_text = prompt_template_value.to_string()
-                prompt_template_chat = prompt_template_value.to_messages()
 
         self.runs[run_id] = {
             "inputs": inputs,
             "parent_run_id": parent_run_id,
-            "prompt_template_text": prompt_template_text,
-            "prompt_template_chat": prompt_template_chat,
             "prompt_event_id": uuid.uuid4(),
         }
 
+        # super hack to extract the prompt if it exists
+        prompt_obj = serialized.get("kwargs", {}).get("prompt")
+        if prompt_obj:
+            prompt_template = loads(json.dumps(prompt_obj))
+            if isinstance(prompt_template, BasePromptTemplate):
+                self.runs[run_id]["prompt_template"] = prompt_template
+
     def on_agent_action(
         self,
         action: AgentAction,
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
@@ -223,124 +243,126 @@
         prompts: List[str],
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         tags: Optional[List[str]] = None,
         **kwargs: Any,
     ):
+        """Run when a text-based LLM runs"""
         if parent_run_id:
             self.parent_run_ids[run_id] = parent_run_id
         logger.info(
             "on_llm_start %s (%s prompts)",
             self._format_run_id(run_id),
             len(prompts),
         )
 
         run = self._get_run(run_id)
         if not run:
             logger.warning("on_llm_start Missing run %s", run_id)
             return
         run["prompts"] = prompts
         run["now"] = time.time()
-        template_text = (
-            self._get_run_metadata(run_id, "prompt_template_text") or self.template_text
-        )
+        template_text = self._resolve_completion_template(run_id)
         # TODO: need to generate a new event id for each prompt
         asyncio.run(
             self._async_send_completion(
                 run_id,
                 template_text,
                 run["inputs"],
                 prompts,
+                parent_event_id=parent_run_id,
             )
         )
 
     def on_chat_model_start(
         self,
         serialized,
         messages: List[List[BaseMessage]],
         run_id,
         parent_run_id,
         tags,
         metadata=None,
         **kwargs,
     ):
+        """Runs when a chat-based LLM runs"""
         if parent_run_id:
             self.parent_run_ids[run_id] = parent_run_id
         logger.info(
             "on_chat_model_start %s (%s prompts)",
             self._format_run_id(run_id),
             len(messages),
         )
         run = self._get_run(run_id)
         if not run:
             return
         run["messages"] = messages
         run["now"] = time.time()
-        template_chat = (
-            self._get_run_metadata(run_id, "prompt_template_chat") or self.template_chat
-        )
+
+        template_chat = self._resolve_chat_template(run_id)
         asyncio.run(
             self._async_send_chat(
                 run_id,
                 template_chat,
                 run["inputs"],
                 messages,
+                parent_event_id=parent_run_id,
             )
         )
 
     def on_llm_end(
         self,
         response: LLMResult,
         *,
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
         **kwargs: Any,
     ):
+        """Runs when either a text-based or chat-based LLM ends"""
         if parent_run_id:
             self.parent_run_ids[run_id] = parent_run_id
         logger.info(
             "on_llm_end          %s (%s responses)",
             self._format_run_id(run_id),
             len(response.generations),
         )
+
         run = self._get_run(run_id)
         if not run:
+            logger.warning("on_llm_end Missing run %s", run_id)
             return
         now = time.time()
         response_time = (now - run["now"]) * 1000
 
         if "messages" in run:
-            template_chat = (
-                self._get_run_metadata(run_id, "prompt_template_chat")
-                or self.template_chat
-            )
+            template_chat = self._resolve_chat_template(run_id)
             asyncio.run(
                 self._async_send_chat(
-                    run["prompt_event_id"],
+                    run_id,
                     template_chat,
                     run["inputs"],
                     run["messages"],
                     response,
                     response_time,
+                    parent_event_id=parent_run_id,
                 )
             )
         elif "prompts" in run:
             template_text = (
-                self._get_run_metadata(run_id, "prompt_template_text")
-                or self.template_text
+                self._get_run_info(run_id, "prompt_template_text") or self.template_text
             )
             asyncio.run(
                 self._async_send_completion(
-                    run["prompt_event_id"],
+                    run_id,
                     template_text,
                     run["inputs"],
                     run["prompts"],
                     response,
                     response_time,
+                    parent_event_id=parent_run_id,
                 )
             )
         else:
             logger.warning("Missing prompts or messages in run %s %s", run_id, run)
 
     def on_llm_error(
         self,
@@ -367,85 +389,196 @@
             "on_chain_end        %s [%s]",
             self._format_run_id(run_id),
             ", ".join(outputs.keys()),
         )
         if run_id in self.runs:
             del self.runs[run_id]
 
-    async def _async_send_completion(
+    async def _async_send(
         self,
-        prompt_event_id: UUID,
-        template_text: str,
+        run_id: UUID,
+        template: List[Dict] | str | None,
         inputs: Dict,
-        prompts: List[str],
+        iterations: List[str] | List[List[BaseMessage]],
         result: LLMResult | None = None,
         response_time: float | None = None,
+        parent_event_id: UUID | None = None,
+        is_chat: bool = False,
     ):
         async with aiohttp.ClientSession() as session:
             generations_lists = result.generations if result else []
-            for prompt, generations in zip_longest(prompts, generations_lists):
+            for iteration, generations in zip_longest(iterations, generations_lists):
                 response_text = (
                     "".join(g.text for g in generations) if generations else None
                 )
                 json_inputs = {
                     key: format_langchain_value(value) for key, value in inputs.items()
                 }
-                # If no template is passed in, pass in the completion prompt instead
-                prompt = {"completion": prompt} if not template_text else None
+
+                if is_chat:
+                    prompt = (
+                        {"chat": format_chat_template(iteration)}  # type: ignore
+                        if not template
+                        else None
+                    )
+                    prompt_template_text = None
+                    prompt_template_chat = template
+                else:
+                    prompt = {"completion": iteration} if not template else None
+                    prompt_template_text = template
+                    prompt_template_chat = None
+
                 # TODO: gather these up and send them all at once
-                await send_event(
+                prompt_event_id = self._get_server_event_id(run_id)
+                id = await client.send_event(
                     session,
                     project_key=self.project_key,
                     api_name=self.api_name,
-                    prompt_template_text=template_text,
-                    prompt_template_chat=None,
+                    prompt_template_text=prompt_template_text,  # type: ignore
+                    prompt_template_chat=prompt_template_chat,  # type: ignore
                     prompt_params=json_inputs,
-                    prompt_event_id=str(prompt_event_id),
+                    prompt_event_id=prompt_event_id,
                     chat_id=None,
                     response=response_text,
                     response_time=response_time,
+                    prompt=prompt,
+                    parent_event_id=str(parent_event_id) if parent_event_id else None,
                 )
+                if id:
+                    self.server_event_ids[run_id] = id
 
     async def _async_send_chat(
         self,
-        prompt_event_id: UUID,
+        run_id: UUID,
         template_chats: List[Dict] | None,
         inputs: Dict,
         messages_list: List[List[BaseMessage]],
         result: LLMResult | None = None,
         response_time: float | None = None,
+        parent_event_id: UUID | None = None,
     ):
-        async with aiohttp.ClientSession() as session:
-            generations_lists = result.generations if result else []
-            for messages, generations in zip_longest(messages_list, generations_lists):
-                response_text = (
-                    "".join(g.text for g in generations) if generations else None
-                )
-                json_inputs = {
-                    key: format_langchain_value(value) for key, value in inputs.items()
-                }
-                # If no template is passed in, pass in the prompt instead
-                prompt = (
-                    {"chat": format_chat_template(messages)}  # type: ignore
-                    if not template_chats
-                    else None
-                )
-                # TODO: gather these up and send them all at once
-                await send_event(
-                    session,
-                    project_key=self.project_key,
-                    api_name=self.api_name,
-                    prompt_template_text=None,
-                    prompt_template_chat=template_chats,
-                    prompt_params=json_inputs,
-                    prompt_event_id=str(prompt_event_id),
-                    chat_id=None,
-                    response=response_text,
-                    response_time=response_time,
-                    prompt=prompt,
-                )
+        await self._async_send(
+            run_id,
+            template_chats,
+            inputs,
+            messages_list,
+            result,
+            response_time,
+            parent_event_id,
+            is_chat=True,
+        )
+
+    async def _async_send_completion(
+        self,
+        prompt_event_id: UUID,
+        template_text: str | None,
+        inputs: Dict,
+        prompts: List[str],
+        result: LLMResult | None = None,
+        response_time: float | None = None,
+        parent_event_id: UUID | None = None,
+    ):
+        await self._async_send(
+            prompt_event_id,
+            template_text,
+            inputs,
+            prompts,
+            result,
+            response_time,
+            parent_event_id=parent_event_id,
+            is_chat=False,
+        )
 
     def _format_run_id(self, run_id: UUID) -> str:
         """Generates a hierarchy of run_ids by recursively walking self.parent_ids"""
         if run_id in self.parent_run_ids:
             return f"{self._format_run_id(self.parent_run_ids[run_id])} -> {run_id}"
         return str(run_id)
+
+    def _resolve_chat_template(self, run_id: UUID):
+        """Resolve the template_chat into a list of dicts"""
+        template: Optional[BasePromptTemplate] = self._get_run_info(
+            run_id, "prompt_template"
+        )
+        inputs: Optional[Dict[str, Any]] = self._get_run_info(run_id, "inputs")
+        template_chat = None
+        if template and inputs:
+            stub_inputs = make_stub_inputs(inputs)
+            # Some of the templat formatters get upset if you pass in extra keys
+            filtered_stub_inputs = {
+                k: v for k, v in stub_inputs.items() if k in template.input_variables
+            }
+            if isinstance(
+                template, (BaseMessagePromptTemplate, BaseChatPromptTemplate)
+            ):
+                # We can't go through format_prompt because it doesn't like formatting the wrong types
+                template_chat = template.format_messages(**filtered_stub_inputs)
+
+            elif isinstance(template, StringPromptTemplate):
+                template_chat = template.format_prompt(
+                    **filtered_stub_inputs
+                ).to_messages()
+            else:
+                raise ValueError(f"Unknown template type {type(template)}")
+            template_chat = format_chat_template(template_chat)  # type: ignore
+        return template_chat
+
+    def _resolve_completion_template(self, run_id: UUID):
+        """Resolve the template_chat into a list of dicts"""
+        template = self._get_run_info(run_id, "prompt_template")
+        inputs = self._get_run_info(run_id, "inputs")
+        template_text: str | None = None
+        if template and inputs:
+            stub_inputs = make_stub_inputs(inputs)
+            filtered_stub_inputs = {
+                k: v for k, v in stub_inputs.items() if k in template.input_variables
+            }
+            if isinstance(template, BaseChatPromptTemplate):
+                # We can't go through format_prompt because it doesn't like formatting the wrong types
+                template_text = template.format(**filtered_stub_inputs)
+            elif isinstance(template, StringPromptTemplate):
+                template_text = template.format_prompt(
+                    **filtered_stub_inputs
+                ).to_string()
+            else:
+                raise ValueError(f"Unknown template type {type(template)}")
+            # template_text = format_chat_template(template_text)  # type: ignore
+        return template_text
+
+
+def make_stub_inputs(inputs: Dict[str, Any]) -> Dict[str, Any]:
+    return make_stub_inputs_raw(inputs, "")  # type: ignore
+
+
+def make_stub_inputs_raw(inputs: Any, prefix: str):
+    if isinstance(inputs, dict):
+        dict_prefix = f"{prefix}." if prefix else ""
+        return {
+            k: make_stub_inputs_raw(v, prefix=f"{dict_prefix}{k}")
+            for k, v in inputs.items()
+        }
+    if isinstance(inputs, (str, int, float, bool)):
+        return f"{{{prefix}}}"
+    if isinstance(inputs, list):
+        # TODO: figure out a way to collapse lists. Right now this will create stuff like:
+        # [
+        #     {
+        #         "role": "{agent_history[0].role}",
+        #         "content": "{agent_history[0].content}",
+        #     },
+        #     {
+        #         "role": "{agent_history[1].role}",
+        #         "content": "{agent_history[1].content}",
+        #     },
+        # ]
+        # return [f"{{{prefix}}}"] * len(inputs)
+        return [
+            make_stub_inputs_raw(v, prefix=f"{prefix}[{i}]")
+            for i, v in enumerate(inputs)
+        ]
+    if isinstance(inputs, tuple):
+        return tuple(
+            make_stub_inputs_raw(v, prefix=f"{prefix}[{i}]")
+            for i, v in enumerate(inputs)
+        )
+    resolved = make_stub_inputs_raw(format_langchain_value(inputs), prefix=prefix)
+    return resolved
```

### Comparing `im_openai-0.6.1/im_openai/patch.py` & `im_openai-0.6.3/im_openai/patch.py`

 * *Files identical despite different names*

### Comparing `im_openai-0.6.1/im_openai.egg-info/PKG-INFO` & `im_openai-0.6.3/im_openai.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: im-openai
-Version: 0.6.1
+Version: 0.6.3
 Summary: Wrapper library for openai to send events to the Imaginary Programming monitor
 Home-page: https://github.com/alecf/im_openai
 Author: Alec Flett
 Author-email: alec@thegp.com
 License: MIT license
 Keywords: im_openai
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -130,8 +130,18 @@
 
 - Handle duplicate callbacks, agents, etc
 
 ## 0.6.1 (2023-07-12)
 
 - Fix prompt retrieval in deep chains
 
+## 0.6.2 (2023-07-13)
+
+- Handle cases where input values are not strings
+
+## 0.6.3 (2023-07-18)
+
+- Better support for server-generated event ids 
+  (pre-llm sends event, post-llm re-uses the same id)
+- more tests for different kinds of templates
+
```

### Comparing `im_openai-0.6.1/im_openai.egg-info/SOURCES.txt` & `im_openai-0.6.3/im_openai.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/readme.rst
 docs/usage.rst
 im_openai/__init__.py
 im_openai/client.py
 im_openai/langchain_util.py
 im_openai/patch.py
 im_openai/template.py
+im_openai/test_langchain_util.py
 im_openai.egg-info/PKG-INFO
 im_openai.egg-info/SOURCES.txt
 im_openai.egg-info/dependency_links.txt
 im_openai.egg-info/not-zip-safe
 im_openai.egg-info/top_level.txt
 tests/__init__.py
 tests/test_im_openai.py
```

### Comparing `im_openai-0.6.1/setup.py` & `im_openai-0.6.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="im_openai",
     name="im_openai",
     packages=find_packages(include=["im_openai", "im_openai.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/alecf/im_openai",
-    version="0.6.1",
+    version="0.6.3",
     zip_safe=False,
 )
```

### Comparing `im_openai-0.6.1/tests/test_im_openai.py` & `im_openai-0.6.3/tests/test_im_openai.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 
 """Tests for `im_openai` package."""
 
 import pytest
 
 
-from im_openai import im_openai
+import im_openai
 
 
 @pytest.fixture
 def response():
     """Sample pytest fixture.
 
     See more at: http://doc.pytest.org/en/latest/fixture.html
```

