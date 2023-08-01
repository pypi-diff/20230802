# Comparing `tmp/scale_llm_engine-0.0.0b7.tar.gz` & `tmp/scale_llm_engine-0.0.0b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scale_llm_engine-0.0.0b7.tar", max compression
+gzip compressed data, was "scale_llm_engine-0.0.0b8.tar", max compression
```

## Comparing `scale_llm_engine-0.0.0b7.tar` & `scale_llm_engine-0.0.0b8.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0     1002 2023-07-21 08:53:27.233160 scale_llm_engine-0.0.0b7/README.md
--rw-r--r--   0        0        0     1576 2023-07-26 17:20:58.423387 scale_llm_engine-0.0.0b7/llmengine/__init__.py
--rw-r--r--   0        0        0     6201 2023-07-26 17:19:44.533261 scale_llm_engine-0.0.0b7/llmengine/api_engine.py
--rw-r--r--   0        0        0    13065 2023-07-21 08:53:27.234217 scale_llm_engine-0.0.0b7/llmengine/completion.py
--rw-r--r--   0        0        0    13437 2023-07-26 17:19:44.533815 scale_llm_engine-0.0.0b7/llmengine/data_types.py
--rw-r--r--   0        0        0     2745 2023-07-18 18:23:40.550782 scale_llm_engine-0.0.0b7/llmengine/errors.py
--rw-r--r--   0        0        0    14021 2023-07-21 08:53:27.235057 scale_llm_engine-0.0.0b7/llmengine/fine_tuning.py
--rw-r--r--   0        0        0    13738 2023-07-21 08:53:27.235405 scale_llm_engine-0.0.0b7/llmengine/model.py
--rw-r--r--   0        0        0      807 2023-07-26 17:20:58.407050 scale_llm_engine-0.0.0b7/pyproject.toml
--rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b7/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-07-21 08:53:27.233160 scale_llm_engine-0.0.0b8/README.md
+-rw-r--r--   0        0        0     1870 2023-08-01 18:32:34.086159 scale_llm_engine-0.0.0b8/llmengine/__init__.py
+-rw-r--r--   0        0        0     7065 2023-08-01 23:09:51.651675 scale_llm_engine-0.0.0b8/llmengine/api_engine.py
+-rw-r--r--   0        0        0    13065 2023-07-21 08:53:27.234217 scale_llm_engine-0.0.0b8/llmengine/completion.py
+-rw-r--r--   0        0        0    15229 2023-08-01 18:32:34.087511 scale_llm_engine-0.0.0b8/llmengine/data_types.py
+-rw-r--r--   0        0        0     2745 2023-07-18 18:23:40.550782 scale_llm_engine-0.0.0b8/llmengine/errors.py
+-rw-r--r--   0        0        0     5290 2023-08-01 18:32:34.088194 scale_llm_engine-0.0.0b8/llmengine/file.py
+-rw-r--r--   0        0        0    14021 2023-07-21 08:53:27.235057 scale_llm_engine-0.0.0b8/llmengine/fine_tuning.py
+-rw-r--r--   0        0        0    14588 2023-07-31 19:50:25.084434 scale_llm_engine-0.0.0b8/llmengine/model.py
+-rw-r--r--   0        0        0      807 2023-08-01 18:32:34.088861 scale_llm_engine-0.0.0b8/pyproject.toml
+-rw-r--r--   0        0        0     1899 1970-01-01 00:00:00.000000 scale_llm_engine-0.0.0b8/PKG-INFO
```

### Comparing `scale_llm_engine-0.0.0b7/README.md` & `scale_llm_engine-0.0.0b8/README.md`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b7/llmengine/__init__.py` & `scale_llm_engine-0.0.0b8/llmengine/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,46 +8,58 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.0.0.beta7"
+__version__ = "0.0.0.beta8"
 
 from typing import Sequence
 
 from llmengine.completion import Completion
 from llmengine.data_types import (
     CancelFineTuneResponse,
     CompletionOutput,
     CompletionStreamOutput,
     CompletionStreamResponse,
     CompletionSyncResponse,
     CreateFineTuneRequest,
     CreateFineTuneResponse,
+    DeleteFileResponse,
     DeleteLLMEndpointResponse,
+    GetFileContentResponse,
+    GetFileResponse,
     GetFineTuneResponse,
     GetLLMEndpointResponse,
+    ListFilesResponse,
     ListFineTunesResponse,
     ListLLMEndpointsResponse,
+    UploadFileResponse,
 )
+from llmengine.file import File
 from llmengine.fine_tuning import FineTune
 from llmengine.model import Model
 
 __all__: Sequence[str] = (
     "CancelFineTuneResponse",
     "Completion",
     "CompletionOutput",
     "CompletionStreamOutput",
     "CompletionStreamResponse",
     "CompletionSyncResponse",
     "CreateFineTuneRequest",
     "CreateFineTuneResponse",
+    "DeleteFileResponse",
     "DeleteLLMEndpointResponse",
+    "GetFileContentResponse",
+    "File",
     "FineTune",
+    "GetFileResponse",
     "GetFineTuneResponse",
     "GetLLMEndpointResponse",
+    "ListFilesResponse",
     "ListFineTunesResponse",
     "ListLLMEndpointsResponse",
     "Model",
+    "UploadFileResponse",
 )
```

### Comparing `scale_llm_engine-0.0.0b7/llmengine/api_engine.py` & `scale_llm_engine-0.0.0b8/llmengine/api_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 # NOTICE - per Apache 2.0 license:
 # This file was copied and modified from the OpenAI Python client library: https://github.com/openai/openai-python
 import json
 import os
 from functools import wraps
+from io import BufferedReader
 from typing import Any, AsyncIterable, Dict, Iterator, Optional
 
 import requests
 from aiohttp import ClientSession, ClientTimeout
 from llmengine.errors import parse_error
 
 SPELLBOOK_API_URL = "https://api.spellbook.scale.com/llm-engine"
 LLM_ENGINE_BASE_PATH = os.getenv("LLM_ENGINE_BASE_PATH", SPELLBOOK_API_URL)
 DEFAULT_TIMEOUT: int = 10
 
+api_key = None
+
+
+def set_api_key(key):
+    global api_key
+    api_key = key
+
 
 def get_api_key() -> str:
+    if api_key is not None:
+        return api_key
     env_api_key = os.getenv("SCALE_API_KEY")
     return env_api_key or "root"
 
 
 def assert_self_hosted(func):
     @wraps(func)
     def inner(*args, **kwargs):
@@ -40,14 +50,15 @@
     @classmethod
     def _get(cls, resource_name: str, timeout: int) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.get(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             timeout=timeout,
             headers={"x-api-key": api_key},
+            auth=(api_key, ""),
         )
         if response.status_code != 200:
             raise parse_error(response.status_code, response.content)
         payload = response.json()
         return payload
 
     @classmethod
@@ -56,41 +67,44 @@
     ) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.put(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             json=data,
             timeout=timeout,
             headers={"x-api-key": api_key},
+            auth=(api_key, ""),
         )
         if response.status_code != 200:
             raise parse_error(response.status_code, response.content)
         payload = response.json()
         return payload
 
     @classmethod
     def _delete(cls, resource_name: str, timeout: int) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.delete(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             timeout=timeout,
             headers={"x-api-key": api_key},
+            auth=(api_key, ""),
         )
         if response.status_code != 200:
             raise parse_error(response.status_code, response.content)
         payload = response.json()
         return payload
 
     @classmethod
     def post_sync(cls, resource_name: str, data: Dict[str, Any], timeout: int) -> Dict[str, Any]:
         api_key = get_api_key()
         response = requests.post(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             json=data,
             timeout=timeout,
             headers={"x-api-key": api_key},
+            auth=(api_key, ""),
         )
         if response.status_code != 200:
             raise parse_error(response.status_code, response.content)
         payload = response.json()
         return payload
 
     @classmethod
@@ -99,14 +113,15 @@
     ) -> Iterator[Dict[str, Any]]:
         api_key = get_api_key()
         response = requests.post(
             os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
             json=data,
             timeout=timeout,
             headers={"x-api-key": api_key},
+            auth=(api_key, ""),
             stream=True,
         )
         if response.status_code != 200:
             raise parse_error(response.status_code, response.content)
         for byte_payload in response.iter_lines():
             # Skip line
             if byte_payload == b"\n":
@@ -121,14 +136,30 @@
                 try:
                     payload_json = json.loads(payload_data)
                     yield payload_json
                 except json.JSONDecodeError:
                     raise ValueError(f"Invalid JSON payload: {payload_data}")
 
     @classmethod
+    def post_file(
+        cls, resource_name: str, files: Dict[str, BufferedReader], timeout: int
+    ) -> Dict[str, Any]:
+        api_key = get_api_key()
+        response = requests.post(
+            os.path.join(LLM_ENGINE_BASE_PATH, resource_name),
+            files=files,
+            timeout=timeout,
+            headers={"x-api-key": api_key},
+        )
+        if response.status_code != 200:
+            raise parse_error(response.status_code, response.content)
+        payload = response.json()
+        return payload
+
+    @classmethod
     async def apost_sync(
         cls, resource_name: str, data: Dict[str, Any], timeout: int
     ) -> Dict[str, Any]:
         api_key = get_api_key()
         async with ClientSession(
             timeout=ClientTimeout(timeout), headers={"x-api-key": api_key}
         ) as session:
```

### Comparing `scale_llm_engine-0.0.0b7/llmengine/completion.py` & `scale_llm_engine-0.0.0b8/llmengine/completion.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b7/llmengine/data_types.py` & `scale_llm_engine-0.0.0b8/llmengine/data_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 class GpuType(str, Enum):
     """Lists allowed GPU types for LLMEngine."""
 
     NVIDIA_TESLA_T4 = "nvidia-tesla-t4"
     NVIDIA_AMPERE_A10 = "nvidia-ampere-a10"
-    NVIDIA_AMPERE_A100 = "nvidia-a100"
+    NVIDIA_AMPERE_A100 = "nvidia-ampere-a100"
 
 
 class ModelEndpointType(str, Enum):
     ASYNC = "async"
     SYNC = "sync"
     STREAMING = "streaming"
 
@@ -127,40 +127,53 @@
 
 class CreateLLMEndpointRequest(BaseModel):
     name: str
 
     # LLM specific fields
     model_name: str
     source: LLMSource = LLMSource.HUGGING_FACE
-    inference_framework: LLMInferenceFramework = LLMInferenceFramework.DEEPSPEED
+    inference_framework: LLMInferenceFramework = LLMInferenceFramework.TEXT_GENERATION_INFERENCE
     inference_framework_image_tag: str
-    num_shards: int
+    num_shards: int = 1
     """
-    Number of shards to distribute the model onto GPUs.
+    Number of shards to distribute the model onto GPUs. Only affects behavior for text-generation-inference models
+    """
+
+    quantize: Optional[Quantization] = None
+    """
+    Quantization for the LLM. Only affects behavior for text-generation-inference models
+    """
+
+    checkpoint_path: Optional[str] = None
+    """
+    Path to the checkpoint to load the model from. Only affects behavior for text-generation-inference models
     """
 
     # General endpoint fields
     metadata: Dict[str, Any]  # TODO: JSON type
     post_inference_hooks: Optional[List[str]]
-    endpoint_type: ModelEndpointType = ModelEndpointType.SYNC
+    endpoint_type: ModelEndpointType = ModelEndpointType.STREAMING
     cpus: CpuSpecificationType
     gpus: int
     memory: StorageSpecificationType
     gpu_type: GpuType
     storage: Optional[StorageSpecificationType]
     optimize_costs: Optional[bool]
     min_workers: int
     max_workers: int
     per_worker: int
     labels: Dict[str, str]
     prewarm: Optional[bool]
     high_priority: Optional[bool]
     default_callback_url: Optional[HttpUrl]
     default_callback_auth: Optional[CallbackAuth]
-    public_inference: Optional[bool] = True  # LLM endpoints are public by default.
+    public_inference: Optional[bool] = True
+    """
+    Whether the endpoint can be used for inference for all users. LLM endpoints are public by default.
+    """
 
 
 class CreateLLMEndpointResponse(BaseModel):
     endpoint_creation_task_id: str
 
 
 class GetLLMEndpointResponse(BaseModel):
@@ -436,7 +449,51 @@
 
 class GetFineTuneEventsResponse(BaseModel):
     """
     Response object for getting events for a FineTune.
     """
 
     events: List[LLMFineTuneEvent] = Field(..., description="List of fine-tuning events.")
+
+
+class UploadFileResponse(BaseModel):
+    """Response object for uploading a file."""
+
+    id: str = Field(..., description="ID of the uploaded file.")
+    """ID of the uploaded file."""
+
+
+class GetFileResponse(BaseModel):
+    """Response object for retrieving a file."""
+
+    id: str = Field(..., description="ID of the requested file.")
+    """ID of the requested file."""
+
+    filename: str = Field(..., description="File name.")
+    """File name."""
+
+    size: int = Field(..., description="Length of the file, in characters.")
+    """Length of the file, in characters."""
+
+
+class ListFilesResponse(BaseModel):
+    """Response object for listing files."""
+
+    files: List[GetFileResponse] = Field(..., description="List of file IDs, names, and sizes.")
+    """List of file IDs, names, and sizes."""
+
+
+class DeleteFileResponse(BaseModel):
+    """Response object for deleting a file."""
+
+    deleted: bool = Field(..., description="Whether deletion was successful.")
+    """Whether deletion was successful."""
+
+
+class GetFileContentResponse(BaseModel):
+    """Response object for retrieving a file's content."""
+
+    id: str = Field(..., description="ID of the requested file.")
+    """ID of the requested file."""
+
+    content: str = Field(..., description="File content.")
+    """File content."""
```

### Comparing `scale_llm_engine-0.0.0b7/llmengine/errors.py` & `scale_llm_engine-0.0.0b8/llmengine/errors.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b7/llmengine/fine_tuning.py` & `scale_llm_engine-0.0.0b8/llmengine/fine_tuning.py`

 * *Files identical despite different names*

### Comparing `scale_llm_engine-0.0.0b7/llmengine/model.py` & `scale_llm_engine-0.0.0b8/llmengine/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     GetLLMEndpointResponse,
     GpuType,
     ListLLMEndpointsResponse,
     LLMInferenceFramework,
     LLMSource,
     ModelEndpointType,
     PostInferenceHooks,
+    Quantization,
 )
 
 
 class Model(APIEngine):
     """
     Model API. This API is used to get, list, and delete models. Models include both base
     models built into LLM Engine, and fine-tuned models that you create through the
@@ -24,20 +25,23 @@
     See [Model Zoo](../../model_zoo) for the list of publicly available base models.
     """
 
     @classmethod
     @assert_self_hosted
     def create(
         cls,
+        name: str,
         # LLM specific fields
         model: str,
         inference_framework_image_tag: str,
         source: LLMSource = LLMSource.HUGGING_FACE,
         inference_framework: LLMInferenceFramework = LLMInferenceFramework.TEXT_GENERATION_INFERENCE,
         num_shards: int = 4,
+        quantize: Optional[Quantization] = None,
+        checkpoint_path: Optional[str] = None,
         # General endpoint fields
         cpus: int = 32,
         memory: str = "192Gi",
         storage: str = "96Gi",
         gpus: int = 4,
         min_workers: int = 0,
         max_workers: int = 1,
@@ -49,29 +53,41 @@
         default_callback_url: Optional[str] = None,
         public_inference: Optional[bool] = True,
         labels: Optional[Dict[str, str]] = None,
     ) -> CreateLLMEndpointResponse:
         """
         Create an LLM model. Note: This feature is only available for self-hosted users.
         Args:
+            name (`str`):
+                Name of the endpoint
+
             model (`str`):
-                Name of the model
+                Name of the base model
 
             inference_framework_image_tag (`str`):
                 Image tag for the inference framework
 
             source (`LLMSource`):
                 Source of the LLM. Currently only HuggingFace is supported
 
             inference_framework (`LLMInferenceFramework`):
                 Inference framework for the LLM. Currently only DeepSpeed is supported
 
             num_shards (`int`):
                 Number of shards for the LLM. When bigger than 1, LLM will be sharded
                 to multiple GPUs. Number of GPUs must be larger than num_shards.
+                Only affects behavior for text-generation-inference models
+
+            quantize (`Optional[Quantization]`):
+                Quantization for the LLM. Only affects behavior for text-generation-inference models
+
+            checkpoint_path (`Optional[str]`):
+                Path to the checkpoint for the LLM. For now we only support loading a tar file from AWS S3.
+                Safetensors are preferred but PyTorch checkpoints are also accepted (model loading will be slower).
+                Only affects behavior for text-generation-inference models
 
             cpus (`int`):
                 Number of cpus each worker should get, e.g. 1, 2, etc. This must be greater
                 than or equal to 1
 
             memory (`str`):
                 Amount of memory each worker should get, e.g. "4Gi", "512Mi", etc. This must
@@ -153,20 +169,22 @@
             for hook in post_inference_hooks:
                 if isinstance(hook, PostInferenceHooks):
                     post_inference_hooks_strs.append(hook.value)
                 else:
                     post_inference_hooks_strs.append(hook)
 
         request = CreateLLMEndpointRequest(
-            name=model,
+            name=name,
             model_name=model,
             source=source,
             inference_framework=inference_framework,
             inference_framework_image_tag=inference_framework_image_tag,
             num_shards=num_shards,
+            quantize=quantize,
+            checkpoint_path=checkpoint_path,
             cpus=cpus,
             endpoint_type=ModelEndpointType(endpoint_type),
             gpus=gpus,
             gpu_type=GpuType(gpu_type) if gpu_type is not None else None,
             labels=labels or {},
             max_workers=max_workers,
             memory=memory,
```

### Comparing `scale_llm_engine-0.0.0b7/pyproject.toml` & `scale_llm_engine-0.0.0b8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scale-llm-engine"
-version = "0.0.0.beta7"
+version = "0.0.0.beta8"
 description = "Scale LLM Engine Python client"
 license = "Apache-2.0"
 authors = ["Phil Chen <phil.chen@scale.com>"]
 maintainers = ["Phil Chen <phil.chen@scale.com>"]
 readme = "README.md"
 homepage = "https://scaleapi.github.io/llm-engine/"
 repository = "https://github.com/scaleapi/llm-engine"
```

### Comparing `scale_llm_engine-0.0.0b7/PKG-INFO` & `scale_llm_engine-0.0.0b8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scale-llm-engine
-Version: 0.0.0b7
+Version: 0.0.0b8
 Summary: Scale LLM Engine Python client
 Home-page: https://scaleapi.github.io/llm-engine/
 License: Apache-2.0
 Author: Phil Chen
 Author-email: phil.chen@scale.com
 Maintainer: Phil Chen
 Maintainer-email: phil.chen@scale.com
```

