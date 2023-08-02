# Comparing `tmp/baseten-0.7.0.tar.gz` & `tmp/baseten-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baseten-0.7.0.tar", max compression
+gzip compressed data, was "baseten-0.8.0.tar", max compression
```

## Comparing `baseten-0.7.0.tar` & `baseten-0.8.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     5041 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/__init__.py
--rw-r--r--   0        0        0    12867 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/baseten_deployed_model.py
--rw-r--r--   0        0        0     5539 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/cli.py
--rw-r--r--   0        0        0      541 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/client_commands/baseten_cli.py
--rw-r--r--   0        0        0     1143 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/client_commands/dataset_cli.py
--rw-r--r--   0        0        0     5953 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/client_commands/finetuning_cli.py
--rw-r--r--   0        0        0     1088 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/client_commands/models_cli.py
--rw-r--r--   0        0        0      927 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/client_commands/pretrained_cli.py
--rw-r--r--   0        0        0        0 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/__init__.py
--rw-r--r--   0        0        0    29719 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/api.py
--rw-r--r--   0        0        0     2512 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/core.py
--rw-r--r--   0        0        0     1475 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/error_handler.py
--rw-r--r--   0        0        0     6576 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/files.py
--rw-r--r--   0        0        0     4292 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/lib_support.py
--rw-r--r--   0        0        0    17743 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/model_deployer.py
--rw-r--r--   0        0        0     2288 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/settings.py
--rw-r--r--   0        0        0     1787 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/tar.py
--rw-r--r--   0        0        0      907 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/types.py
--rw-r--r--   0        0        0     3413 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/common/util.py
--rw-r--r--   0        0        0      207 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/models/__init__.py
--rw-r--r--   0        0        0     7086 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/models/flan_t5.py
--rw-r--r--   0        0        0      284 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/models/foundational_model.py
--rw-r--r--   0        0        0     5130 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/models/llama.py
--rw-r--r--   0        0        0    13478 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/models/stable_diffusion.py
--rw-r--r--   0        0        0     4878 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/models/util.py
--rw-r--r--   0        0        0     3481 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/models/whisper.py
--rw-r--r--   0        0        0      389 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/training/__init__.py
--rw-r--r--   0        0        0     2852 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/training/datasets.py
--rw-r--r--   0        0        0    33964 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/training/finetuning.py
--rw-r--r--   0        0        0     6681 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/training/logs.py
--rw-r--r--   0        0        0      479 2023-08-01 14:15:37.152288 baseten-0.7.0/baseten/training/utils.py
--rw-r--r--   0        0        0      763 2023-08-01 14:15:37.160288 baseten-0.7.0/pypi_readme.md
--rw-r--r--   0        0        0     1961 2023-08-01 14:16:38.224750 baseten-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 baseten-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     5041 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/__init__.py
+-rw-r--r--   0        0        0    11700 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/baseten_deployed_model.py
+-rw-r--r--   0        0        0     5539 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/cli.py
+-rw-r--r--   0        0        0      541 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/client_commands/baseten_cli.py
+-rw-r--r--   0        0        0     1143 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/client_commands/dataset_cli.py
+-rw-r--r--   0        0        0     5953 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/client_commands/finetuning_cli.py
+-rw-r--r--   0        0        0     1088 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/client_commands/models_cli.py
+-rw-r--r--   0        0        0      927 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/client_commands/pretrained_cli.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/common/__init__.py
+-rw-r--r--   0        0        0    28950 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/common/api.py
+-rw-r--r--   0        0        0     2512 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/common/core.py
+-rw-r--r--   0        0        0     1475 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/common/error_handler.py
+-rw-r--r--   0        0        0     6576 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/common/files.py
+-rw-r--r--   0        0        0     4292 2023-08-02 16:17:49.800257 baseten-0.8.0/baseten/common/lib_support.py
+-rw-r--r--   0        0        0    17743 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/common/model_deployer.py
+-rw-r--r--   0        0        0     2288 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/common/settings.py
+-rw-r--r--   0        0        0     1787 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/common/tar.py
+-rw-r--r--   0        0        0      907 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/common/types.py
+-rw-r--r--   0        0        0     3413 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/common/util.py
+-rw-r--r--   0        0        0      207 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/models/__init__.py
+-rw-r--r--   0        0        0     7086 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/models/flan_t5.py
+-rw-r--r--   0        0        0      284 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/models/foundational_model.py
+-rw-r--r--   0        0        0     5130 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/models/llama.py
+-rw-r--r--   0        0        0    13478 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/models/stable_diffusion.py
+-rw-r--r--   0        0        0     4878 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/models/util.py
+-rw-r--r--   0        0        0     3481 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/models/whisper.py
+-rw-r--r--   0        0        0      389 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/training/__init__.py
+-rw-r--r--   0        0        0     2852 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/training/datasets.py
+-rw-r--r--   0        0        0    33964 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/training/finetuning.py
+-rw-r--r--   0        0        0     6681 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/training/logs.py
+-rw-r--r--   0        0        0      479 2023-08-02 16:17:49.804257 baseten-0.8.0/baseten/training/utils.py
+-rw-r--r--   0        0        0      763 2023-08-02 16:17:49.808257 baseten-0.8.0/pypi_readme.md
+-rw-r--r--   0        0        0     1961 2023-08-02 16:18:43.464360 baseten-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2350 1970-01-01 00:00:00.000000 baseten-0.8.0/PKG-INFO
```

### Comparing `baseten-0.7.0/baseten/__init__.py` & `baseten-0.8.0/baseten/__init__.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/baseten_deployed_model.py` & `baseten-0.8.0/baseten/baseten_deployed_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,19 +10,15 @@
 import requests
 import yaml
 from truss.truss_handle import TrussHandle
 
 from baseten.common import api, settings
 from baseten.common.core import raises_api_error
 from baseten.common.error_handler import error_handling
-from baseten.common.lib_support import (
-    build_h5_data_object,
-    coerce_input_to_json,
-    version_gte,
-)
+from baseten.common.lib_support import build_h5_data_object
 
 logger = logging.getLogger(__name__)
 
 REQUIREMENTS_INSTALLATION_STATUS_RETRY_INTERVAL_SEC = 3
 REQUIREMENTS_INSTALLATION_STATUS_MAX_TRIES = 20
 
 
@@ -160,48 +156,31 @@
         if self._model_version_id:
             return api.get_model_version_status(self._model_version_id)
         else:
             return api.get_primary_model_version_status(self._model_id)
 
     @raises_api_error
     @error_handling(error_prefix="Failed to invoke model.")
-    def predict(
-        self, inputs, metadata=None, prediction_only: bool = True
-    ) -> Union[List[List], Dict]:
+    def predict(self, inputs) -> Union[List[List], Dict]:
         """Invokes the model given the input dataframe.
 
         Args:
-            inputs (list | pandas.DataFrame | numpy.ndarray):
-                The data representing one or more inputs to call the model with.
-            metadata (Union[pd.DataFrame, List[Dict]]): Metadata key/value pairs (e.g. name, url), one for each input.
-            prediction_only (bool): set to `False` for the full response (including probablities).
+            inputs:
+                The data representing the input to call the model with.
 
         Returns:
-            A list of inferences for each given input; e.g.: [[3], [9]] would indicate the prediction for the
-            first input in inputs_df is [3], and the prediction for the second is [9].
+            The model output
 
         Raises:
-            TypeError: If the provided inputs is not of a supported type.
             ApiError: If there was an error communicating with the server.
         """
-        if self._truss_spec_version is None:
-            self._truss_spec_version = self.get_truss_spec_version()
-
-        if version_gte(self._truss_spec_version, "2.0"):
-            if self._model_version_id:
-                return api.predict_for_model_version(self._model_version_id, inputs, v2=True)
-            return api.predict_for_model(self._model_id, inputs, v2=True)
-
-        inputs_list, metadata = coerce_input_to_json(inputs, metadata)
 
         if self._model_version_id:
-            return api.predict_for_model_version(
-                self._model_version_id, inputs_list, metadata, prediction_only
-            )
-        return api.predict_for_model(self._model_id, inputs_list, metadata, prediction_only)
+            return api.predict_for_model_version(self._model_version_id, inputs)
+        return api.predict_for_model(self._model_id, inputs)
 
     @raises_api_error
     def update_model_features(self, model_config_file_path: str):
         """Update the model's feature names and output class labels (if any) based on the config
         found at `model_config_file_path`
 
         Args:
```

### Comparing `baseten-0.7.0/baseten/cli.py` & `baseten-0.8.0/baseten/cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/client_commands/baseten_cli.py` & `baseten-0.8.0/baseten/client_commands/baseten_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/client_commands/dataset_cli.py` & `baseten-0.8.0/baseten/client_commands/dataset_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/client_commands/finetuning_cli.py` & `baseten-0.8.0/baseten/client_commands/finetuning_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/client_commands/models_cli.py` & `baseten-0.8.0/baseten/client_commands/models_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/client_commands/pretrained_cli.py` & `baseten-0.8.0/baseten/client_commands/pretrained_cli.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/api.py` & `baseten-0.8.0/baseten/common/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -508,63 +508,60 @@
 
 
 @with_api_key_or_jwt
 def predict_for_model(
     auth_token: AuthToken,
     model_id: str,
     inputs: Union[List, Dict],
-    metadata: Optional[List[Dict]] = None,
-    prediction_only: bool = True,
-    v2: bool = False,
 ) -> Union[List[List], Dict]:
     """Call the model's predict given the input json.
 
     Args:
         auth_token (AuthToken)
         model_id (str)
         inputs (List)
-        metadata (List[Dict]): Metadata key/value pairs (e.g. name, url), one for each input.
-        prediction_only(bool)
+
+    Returns
+        The model output
 
     Raises:
         RequestException: If there was an error communicating with the server.
     """
 
     # We have a special predict endpoint for internal use that we use
     # if a JWT is present.
     if isinstance(auth_token, ApiKey):
         predict_url = f"{settings.get_server_url()}/models/{model_id}/predict"
     elif isinstance(auth_token, JWT):
         predict_url = f"{settings.get_server_url()}/models/{model_id}/predict_internal"
 
-    return _predict(auth_token, predict_url, inputs, metadata, prediction_only, v2=v2)
+    return _predict(auth_token, predict_url, inputs)
 
 
 @with_api_key
 def predict_for_model_version(
     api_key: ApiKey,
     model_version_id: str,
     inputs: Union[List, Dict],
-    metadata: Optional[List[Dict]] = None,
-    prediction_only: bool = True,
-    v2: bool = False,
 ) -> Union[List[List], Dict]:
     """Call the model version's predict given the input json.
 
     Args:
         api_key (str)
         model_version_id (str)
-        inputs (List)
-        metadata (List[Dict]): Metadata key/value pairs (e.g. name, url), one for each input.
+        inputs (List|Dict)
+
+    Returns
+        The model output
 
     Raises:
         RequestException: If there was an error communicating with the server.
     """
     predict_url = f"{settings.get_server_url()}/model_versions/{model_version_id}/predict"
-    return _predict(api_key, predict_url, inputs, metadata, prediction_only, v2=v2)
+    return _predict(api_key, predict_url, inputs)
 
 
 @with_api_key
 def set_primary(api_key, model_version_id: str):
     """Promote this version of the model as the primary version.
 
     Args:
@@ -659,33 +656,23 @@
         return inputs
 
 
 def _predict(
     auth_token: AuthToken,
     predict_url: str,
     inputs: Union[List, Dict],
-    metadata: Optional[List[Dict]] = None,
-    prediction_only: bool = True,
-    v2: bool = False,
 ):
-    if v2:
-        resp = _post_rest_query(auth_token, predict_url, inputs, stream=True)
+    resp = _post_rest_query(auth_token, predict_url, inputs, stream=True)
+
+    if resp.headers.get("transfer-encoding") == "chunked":
+        # Case of streaming response
+        return resp.raw.stream()
 
-        if resp.headers.get("transfer-encoding") == "chunked":
-            # Case of streaming response
-            return resp.raw.stream()
-
-        resp_json = json.loads(resp.content)
-        return resp_json["model_output"]
-
-    resp = _post_rest_query(
-        auth_token, predict_url, _format_inputs_for_v1(auth_token, inputs, metadata)
-    )
     resp_json = json.loads(resp.content)
-    return resp_json["predictions"] if prediction_only else resp_json
+    return resp_json["model_output"]
 
 
 def _post_graphql_query(auth_token: AuthToken, query_string: str) -> dict:
     headers = auth_token.headers()
 
     resp = requests.post(
         f"{settings.get_server_url()}/graphql/", data={"query": query_string}, headers=headers
```

### Comparing `baseten-0.7.0/baseten/common/core.py` & `baseten-0.8.0/baseten/common/core.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/error_handler.py` & `baseten-0.8.0/baseten/common/error_handler.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/files.py` & `baseten-0.8.0/baseten/common/files.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/lib_support.py` & `baseten-0.8.0/baseten/common/lib_support.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/model_deployer.py` & `baseten-0.8.0/baseten/common/model_deployer.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/settings.py` & `baseten-0.8.0/baseten/common/settings.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/tar.py` & `baseten-0.8.0/baseten/common/tar.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/types.py` & `baseten-0.8.0/baseten/common/types.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/common/util.py` & `baseten-0.8.0/baseten/common/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/models/flan_t5.py` & `baseten-0.8.0/baseten/models/flan_t5.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/models/llama.py` & `baseten-0.8.0/baseten/models/llama.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/models/stable_diffusion.py` & `baseten-0.8.0/baseten/models/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/models/util.py` & `baseten-0.8.0/baseten/models/util.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/models/whisper.py` & `baseten-0.8.0/baseten/models/whisper.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/training/datasets.py` & `baseten-0.8.0/baseten/training/datasets.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/training/finetuning.py` & `baseten-0.8.0/baseten/training/finetuning.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/baseten/training/logs.py` & `baseten-0.8.0/baseten/training/logs.py`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/pypi_readme.md` & `baseten-0.8.0/pypi_readme.md`

 * *Files identical despite different names*

### Comparing `baseten-0.7.0/pyproject.toml` & `baseten-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baseten"
-version = "0.7.0"
+version = "0.8.0"
 description = "Deploy machine learning models to Baseten"
 readme = "pypi_readme.md"
 authors = [
     "Amir Haghighat <amir@baseten.co>",
     "Phil Howes <phil@baseten.co>",
     "Tuhin Srivastava <tuhin@baseten.co>",
 ]
```

### Comparing `baseten-0.7.0/PKG-INFO` & `baseten-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baseten
-Version: 0.7.0
+Version: 0.8.0
 Summary: Deploy machine learning models to Baseten
 Keywords: MLOps,AI,Model Serving,Model Deployment,Machine Learning
 Author: Amir Haghighat
 Author-email: amir@baseten.co
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

