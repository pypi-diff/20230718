# Comparing `tmp/scale_llm_engine-0.0.0b2.tar.gz` & `tmp/scale_llm_engine-0.0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b2.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b3.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b2.tar` & `scale_llm_engine-0.0.0b3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1001 2023-07-17 21:24:00.034378 scale_llm_engine-0.0.0b2/README.md
--rw-r--r--   0        0        0     1584 2023-07-17 22:16:53.234768 scale_llm_engine-0.0.0b2/llmengine/__init__.py
--rw-r--r--   0        0        0     6190 2023-07-17 21:57:41.640716 scale_llm_engine-0.0.0b2/llmengine/api_engine.py
--rw-r--r--   0        0        0    11436 2023-07-17 22:13:22.416895 scale_llm_engine-0.0.0b2/llmengine/completion.py
--rw-r--r--   0        0        0    10146 2023-07-17 22:13:22.418064 scale_llm_engine-0.0.0b2/llmengine/data_types.py
--rw-r--r--   0        0        0     2745 2023-07-17 10:30:37.104747 scale_llm_engine-0.0.0b2/llmengine/errors.py
--rw-r--r--   0        0        0     7795 2023-07-17 21:57:41.642849 scale_llm_engine-0.0.0b2/llmengine/fine_tuning.py
--rw-r--r--   0        0        0     5391 2023-07-17 21:57:41.643669 scale_llm_engine-0.0.0b2/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-07-17 22:16:53.235607 scale_llm_engine-0.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1001 2023-07-17 21:09:48.759908 scale_llm_engine-0.0.0b3/README.md
+-rw-r--r--   0        0        0     1576 2023-07-18 04:36:10.686982 scale_llm_engine-0.0.0b3/llmengine/__init__.py
+-rw-r--r--   0        0        0     6190 2023-07-18 04:31:34.842871 scale_llm_engine-0.0.0b3/llmengine/api_engine.py
+-rw-r--r--   0        0        0    12958 2023-07-18 04:31:39.203554 scale_llm_engine-0.0.0b3/llmengine/completion.py
+-rw-r--r--   0        0        0    11851 2023-07-18 04:31:39.203919 scale_llm_engine-0.0.0b3/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-16 18:41:46.698514 scale_llm_engine-0.0.0b3/llmengine/errors.py
+-rw-r--r--   0        0        0    11100 2023-07-18 04:31:39.204232 scale_llm_engine-0.0.0b3/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0     7052 2023-07-18 03:09:52.904995 scale_llm_engine-0.0.0b3/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-07-18 04:32:04.597570 scale_llm_engine-0.0.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b3/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b2/README.md` & `scale_llm_engine-0.0.0b3/README.md`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b2/llmengine/__init__.py` & `scale_llm_engine-0.0.0b3/llmengine/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,25 +8,25 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.beta2"
+__version__ = "0.0.0.beta3"
 
 from typing import Sequence
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CompletionOutput,
     CompletionStreamOutput,
-    CompletionStreamV1Response,
-    CompletionSyncV1Response,
+    CompletionStreamResponse,
+    CompletionSyncResponse,
     CreateFineTuneRequest,
     CreateFineTuneResponse,
     DeleteLLMEndpointResponse,
     GetFineTuneResponse,
     GetLLMEndpointResponse,
     ListFineTunesResponse,
     ListLLMEndpointsResponse,
@@ -35,16 +35,16 @@
 from llmengine.model import Model
 
 __all__: Sequence[str] = (
     "CancelFineTuneResponse",
     "Completion",
     "CompletionOutput",
     "CompletionStreamOutput",
-    "CompletionStreamV1Response",
-    "CompletionSyncV1Response",
+    "CompletionStreamResponse",
+    "CompletionSyncResponse",
     "CreateFineTuneRequest",
     "CreateFineTuneResponse",
     "DeleteLLMEndpointResponse",
     "FineTune",
     "GetFineTuneResponse",
     "GetLLMEndpointResponse",
     "ListFineTunesResponse",
```

### Comparing `scale_llm_engine-0.0.0b2/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b3/llmengine/api_engine.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b2/llmengine/completion.py` & `scale_llm_engine-0.0.0b3/llmengine/completion.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,83 @@
 from typing import AsyncIterable, Iterator, Union
 
 from llmengine.api_engine import APIEngine
 from llmengine.data_types import (
+    CompletionStreamResponse,
     CompletionStreamV1Request,
-    CompletionStreamV1Response,
+    CompletionSyncResponse,
     CompletionSyncV1Request,
-    CompletionSyncV1Response,
 )
 
 
 class Completion(APIEngine):
     """
     Completion API. This API is used to generate text completions.
 
-    Language Models are trained to understand natural language and provide text outputs as a response to
-    their inputs. The inputs are called _prompts_ and outputs are referred to as _completions_.
-    LLMs take the input _prompts_ and chunk them smaller units called _tokens_ to process and generate
+    Language models are trained to understand natural language and predict text outputs as a response to
+    their inputs. The inputs are called _prompts_ and the outputs are referred to as _completions_.
+    LLMs take the input prompts and chunk them into smaller units called _tokens_ to process and generate
     language. Tokens may include trailing spaces and even sub-words; this process is language dependent.
 
-    The Completions API can be run either
-    synchronous or asynchronously (via Python `asyncio`); for each of these modes, you can also choose to
-    stream token responses or not.
+    The Completion API can be run either synchronous or asynchronously (via Python `asyncio`).
+    For each of these modes, you can also choose whether to stream token responses or not.
     """
 
     @classmethod
     async def acreate(
         cls,
         model: str,
         prompt: str,
         max_new_tokens: int = 20,
         temperature: float = 0.2,
         timeout: int = 10,
         stream: bool = False,
-    ) -> Union[CompletionSyncV1Response, AsyncIterable[CompletionStreamV1Response]]:
+    ) -> Union[CompletionSyncResponse, AsyncIterable[CompletionStreamResponse]]:
         """
         Creates a completion for the provided prompt and parameters asynchronously (with `asyncio`).
 
+        This API can be used to get the LLM to generate a completion *asynchronously*.
+        It takes as parameters the `model` ([see Model Zoo](../../model_zoo)) and the `prompt`.
+        Optionally it takes `max_new_tokens`, `temperature`, `timeout` and `stream`.
+        It returns
+        [CompletionSyncV1Response](../../api/data_types/#llmengine.CompletionSyncV1Response)
+        if `stream=False` or an async iterator of
+        [CompletionStreamV1Response](../../api/data_types/#llmengine.CompletionStreamV1Response)
+        with `request_id` and `outputs` fields.
+
         Args:
             model (str):
-                Name of the model to use. See [Model Zoo](../model_zoo/) for a list of Models that are supported.
-
+                Name of the model to use. See [Model Zoo](../../model_zoo) for a list of Models that are supported.
             prompt (str):
                 The prompt to generate completions for, encoded as a string.
 
             max_new_tokens (int):
                 The maximum number of tokens to generate in the completion.
 
                 The token count of your prompt plus `max_new_tokens` cannot exceed the model's context length. See
-                [Model Zoo](../model_zoo/) for information on each supported model's context length.
+                [Model Zoo](../../model_zoo) for information on each supported model's context length.
 
             temperature (float):
                 What sampling temperature to use, in the range `(0, 1]`. Higher values like 0.8 will make the output
                 more random, while lower values like 0.2 will make it more focused and deterministic.
 
             timeout (int):
                 Timeout in seconds. This is the maximum amount of time you are willing to wait for a response.
 
             stream (bool):
                 Whether to stream the response. If true, the return type is an
-                `Iterator[CompletionStreamV1Response]`. Otherwise, the return type is a `CompletionSyncV1Response`.
+                `Iterator[CompletionStreamResponse]`. Otherwise, the return type is a `CompletionSyncResponse`.
                 When streaming, tokens will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#event_stream_format).
 
         Returns:
-            response (Union[CompletionSyncV1Response, AsyncIterable[CompletionStreamV1Response]]): The generated response (if `streaming=False`) or iterator of response chunks (if `streaming=True`)
+            response (Union[CompletionSyncResponse, AsyncIterable[CompletionStreamResponse]]): The generated response (if `stream=False`) or iterator of response chunks (if `stream=True`)
+
+        Token streaming can be used to reduce _percieved_ latency for applications:
 
-        Example without token streaming:
+        === "Asynchronous completion without token streaming in python"
             ```python
             import asyncio
             from llmengine import Completion
 
             async def main():
                 response = await Completion.acreate(
                     model="llama-7b",
@@ -77,29 +86,31 @@
                     temperature=0.2,
                 )
                 print(response.json())
 
             asyncio.run(main())
             ```
 
-        JSON response:
+        === "Response in json"
             ```json
             {
                 "request_id": "b1b2c3d4e5f6g7h8i9j0",
                 "outputs":
                 [
                     {
                         "text": "_______, and I am a _____",
                         "num_completion_tokens": 10
                     }
                 ],
             }
             ```
 
-        Example with token streaming:
+        Here is how applications can use streaming:
+
+        === "Asynchronous completion with token streaming in python"
             ```python
             import asyncio
             from llmengine import Completion
 
             async def main():
                 stream = await Completion.acreate(
                     model="llama-7b",
@@ -112,131 +123,144 @@
                 async for response in stream:
                     if response.output:
                         print(response.json())
 
             asyncio.run(main())
             ```
 
-        JSON responses:
+        === "Response in json"
             ```json
             {"request_id": "0123456789", "output": {"text": "\\n", "finished": false, "num_completion_tokens": 1}}
             {"request_id": "0123456789", "output": {"text": "I", "finished": false, "num_completion_tokens": 2}}
             {"request_id": "0123456789", "output": {"text": " think", "finished": false, "num_completion_tokens": 3}}
             {"request_id": "0123456789", "output": {"text": " the", "finished": false, "num_completion_tokens": 4}}
             {"request_id": "0123456789", "output": {"text": " sky", "finished": true, "num_completion_tokens": 5}}
             ```
         """
         if stream:
 
             async def _acreate_stream(
                 **kwargs,
-            ) -> AsyncIterable[CompletionStreamV1Response]:
+            ) -> AsyncIterable[CompletionStreamResponse]:
                 data = CompletionStreamV1Request(**kwargs).dict()
                 response = cls.apost_stream(
                     resource_name=f"v1/llm/completions-stream?model_endpoint_name={model}",
                     data=data,
                     timeout=timeout,
                 )
                 async for chunk in response:
-                    yield CompletionStreamV1Response.parse_obj(chunk)
+                    yield CompletionStreamResponse.parse_obj(chunk)
 
             return _acreate_stream(
                 model=model,
                 prompt=prompt,
                 max_new_tokens=max_new_tokens,
                 temperature=temperature,
                 timeout=timeout,
             )
 
         else:
 
-            async def _acreate_sync(**kwargs) -> CompletionSyncV1Response:
+            async def _acreate_sync(**kwargs) -> CompletionSyncResponse:
                 data = CompletionSyncV1Request(**kwargs).dict()
                 response = await cls.apost_sync(
                     resource_name=f"v1/llm/completions-sync?model_endpoint_name={model}",
                     data=data,
                     timeout=timeout,
                 )
-                return CompletionSyncV1Response.parse_obj(response)
+                return CompletionSyncResponse.parse_obj(response)
 
             return await _acreate_sync(
-                prompts=[prompt], max_new_tokens=max_new_tokens, temperature=temperature
+                prompt=prompt, max_new_tokens=max_new_tokens, temperature=temperature
             )
 
     @classmethod
     def create(
         cls,
         model: str,
         prompt: str,
         max_new_tokens: int = 20,
         temperature: float = 0.2,
         timeout: int = 10,
         stream: bool = False,
-    ) -> Union[CompletionSyncV1Response, Iterator[CompletionStreamV1Response]]:
+    ) -> Union[CompletionSyncResponse, Iterator[CompletionStreamResponse]]:
         """
         Creates a completion for the provided prompt and parameters synchronously.
 
+        This API can be used to get the LLM to generate a completion *synchronously*.
+        It takes as parameters the `model` ([see Model Zoo](../../model_zoo)) and the `prompt`.
+        Optionally it takes `max_new_tokens`, `temperature`, `timeout` and `stream`.
+        It returns
+        [CompletionSyncV1Response](../../api/data_types/#llmengine.CompletionSyncV1Response)
+        if `stream=False` or an async iterator of
+        [CompletionStreamV1Response](../../api/data_types/#llmengine.CompletionStreamV1Response)
+        with `request_id` and `outputs` fields.
+
         Args:
             model (str):
-                Name of the model to use. See [Model Zoo](../model_zoo/) for a list of Models that are supported.
+                Name of the model to use. See [Model Zoo](../../model_zoo) for a list of Models that are supported.
 
             prompt (str):
                 The prompt to generate completions for, encoded as a string.
 
             max_new_tokens (int):
                 The maximum number of tokens to generate in the completion.
 
                 The token count of your prompt plus `max_new_tokens` cannot exceed the model's context length. See
-                [Model Zoo](../model_zoo/) for information on each supported model's context length.
+                [Model Zoo](../../model_zoo) for information on each supported model's context length.
 
             temperature (float):
                 What sampling temperature to use, in the range `(0, 1]`. Higher values like 0.8 will make the output
                 more random, while lower values like 0.2 will make it more focused and deterministic.
 
             timeout (int):
                 Timeout in seconds. This is the maximum amount of time you are willing to wait for a response.
 
             stream (bool):
                 Whether to stream the response. If true, the return type is an
-                `Iterator[CompletionStreamV1Response]`. Otherwise, the return type is a `CompletionSyncV1Response`.
+                `Iterator[CompletionStreamResponse]`. Otherwise, the return type is a `CompletionSyncResponse`.
                 When streaming, tokens will be sent as data-only [server-sent events](https://developer.mozilla.org/en-US/docs/Web/API/Server-sent_events/Using_server-sent_events#event_stream_format).
 
 
         Returns:
-            response (Union[CompletionSyncV1Response, AsyncIterable[CompletionStreamV1Response]]): The generated response (if `streaming=False`) or iterator of response chunks (if `streaming=True`)
+            response (Union[CompletionSyncResponse, AsyncIterable[CompletionStreamResponse]]): The generated response (if `stream=False`) or iterator of response chunks (if `stream=True`)
+
+        Token streaming can be used to reduce _percieved_ latency for applications:
 
-        Example request without token streaming:
+        === "Synchronous completion without token streaming in python"
             ```python
             from llmengine import Completion
 
             response = Completion.create(
                 model="llama-7b",
                 prompt="Hello, my name is",
                 max_new_tokens=10,
                 temperature=0.2,
             )
             print(response.json())
             ```
 
-        JSON Response:
+        === "Response in json"
             ```json
             {
                 "request_id": "0123456789",
                 "outputs":
                 [
                     {
                         "text": "_______ and I am a _______",
                         "num_completion_tokens": 10
                     }
                 ],
                 "traceback": null
             }
             ```
 
-        Example request with token streaming:
+        Here is how applications can use streaming:
+
+        === "Synchronous completion with token streaming in python"
             ```python
             from llmengine import Completion
 
             stream = Completion.create(
                 model="llama-7b",
                 prompt="why is the sky blue?",
                 max_new_tokens=5,
@@ -245,15 +269,15 @@
             )
 
             for response in stream:
                 if response.output:
                     print(response.json())
             ```
 
-        JSON responses:
+        === "Response in json"
             ```json
             {"request_id": "0123456789", "output": {"text": "\\n", "finished": false, "num_completion_tokens": 1 } }
             {"request_id": "0123456789", "output": {"text": "I", "finished": false, "num_completion_tokens": 2 } }
             {"request_id": "0123456789", "output": {"text": " don", "finished": false, "num_completion_tokens": 3 } }
             {"request_id": "0123456789", "output": {"text": "’", "finished": false, "num_completion_tokens": 4 } }
             {"request_id": "0123456789", "output": {"text": "t", "finished": true, "num_completion_tokens": 5 } }
             ```
@@ -264,23 +288,23 @@
                 data_stream = CompletionStreamV1Request(**kwargs).dict()
                 response_stream = cls.post_stream(
                     resource_name=f"v1/llm/completions-stream?model_endpoint_name={model}",
                     data=data_stream,
                     timeout=timeout,
                 )
                 for chunk in response_stream:
-                    yield CompletionStreamV1Response.parse_obj(chunk)
+                    yield CompletionStreamResponse.parse_obj(chunk)
 
             return _create_stream(
                 prompt=prompt, max_new_tokens=max_new_tokens, temperature=temperature
             )
 
         else:
             data = CompletionSyncV1Request(
-                prompts=[prompt], max_new_tokens=max_new_tokens, temperature=temperature
+                prompt=prompt, max_new_tokens=max_new_tokens, temperature=temperature
             ).dict()
             response = cls.post_sync(
                 resource_name=f"v1/llm/completions-sync?model_endpoint_name={model}",
                 data=data,
                 timeout=timeout,
             )
-            return CompletionSyncV1Response.parse_obj(response)
+            return CompletionSyncResponse.parse_obj(response)
```

### Comparing `scale_llm_engine-0.0.0b2/llmengine/data_types.py` & `scale_llm_engine-0.0.0b3/llmengine/data_types.py`

 * *Files 27% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     TEXT_GENERATION_INFERENCE = "text_generation_inference"
 
 
 class LLMSource(str, Enum):
     HUGGING_FACE = "hugging_face"
 
 
+class Quantization(str, Enum):
+    BITSANDBYTES = "bitsandbytes"
+
+
 class GpuType(str, Enum):
     """Lists allowed GPU types for LLMEngine."""
 
     NVIDIA_TESLA_T4 = "nvidia-tesla-t4"
     NVIDIA_AMPERE_A10 = "nvidia-ampere-a10"
     NVIDIA_AMPERE_A100 = "nvidia-a100"
 
@@ -81,15 +85,15 @@
     gpus: int = Field(..., ge=0)
     memory: StorageSpecificationType
     gpu_type: Optional[GpuType]
     storage: Optional[StorageSpecificationType]
     optimize_costs: Optional[bool]
 
 
-class GetModelEndpointV1Response(BaseModel):
+class GetModelEndpointResponse(BaseModel):
     id: str
     name: str
     endpoint_type: ModelEndpointType
     destination: str
     deployment_name: Optional[str] = Field(default=None)
     metadata: Optional[Dict[str, Any]] = Field(default=None)  # TODO: JSON type
     bundle_name: str
@@ -148,38 +152,60 @@
 
 
 class GetLLMEndpointResponse(BaseModel):
     """
     Response object for retrieving a Model.
     """
 
-    id: str = Field(description="The autogenerated ID of the Launch endpoint.")
-    """The autogenerated ID of the Launch endpoint."""
-    name: str = Field(description="The name of the Launch endpoint.")
-    """The name of the Launch endpoint."""
-    model_name: str = Field(description="The name of the model.")
-    """The name of the model."""
-    source: LLMSource = Field(description="The source of the model.")
-    """The source of the model."""
+    id: Optional[str] = Field(
+        default=None, description="(For self-hosted users) The autogenerated ID of the model."
+    )
+    """(For self-hosted users) The autogenerated ID of the model."""
+    name: str = Field(
+        description="The name of the model. Use this for making inference requests to the model."
+    )
+    """The name of the model. Use this for making inference requests to the model."""
+    model_name: Optional[str] = Field(
+        default=None,
+        description="(For self-hosted users) For fine-tuned models, the base model. For base models, this will be the same as `name`.",
+    )
+    """(For self-hosted users) For fine-tuned models, the base model. For base models, this will be the same as `name`."""
+    source: LLMSource = Field(description="The source of the model, e.g. Hugging Face.")
+    """The source of the model, e.g. Hugging Face."""
     inference_framework: LLMInferenceFramework = Field(
-        description="The inference framework used by the endpoint."
+        description="The inference framework used by the model."
     )
-    """The inference framework used by the endpoint."""
-    num_shards: int = Field(description="The number of shards.")
-    """The number of shards."""
+    """The inference framework used by the model."""
+    inference_framework_tag: Optional[str] = Field(
+        default=None,
+        description="(For self-hosted users) The Docker image tag used to run the model.",
+    )
+    """(For self-hosted users) The Docker image tag used to run the model."""
+    num_shards: Optional[int] = Field(
+        default=None, description="(For self-hosted users) The number of shards."
+    )
+    """(For self-hosted users) The number of shards."""
+    quantize: Optional[Quantization] = Field(
+        default=None, description="(For self-hosted users) The quantization method."
+    )
+    """(For self-hosted users) The quantization method."""
+    spec: Optional[GetModelEndpointResponse] = Field(
+        default=None, description="(For self-hosted users) Model endpoint details."
+    )
+    """(For self-hosted users) Model endpoint details."""
 
 
 class ListLLMEndpointsResponse(BaseModel):
     """
     Response object for listing Models.
     """
 
     model_endpoints: List[GetLLMEndpointResponse] = Field(
         ...,
-        description="The list of LLM endpoints.",
+        description="The list of models.",
     )
     """
     A list of Models, represented as `GetLLMEndpointResponse`s.
     """
 
 
 class DeleteLLMEndpointResponse(BaseModel):
@@ -189,17 +215,14 @@
 
     deleted: bool = Field(..., description="Whether deletion was successful.")
     """
     Whether the deletion succeeded.
     """
 
 
-# Update uses the default LLMEngine endpoint APIs.
-
-
 class CompletionSyncV1Request(BaseModel):
     """
     Request object for a synchronous prompt completion task.
     """
 
     prompt: str = Field(..., min_length=1)
     max_new_tokens: int = Field(..., gt=0)
@@ -214,15 +237,15 @@
     text: str
     """The text of the completion."""
 
     num_completion_tokens: int
     """Number of tokens in the completion."""
 
 
-class CompletionSyncV1Response(BaseModel):
+class CompletionSyncResponse(BaseModel):
     """
     Response object for a synchronous prompt completion.
     """
 
     request_id: str
     """Unique ID of request."""
 
@@ -247,15 +270,15 @@
     finished: bool
     """Whether the completion is finished."""
 
     num_completion_tokens: Optional[int] = None
     """Number of tokens in the completion."""
 
 
-class CompletionStreamV1Response(BaseModel):
+class CompletionStreamResponse(BaseModel):
     """
     Response object for a stream prompt completion task.
     """
 
     request_id: str
     """Unique ID of request."""
 
@@ -350,7 +373,28 @@
     Response object for cancelling a FineTune.
     """
 
     success: bool = Field(..., description="Whether cancellation was successful.")
     """
     Whether the cancellation succeeded.
     """
+
+
+class LLMFineTuneEvent(BaseModel):
+    """
+    Response object one FineTune event.
+    """
+
+    timestamp: Optional[float] = Field(
+        description="Timestamp of the event.",
+        default=None,
+    )
+    message: str = Field(description="Message of the event.")
+    level: str = Field(description="Logging level of the event.")
+
+
+class GetFineTuneEventsResponse(BaseModel):
+    """
+    Response object for getting events for a FineTune.
+    """
+
+    events: List[LLMFineTuneEvent] = Field(..., description="List of fine-tuning events.")
```

### Comparing `scale_llm_engine-0.0.0b2/llmengine/errors.py` & `scale_llm_engine-0.0.0b3/llmengine/errors.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b2/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b3/llmengine/fine_tuning.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 from typing import Dict, Optional
 
 from llmengine.api_engine import DEFAULT_TIMEOUT, APIEngine
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CreateFineTuneRequest,
     CreateFineTuneResponse,
+    GetFineTuneEventsResponse,
     GetFineTuneResponse,
     ListFineTunesResponse,
 )
 
 
 class FineTune(APIEngine):
     """
     FineTune API. This API is used to fine-tune models.
 
-    Fine-tuning is a process where the LLM is further trained on a task-specific dataset, allowing the model to adjust its parameters to better align with the task at hand. Fine-tuning involves the supervised training phase, where prompt/response pairs are provided to optimize the performance of the LLM.
+    Fine-tuning is a process where the LLM is further trained on a task-specific dataset, allowing the model to adjust its parameters to better align with the task at hand. Fine-tuning is a supervised training phase, where prompt/response pairs are provided to optimize the performance of the LLM.
 
-    Scale LLMEngine provides APIs to create fine-tunes on a base-model with training & validation data-sets. APIs are also provided to get, list and cancel fine-tuning jobs.and cancel fine-tuning jobs.
+    LLM Engine provides APIs to create fine-tunes on a base model with training & validation datasets. APIs are also provided to list, cancel and retrieve fine-tuning jobs.
 
     Creating a fine-tune will end with the creation of a Model, which you can view using `Model.get(model_name)` or delete using `Model.delete(model_name)`.
     """
 
     @classmethod
     def create(
         cls,
@@ -29,42 +30,52 @@
         validation_file: Optional[str] = None,
         hyperparameters: Optional[Dict[str, str]] = None,
         suffix: Optional[str] = None,
     ) -> CreateFineTuneResponse:
         """
         Creates a job that fine-tunes a specified model from a given dataset.
 
+        This API can be used to fine-tune a model. The _model_ is the name of base model
+        ([Model Zoo](../../model_zoo) for available models) to fine-tune. The training
+        file should consist of prompt and response pairs. Your data must be formatted as a CSV file
+        that includes two columns: `prompt` and `response`. A maximum of 100,000 rows of data is
+        currently supported. At least 200 rows of data is recommended to start to see benefits from
+        fine-tuning.
+
         Args:
             model (`str`):
                 The name of the base model to fine-tune. See [Model Zoo](../../model_zoo) for the list of available models to fine-tune.
 
             training_file (`str`):
-                Path to file of training dataset
+                Publicly accessible URL to a CSV file for training.
 
             validation_file (`Optional[str]`):
-                Path to file of validation dataset
+                Publicly accessible URL to a CSV file for validation.
+
+            hyperparameters (`Optional[Dict[str, str]]`):
+                A dict of hyperparameters to customize fine-tuning behavior.
+
+                Currently supported hyperparameters:
 
-            hyperparameters (`str`):
-                Hyperparameters
+                * `lr`: Peak learning rate used during fine-tuning. It decays with a cosine schedule afterward. (Default: 2e-5)
+                * `warmup_ratio`: Ratio of training steps used for learning rate warmup. (Default: 0.03)
+                * `epochs`: Number of fine-tuning epochs. (Default: 5)
+                * `weight_decay`: Regularization penalty applied to learned weights. (Default: 0.001)
+                * `max_seq_length`: Maximum number of tokens per sequence in the dataset. (Default: 1024)
 
             suffix (`Optional[str]`):
                 A string that will be added to your fine-tuned model name.
 
         Returns:
             CreateFineTuneResponse: an object that contains the ID of the created fine-tuning job
 
-        The _model_ is the name of base model ([Model Zoo](../../model_zoo) for available models) to fine. The training
-        file should consist of prompt and response pairs. Your data must be formatted as a CSV file
-        that includes two columns: `prompt` and `response`. A maximum of 100,000 rows of data is
-        currently supported. At least 200 rows of data is recommended to start to see benefits from
-        fine-tuning.
-
         Here is an example script to create a 5-row CSV of properly formatted data for fine-tuning
         an airline question answering bot:
 
+        === "Formatting data in python"
         ```python
         import csv
 
         # Define data
         data = [
           ("What is your policy on carry-on luggage?", "Our policy allows each passenger to bring one piece of carry-on luggage and one personal item such as a purse or briefcase. The maximum size for carry-on luggage is 22 x 14 x 9 inches."),
           ("How can I change my flight?", "You can change your flight through our website or mobile app. Go to 'Manage my booking' section, enter your booking reference and last name, then follow the prompts to change your flight."),
@@ -77,26 +88,27 @@
         with open('customer_service_data.csv', 'w', newline='') as file:
             writer = csv.writer(file)
             writer.writerow(["prompt", "response"])
             writer.writerows(data)
         ```
 
         Example code for fine-tuning:
+        === "Fine-tuning in python"
             ```python
             from llmengine import FineTune
 
             response = FineTune.create(
                 model="llama-7b",
-                training_file="s3://my-bucket/path/to/training-file.csv",
+                training_file="https://my-bucket.s3.us-west-2.amazonaws.com/path/to/training-file.csv",
             )
 
             print(response.json())
             ```
 
-        JSON Response:
+        === "Response in json"
             ```json
             {
                 "fine_tune_id": "ft_abc123"
             }
             ```
 
         """
@@ -116,68 +128,79 @@
 
     @classmethod
     def get(
         cls,
         fine_tune_id: str,
     ) -> GetFineTuneResponse:
         """
-        Get status of a fine-tuning job
+        Get status of a fine-tuning job.
+
+        This API can be used to get the status of an already running
+        fine-tuning job. It takes as a single parameter the `fine_tune_id`
+        and returns a
+        [GetFineTuneResponse](../../api/data_types/#llmengine.GetFineTuneResponse)
+        object with the id and status (`PENDING`, `STARTED`,
+        `UNDEFINED`, `FAILURE` or `SUCCESS`).
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
             GetFineTuneResponse: an object that contains the ID and status of the requested job
 
-        Example:
+        === "Getting status of fine-tuning in python"
             ```python
             from llmengine import FineTune
 
             response = FineTune.get(
                 fine_tune_id="ft_abc123",
             )
 
             print(response.json())
             ```
 
-        JSON Response:
+        === "Response in json"
             ```json
             {
                 "fine_tune_id": "ft_abc123",
-                "status": "RUNNING"
+                "status": "STARTED"
             }
             ```
         """
         response = cls._get(f"v1/llm/fine-tunes/{fine_tune_id}", timeout=DEFAULT_TIMEOUT)
         return GetFineTuneResponse.parse_obj(response)
 
     @classmethod
     def list(cls) -> ListFineTunesResponse:
         """
-        List fine-tuning jobs
+        List fine-tuning jobs.
+
+        This API can be used to list all the fine-tuning jobs.
+        It returns a list of pairs of `fine_tune_id` and `status` for
+        all existing jobs.
 
         Returns:
             ListFineTunesResponse: an object that contains a list of all fine-tuning jobs and their statuses
 
-        Example:
+        === "Listing fine-tuning jobs in python"
             ```python
             from llmengine import FineTune
 
             response = FineTune.list()
             print(response.json())
             ```
 
-        JSON Response:
+        === "Response in json"
             ```json
             {
                 "jobs": [
                     {
                         "fine_tune_id": "ft_abc123",
-                        "status": "RUNNING"
+                        "status": "STARTED"
                     },
                     {
                         "fine_tune_id": "ft_def456",
                         "status": "SUCCESS"
                     }
                 ]
             }
@@ -185,37 +208,92 @@
         """
         response = cls._get("v1/llm/fine-tunes", timeout=DEFAULT_TIMEOUT)
         return ListFineTunesResponse.parse_obj(response)
 
     @classmethod
     def cancel(cls, fine_tune_id: str) -> CancelFineTuneResponse:
         """
-        Cancel a fine-tuning job
+        Cancel a fine-tuning job.
+
+        This API can be used to cancel an existing fine-tuning job if
+        it's no longer required. It takes as parameter the `fine_tune_id`
+        and returns a response object which has a `success` field
+        confirming if the cancellation was successful.
 
         Args:
             fine_tune_id (`str`):
                 ID of the fine-tuning job
 
         Returns:
             CancelFineTuneResponse: an object that contains whether the cancellation was successful
 
-        Example:
+        === "Cancelling fine-tuning job in python"
             ```python
             from llmengine import FineTune
 
             response = FineTune.cancel(fine_tune_id="ft_abc123")
             print(response.json())
             ```
 
-        JSON Response:
+        === "Response in json"
             ```json
             {
                 "success": true
             }
             ```
         """
         response = cls.put(
             f"v1/llm/fine-tunes/{fine_tune_id}/cancel",
             data=None,
             timeout=DEFAULT_TIMEOUT,
         )
         return CancelFineTuneResponse.parse_obj(response)
+
+    @classmethod
+    def get_events(cls, fine_tune_id: str) -> GetFineTuneEventsResponse:
+        """
+        Get events of a fine-tuning job.
+
+        This API can be used to get the list of events for a fine-tuning job.
+        It takes as parameter the `fine_tune_id` and returns a response object
+        which has a list of events that has happened for the fine-tuning job.
+
+        Args:
+            fine_tune_id (`str`):
+                ID of the fine-tuning job
+
+        Returns:
+            GetFineTuneEventsResponse: an object that contains the list of events for the fine-tuning job
+
+        Example:
+            ```python
+            from llmengine import FineTune
+
+            response = FineTune.get_events(fine_tune_id="ft_abc123")
+            print(response.json())
+            ```
+
+        JSON Response:
+            ```json
+            {
+                [
+                    {
+                        "timestamp": 1689644480.0,
+                        "message": "Fine-tune job created",
+                        "level": "INFO"
+                    }
+                ],
+                [
+                    {
+                        "timestamp": 1689645480.0,
+                        "message": "Fine-tune job finished",
+                        "level": "INFO"
+                    }
+                ]
+            }
+            ```
+        """
+        response = cls._get(
+            f"v1/llm/fine-tunes/{fine_tune_id}/events",
+            timeout=DEFAULT_TIMEOUT,
+        )
+        return GetFineTuneEventsResponse.parse_obj(response)
```

### Comparing `scale_llm_engine-0.0.0b2/pyproject.toml` & `scale_llm_engine-0.0.0b3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta2"
+version = "0.0.0.beta3"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b2/PKG-INFO` & `scale_llm_engine-0.0.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b2
+Version: 0.0.0b3
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
```

