# Comparing `tmp/grpc_prometheus_metrics-0.0.1.tar.gz` & `tmp/grpc_prometheus_metrics-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpc_prometheus_metrics-0.0.1.tar", max compression
+gzip compressed data, was "grpc_prometheus_metrics-0.0.2.tar", max compression
```

## Comparing `grpc_prometheus_metrics-0.0.1.tar` & `grpc_prometheus_metrics-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-03-21 10:34:33.856273 grpc_prometheus_metrics-0.0.1/LICENSE
--rw-r--r--   0        0        0     5151 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/__init__.py
--rw-r--r--   0        0        0        0 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/aio/__init__.py
--rw-r--r--   0        0        0     7994 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/aio/prometheus_aio_client_interceptor.py
--rw-r--r--   0        0        0     8979 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/aio/prometheus_aio_server_interceptor.py
--rw-r--r--   0        0        0     2789 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/client_metrics.py
--rw-r--r--   0        0        0     1499 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/grpc_utils.py
--rw-r--r--   0        0        0     7911 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/prometheus_client_interceptor.py
--rw-r--r--   0        0        0     8131 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/prometheus_server_interceptor.py
--rw-r--r--   0        0        0     2224 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/server_metrics.py
--rw-r--r--   0        0        0      693 2023-03-21 10:34:33.860273 grpc_prometheus_metrics-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     5766 1970-01-01 00:00:00.000000 grpc_prometheus_metrics-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/LICENSE
+-rw-r--r--   0        0        0     5151 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/aio/__init__.py
+-rw-r--r--   0        0        0     7994 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/aio/prometheus_aio_client_interceptor.py
+-rw-r--r--   0        0        0     8979 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/aio/prometheus_aio_server_interceptor.py
+-rw-r--r--   0        0        0     2899 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/client_metrics.py
+-rw-r--r--   0        0        0     1499 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/grpc_utils.py
+-rw-r--r--   0        0        0     7911 2023-08-02 07:14:28.355825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/prometheus_client_interceptor.py
+-rw-r--r--   0        0        0     8131 2023-08-02 07:14:28.359825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/prometheus_server_interceptor.py
+-rw-r--r--   0        0        0     2224 2023-08-02 07:14:28.359825 grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/server_metrics.py
+-rw-r--r--   0        0        0      693 2023-08-02 07:14:28.359825 grpc_prometheus_metrics-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     5766 1970-01-01 00:00:00.000000 grpc_prometheus_metrics-0.0.2/PKG-INFO
```

### Comparing `grpc_prometheus_metrics-0.0.1/LICENSE` & `grpc_prometheus_metrics-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `grpc_prometheus_metrics-0.0.1/README.md` & `grpc_prometheus_metrics-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/aio/prometheus_aio_client_interceptor.py` & `grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/aio/prometheus_aio_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/aio/prometheus_aio_server_interceptor.py` & `grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/aio/prometheus_aio_server_interceptor.py`

 * *Files identical despite different names*

### Comparing `grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/client_metrics.py` & `grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/client_metrics.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,20 @@
 from prometheus_client import Counter
 from prometheus_client import Histogram
 
 
+__METRICS = None
+
+
 def init_metrics(registry):
-    return {
+    global __METRICS
+    if __METRICS is not None:
+        return __METRICS
+
+    __METRICS = {
         "grpc_client_started_counter": Counter(
             "grpc_client_started_total",
             "Total number of RPCs started on the client",
             ["grpc_type", "grpc_service", "grpc_method"],
             registry=registry,
         ),
         "grpc_client_handled_counter": Counter(
@@ -26,16 +33,15 @@
             "grpc_client_msg_sent_total",
             "Total number of gRPC stream messages sent by the client.",
             ["grpc_type", "grpc_service", "grpc_method"],
             registry=registry,
         ),
         "grpc_client_handled_histogram": Histogram(
             "grpc_client_handling_seconds",
-            "Histogram of response latency (seconds) of the gRPC until"
-            "it is finished by the application.",
+            "Histogram of response latency (seconds) of the gRPC until" "it is finished by the application.",
             ["grpc_type", "grpc_service", "grpc_method"],
             registry=registry,
         ),
         "grpc_client_stream_recv_histogram": Histogram(
             "grpc_client_msg_recv_handling_seconds",
             "Histogram of response latency (seconds) of the gRPC single message receive.",
             ["grpc_type", "grpc_service", "grpc_method"],
@@ -57,7 +63,8 @@
         "legacy_grpc_client_completed_latency_seconds_histogram": Histogram(
             "grpc_client_completed_latency_seconds",
             "Histogram of rpc response latency (in seconds) for completed rpcs.",
             ["grpc_type", "grpc_service", "grpc_method"],
             registry=registry,
         ),
     }
+    return __METRICS
```

### Comparing `grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/grpc_utils.py` & `grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/grpc_utils.py`

 * *Files identical despite different names*

### Comparing `grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/prometheus_client_interceptor.py` & `grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/prometheus_client_interceptor.py`

 * *Files identical despite different names*

### Comparing `grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/prometheus_server_interceptor.py` & `grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/prometheus_server_interceptor.py`

 * *Files identical despite different names*

### Comparing `grpc_prometheus_metrics-0.0.1/grpc_prometheus_metrics/server_metrics.py` & `grpc_prometheus_metrics-0.0.2/grpc_prometheus_metrics/server_metrics.py`

 * *Files identical despite different names*

### Comparing `grpc_prometheus_metrics-0.0.1/pyproject.toml` & `grpc_prometheus_metrics-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grpc-prometheus-metrics"
-version = "0.0.1"
+version = "0.0.2"
 description = "Python gRPC Prometheus Interceptors, py-grpc-prometheus fork"
 authors = ["Sergio Soldatov <soldatovsr97@gmail.com>", "Lin Chen <linchen04@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 packages = [{include = "grpc_prometheus_metrics"}]
 
 [tool.poetry.dependencies]
```

### Comparing `grpc_prometheus_metrics-0.0.1/PKG-INFO` & `grpc_prometheus_metrics-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grpc-prometheus-metrics
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python gRPC Prometheus Interceptors, py-grpc-prometheus fork
 License: Apache-2.0
 Author: Sergio Soldatov
 Author-email: soldatovsr97@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

