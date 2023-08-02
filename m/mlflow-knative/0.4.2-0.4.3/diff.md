# Comparing `tmp/mlflow_knative-0.4.2.tar.gz` & `tmp/mlflow_knative-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlflow_knative-0.4.2.tar", max compression
+gzip compressed data, was "mlflow_knative-0.4.3.tar", max compression
```

## Comparing `mlflow_knative-0.4.2.tar` & `mlflow_knative-0.4.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1085 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/LICENSE.md
--rw-r--r--   0        0        0     5794 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/README.md
--rw-r--r--   0        0        0      526 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/mlflow_knative/__init__.py
--rw-r--r--   0        0        0    17659 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/mlflow_knative/deployment_client.py
--rw-r--r--   0        0        0     6330 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/mlflow_knative/knative.py
--rw-r--r--   0        0        0     2232 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/mlflow_knative/mlflow_docker.py
--rw-r--r--   0        0        0      808 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/mlflow_knative/service.yaml
--rw-r--r--   0        0        0     1089 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/mlflow_knative/templating.py
--rw-r--r--   0        0        0     1616 2023-07-31 16:14:28.000000 mlflow_knative-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     6637 1970-01-01 00:00:00.000000 mlflow_knative-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/LICENSE.md
+-rw-r--r--   0        0        0     5794 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/README.md
+-rw-r--r--   0        0        0      526 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/mlflow_knative/__init__.py
+-rw-r--r--   0        0        0    17771 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/mlflow_knative/deployment_client.py
+-rw-r--r--   0        0        0     6330 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/mlflow_knative/knative.py
+-rw-r--r--   0        0        0     2232 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/mlflow_knative/mlflow_docker.py
+-rw-r--r--   0        0        0      808 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/mlflow_knative/service.yaml
+-rw-r--r--   0        0        0     1089 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/mlflow_knative/templating.py
+-rw-r--r--   0        0        0     1616 2023-08-02 14:05:01.000000 mlflow_knative-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     6637 1970-01-01 00:00:00.000000 mlflow_knative-0.4.3/PKG-INFO
```

### Comparing `mlflow_knative-0.4.2/LICENSE.md` & `mlflow_knative-0.4.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.4.2/README.md` & `mlflow_knative-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.4.2/mlflow_knative/__init__.py` & `mlflow_knative-0.4.3/mlflow_knative/__init__.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.4.2/mlflow_knative/deployment_client.py` & `mlflow_knative-0.4.3/mlflow_knative/deployment_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,18 +56,22 @@
 
     def __init__(self, uri: str):
         super().__init__(target_uri=uri)
         self._docker_client = docker.from_env()
 
         # Use `load_config` to allow the client to fall back to in-cluster config
         kubernetes_client_config = type.__call__(kubernetes.client.Configuration)
+
+        # Do not pass `context` to `load_config` if no context is provided!
+        # This is required for in-cluster compatibility.
+        kwargs = (
+            {"context": context} if (context := uri.removeprefix("knative:/")) else {}
+        )
         kubernetes.config.load_config(
-            client_configuration=kubernetes_client_config,
-            # Defaulting to `None` ensures `load_config` falls back to default behavior
-            context=uri.removeprefix("knative:/") or None,
+            client_configuration=kubernetes_client_config, **kwargs
         )
         self._kubernetes_client = kubernetes.client.ApiClient(
             configuration=kubernetes_client_config
         )
 
     def create_deployment(
         self,
```

### Comparing `mlflow_knative-0.4.2/mlflow_knative/knative.py` & `mlflow_knative-0.4.3/mlflow_knative/knative.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.4.2/mlflow_knative/mlflow_docker.py` & `mlflow_knative-0.4.3/mlflow_knative/mlflow_docker.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.4.2/mlflow_knative/service.yaml` & `mlflow_knative-0.4.3/mlflow_knative/service.yaml`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.4.2/mlflow_knative/templating.py` & `mlflow_knative-0.4.3/mlflow_knative/templating.py`

 * *Files identical despite different names*

### Comparing `mlflow_knative-0.4.2/pyproject.toml` & `mlflow_knative-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlflow-knative"
-version = "0.4.2"
+version = "0.4.3"
 description = "MLflow plugin adding a Knative deployment target"
 authors = ["Loris Zinsou <lzinsou@protonmail.com>"]
 readme = "README.md"
 keywords = ["mlflow", "plugin", "mlops", "deployment", "deployments", "knative", "kubernetes", "kn", "k8s"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Plugins",
```

### Comparing `mlflow_knative-0.4.2/PKG-INFO` & `mlflow_knative-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlflow-knative
-Version: 0.4.2
+Version: 0.4.3
 Summary: MLflow plugin adding a Knative deployment target
 Home-page: https://gitlab.com/lzinsou/mlflow-knative
 Keywords: mlflow,plugin,mlops,deployment,deployments,knative,kubernetes,kn,k8s
 Author: Loris Zinsou
 Author-email: lzinsou@protonmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
```

