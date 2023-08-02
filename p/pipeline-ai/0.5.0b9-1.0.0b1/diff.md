# Comparing `tmp/pipeline_ai-0.5.0b9.tar.gz` & `tmp/pipeline_ai-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline_ai-0.5.0b9.tar", max compression
+gzip compressed data, was "pipeline_ai-1.0.0b1.tar", max compression
```

## Comparing `pipeline_ai-0.5.0b9.tar` & `pipeline_ai-1.0.0b1.tar`

### file list

```diff
@@ -1,76 +1,38 @@
--rw-r--r--   0        0        0    10176 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/LICENSE
--rw-r--r--   0        0        0     6130 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/README.md
--rw-r--r--   0        0        0      434 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/__init__.py
--rw-r--r--   0        0        0      135 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/__main__.py
--rw-r--r--   0        0        0       62 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/api/__init__.py
--rw-r--r--   0        0        0       62 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/api/asyncio/__init__.py
--rw-r--r--   0        0        0     8379 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/api/asyncio/cloud.py
--rw-r--r--   0        0        0    29923 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/api/cloud.py
--rw-r--r--   0        0        0      974 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/api/environments.py
--rw-r--r--   0        0        0     3231 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/configuration/__init__.py
--rw-r--r--   0        0        0     1392 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/console/__init__.py
--rw-r--r--   0        0        0     2969 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/console/cluster.py
--rw-r--r--   0        0        0     2930 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/console/commands.py
--rw-r--r--   0        0        0        0 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/console/targets/__init__.py
--rw-r--r--   0        0        0      410 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/console/targets/environments.py
--rw-r--r--   0        0        0     2904 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/console/targets/pipelines.py
--rw-r--r--   0        0        0     4887 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/console/targets/pointers.py
--rw-r--r--   0        0        0     1919 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/console/targets/resources.py
--rw-r--r--   0        0        0     4868 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/docker/__init__.py
--rw-r--r--   0        0        0      276 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/exceptions/InvalidSchema.py
--rw-r--r--   0        0        0      283 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/exceptions/MissingActiveToken.py
--rw-r--r--   0        0        0      312 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/exceptions/NonChargeableProfile.py
--rw-r--r--   0        0        0      309 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/exceptions/PipelineNotDeployed.py
--rw-r--r--   0        0        0      546 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/__init__.py
--rw-r--r--   0        0        0     4751 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/decorators.py
--rw-r--r--   0        0        0     1528 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/environment/__init__.py
--rw-r--r--   0        0        0     2015 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/function.py
--rw-r--r--   0        0        0    11039 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/graph.py
--rw-r--r--   0        0        0      877 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/graph_node.py
--rw-r--r--   0        0        0     1090 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/huggingface/TransformersModelForCausalLM.py
--rw-r--r--   0        0        0        0 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/huggingface/__init__.py
--rw-r--r--   0        0        0     1160 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/model.py
--rw-r--r--   0        0        0     3672 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/pipeline.py
--rw-r--r--   0        0        0     1913 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/variable.py
--rw-r--r--   0        0        0     1712 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/objects/wrappers.py
--rw-r--r--   0        0        0        0 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/schemas/__init__.py
--rw-r--r--   0        0        0     1821 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/schemas/base.py
--rw-r--r--   0        0        0      369 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/schemas/compute_requirements.py
--rw-r--r--   0        0        0      558 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/schemas/data.py
--rw-r--r--   0        0        0      573 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/schemas/deployment.py
--rw-r--r--   0        0        0      516 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/schemas/environment.py
--rw-r--r--   0        0        0      714 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/schemas/file.py
--rw-r--r--   0        0        0     2426 2023-06-22 15:18:25.948461 pipeline_ai-0.5.0b9/pipeline/schemas/function.py
--rw-r--r--   0        0        0     5236 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/metrics.py
--rw-r--r--   0        0        0      569 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/milestones_register.py
--rw-r--r--   0        0        0     1599 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/model.py
--rw-r--r--   0        0        0      739 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/onboarding.py
--rw-r--r--   0        0        0      943 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/pagination.py
--rw-r--r--   0        0        0     5817 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/pipeline.py
--rw-r--r--   0        0        0     1261 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/pipeline_file.py
--rw-r--r--   0        0        0      537 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/project.py
--rw-r--r--   0        0        0        0 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/redis/__init__.py
--rw-r--r--   0        0        0      234 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/redis/command.py
--rw-r--r--   0        0        0      337 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/request.py
--rw-r--r--   0        0        0      261 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/resource.py
--rw-r--r--   0        0        0     3839 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/run.py
--rw-r--r--   0        0        0     1031 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/runnable.py
--rw-r--r--   0        0        0      167 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/tag.py
--rw-r--r--   0        0        0     1668 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/token.py
--rw-r--r--   0        0        0     3827 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/user.py
--rw-r--r--   0        0        0     2493 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/validators.py
--rw-r--r--   0        0        0      320 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/schemas/worker.py
--rw-r--r--   0        0        0     1924 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/util/__init__.py
--rw-r--r--   0        0        0     1127 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/util/logging.py
--rw-r--r--   0        0        0      241 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/util/torch_utils/__init__.py
--rw-r--r--   0        0        0        0 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/__init__.py
--rw-r--r--   0        0        0      286 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/environments.py
--rw-r--r--   0        0        0     3119 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/http.py
--rw-r--r--   0        0        0     5462 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/pipelines.py
--rw-r--r--   0        0        0      706 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/schemas/__init__.py
--rw-r--r--   0        0        0      415 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/schemas/pipelines.py
--rw-r--r--   0        0        0      698 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/schemas/pointers.py
--rw-r--r--   0        0        0     3783 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/schemas/runs.py
--rw-r--r--   0        0        0     4571 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pipeline/v3/uploading.py
--rw-r--r--   0        0        0     1250 2023-06-22 15:18:25.952462 pipeline_ai-0.5.0b9/pyproject.toml
--rw-r--r--   0        0        0     7132 1970-01-01 00:00:00.000000 pipeline_ai-0.5.0b9/PKG-INFO
+-rw-r--r--   0        0        0    10176 2023-08-02 11:56:14.698178 pipeline_ai-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     6130 2023-08-02 11:56:14.698178 pipeline_ai-1.0.0b1/README.md
+-rw-r--r--   0        0        0      368 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/__init__.py
+-rw-r--r--   0        0        0      135 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/__main__.py
+-rw-r--r--   0        0        0      300 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/__init__.py
+-rw-r--r--   0        0        0      707 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/compute_requirements.py
+-rw-r--r--   0        0        0      650 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/environments.py
+-rw-r--r--   0        0        0     3827 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/http.py
+-rw-r--r--   0        0        0     7936 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/pipelines.py
+-rw-r--r--   0        0        0     1061 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/pointers.py
+-rw-r--r--   0        0        0      706 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/schemas/__init__.py
+-rw-r--r--   0        0        0     1209 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/schemas/pipelines.py
+-rw-r--r--   0        0        0      701 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/schemas/pointers.py
+-rw-r--r--   0        0        0     4268 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/cloud/schemas/runs.py
+-rw-r--r--   0        0        0     3347 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/configuration/__init__.py
+-rw-r--r--   0        0        0     1392 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/__init__.py
+-rw-r--r--   0        0        0     2924 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/cluster.py
+-rw-r--r--   0        0        0     2961 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/commands.py
+-rw-r--r--   0        0        0        0 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/__init__.py
+-rw-r--r--   0        0        0      410 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/environments.py
+-rw-r--r--   0        0        0     4561 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/pipelines.py
+-rw-r--r--   0        0        0     4960 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/pointers.py
+-rw-r--r--   0        0        0     1859 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/console/targets/resources.py
+-rw-r--r--   0        0        0      509 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/__init__.py
+-rw-r--r--   0        0        0     4764 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/decorators.py
+-rw-r--r--   0        0        0     1528 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/environment/__init__.py
+-rw-r--r--   0        0        0     1374 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/function.py
+-rw-r--r--   0        0        0    13525 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/graph.py
+-rw-r--r--   0        0        0     1090 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/huggingface/TransformersModelForCausalLM.py
+-rw-r--r--   0        0        0        0 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/huggingface/__init__.py
+-rw-r--r--   0        0        0      744 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/model.py
+-rw-r--r--   0        0        0     1773 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/pipeline.py
+-rw-r--r--   0        0        0     1712 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/objects/wrappers.py
+-rw-r--r--   0        0        0     2210 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/util/__init__.py
+-rw-r--r--   0        0        0     1127 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/util/logging.py
+-rw-r--r--   0        0        0      241 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pipeline/util/torch_utils/__init__.py
+-rw-r--r--   0        0        0     1217 2023-08-02 11:56:14.702178 pipeline_ai-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     7083 1970-01-01 00:00:00.000000 pipeline_ai-1.0.0b1/PKG-INFO
```

### Comparing `pipeline_ai-0.5.0b9/LICENSE` & `pipeline_ai-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b9/README.md` & `pipeline_ai-1.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b9/pipeline/configuration/__init__.py` & `pipeline_ai-1.0.0b1/pipeline/configuration/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,21 +55,24 @@
 
     def load(self) -> None:
         path = PIPELINE_DIR / "config.yaml"
         if not path.exists():
             self._config = _ConfigurationModel()
             return
 
-        with open(path, "r") as configuration_file:
-            self._config = _ConfigurationModel.parse_obj(
-                yaml.load(
-                    configuration_file,
-                    Loader=yaml.FullLoader,
-                ),
-            )
+        try:
+            with open(path, "r") as configuration_file:
+                self._config = _ConfigurationModel.parse_obj(
+                    yaml.load(
+                        configuration_file,
+                        Loader=yaml.FullLoader,
+                    ),
+                )
+        except Exception:
+            self._config = _ConfigurationModel()
 
     def save(self) -> None:
         path = PIPELINE_DIR / "config.yaml"
 
         PIPELINE_DIR.mkdir(exist_ok=True)
 
         with open(path, "w") as configuration_file:
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/console/__init__.py` & `pipeline_ai-1.0.0b1/pipeline/console/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b9/pipeline/console/cluster.py` & `pipeline_ai-1.0.0b1/pipeline/console/cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from argparse import ArgumentParser, Namespace, _SubParsersAction
 
-from pipeline import PipelineCloud, current_configuration
-from pipeline.exceptions.MissingActiveToken import MissingActiveToken
+from pipeline import current_configuration
+from pipeline.cloud import authenticate
 from pipeline.util.logging import _print
 
 
 def login_parser(command_parser: "_SubParsersAction[ArgumentParser]") -> None:
     login_parser = command_parser.add_parser(
         "login", help="Login with a compute cluster."
     )
@@ -66,16 +66,19 @@
 def _login(namespace: Namespace) -> None:
     alias = getattr(namespace, "alias")
     url = getattr(namespace, "url")
     token = getattr(namespace, "token")
     active = getattr(namespace, "token", False)
 
     try:
-        PipelineCloud(token=token, url=url, verbose=False)
-    except MissingActiveToken:
+        authenticate(
+            token,
+            url,
+        )
+    except Exception:
         _print(f"Couldn't authenticate with {url}", level="ERROR")
         return
 
     current_configuration.add_remote(
         alias=alias,
         url=url,
         token=token,
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/console/commands.py` & `pipeline_ai-1.0.0b1/pipeline/console/commands.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     pointers.get_parser(get_sub_parser)
     resources.get_parser(get_sub_parser)
 
 
 def delete_parser(command_parser: "_SubParsersAction[ArgumentParser]") -> None:
     delete_parser = command_parser.add_parser(
         "delete",
+        aliases=["del", "rm"],
         description="Delete an object.",
         help="Delete an object.",
     )
     delete_parser.set_defaults(func=lambda _: delete_parser.print_help())
 
     delete_sub_parser = delete_parser.add_subparsers(
         dest="target",
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/console/targets/pointers.py` & `pipeline_ai-1.0.0b1/pipeline/console/targets/pointers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 import re
 from argparse import ArgumentParser, Namespace, _SubParsersAction
 
 from tabulate import tabulate
 
-from pipeline.api import PipelineCloud
+from pipeline.cloud import http
+from pipeline.cloud.schemas import pointers as pointers_schema
 from pipeline.util.logging import _print
-from pipeline.v3.schemas import pointers as pointers_schema
 
 VALID_TAG_NAME = re.compile(
     r"^[a-z0-9][a-z0-9-._/]*[a-z0-9]:[0-9A-Za-z_][0-9A-Za-z-_.]{0,127}$"
 )
 
 
 def create_parser(command_parser: "_SubParsersAction[ArgumentParser]") -> None:
@@ -80,14 +80,21 @@
         "pointers",
         aliases=["pointer"],
         help="Get pointer information.",
     )
 
     get_parser.set_defaults(func=_get_pointer)
 
+    get_parser.add_argument(
+        "--name",
+        "-n",
+        type=str,
+        help="Pipeline name.",
+    )
+
 
 def delete_parser(command_parser: "_SubParsersAction[ArgumentParser]") -> None:
     delete_parser = command_parser.add_parser(
         "pointers",
         aliases=["pointer"],
         help="Delete a pointer.",
     )
@@ -100,29 +107,32 @@
 
     delete_parser.set_defaults(func=_delete_pointer)
 
 
 def _get_pointer(namespace: Namespace) -> None:
     _print("Getting pointers")
 
-    cluster_api = PipelineCloud(verbose=False)
-    pointers_raw = cluster_api._get("/v3/pointers")
+    pipeline_name = getattr(namespace, "name", None)
+    query_params = dict()
+    if pipeline_name:
+        query_params["pipeline_name"] = pipeline_name
+    pointers_raw = http.get("/v3/pointers", params=query_params).json()
 
     pointers = [
         [
             pointer_raw["pointer"],
             pointer_raw["pipeline_id"],
         ]
         for pointer_raw in pointers_raw
     ]
 
     table = tabulate(
         pointers,
         headers=["Pointer", "Pipeline ID"],
-        tablefmt="outline",
+        tablefmt="psql",
     )
     print(table)
 
 
 def _create_pointer(namespace: Namespace) -> None:
     new_pointer = getattr(namespace, "new_pointer")
     pipeline_id_or_pointer = getattr(namespace, "pipeline_id_or_pointer")
@@ -132,16 +142,15 @@
 
     create_schema = pointers_schema.PointerCreate(
         pointer=new_pointer,
         pointer_or_pipeline_id=pipeline_id_or_pointer,
         locked=locked,
     )
 
-    cluster_api = PipelineCloud(verbose=False)
-    cluster_api._post(
+    http.post(
         "/v3/pointers",
         json.loads(
             create_schema.json(),
         ),
     )
     _print("Pointer created!")
 
@@ -163,29 +172,27 @@
     _print(f"Editing pointer ({pointer})")
 
     edit_schema = pointers_schema.PointerPatch(
         pointer_or_pipeline_id=new_pipeline_id_or_pointer,
         locked=locked if locked is not None else not unlocked,
     )
 
-    cluster_api = PipelineCloud(verbose=False)
-    cluster_api._patch(
+    http.patch(
         f"/v3/pointers/{pointer}",
         json.loads(
             edit_schema.json(),
         ),
     )
 
     _print("Pointer edited!")
 
 
 def _delete_pointer(namespace: Namespace) -> None:
     pointer = getattr(namespace, "pointer")
 
     _print(f"Deleting pointer ({pointer})")
 
-    cluster_api = PipelineCloud(verbose=False)
-    cluster_api._delete(
+    http.delete(
         f"/v3/pointers/{pointer}",
     )
 
     _print("Pointer deleted!")
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/console/targets/resources.py` & `pipeline_ai-1.0.0b1/pipeline/console/targets/resources.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 from argparse import ArgumentParser, _SubParsersAction
 
 from tabulate import tabulate
 
-from pipeline import PipelineCloud
+from pipeline.cloud import http
 
 # Parser builder
 
 
 def create_parser(command_parser: "_SubParsersAction[ArgumentParser]") -> None:
     ...
 
@@ -29,16 +29,15 @@
 def _shorten_id(id: str, leading_length: int = 4, trailing_length: int = 4) -> str:
     if id == "None":
         return "None"
     return id[:leading_length] + "..." + id[-trailing_length:]
 
 
 def list_resources() -> None:
-    remote_service = PipelineCloud(verbose=False)
-    resource_information = remote_service._get("/v3/core/resources")
+    resource_information = http.get("/v3/core/resources").json()
     resource_information = [json.loads(resource) for resource in resource_information]
 
     resource_data = [
         [
             _shorten_id(resource["id"]),
             [
                 _shorten_id(p_id)
@@ -61,11 +60,11 @@
         headers=[
             "ID",
             "Pipelines",
             "Current run",
             "Run queue",
             "GPUs",
         ],
-        tablefmt="outline",
+        tablefmt="psql",
     )
 
     print(table)
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/objects/decorators.py` & `pipeline_ai-1.0.0b1/pipeline/objects/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import typing
 from functools import partial, wraps
 
 from pipeline.objects.function import Function
-from pipeline.objects.graph_node import GraphNode
+from pipeline.objects.graph import GraphNode, Variable
 from pipeline.objects.model import Model
 from pipeline.objects.pipeline import Pipeline
-from pipeline.objects.variable import Variable
 
 
 def pipeline_function(function=None, *, run_once=False, on_startup=False):
     """_summary_
 
     Args:
         function (callable, optional): _description_. This is the function to be
@@ -64,25 +63,26 @@
                     )
 
             node_outputs: typing.List[Variable] = []
 
             function_output = function.__annotations__["return"]
             if getattr(function_output, "__origin__", None) == tuple:
                 context_manager_variables = node_outputs = tuple(
-                    Variable(type_class=output_variable)
+                    Variable(type_class=output_variable, is_input=False)
                     for output_variable in function_output.__args__
                 )
 
             else:
                 context_manager_variables = Variable(
-                    type_class=function.__annotations__["return"]
+                    type_class=function.__annotations__["return"],
+                    is_input=False,
                 )
                 node_outputs = [context_manager_variables]
 
-            Pipeline.add_variables(*node_outputs)
+            # Pipeline.add_variables(*node_outputs)
             Pipeline.add_function(function.__pipeline_function__)
 
             new_node = GraphNode(
                 function=function.__pipeline_function__,
                 inputs=processed_args,
                 outputs=node_outputs,
             )
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/objects/environment/__init__.py` & `pipeline_ai-1.0.0b1/pipeline/objects/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b9/pipeline/objects/function.py` & `pipeline_ai-1.0.0b1/pipeline/objects/function.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import inspect
 import uuid
 from hashlib import sha256
 from typing import Any, Callable, Dict, Optional
 
-from pipeline.schemas.function import FunctionGet
-from pipeline.util import generate_id, load_object
+from pipeline.util import generate_id
 
 
 class Function:
     local_id: str
     remote_id: str
 
     name: str
@@ -46,23 +45,7 @@
         self.typing_inputs = {
             function_i: function.__annotations__[function_i]
             for function_i in function.__annotations__
             if not function_i == "return"
         }
 
         self.local_id = generate_id(10)
-
-    @classmethod
-    def from_schema(cls, schema: FunctionGet):
-        unpickled_data = load_object(schema.hex_file.data)
-        if isinstance(unpickled_data, Function):
-            function = unpickled_data
-        else:
-            function = cls(
-                unpickled_data,
-                remote_id=schema.id,
-            )
-        # This assumes that whenever a Function is uploaded, any GraphNode
-        # referencing it has its `function` property updated to the remote ID
-        # of the Function.
-        function.local_id = schema.id
-        return function
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/objects/graph.py` & `pipeline_ai-1.0.0b1/pipeline/objects/graph.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,225 @@
-from typing import List
+import tempfile
+from typing import Any, Iterable, List, Optional
 
 from cloudpickle import dumps
 from dill import loads
+from pydantic import BaseModel
 
+from pipeline.cloud.schemas.pipelines import IOVariable
+from pipeline.cloud.schemas.runs import RunIOType
 from pipeline.objects.function import Function
-from pipeline.objects.graph_node import GraphNode
 from pipeline.objects.model import Model
-from pipeline.objects.variable import PipelineFile, Variable
-from pipeline.schemas.pipeline import PipelineGet
-from pipeline.util import generate_id
+from pipeline.util import dump_object, generate_id
+
+
+class VariableException(Exception):
+    ...
+
+
+class Variable:
+    local_id: str
+    remote_id: str
+
+    name: str
+
+    type_class: Any
+
+    is_input: bool
+    is_output: bool
+
+    def __init__(
+        self,
+        type_class: Any,
+        *,
+        is_input: bool = True,
+        is_output: bool = False,
+        local_id: str = None,
+        # default: Any | None = None, # TODO: Implement default values
+        title: str | None = None,
+        description: str | None = None,
+        examples: list[Any] | None = None,
+        gt: int | None = None,
+        ge: int | None = None,
+        lt: int | None = None,
+        le: int | None = None,
+        multiple_of: int | None = None,
+        allow_inf_nan: bool | None = None,
+        max_digits: int | None = None,
+        decimal_places: int | None = None,
+        min_length: int | None = None,
+        max_length: int | None = None,
+        choices: list[Any] | None = None,
+        dict_schema: BaseModel | None = None,
+    ):
+        from pipeline.objects.pipeline import Pipeline
+
+        self.type_class = type_class
+        self.is_input = is_input
+        self.is_output = is_output
+
+        self.title = title
+        self.description = description
+        self.examples = examples
+        self.gt = gt
+        self.ge = ge
+        self.lt = lt
+        self.le = le
+        self.multiple_of = multiple_of
+        self.allow_inf_nan = allow_inf_nan
+        self.max_digits = max_digits
+        self.decimal_places = decimal_places
+        self.min_length = min_length
+        self.max_length = max_length
+        self.choices = choices
+        self.dict_schema = dict_schema.schema() if dict_schema is not None else None
+
+        if not Pipeline._pipeline_context_active:
+            raise Exception("Cant add a variable when not defining a pipeline")
+
+        Pipeline._current_pipeline.variables.append(self)
+
+        self.local_id = generate_id(10) if not local_id else local_id
+
+    def validate_variable(self, value: Any) -> None:
+        # if not isinstance(value, self.type_class):
+        #     return
+
+        if self.choices is not None:
+            if value not in self.choices:
+                raise VariableException(
+                    f"Value is not in the choices of {self.choices}"
+                )
+
+        if self.gt is not None:
+            if value <= self.gt:
+                raise VariableException(f"Value is not greater than {self.gt}")
+
+        if self.ge is not None:
+            if value < self.ge:
+                raise VariableException(
+                    f"Value is not greater than or equal to {self.ge}"
+                )
+
+        if self.lt is not None:
+            if value >= self.lt:
+                raise VariableException(f"Value is not less than {self.lt}")
+
+        if self.le is not None:
+            if value > self.le:
+                raise VariableException(f"Value is not less than or equal to {self.le}")
+
+        if self.multiple_of is not None:
+            if value % self.multiple_of != 0:
+                raise VariableException(
+                    f"Value is not a multiple of {self.multiple_of}"
+                )
+
+        if self.allow_inf_nan is not None:
+            if not self.allow_inf_nan and (
+                value == float("inf") or value == float("-inf") or value == float("nan")
+            ):
+                raise VariableException("Value is not allowed to be infinity or nan")
+
+        if self.max_digits is not None:
+            if len(str(value)) > self.max_digits:
+                raise VariableException(f"Value has more than {self.max_digits} digits")
+
+        if self.decimal_places is not None:
+            if len(str(value).split(".")[1]) > self.decimal_places:
+                raise VariableException(
+                    f"Value has more than {self.decimal_places} decimal places"
+                )
+
+        if self.min_length is not None:
+            if len(str(value)) < self.min_length:
+                raise VariableException(
+                    f"Value has less than {self.min_length} characters"
+                )
+
+        if self.max_length is not None:
+            if len(str(value)) > self.max_length:
+                raise VariableException(
+                    f"Value has more than {self.max_length} characters"
+                )
+
+    def to_io_schema(self) -> IOVariable:
+        return IOVariable(
+            run_io_type=RunIOType.from_object(self.type_class),
+            title=self.title,
+            description=self.description,
+            examples=self.examples,
+            gt=self.gt,
+            ge=self.ge,
+            lt=self.lt,
+            le=self.le,
+            multiple_of=self.multiple_of,
+            allow_inf_nan=self.allow_inf_nan,
+            max_digits=self.max_digits,
+            decimal_places=self.decimal_places,
+            min_length=self.min_length,
+            max_length=self.max_length,
+            choices=self.choices,
+            dict_schema=self.dict_schema,
+        )
+
+
+class PipelineFile(Variable):
+    path: str
+
+    def __init__(
+        self,
+        *,
+        path: str = None,
+        title: str = None,
+        local_id: str = None,
+    ) -> None:
+        super().__init__(
+            type_class=self.__class__,
+            is_input=False,
+            is_output=False,
+            title=title,
+            local_id=local_id,
+        )
+        self.path = path
+
+    @classmethod
+    def from_object(
+        cls,
+        obj: Any,
+        modules: Optional[List[str]] = None,
+    ):
+        temp_file = tempfile.NamedTemporaryFile(delete=False)
+
+        bytes = dump_object(obj, modules=modules)
+        temp_file.write(bytes)
+        temp_file.seek(0)
+
+        return cls(
+            path=temp_file.name,
+            name=temp_file.name,
+        )
+
+
+class Stream(Variable, Iterable):
+    ...
+
+
+class GraphNode:
+    local_id: str
+    function: Function
+    inputs: List[Variable] = []
+    outputs: List[Variable] = []
+
+    def __init__(self, function, inputs, outputs, *, local_id=None):
+        self.function = function
+        self.inputs = inputs
+        self.outputs = outputs
+
+        self.local_id = generate_id(10) if local_id is None else local_id
 
 
 class Graph:
     local_id: str
     remote_id: str
 
     name: str
@@ -22,47 +229,34 @@
 
     outputs: List[Variable]
 
     nodes: List[GraphNode]
 
     models: List[Model]
 
-    # TODO: Add generic objects (e.g. Model) to be included in the graph
-
-    compute_type: str
-    min_gpu_vram_mb: int
-
-    minimum_cache_number: int
-
     def __init__(
         self,
         *,
         name: str = "",
         variables: List[Variable] = None,
         functions: List[Function] = None,
         outputs: List[Variable] = None,
         nodes: List[GraphNode] = None,
         models: List[Model] = None,
-        compute_type: str = "gpu",
-        min_gpu_vram_mb: int = None,
-        minimum_cache_number: int = None,
     ):
         self.name = name
         self.local_id = generate_id(10)
 
         self.variables = variables if variables is not None else []
         self.functions = functions if functions is not None else []
         self.outputs = outputs if outputs is not None else []
         self.nodes = nodes if nodes is not None else []
         self.models = models if models is not None else []
         # Flag set when all functions with the on_startup field have run
         self._has_run_startup = False
-        self.compute_type = compute_type
-        self.min_gpu_vram_mb = min_gpu_vram_mb
-        self.minimum_cache_number = minimum_cache_number
 
     def _startup(self):
         if self._has_run_startup:
             return
 
         startup_variables = {}
 
@@ -207,107 +401,14 @@
         return_variables = []
 
         for output_variable in self.outputs:
             return_variables.append(running_variables[output_variable.local_id])
 
         return return_variables
 
-    def _update_function_local_id(self, old_id: str, new_id: str) -> None:
-        for func in self.functions:
-            if func.local_id == old_id:
-                func.local_id = new_id
-                return
-        raise Exception("Function with local_id:%s not found" % old_id)
-
-    @classmethod
-    def from_schema(cls, schema: PipelineGet):
-        variables = [Variable.from_schema(_var) for _var in schema.variables]
-        functions = [Function.from_schema(_func) for _func in schema.functions]
-        models = [Model.from_schema(_model) for _model in schema.models]
-
-        # Rebind functions -> models
-        update_functions = []
-        for _func in functions:
-            if hasattr(_func.class_instance, "__pipeline_model__"):
-                model = _func.class_instance
-                is_bound = False
-                for _model in models:
-                    if _model.model.local_id == model.local_id:
-                        bound_method = _func.function.__get__(
-                            _model.model, _model.model.__class__
-                        )
-                        setattr(_model.model, _func.function.__name__, bound_method)
-                        is_bound = True
-                        _func.class_instance = _model.model
-                if not is_bound:
-                    raise Exception(
-                        "Did not find a class to bind for model (local_id:%s)"
-                        % model.local_id
-                    )
-            elif _func.class_instance is not None:
-                raise Exception(
-                    "Incorrect bound class:%s\ndir:%s"
-                    % (_func.class_instance, dir(_func.class_instance))
-                )
-            update_functions.append(_func)
-        functions = update_functions
-
-        outputs = []
-        for _output in schema.outputs:
-            for _var in variables:
-                if _var.local_id == _output:
-                    outputs.append(_var)
-
-        nodes = []
-
-        for _node in schema.graph_nodes:
-            node_inputs = []
-            for node_str in _node.inputs:
-                for _var in variables:
-                    if _var.local_id == node_str:
-                        node_inputs.append(_var)
-                        break
-
-            node_outputs = []
-            for node_str in _node.outputs:
-                for _var in variables:
-                    if _var.local_id == node_str:
-                        node_outputs.append(_var)
-                        break
-
-            function = None
-
-            for _func in functions:
-                if _func.local_id == _node.function:
-                    function = _func
-                    break
-
-            if function is None:
-                raise Exception("Function not found:%s" % _node.function)
-
-            nodes.append(
-                GraphNode(
-                    function=function,
-                    inputs=node_inputs,
-                    outputs=node_outputs,
-                    local_id=_node.local_id,
-                )
-            )
-
-        remade_graph = cls(
-            name=schema.name,
-            variables=variables,
-            functions=functions,
-            outputs=outputs,
-            nodes=nodes,
-            models=models,
-        )
-
-        return remade_graph
-
     def save(self, save_path):
         with open(save_path, "wb") as save_file:
             save_file.write(dumps(self))
 
     @classmethod
     def load(cls, load_path):
         with open(load_path, "rb") as load_file:
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/objects/huggingface/TransformersModelForCausalLM.py` & `pipeline_ai-1.0.0b1/pipeline/objects/huggingface/TransformersModelForCausalLM.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b9/pipeline/objects/wrappers.py` & `pipeline_ai-1.0.0b1/pipeline/objects/wrappers.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b9/pipeline/util/__init__.py` & `pipeline_ai-1.0.0b1/pipeline/util/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,39 +1,45 @@
+import importlib
 import importlib.metadata
 import io
 import random
 import string
-from typing import Any, Callable, Optional, Union
+from typing import Any, Callable, List, Optional, Union
 
-from cloudpickle import dumps
+from cloudpickle import dumps, register_pickle_by_value
 from dill import loads
 
-from pipeline.schemas.file import FileCreate
-
 
 def package_version() -> str:
     """Return the version of the installed `pipeline-ai` package."""
     return importlib.metadata.version("pipeline-ai")
 
 
 def generate_id(length: int) -> str:
     return "".join((random.choice(string.ascii_letters) for i in range(length)))
 
 
-def python_object_to_hex(obj: Any) -> str:
-    return dumps(obj).hex()
+def python_object_to_hex(
+    obj: Any,
+    modules: Optional[List[str]] = None,
+) -> str:
+    return dump_object(obj, modules=modules).hex()
 
 
 def hex_to_python_object(hex: str) -> Any:
     h = bytes.fromhex(hex)
     return loads(h)
 
 
-def dump_object(obj: Any) -> bytes:
+def dump_object(obj: Any, modules: Optional[List[str]] = None) -> bytes:
     """Serialize `obj` as bytes."""
+    if modules is not None:
+        for module_name in modules:
+            module = importlib.import_module(module_name)
+            register_pickle_by_value(module)
     return dumps(obj)
 
 
 def load_object(pickled: Union[bytes, str]) -> Any:
     """Deserialize an object from the payload."""
     if isinstance(pickled, str):
         return hex_to_python_object(pickled)
@@ -44,19 +50,19 @@
 def python_object_to_name(obj: Any) -> Optional[str]:
     # Consider limiting the size of the name in future releases
     name = getattr(obj, "__name__", str(obj))
 
     return name
 
 
-def python_object_to_file_create(obj: Any, name: str = None):
-    if name is None:
-        name = generate_id(20)
+# def python_object_to_file_create(obj: Any, name: str = None):
+#     if name is None:
+#         name = generate_id(20)
 
-    return FileCreate(name=name, file_bytes=python_object_to_hex)
+#     return FileCreate(name=name, file_bytes=python_object_to_hex)
 
 
 class CallbackBytesIO(io.BytesIO):
     """Provides same interface as BytesIO but additionally calls a callback function
     whenever the 'read' method is called.
 
     This is similar to tqdm's own CallbackIOWrapper but this does not play nicely with
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/util/logging.py` & `pipeline_ai-1.0.0b1/pipeline/util/logging.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b9/pipeline/v3/http.py` & `pipeline_ai-1.0.0b1/pipeline/cloud/http.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import io
+import os
 import typing as t
 
 import httpx
 
 # from httpx import _GeneratorContextManager
 import requests
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
@@ -10,21 +11,27 @@
 
 from pipeline import current_configuration
 from pipeline.util.logging import PIPELINE_STR
 
 ACTIVE_IP = (
     active_remote.url
     if (active_remote := current_configuration.active_remote) is not None
-    else None
+    else os.environ.get("PIPELINE_API_URL", None)
+)
+
+ACTIVE_TOKEN = (
+    current_configuration.active_remote.token
+    if current_configuration.active_remote is not None
+    else os.environ.get("PIPELINE_API_TOKEN", None)
 )
 
 _client = httpx.Client(
     base_url=ACTIVE_IP,
     headers={
-        "Authorization": f"Bearer {current_configuration.active_remote.token}",
+        "Authorization": f"Bearer {ACTIVE_TOKEN}",
     },
     timeout=300,
 )
 
 
 def post(
     endpoint: str,
@@ -37,20 +44,44 @@
     )
     if raise_for_status:
         response.raise_for_status()
 
     return response
 
 
-def get(
+def patch(
     endpoint: str,
+    json_data: dict = None,
+    raise_for_status: bool = True,
 ) -> httpx.Response:
-    response = _client.get(
+    response = _client.patch(
         endpoint,
+        json=json_data,
     )
+    if raise_for_status:
+        response.raise_for_status()
+
+    return response
+
+
+def get(
+    endpoint: str,
+    **kwargs,
+) -> httpx.Response:
+    response = _client.get(endpoint, **kwargs)
+    response.raise_for_status()
+
+    return response
+
+
+def delete(
+    endpoint: str,
+    **kwargs,
+) -> httpx.Response:
+    response = _client.delete(endpoint, **kwargs)
     response.raise_for_status()
 
     return response
 
 
 def create_callback(encoder: MultipartEncoder) -> t.Callable:
     encoder_len = encoder.len
@@ -103,14 +134,15 @@
     )
 
 
 def post_files(
     endpoint: str,
     files: t.Dict[str, t.Any],
     params: t.Dict[str, t.Any] = dict(),
+    data: t.Dict[str, t.Any] = dict(),
     progress: bool = False,
 ) -> httpx.Response:
     if progress:
         monitor = get_progress_bar_uploader(files=files, params=params)
         response = requests.post(
             f"{ACTIVE_IP}{endpoint}",
             data=monitor,
@@ -119,14 +151,15 @@
                 "Authorization": f"Bearer {current_configuration.active_remote.token}",
             },
         )
     else:
         response = _client.post(
             endpoint,
             files=files,
+            data=data,
             params=params,
         )
 
     return response
 
 
 def stream_post(
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/v3/schemas/__init__.py` & `pipeline_ai-1.0.0b1/pipeline/cloud/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `pipeline_ai-0.5.0b9/pipeline/v3/schemas/pointers.py` & `pipeline_ai-1.0.0b1/pipeline/cloud/schemas/pointers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import re
 import typing as t
 
 from pydantic import validator
 
-from pipeline.v3.schemas import BaseModel
+from pipeline.cloud.schemas import BaseModel
 
 POINTER_REGEX = re.compile(
     r"^[a-z0-9][a-z0-9-._/]*[a-z0-9]:[0-9A-Za-z_][0-9A-Za-z-_.]{0,127}$"
 )
 
 
 class PointerGet(BaseModel):
```

### Comparing `pipeline_ai-0.5.0b9/pipeline/v3/schemas/runs.py` & `pipeline_ai-1.0.0b1/pipeline/cloud/schemas/runs.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     # starting subrprocess running worker in custom environment
     starting_worker: int = 4
     downloading_graph: int = 5
     caching_graph: int = 6
     running: int = 7
     resource_returning: int = 8
     api_received: int = 9
+    celery_worker_received: int = 22
 
     in_queue: int = 16
     denied: int = 11
     resource_rejected: int = 14
     resource_died: int = 15
     retrying: int = 13
     rerouting: int = 21
@@ -84,37 +85,48 @@
 class RunIOType(str, Enum):
     integer: str = "integer"
     string: str = "string"
     fp: str = "fp"
     dictionary: str = "dictionary"
     boolean: str = "boolean"
     none: str = "none"
+    array: str = "array"
 
     pkl: str = "pkl"
     file: str = "file"
 
     @classmethod
     def from_object(cls, obj: t.Any):
         # Get the enum type for the object.
-        if isinstance(obj, int):
+        if isinstance(obj, int) or obj is int:
             return cls.integer
-        elif isinstance(obj, float):
+        elif isinstance(obj, float) or obj is float:
             return cls.fp
-        elif isinstance(obj, str):
+        elif isinstance(obj, str) or obj is str:
             return cls.string
-        elif isinstance(obj, bool):
+        elif isinstance(obj, bool) or obj is bool:
             return cls.boolean
         elif obj is None:
             return cls.none
-        elif isinstance(obj, dict):
+        elif isinstance(obj, dict) or obj is dict:
+            if obj is dict:
+                return cls.dictionary
             try:
                 json.dumps(obj)
             except (TypeError, OverflowError):
                 return cls.pkl
             return cls.dictionary
+        elif isinstance(obj, list) or obj is list:
+            if obj is list:
+                return cls.array
+            try:
+                json.dumps(obj)
+            except (TypeError, OverflowError):
+                return cls.pkl
+            return cls.array
         elif isinstance(obj, io.BufferedIOBase):
             return cls.file
         else:
             return cls.pkl
 
 
 class RunOutputFile(BaseModel):
@@ -144,15 +156,16 @@
     created_at: datetime
 
     pipeline_id: str
     environment_id: str
     environment_hash: str
 
     state: RunState
-    error: t.Optional[RunError]
+
+    error: t.Optional[t.Tuple[RunError, str]]
 
     result: t.Optional[RunResult]
 
     class Config:
         # use_enum_values = True
         orm_mode = True
```

### Comparing `pipeline_ai-0.5.0b9/pyproject.toml` & `pipeline_ai-1.0.0b1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "pipeline-ai"
-version = "0.5.0b9"
+version = "1.0.0b1"
 
 
 description = "Pipelines for machine learning workloads."
 authors = [
   "Paul Hetherington <ph@mystic.ai>",
-  "Alex Pearwin <alex@mystic.ai>",
-  "Neil Wang <neil@mystic.ai>",
   "Ross Gray <ross@mystic.ai>",
+  "Yvan Buggy <yvan@mystic.ai>",
 ]
 packages = [{ include = "pipeline" }]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   'License :: OSI Approved :: Apache Software License',
   'Programming Language :: Python :: 3',
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = "^3.10"
 pydantic = "^1.8.2"
 setuptools = "^65.4.1"
 pyhumps = "^3.0.2"
 tqdm = "^4.62.3"
 PyYAML = "^6.0"
 cloudpickle = "^2.2.0"
 dill = "^0.3.6"
```

### Comparing `pipeline_ai-0.5.0b9/PKG-INFO` & `pipeline_ai-1.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: pipeline-ai
-Version: 0.5.0b9
+Version: 1.0.0b1
 Summary: Pipelines for machine learning workloads.
 License: Apache-2.0
 Author: Paul Hetherington
 Author-email: ph@mystic.ai
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: cloudpickle (>=2.2.0,<3.0.0)
 Requires-Dist: dill (>=0.3.6,<0.4.0)
 Requires-Dist: httpx (>=0.23.1,<0.24.0)
 Requires-Dist: packaging (>=21.0)
```

