# Comparing `tmp/func_ai-0.0.8.tar.gz` & `tmp/func_ai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_ai-0.0.8.tar", max compression
+gzip compressed data, was "func_ai-0.0.9.tar", max compression
```

## Comparing `func_ai-0.0.8.tar` & `func_ai-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0     1076 2023-07-04 07:21:24.340481 func_ai-0.0.8/LICENSE
--rw-r--r--   0        0        0     4791 2023-07-04 07:21:24.340481 func_ai-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/__init__.py
--rw-r--r--   0        0        0     4082 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/function_indexer.py
--rw-r--r--   0        0        0        0 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/__init__.py
--rw-r--r--   0        0        0     4852 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/jinja_template_functions.py
--rw-r--r--   0        0        0    15515 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/llm_tools.py
--rw-r--r--   0        0        0    11280 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/openapi_function_parser.py
--rw-r--r--   0        0        0     3444 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/utils/py_function_parser.py
--rw-r--r--   0        0        0     5337 2023-07-04 07:21:24.340481 func_ai-0.0.8/func_ai/workflow_creator.py
--rw-r--r--   0        0        0      907 2023-07-04 07:21:24.344481 func_ai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5863 1970-01-01 00:00:00.000000 func_ai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-07-06 09:02:35.614006 func_ai-0.0.9/LICENSE
+-rw-r--r--   0        0        0     6277 2023-07-06 09:02:35.614006 func_ai-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/__init__.py
+-rw-r--r--   0        0        0     5383 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/function_indexer.py
+-rw-r--r--   0        0        0        0 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/ui_demos/__init__.py
+-rw-r--r--   0        0        0     1355 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/ui_demos/api_qa.py
+-rw-r--r--   0        0        0        0 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/utils/__init__.py
+-rw-r--r--   0        0        0      387 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/utils/api_qa_system_prompt.txt
+-rw-r--r--   0        0        0      313 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/utils/common.py
+-rw-r--r--   0        0        0     4852 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/utils/jinja_template_functions.py
+-rw-r--r--   0        0        0    17405 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/utils/llm_tools.py
+-rw-r--r--   0        0        0    16370 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/utils/openapi_function_parser.py
+-rw-r--r--   0        0        0     3444 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/utils/py_function_parser.py
+-rw-r--r--   0        0        0     5337 2023-07-06 09:02:35.614006 func_ai-0.0.9/func_ai/workflow_creator.py
+-rw-r--r--   0        0        0      926 2023-07-06 09:02:35.618006 func_ai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7390 1970-01-01 00:00:00.000000 func_ai-0.0.9/PKG-INFO
```

### Comparing `func_ai-0.0.8/LICENSE` & `func_ai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.8/README.md` & `func_ai-0.0.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -115,13 +115,68 @@
 assert "Age: 20" in resp
 # prints
 """
 Name: John 
 Age: 20
 """
 ```
+### OpenAPI Spec Chat Bot
+
+This example starts a `gradio` server that allows you to interact with the OpenAPI spec.
+
+```python
+import gradio as gr
+from dotenv import load_dotenv
+
+from func_ai.utils.llm_tools import OpenAIInterface
+from func_ai.utils.openapi_function_parser import OpenAPISpecOpenAIWrapper
+
+_chat_message = []
+
+_spec = None
+
+
+def add_text(history, text):
+    global _chat_message
+    history = history + [(text, None)]
+    _chat_message.append(_spec.api_qa(text, max_tokens=500))
+    return history, ""
+
+
+def add_file(history, file):
+    history = history + [((file.name,), None)]
+    return history
+
+
+def bot(history):
+    global _chat_message
+    # print(temp_callback_handler.get_output())
+    # response = temp_callback_handler.get_output()['output']
+    history[-1][1] = _chat_message[-1]
+    return history
+
+
+with gr.Blocks() as demo:
+    chatbot = gr.Chatbot([], elem_id="chatbot").style(height=1500)
+
+    with gr.Row():
+        with gr.Column(scale=1):
+            txt = gr.Textbox(
+                show_label=False,
+                placeholder="Enter text and press enter",
+            ).style(container=False)
+    txt.submit(add_text, [chatbot, txt], [chatbot, txt]).then(
+        bot, chatbot, chatbot
+    )
+
+if __name__ == "__main__":
+    load_dotenv()
+    _spec = OpenAPISpecOpenAIWrapper.from_url('http://petstore.swagger.io/v2/swagger.json',
+                                              llm_interface=OpenAIInterface(), index=True)
+    demo.launch()
+```
 
 ## Inspiration
 
 - https://github.com/jxnl/openai_function_call
 - https://github.com/rizerphe/openai-functions
 - https://github.com/aurelio-labs/funkagent
```

### Comparing `func_ai-0.0.8/func_ai/function_indexer.py` & `func_ai-0.0.9/func_ai/function_indexer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,44 @@
 import inspect
-import json
+import logging
 
 import chromadb
 from chromadb import Settings
 from chromadb.utils import embedding_functions
 from ulid import ULID
 
+from func_ai.utils.llm_tools import OpenAIFunctionWrapper
 from func_ai.utils.py_function_parser import func_to_json
 
-openai_ef = embedding_functions.OpenAIEmbeddingFunction(
-    model_name="text-embedding-ada-002"
-)
+logging.basicConfig(format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', level=logging.DEBUG)
+logger = logging.getLogger(__name__)
 
 
 class FunctionIndexer(object):
     """
     Index functions
     """
 
-    def __init__(self, db_path: str) -> None:
+    def __init__(self, db_path: str, collection_name: str = "function_index") -> None:
         """
         Initialize function indexer
-        :param db_path:
+        :param db_path: The path where to store the database
+        :param collection_name: The name of the collection
         """
         self._client = chromadb.Client(Settings(
             chroma_db_impl="duckdb+parquet",
             persist_directory=db_path  # Optional, defaults to .chromadb/ in the current directory
         ))
+        self.collection_name = collection_name
         self._fns_map = {}
         self._fns_index_map = {}
         self._open_ai_function_map = []
+        self.openai_ef = embedding_functions.OpenAIEmbeddingFunction(
+            model_name="text-embedding-ada-002"
+        )
 
     def reset_function_index(self) -> None:
         """
         Reset function index
 
         :return:
         """
@@ -46,26 +51,42 @@
         Note: Function uniqueness is not checked in this version
 
         :param functions:
         :return:
         """
 
         _ai_fun_map, _fns_map, _fns_index_map = FunctionIndexer.get_functions(functions)
-        collection = self._client.get_or_create_collection(name="function_index", metadata={"hnsw:space": "cosine"},
-                                                           embedding_function=openai_ef)
+        collection = self._client.get_or_create_collection(name=self.collection_name, metadata={"hnsw:space": "cosine"},
+                                                           embedding_function=self.openai_ef)
         self._fns_map.update(_fns_map)
         self._open_ai_function_map.extend(_ai_fun_map)
         self._fns_index_map.update(_fns_index_map)
         collection.add(documents=[f['description'] for f in _fns_index_map.values()],
                        metadatas=[{"name": f,
                                    "file": str(inspect.getfile(_fns_map[f])),
                                    "module": inspect.getmodule(_fns_map[f]).__name__} for f, v in
                                   _fns_index_map.items()],
                        ids=[str(ULID()) for _ in _fns_index_map.values()])
 
+    def index_wrapper_functions(self, functions: list[OpenAIFunctionWrapper]):
+        """
+        Index one or more functions
+        Note: Function uniqueness is not checked in this version
+        :param functions:
+        :return:
+        """
+        collection = self._client.get_or_create_collection(name=self.collection_name,
+                                                           metadata={"hnsw:space": "cosine"},
+                                                           embedding_function=self.openai_ef)
+        # print(f"Docs: {collection.get()}")
+        collection.add(documents=[f.description for f in functions],
+                       metadatas=[{"name": f.name, **f.metadata_dict} for f in
+                                  functions],
+                       ids=[str(ULID()) for _ in functions])
+
     def rehydrate_function_map(self, functions: list[callable]) -> None:
         """
         Rehydrate function map
 
         :param functions:
         :return:
         """
@@ -88,21 +109,22 @@
         """
         Find functions by description
 
         :param query: Query string
         :return:
         """
         _response = []
-        collection = self._client.get_or_create_collection(name="function_index", metadata={"hnsw:space": "cosine"},
-                                                           embedding_function=openai_ef)
-        print(collection.get())
+        collection = self._client.get_or_create_collection(name=self.collection_name,
+                                                           metadata={"hnsw:space": "cosine"},
+                                                           embedding_function=self.openai_ef)
+        # print(collection.get())
         res = collection.query(query_texts=[query], n_results=max_results)
         print(f"Got response for sematic search: {res}")
         for r in res['metadatas'][0]:
-            _response.append(self._fns_map[r['name']])
+            _response.append(r['name'])
         return _response
 
     @staticmethod
     def get_functions(functions: list[callable]) -> (list, dict):
         """
         Get functions and function map.
```

### Comparing `func_ai-0.0.8/func_ai/utils/jinja_template_functions.py` & `func_ai-0.0.9/func_ai/utils/jinja_template_functions.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.8/func_ai/utils/llm_tools.py` & `func_ai-0.0.9/func_ai/utils/llm_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from typing import Any
 
 import openai
 from tenacity import retry, wait_fixed, stop_after_attempt
 
 from pydantic import BaseModel, Field
 
-from func_ai.utils.py_function_parser import type_mapping
+from func_ai.utils.common import arg_in_func
+from func_ai.utils.py_function_parser import type_mapping, func_to_json
 
 logging.basicConfig(format='%(asctime)s - %(name)s - %(levelname)s - %(message)s', level=logging.DEBUG)
 logger = logging.getLogger(__name__)
 
 
 class ConversationStore(BaseModel):
     """
@@ -40,14 +41,21 @@
     def get_conversation(self) -> list:
         """
         Returns the conversation
         :return:
         """
         return self.conversation
 
+    def get_last_message(self) -> Any:
+        """
+        Returns the last message
+        :return:
+        """
+        return self.conversation[-1]
+
 
 class OpenAIConversationStore(ConversationStore):
 
     def add_message(self, message: Any):
         self.conversation.append(message)
 
     def add_system_message(self, message: str):
@@ -125,23 +133,36 @@
     def get_conversation(self) -> list[any]:
         """
         Returns the conversation
         :return:
         """
         return self.conversation_store.get_conversation()
 
-    def add_conversation_message(self, message: any) -> "LLMInterface":
+    def add_conversation_message(self, message: any, update_llm: bool = False, **kwargs) -> "LLMInterface":
         """
         Adds a message to the conversation
-        :param message:
+        :param message: The message to add
+        :param update_llm: Whether to update the LLM with the new conversation
+        :param kwargs: Parameters to pass to the API
         :return:
         """
         self.conversation_store.add_message(message)
+        if update_llm:
+            self.update_llm_conversation(**kwargs)
         return self
 
+    def update_llm_conversation(self, **kwargs) -> "LLMInterface":
+        """
+        Sends the updated conversation to the LLM
+
+        :param kwargs: Parameters to pass to the API
+        :return:
+        """
+        raise NotImplementedError
+
 
 class OpenAIInterface(LLMInterface):
     """
     Interface for interacting with the OpenAI API
     """
     max_tokens: int = Field(default=256, description="The maximum number of tokens to return")
     model: str = Field(default="gpt-3.5-turbo-0613", description="The model to use")
@@ -154,20 +175,23 @@
                          model=kwargs.get("model", "gpt-3.5-turbo-0613"),
                          temperature=kwargs.get("temperature", 0.0),
                          conversation_store=OpenAIConversationStore())
         openai.api_key = kwargs.get("api_key", os.getenv("OPENAI_API_KEY"))
 
     @retry(stop=stop_after_attempt(3), reraise=True, wait=wait_fixed(1),
            retry_error_callback=lambda x: logger.warning(x))
-    def send(self, prompt: str, **kwargs) -> dict:
+    def update_llm_conversation(self, **kwargs) -> "OpenAIInterface":
+        """
+        Sends the updated conversation to the LLM
+
+        :param kwargs: Parameters to pass to the API
+        :return:
+        """
         _functions = kwargs.get("functions", None)
         _model = kwargs.get("model", self.model)
-        # print(type(self._conversation_store))
-        self.conversation_store.add_message({"role": "user", "content": prompt})
-        logger.debug(f"Prompt: {prompt}")
         try:
             if _functions:
                 response = openai.ChatCompletion.create(
                     model=_model,
                     messages=self.conversation_store.get_conversation(),
                     functions=_functions,
                     function_call="auto",
@@ -195,20 +219,28 @@
             if "function_call" in response["choices"][0]["message"] and response["choices"][0]["message"][
                 "function_call"]:
                 response["choices"][0]["message"]["function_call"]["arguments"] = \
                     response["choices"][0]["message"]["function_call"]["arguments"].encode('utf-8').decode("utf-8")
             self.update_cost(_model, response)
             _response_message = response["choices"][0]["message"]
             self.conversation_store.add_message(_response_message)
-            return _response_message
+            return self
         except Exception as e:
             logger.error(f"Error: {e}")
             traceback.print_exc()
             raise e
 
+    def send(self, prompt: str, **kwargs) -> dict[str, any]:
+        # print(type(self._conversation_store))
+        self.conversation_store.add_message({"role": "user", "content": prompt})
+        logger.debug(f"Prompt: {prompt}")
+        response = self.update_llm_conversation(**kwargs)
+        logger.debug(f"Response: {response}")
+        return self.conversation_store.get_last_message()
+
     def load_cost_mapping(self, file_path: str) -> None:
         with open(file_path) as f:
             self.cost_mapping = json.load(f)
 
     def update_cost(self, model, api_response) -> None:
         if model not in self.usage:
             self.usage[model] = {
@@ -217,15 +249,14 @@
                 "total_tokens": 0
             }
         self.usage[model]["prompt_tokens"] += api_response['usage']['prompt_tokens']
         self.usage[model]["completion_tokens"] += api_response['usage']['completion_tokens']
         self.usage[model]["total_tokens"] += api_response['usage']['total_tokens']
 
 
-
 class OpenAISchema(BaseModel):
     @classmethod
     @property
     def openai_schema(cls):
         schema = cls.schema()
 
         return {
@@ -316,15 +347,18 @@
         """
         self.llm_interface = llm_interface
         self._name = name
         self._description = description
         assert "required" in parameters, "Required field not present in parameters"
         self._parameters = parameters
         assert callable(func) or isinstance(func, functools.partial), "Function must be callable"
-        self.func = functools.partial(func, action=self)
+        if arg_in_func(func, "action"):
+            self.func = functools.partial(func, action=self)
+        else:
+            self.func = func
         self._metadata = kwargs
         self._llm_calls = []
 
     @property
     def name(self) -> str:
         """
         Returns the name of the function
@@ -366,14 +400,23 @@
         Returns the metadata of the function
 
         :return: dict containing the metadata
         """
         return self._metadata
 
     @property
+    def metadata_dict(self) -> dict[str, str]:
+        """
+        Returns the metadata of the function as a
+
+        :return:
+        """
+        return {k: str(v) for k, v in self._metadata.items()}
+
+    @property
     def schema(self) -> dict[str, any]:
         """
         Returns the schema of the function that can be passed to OpenAI API
 
         :return: dict containing the schema
         """
         return {
@@ -453,7 +496,20 @@
 
         :param prompt: User prompt
         :param kwargs: arguments to be passed to the function
         :return: The response from the function call
         """
         self.from_response(self.llm_interface.send(prompt, functions=[self.schema]))
         return self
+
+    @classmethod
+    def from_python_function(cls, func: callable, llm_interface: LLMInterface, **kwargs) -> "OpenAIFunctionWrapper":
+        """
+        Returns an instance of the class from Python function
+
+        :param func: Python function
+        :param llm_interface: LLM interface
+        :param kwargs: arguments to be passed to the function
+        :return:
+        """
+        _func = func_to_json(func)
+        return cls(llm_interface=llm_interface, func=func, **_func, **kwargs)
```

### Comparing `func_ai-0.0.8/func_ai/utils/py_function_parser.py` & `func_ai-0.0.9/func_ai/utils/py_function_parser.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.8/func_ai/workflow_creator.py` & `func_ai-0.0.9/func_ai/workflow_creator.py`

 * *Files identical despite different names*

### Comparing `func_ai-0.0.8/pyproject.toml` & `func_ai-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "func-ai"
-version = "0.0.8"
+version = "0.0.9"
 description = "AI Functional Catalog - OpenAI functions on steriods"
 authors = ["Trayan Azarov <trayan.azarov@amikos.tech>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "func_ai" }]
 
 [tool.poetry.urls]
@@ -14,20 +14,21 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 openai = "^0.27.8"
 requests = "^2.31.0"
 chromadb = "^0.3.26"
 python-ulid = "^1.1.0"
-fastapi = "^0.98.0"
+fastapi = "^0.99.1"
 pyyaml = "^6.0"
 jsonschema = "^4.17.3"
 python-dotenv = "^1.0.0"
 tenacity = "^8.2.2"
 jinja2 = "^3.1.2"
+gradio = "^3.35.2"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.0"
 pytest-env = "^0.8.2"
 pytest-html = "^3.2.0"
 pytest-metadata = "^3.0.0"
```

### Comparing `func_ai-0.0.8/PKG-INFO` & `func_ai-0.0.9/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: func-ai
-Version: 0.0.8
+Version: 0.0.9
 Summary: AI Functional Catalog - OpenAI functions on steriods
 License: MIT
 Author: Trayan Azarov
 Author-email: trayan.azarov@amikos.tech
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chromadb (>=0.3.26,<0.4.0)
-Requires-Dist: fastapi (>=0.98.0,<0.99.0)
+Requires-Dist: fastapi (>=0.99.1,<0.100.0)
+Requires-Dist: gradio (>=3.35.2,<4.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: jsonschema (>=4.17.3,<5.0.0)
 Requires-Dist: openai (>=0.27.8,<0.28.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: python-ulid (>=1.1.0,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
@@ -142,13 +143,68 @@
 assert "Age: 20" in resp
 # prints
 """
 Name: John 
 Age: 20
 """
 ```
+### OpenAPI Spec Chat Bot
+
+This example starts a `gradio` server that allows you to interact with the OpenAPI spec.
+
+```python
+import gradio as gr
+from dotenv import load_dotenv
+
+from func_ai.utils.llm_tools import OpenAIInterface
+from func_ai.utils.openapi_function_parser import OpenAPISpecOpenAIWrapper
+
+_chat_message = []
+
+_spec = None
+
+
+def add_text(history, text):
+    global _chat_message
+    history = history + [(text, None)]
+    _chat_message.append(_spec.api_qa(text, max_tokens=500))
+    return history, ""
+
+
+def add_file(history, file):
+    history = history + [((file.name,), None)]
+    return history
+
+
+def bot(history):
+    global _chat_message
+    # print(temp_callback_handler.get_output())
+    # response = temp_callback_handler.get_output()['output']
+    history[-1][1] = _chat_message[-1]
+    return history
+
+
+with gr.Blocks() as demo:
+    chatbot = gr.Chatbot([], elem_id="chatbot").style(height=1500)
+
+    with gr.Row():
+        with gr.Column(scale=1):
+            txt = gr.Textbox(
+                show_label=False,
+                placeholder="Enter text and press enter",
+            ).style(container=False)
+    txt.submit(add_text, [chatbot, txt], [chatbot, txt]).then(
+        bot, chatbot, chatbot
+    )
+
+if __name__ == "__main__":
+    load_dotenv()
+    _spec = OpenAPISpecOpenAIWrapper.from_url('http://petstore.swagger.io/v2/swagger.json',
+                                              llm_interface=OpenAIInterface(), index=True)
+    demo.launch()
+```
 
 ## Inspiration
 
 - https://github.com/jxnl/openai_function_call
 - https://github.com/rizerphe/openai-functions
 - https://github.com/aurelio-labs/funkagent
```

