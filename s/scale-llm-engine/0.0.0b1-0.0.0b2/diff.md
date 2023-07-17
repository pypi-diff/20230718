# Comparing `tmp/scale_llm_engine-0.0.0b1.tar.gz` & `tmp/scale_llm_engine-0.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b1.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b2.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b1.tar` & `scale_llm_engine-0.0.0b2.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1006 2023-07-16 19:49:15.428915 scale_llm_engine-0.0.0b1/README.md
--rw-r--r--   0        0        0     1434 2023-07-16 22:32:20.465394 scale_llm_engine-0.0.0b1/llmengine/__init__.py
--rw-r--r--   0        0        0     5716 2023-07-16 21:02:55.721851 scale_llm_engine-0.0.0b1/llmengine/api_engine.py
--rw-r--r--   0        0        0    17749 2023-07-16 21:37:09.852272 scale_llm_engine-0.0.0b1/llmengine/client.py
--rw-r--r--   0        0        0     9561 2023-07-16 21:37:09.852593 scale_llm_engine-0.0.0b1/llmengine/completion.py
--rw-r--r--   0        0        0     8506 2023-07-16 21:37:09.852948 scale_llm_engine-0.0.0b1/llmengine/data_types.py
--rw-r--r--   0        0        0     2745 2023-07-16 19:49:15.429730 scale_llm_engine-0.0.0b1/llmengine/errors.py
--rw-r--r--   0        0        0     4179 2023-07-16 21:37:09.853211 scale_llm_engine-0.0.0b1/llmengine/fine_tuning.py
--rw-r--r--   0        0        0     2083 2023-07-16 19:49:15.429911 scale_llm_engine-0.0.0b1/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-07-16 22:32:20.462460 scale_llm_engine-0.0.0b1/pyproject.toml
--rw-r--r--   0        0        0     1903 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0     1001 2023-07-17 21:24:00.034378 scale_llm_engine-0.0.0b2/README.md
+-rw-r--r--   0        0        0     1584 2023-07-17 22:16:53.234768 scale_llm_engine-0.0.0b2/llmengine/__init__.py
+-rw-r--r--   0        0        0     6190 2023-07-17 21:57:41.640716 scale_llm_engine-0.0.0b2/llmengine/api_engine.py
+-rw-r--r--   0        0        0    11436 2023-07-17 22:13:22.416895 scale_llm_engine-0.0.0b2/llmengine/completion.py
+-rw-r--r--   0        0        0    10146 2023-07-17 22:13:22.418064 scale_llm_engine-0.0.0b2/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-17 10:30:37.104747 scale_llm_engine-0.0.0b2/llmengine/errors.py
+-rw-r--r--   0        0        0     7795 2023-07-17 21:57:41.642849 scale_llm_engine-0.0.0b2/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0     5391 2023-07-17 21:57:41.643669 scale_llm_engine-0.0.0b2/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-07-17 22:16:53.235607 scale_llm_engine-0.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1898 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b2/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b1/README.md` & `scale_llm_engine-0.0.0b2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 `LLM_ENGINE_SERVE_BASE_PATH` environment variable to the base URL of your
 self-hosted `llmengine` endpoint.
 
 ```python
 from llmengine import Completion
 
 response = Completion.create(
-    model_name="llama-7b",
+    model="llama-7b",
     prompt="Hello, my name is",
     max_new_tokens=10,
     temperature=0.2,
 )
 print(response.outputs[0].text)
 ```
```

### Comparing `scale_llm_engine-0.0.0b1/llmengine/__init__.py` & `scale_llm_engine-0.0.0b2/llmengine/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,42 +8,46 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.beta1"
+__version__ = "0.0.0.beta2"
 
 from typing import Sequence
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CompletionOutput,
     CompletionStreamOutput,
     CompletionStreamV1Response,
     CompletionSyncV1Response,
     CreateFineTuneRequest,
     CreateFineTuneResponse,
+    DeleteLLMEndpointResponse,
     GetFineTuneResponse,
+    GetLLMEndpointResponse,
     ListFineTunesResponse,
-    TaskStatus,
+    ListLLMEndpointsResponse,
 )
 from llmengine.fine_tuning import FineTune
 from llmengine.model import Model
 
 __all__: Sequence[str] = (
     "CancelFineTuneResponse",
     "Completion",
     "CompletionOutput",
     "CompletionStreamOutput",
     "CompletionStreamV1Response",
     "CompletionSyncV1Response",
     "CreateFineTuneRequest",
     "CreateFineTuneResponse",
+    "DeleteLLMEndpointResponse",
     "FineTune",
     "GetFineTuneResponse",
+    "GetLLMEndpointResponse",
     "ListFineTunesResponse",
+    "ListLLMEndpointsResponse",
     "Model",
-    "TaskStatus",
 )
```

### Comparing `scale_llm_engine-0.0.0b1/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b2/llmengine/api_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def validate_api_key(cls):
         if SPELLBOOK_API_URL == LLM_ENGINE_BASE_PATH and not SCALE_API_KEY:
             raise ValueError(
                 "You must set SCALE_API_KEY in your environment to to use the LLM Engine API."
             )
 
     @classmethod
-    def get(cls, resource_name: str, timeout: int) -> Dict[str, Any]:
+    def _get(cls, resource_name: str, timeout: int) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.get(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             timeout=timeout,
             headers={"x-api-key": api_key},
         )
         if response.status_code != 200:
@@ -61,14 +61,27 @@
             timeout=timeout,
             headers={"x-api-key": api_key},
         )
         if response.status_code != 200:
             raise parse_error(response.status_code, response.content)
         payload = response.json()
         return payload
+
+    @classmethod
+    def _delete(cls, resource_name: str, timeout: int) -> Dict[str, Any]:
+        api_key = get_api_key()
+        response = requests.delete(
+            os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
+            timeout=timeout,
+            headers={"x-api-key": api_key},
+        )
+        if response.status_code != 200:
+            raise parse_error(response.status_code, response.content)
+        payload = response.json()
+        return payload
 
     @classmethod
     def post_sync(cls, resource_name: str, data: Dict[str, Any], timeout: int) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.post(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             json=data,
```

### Comparing `scale_llm_engine-0.0.0b1/llmengine/data_types.py` & `scale_llm_engine-0.0.0b2/llmengine/data_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 CpuSpecificationType = Union[str, int, float]
 StorageSpecificationType = Union[str, int, float]  # TODO(phil): we can make this more specific.
 
 
 class LLMInferenceFramework(str, Enum):
     DEEPSPEED = "deepspeed"
+    TEXT_GENERATION_INFERENCE = "text_generation_inference"
 
 
 class LLMSource(str, Enum):
     HUGGING_FACE = "hugging_face"
 
 
 class GpuType(str, Enum):
@@ -104,23 +105,15 @@
     last_updated_at: datetime.datetime
     deployment_state: Optional[ModelEndpointDeploymentState] = Field(default=None)
     resource_state: Optional[ModelEndpointResourceState] = Field(default=None)
     num_queued_items: Optional[int] = Field(default=None)
     public_inference: Optional[bool] = Field(default=None)
 
 
-class TaskStatus(str, Enum):
-    PENDING = "PENDING"
-    STARTED = "STARTED"
-    SUCCESS = "SUCCESS"
-    FAILURE = "FAILURE"
-    UNDEFINED = "UNDEFINED"
-
-
-class CreateLLMModelEndpointV1Request(BaseModel):
+class CreateLLMEndpointRequest(BaseModel):
     name: str
 
     # LLM specific fields
     model_name: str
     source: LLMSource = LLMSource.HUGGING_FACE
     inference_framework: LLMInferenceFramework = LLMInferenceFramework.DEEPSPEED
     inference_framework_image_tag: str
@@ -146,144 +139,218 @@
     prewarm: Optional[bool]
     high_priority: Optional[bool]
     default_callback_url: Optional[HttpUrl]
     default_callback_auth: Optional[CallbackAuth]
     public_inference: Optional[bool] = True  # LLM endpoints are public by default.
 
 
-class CreateLLMModelEndpointV1Response(BaseModel):
+class CreateLLMEndpointResponse(BaseModel):
     endpoint_creation_task_id: str
 
 
-class GetLLMModelEndpointV1Response(BaseModel):
-    id: str
+class GetLLMEndpointResponse(BaseModel):
     """
-    The autogenerated ID of the LLMEngine endpoint.
+    Response object for retrieving a Model.
     """
 
-    name: str
-    model_name: str
-    source: LLMSource
-    inference_framework: LLMInferenceFramework
-    inference_framework_image_tag: str
-    num_shards: int
-    spec: GetModelEndpointV1Response
+    id: str = Field(description="The autogenerated ID of the Launch endpoint.")
+    """The autogenerated ID of the Launch endpoint."""
+    name: str = Field(description="The name of the Launch endpoint.")
+    """The name of the Launch endpoint."""
+    model_name: str = Field(description="The name of the model.")
+    """The name of the model."""
+    source: LLMSource = Field(description="The source of the model.")
+    """The source of the model."""
+    inference_framework: LLMInferenceFramework = Field(
+        description="The inference framework used by the endpoint."
+    )
+    """The inference framework used by the endpoint."""
+    num_shards: int = Field(description="The number of shards.")
+    """The number of shards."""
 
 
-class ListLLMModelEndpointsV1Response(BaseModel):
-    model_endpoints: List[GetLLMModelEndpointV1Response]
+class ListLLMEndpointsResponse(BaseModel):
+    """
+    Response object for listing Models.
+    """
 
+    model_endpoints: List[GetLLMEndpointResponse] = Field(
+        ...,
+        description="The list of LLM endpoints.",
+    )
+    """
+    A list of Models, represented as `GetLLMEndpointResponse`s.
+    """
 
-# Delete and update use the default LLMEngine endpoint APIs.
+
+class DeleteLLMEndpointResponse(BaseModel):
+    """
+    Response object for deleting a Model.
+    """
+
+    deleted: bool = Field(..., description="Whether deletion was successful.")
+    """
+    Whether the deletion succeeded.
+    """
+
+
+# Update uses the default LLMEngine endpoint APIs.
 
 
 class CompletionSyncV1Request(BaseModel):
     """
     Request object for a synchronous prompt completion task.
     """
 
-    prompts: List[str] = Field(..., min_items=1)
+    prompt: str = Field(..., min_length=1)
     max_new_tokens: int = Field(..., gt=0)
     temperature: float = Field(..., gt=0.0)
 
 
 class CompletionOutput(BaseModel):
-    text: str
-    """Text"""
+    """
+    Represents the output of a completion request to a model.
+    """
 
-    num_prompt_tokens: Optional[int]
-    """Number of tokens in the prompt."""
+    text: str
+    """The text of the completion."""
 
     num_completion_tokens: int
     """Number of tokens in the completion."""
 
 
 class CompletionSyncV1Response(BaseModel):
     """
-    Response object for a synchronous prompt completion task.
+    Response object for a synchronous prompt completion.
     """
 
-    status: TaskStatus
-    """Task status."""
+    request_id: str
+    """Unique ID of request."""
 
-    outputs: List[CompletionOutput]
-    """List of completion outputs."""
-
-    traceback: Optional[str] = None
-    """Traceback if the task failed."""
+    output: CompletionOutput
+    """Completion output."""
 
 
 class CompletionStreamV1Request(BaseModel):
     """
-    Request object for a stream prompt completion task.
+    Request object for a streaming prompt completion.
     """
 
     prompt: str = Field(..., min_length=1)
     max_new_tokens: int = Field(..., gt=0)
     temperature: float = Field(..., gt=0.0)
 
 
 class CompletionStreamOutput(BaseModel):
     text: str
-    """Text"""
+    """The text of the completion."""
 
     finished: bool
     """Whether the completion is finished."""
 
-    num_prompt_tokens: Optional[int] = None
-    """Number of tokens in the prompt."""
-
     num_completion_tokens: Optional[int] = None
     """Number of tokens in the completion."""
 
 
 class CompletionStreamV1Response(BaseModel):
     """
     Response object for a stream prompt completion task.
     """
 
-    status: TaskStatus
-    """Task status."""
+    request_id: str
+    """Unique ID of request."""
 
     output: Optional[CompletionStreamOutput] = None
     """Completion output."""
 
-    traceback: Optional[str] = None
-    """Traceback if the task failed."""
-
-
-# everything below copied from scaleapi/packages/spellbook-backend/server/spellbook_server/dtos.py
-
 
 class CreateFineTuneRequest(BaseModel):
+    """
+    Request object for creating a FineTune.
+    """
+
     model: str = Field(..., description="Identifier of base model to train from.")
-    training_file: str = Field(..., description="Path to file of training dataset. Dataset must be a csv with columns 'prompt' and 'response'.")
-    validation_file: Optional[str] = Field(default=None, description="Path to file of validation dataset. Has the same format as training_file. If not provided, we will generate a split from the training dataset.")
-    hyperparameters: Optional[Dict[str, Any]] = Field(default=None, description="Hyperparameters to pass in to training job.")
-    suffix: Optional[str] = Field(default=None, description="Optional user-provided identifier suffix for the fine-tuned model.")
+    """Identifier of base model to train from."""
+
+    training_file: str = Field(
+        ...,
+        description="Path to file of training dataset. Dataset must be a csv with columns 'prompt' and 'response'.",
+    )
+    """Path to file of training dataset. Dataset must be a csv with columns 'prompt' and 'response'."""
+
+    validation_file: Optional[str] = Field(
+        default=None,
+        description="Path to file of validation dataset. Has the same format as training_file. If not provided, we will generate a split from the training dataset.",
+    )
+    """Path to file of validation dataset. Has the same format as training_file. If not provided, we will generate a split from the training dataset."""
+
+    hyperparameters: Optional[Dict[str, Any]] = Field(
+        default=None, description="Hyperparameters to pass in to training job."
+    )
+    """Hyperparameters to pass in to training job."""
+
+    suffix: Optional[str] = Field(
+        default=None,
+        description="Optional user-provided identifier suffix for the fine-tuned model.",
+    )
+    """Optional user-provided identifier suffix for the fine-tuned model."""
 
 
 class CreateFineTuneResponse(BaseModel):
+    """
+    Response object for creating a FineTune.
+    """
+
     fine_tune_id: str = Field(..., description="ID of the created fine-tuning job.")
+    """
+    The ID of the FineTune.
+    """
 
 
 class BatchJobStatus(str, Enum):
     PENDING = "PENDING"
     RUNNING = "RUNNING"
     SUCCESS = "SUCCESS"
     FAILURE = "FAILURE"
     CANCELLED = "CANCELLED"
     UNDEFINED = "UNDEFINED"
     TIMEOUT = "TIMEOUT"
 
 
 class GetFineTuneResponse(BaseModel):
+    """
+    Response object for retrieving a FineTune.
+    """
+
     fine_tune_id: str = Field(..., description="ID of the requested job.")
+    """
+    The ID of the FineTune.
+    """
+
     status: BatchJobStatus = Field(..., description="Status of the requested job.")
+    """
+    The status of the FineTune job.
+    """
 
 
 class ListFineTunesResponse(BaseModel):
-    jobs: List[GetFineTuneResponse] = Field(..., description="List of fine-tuning jobs and their statuses.")
+    """
+    Response object for listing FineTunes.
+    """
+
+    jobs: List[GetFineTuneResponse] = Field(
+        ..., description="List of fine-tuning jobs and their statuses."
+    )
+    """
+    A list of FineTunes, represented as `GetFineTuneResponse`s.
+    """
 
 
 class CancelFineTuneResponse(BaseModel):
+    """
+    Response object for cancelling a FineTune.
+    """
+
     success: bool = Field(..., description="Whether cancellation was successful.")
+    """
+    Whether the cancellation succeeded.
+    """
```

### Comparing `scale_llm_engine-0.0.0b1/llmengine/errors.py` & `scale_llm_engine-0.0.0b2/llmengine/errors.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b1/pyproject.toml` & `scale_llm_engine-0.0.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta1"
+version = "0.0.0.beta2"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b1/PKG-INFO` & `scale_llm_engine-0.0.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b1
+Version: 0.0.0b2
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
@@ -46,15 +46,15 @@
 `LLM_ENGINE_SERVE_BASE_PATH` environment variable to the base URL of your
 self-hosted `llmengine` endpoint.
 
 ```python
 from llmengine import Completion
 
 response = Completion.create(
-    model_name="llama-7b",
+    model="llama-7b",
     prompt="Hello, my name is",
     max_new_tokens=10,
     temperature=0.2,
 )
 print(response.outputs[0].text)
 ```
```

