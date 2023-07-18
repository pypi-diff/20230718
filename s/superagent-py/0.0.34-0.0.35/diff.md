# Comparing `tmp/superagent_py-0.0.34.tar.gz` & `tmp/superagent_py-0.0.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superagent_py-0.0.34.tar", max compression
+gzip compressed data, was "superagent_py-0.0.35.tar", max compression
```

## Comparing `superagent_py-0.0.34.tar` & `superagent_py-0.0.35.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0     1073 2023-07-17 11:38:46.217009 superagent_py-0.0.34/LICENSE
--rw-r--r--   0        0        0     3251 2023-07-17 11:38:46.217009 superagent_py-0.0.34/README.md
--rw-r--r--   0        0        0      380 2023-07-17 11:38:46.217009 superagent_py-0.0.34/pyproject.toml
--rw-r--r--   0        0        0      589 2023-07-17 11:38:46.217009 superagent_py-0.0.34/src/superagent/__init__.py
--rw-r--r--   0        0        0     2956 2023-07-17 11:38:46.217009 superagent_py-0.0.34/src/superagent/client.py
--rw-r--r--   0        0        0      348 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/__init__.py
--rw-r--r--   0        0        0      426 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/api_error.py
--rw-r--r--   0        0        0     1047 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/datetime_utils.py
--rw-r--r--   0        0        0     3710 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/jsonable_encoder.py
--rw-r--r--   0        0        0      385 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/core/remove_none_from_headers.py
--rw-r--r--   0        0        0      170 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/errors/__init__.py
--rw-r--r--   0        0        0      313 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0        0 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/py.typed
--rw-r--r--   0        0        0      343 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/__init__.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent/__init__.py
--rw-r--r--   0        0        0    14309 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent_documents/__init__.py
--rw-r--r--   0        0        0     9260 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent_documents/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent_tools/__init__.py
--rw-r--r--   0        0        0     9132 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/agent_tools/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/api_token/__init__.py
--rw-r--r--   0        0        0     8538 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/api_token/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/auth/__init__.py
--rw-r--r--   0        0        0     5901 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/auth/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/documents/__init__.py
--rw-r--r--   0        0        0    10039 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/documents/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/prompts/__init__.py
--rw-r--r--   0        0        0    10865 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/prompts/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/tools/__init__.py
--rw-r--r--   0        0        0     9383 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/tools/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/traces/__init__.py
--rw-r--r--   0        0        0     2236 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/traces/client.py
--rw-r--r--   0        0        0       65 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/user/__init__.py
--rw-r--r--   0        0        0     4328 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/resources/user/client.py
--rw-r--r--   0        0        0      308 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/types/__init__.py
--rw-r--r--   0        0        0      843 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/types/http_validation_error.py
--rw-r--r--   0        0        0      869 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/types/validation_error.py
--rw-r--r--   0        0        0      128 2023-07-17 11:38:46.221009 superagent_py-0.0.34/src/superagent/types/validation_error_loc_item.py
--rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.34/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-07-18 13:21:10.799642 superagent_py-0.0.35/LICENSE
+-rw-r--r--   0        0        0     3251 2023-07-18 13:21:10.799642 superagent_py-0.0.35/README.md
+-rw-r--r--   0        0        0      380 2023-07-18 13:21:10.799642 superagent_py-0.0.35/pyproject.toml
+-rw-r--r--   0        0        0      656 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/__init__.py
+-rw-r--r--   0        0        0     3186 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/client.py
+-rw-r--r--   0        0        0      348 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/__init__.py
+-rw-r--r--   0        0        0      426 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/api_error.py
+-rw-r--r--   0        0        0     1047 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/datetime_utils.py
+-rw-r--r--   0        0        0     3710 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      385 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/core/remove_none_from_headers.py
+-rw-r--r--   0        0        0      170 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/errors/__init__.py
+-rw-r--r--   0        0        0      313 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0        0 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/py.typed
+-rw-r--r--   0        0        0      361 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/__init__.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent/__init__.py
+-rw-r--r--   0        0        0    14309 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent_documents/__init__.py
+-rw-r--r--   0        0        0     9260 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent_documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent_tools/__init__.py
+-rw-r--r--   0        0        0     9132 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/agent_tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/api_token/__init__.py
+-rw-r--r--   0        0        0     8538 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/api_token/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/auth/__init__.py
+-rw-r--r--   0        0        0     5901 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/auth/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/documents/__init__.py
+-rw-r--r--   0        0        0    10485 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/documents/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/prompts/__init__.py
+-rw-r--r--   0        0        0    10865 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/prompts/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/tags/__init__.py
+-rw-r--r--   0        0        0    10575 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/tags/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/tools/__init__.py
+-rw-r--r--   0        0        0    11638 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/tools/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.799642 superagent_py-0.0.35/src/superagent/resources/traces/__init__.py
+-rw-r--r--   0        0        0     2236 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/resources/traces/client.py
+-rw-r--r--   0        0        0       65 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/resources/user/__init__.py
+-rw-r--r--   0        0        0     4328 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/resources/user/client.py
+-rw-r--r--   0        0        0      308 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/types/__init__.py
+-rw-r--r--   0        0        0      843 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/types/http_validation_error.py
+-rw-r--r--   0        0        0      869 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/types/validation_error.py
+-rw-r--r--   0        0        0      128 2023-07-18 13:21:10.803640 superagent_py-0.0.35/src/superagent/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0     3762 1970-01-01 00:00:00.000000 superagent_py-0.0.35/PKG-INFO
```

### Comparing `superagent_py-0.0.34/LICENSE` & `superagent_py-0.0.35/LICENSE`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/README.md` & `superagent_py-0.0.35/README.md`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/__init__.py` & `superagent_py-0.0.35/src/superagent/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 from .errors import UnprocessableEntityError
-from .resources import agent, agent_documents, agent_tools, api_token, auth, documents, prompts, tools, traces, user
+from .resources import (
+    agent,
+    agent_documents,
+    agent_tools,
+    api_token,
+    auth,
+    documents,
+    prompts,
+    tags,
+    tools,
+    traces,
+    user,
+)
 from .types import HttpValidationError, ValidationError, ValidationErrorLocItem
 
 __all__ = [
     "HttpValidationError",
     "UnprocessableEntityError",
     "ValidationError",
     "ValidationErrorLocItem",
     "agent",
     "agent_documents",
     "agent_tools",
     "api_token",
     "auth",
     "documents",
     "prompts",
+    "tags",
     "tools",
     "traces",
     "user",
 ]
```

### Comparing `superagent_py-0.0.34/src/superagent/client.py` & `superagent_py-0.0.35/src/superagent/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from .resources.agent.client import AgentClient, AsyncAgentClient
 from .resources.agent_documents.client import AgentDocumentsClient, AsyncAgentDocumentsClient
 from .resources.agent_tools.client import AgentToolsClient, AsyncAgentToolsClient
 from .resources.api_token.client import ApiTokenClient, AsyncApiTokenClient
 from .resources.auth.client import AsyncAuthClient, AuthClient
 from .resources.documents.client import AsyncDocumentsClient, DocumentsClient
 from .resources.prompts.client import AsyncPromptsClient, PromptsClient
+from .resources.tags.client import AsyncTagsClient, TagsClient
 from .resources.tools.client import AsyncToolsClient, ToolsClient
 from .resources.traces.client import AsyncTracesClient, TracesClient
 from .resources.user.client import AsyncUserClient, UserClient
 
 
 class Superagent:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
         self.agent = AgentClient(environment=self._environment, token=self._token)
         self.agent_documents = AgentDocumentsClient(environment=self._environment, token=self._token)
+        self.tags = TagsClient(environment=self._environment, token=self._token)
         self.agent_tools = AgentToolsClient(environment=self._environment, token=self._token)
         self.auth = AuthClient(environment=self._environment, token=self._token)
         self.user = UserClient(environment=self._environment, token=self._token)
         self.api_token = ApiTokenClient(environment=self._environment, token=self._token)
         self.documents = DocumentsClient(environment=self._environment, token=self._token)
         self.prompts = PromptsClient(environment=self._environment, token=self._token)
         self.tools = ToolsClient(environment=self._environment, token=self._token)
@@ -32,14 +34,15 @@
 
 class AsyncSuperagent:
     def __init__(self, *, environment: str, token: typing.Optional[str] = None):
         self._environment = environment
         self._token = token
         self.agent = AsyncAgentClient(environment=self._environment, token=self._token)
         self.agent_documents = AsyncAgentDocumentsClient(environment=self._environment, token=self._token)
+        self.tags = AsyncTagsClient(environment=self._environment, token=self._token)
         self.agent_tools = AsyncAgentToolsClient(environment=self._environment, token=self._token)
         self.auth = AsyncAuthClient(environment=self._environment, token=self._token)
         self.user = AsyncUserClient(environment=self._environment, token=self._token)
         self.api_token = AsyncApiTokenClient(environment=self._environment, token=self._token)
         self.documents = AsyncDocumentsClient(environment=self._environment, token=self._token)
         self.prompts = AsyncPromptsClient(environment=self._environment, token=self._token)
         self.tools = AsyncToolsClient(environment=self._environment, token=self._token)
```

### Comparing `superagent_py-0.0.34/src/superagent/core/datetime_utils.py` & `superagent_py-0.0.35/src/superagent/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/core/jsonable_encoder.py` & `superagent_py-0.0.35/src/superagent/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/resources/agent/client.py` & `superagent_py-0.0.35/src/superagent/resources/agent/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/resources/agent_documents/client.py` & `superagent_py-0.0.35/src/superagent/resources/agent_documents/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/resources/agent_tools/client.py` & `superagent_py-0.0.35/src/superagent/resources/agent_tools/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/resources/api_token/client.py` & `superagent_py-0.0.35/src/superagent/resources/api_token/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/resources/auth/client.py` & `superagent_py-0.0.35/src/superagent/resources/auth/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/resources/documents/client.py` & `superagent_py-0.0.35/src/superagent/resources/documents/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,24 +39,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_document(
         self,
         *,
         type: str,
-        url: str,
+        url: typing.Optional[str] = OMIT,
         name: str,
         authorization: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         from_page: typing.Optional[int] = OMIT,
         to_page: typing.Optional[int] = OMIT,
         splitter: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
     ) -> typing.Any:
-        _request: typing.Dict[str, typing.Any] = {"type": type, "url": url, "name": name}
+        _request: typing.Dict[str, typing.Any] = {"type": type, "name": name}
+        if url is not OMIT:
+            _request["url"] = url
         if authorization is not OMIT:
             _request["authorization"] = authorization
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         if from_page is not OMIT:
             _request["from_page"] = from_page
         if to_page is not OMIT:
             _request["to_page"] = to_page
         if splitter is not OMIT:
             _request["splitter"] = splitter
         _response = httpx.request(
@@ -140,24 +145,29 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_document(
         self,
         *,
         type: str,
-        url: str,
+        url: typing.Optional[str] = OMIT,
         name: str,
         authorization: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
+        metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         from_page: typing.Optional[int] = OMIT,
         to_page: typing.Optional[int] = OMIT,
         splitter: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
     ) -> typing.Any:
-        _request: typing.Dict[str, typing.Any] = {"type": type, "url": url, "name": name}
+        _request: typing.Dict[str, typing.Any] = {"type": type, "name": name}
+        if url is not OMIT:
+            _request["url"] = url
         if authorization is not OMIT:
             _request["authorization"] = authorization
+        if metadata is not OMIT:
+            _request["metadata"] = metadata
         if from_page is not OMIT:
             _request["from_page"] = from_page
         if to_page is not OMIT:
             _request["to_page"] = to_page
         if splitter is not OMIT:
             _request["splitter"] = splitter
         async with httpx.AsyncClient() as _client:
```

### Comparing `superagent_py-0.0.34/src/superagent/resources/prompts/client.py` & `superagent_py-0.0.35/src/superagent/resources/prompts/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/resources/tools/client.py` & `superagent_py-0.0.35/src/superagent/resources/tools/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -40,18 +40,19 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_a_tool(
         self,
         *,
         name: str,
         type: str,
+        description: str,
         authorization: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
     ) -> typing.Any:
-        _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
+        _request: typing.Dict[str, typing.Any] = {"name": name, "type": type, "description": description}
         if authorization is not OMIT:
             _request["authorization"] = authorization
         if metadata is not OMIT:
             _request["metadata"] = metadata
         _response = httpx.request(
             "POST",
             urllib.parse.urljoin(f"{self._environment}/", "api/v1/tools"),
@@ -86,14 +87,34 @@
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
+    def patch_tool(self, tool_id: str, *, request: typing.Dict[str, typing.Any]) -> typing.Any:
+        _response = httpx.request(
+            "PATCH",
+            urllib.parse.urljoin(f"{self._environment}/", f"api/v1/tools/{tool_id}"),
+            json=jsonable_encoder(request),
+            headers=remove_none_from_headers(
+                {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+            ),
+            timeout=60,
+        )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
     def delete_tool(self, tool_id: str) -> typing.Any:
         _response = httpx.request(
             "DELETE",
             urllib.parse.urljoin(f"{self._environment}/", f"api/v1/tools/{tool_id}"),
             headers=remove_none_from_headers(
                 {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
             ),
@@ -134,18 +155,19 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_a_tool(
         self,
         *,
         name: str,
         type: str,
+        description: str,
         authorization: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
         metadata: typing.Optional[typing.Dict[str, typing.Any]] = OMIT,
     ) -> typing.Any:
-        _request: typing.Dict[str, typing.Any] = {"name": name, "type": type}
+        _request: typing.Dict[str, typing.Any] = {"name": name, "type": type, "description": description}
         if authorization is not OMIT:
             _request["authorization"] = authorization
         if metadata is not OMIT:
             _request["metadata"] = metadata
         async with httpx.AsyncClient() as _client:
             _response = await _client.request(
                 "POST",
@@ -174,14 +196,35 @@
                 headers=remove_none_from_headers(
                     {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
                 ),
                 timeout=60,
             )
         if 200 <= _response.status_code < 300:
             return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
+        if _response.status_code == 422:
+            raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
+        try:
+            _response_json = _response.json()
+        except JSONDecodeError:
+            raise ApiError(status_code=_response.status_code, body=_response.text)
+        raise ApiError(status_code=_response.status_code, body=_response_json)
+
+    async def patch_tool(self, tool_id: str, *, request: typing.Dict[str, typing.Any]) -> typing.Any:
+        async with httpx.AsyncClient() as _client:
+            _response = await _client.request(
+                "PATCH",
+                urllib.parse.urljoin(f"{self._environment}/", f"api/v1/tools/{tool_id}"),
+                json=jsonable_encoder(request),
+                headers=remove_none_from_headers(
+                    {"Authorization": f"Bearer {self._token}" if self._token is not None else None}
+                ),
+                timeout=60,
+            )
+        if 200 <= _response.status_code < 300:
+            return pydantic.parse_obj_as(typing.Any, _response.json())  # type: ignore
         if _response.status_code == 422:
             raise UnprocessableEntityError(pydantic.parse_obj_as(HttpValidationError, _response.json()))  # type: ignore
         try:
             _response_json = _response.json()
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
```

### Comparing `superagent_py-0.0.34/src/superagent/resources/traces/client.py` & `superagent_py-0.0.35/src/superagent/resources/traces/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/resources/user/client.py` & `superagent_py-0.0.35/src/superagent/resources/user/client.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/types/http_validation_error.py` & `superagent_py-0.0.35/src/superagent/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/src/superagent/types/validation_error.py` & `superagent_py-0.0.35/src/superagent/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `superagent_py-0.0.34/PKG-INFO` & `superagent_py-0.0.35/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superagent-py
-Version: 0.0.34
+Version: 0.0.35
 Summary: 
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

