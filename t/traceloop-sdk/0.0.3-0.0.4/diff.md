# Comparing `tmp/traceloop_sdk-0.0.3.tar.gz` & `tmp/traceloop_sdk-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceloop_sdk-0.0.3.tar", max compression
+gzip compressed data, was "traceloop_sdk-0.0.4.tar", max compression
```

## Comparing `traceloop_sdk-0.0.3.tar` & `traceloop_sdk-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,18 @@
--rw-r--r--   0        0        0        0 2023-08-02 09:25:16.062473 traceloop_sdk-0.0.3/README.md
--rw-r--r--   0        0        0      621 2023-08-02 13:01:06.288704 traceloop_sdk-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-30 14:54:26.714515 traceloop_sdk-0.0.3/traceloop/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:29:56.846025 traceloop_sdk-0.0.3/traceloop/agent/__init__.py
--rw-r--r--   0        0        0      238 2023-08-01 13:49:46.129127 traceloop_sdk-0.0.3/traceloop/agent/decorator.py
--rw-r--r--   0        0        0        0 2023-08-01 13:30:02.778279 traceloop_sdk-0.0.3/traceloop/agent/tool/__init__.py
--rw-r--r--   0        0        0      236 2023-08-01 14:31:03.279362 traceloop_sdk-0.0.3/traceloop/agent/tool/decorator.py
--rw-r--r--   0        0        0      239 2023-08-01 13:41:08.608117 traceloop_sdk-0.0.3/traceloop/semconv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 15:13:41.585793 traceloop_sdk-0.0.3/traceloop/task/__init__.py
--rw-r--r--   0        0        0      729 2023-08-01 14:01:15.919064 traceloop_sdk-0.0.3/traceloop/task/decorator.py
--rw-r--r--   0        0        0        0 2023-07-30 15:42:25.834193 traceloop_sdk-0.0.3/traceloop/tracing/__init__.py
--rw-r--r--   0        0        0     1424 2023-08-02 13:02:07.803039 traceloop_sdk-0.0.3/traceloop/tracing/tracer.py
--rw-r--r--   0        0        0        0 2023-08-01 09:57:19.484179 traceloop_sdk-0.0.3/traceloop/workflow/__init__.py
--rw-r--r--   0        0        0      644 2023-08-01 14:01:15.916149 traceloop_sdk-0.0.3/traceloop/workflow/decorator.py
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 traceloop_sdk-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 09:25:16.062473 traceloop_sdk-0.0.4/README.md
+-rw-r--r--   0        0        0      562 2023-08-02 14:04:11.214099 traceloop_sdk-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:35:06.247470 traceloop_sdk-0.0.4/traceloop/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:29:56.846025 traceloop_sdk-0.0.4/traceloop/agent/__init__.py
+-rw-r--r--   0        0        0      238 2023-08-01 13:49:46.129127 traceloop_sdk-0.0.4/traceloop/agent/decorator.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:30:02.778279 traceloop_sdk-0.0.4/traceloop/agent/tool/__init__.py
+-rw-r--r--   0        0        0      236 2023-08-01 14:31:03.279362 traceloop_sdk-0.0.4/traceloop/agent/tool/decorator.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:18:36.291777 traceloop_sdk-0.0.4/traceloop/instrumentation/__init__.py
+-rw-r--r--   0        0        0    11253 2023-08-02 13:37:44.238046 traceloop_sdk-0.0.4/traceloop/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-02 13:35:46.090364 traceloop_sdk-0.0.4/traceloop/instrumentation/openai/package.py
+-rw-r--r--   0        0        0      239 2023-08-01 13:41:08.608117 traceloop_sdk-0.0.4/traceloop/semconv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:13:41.585793 traceloop_sdk-0.0.4/traceloop/task/__init__.py
+-rw-r--r--   0        0        0      729 2023-08-01 14:01:15.919064 traceloop_sdk-0.0.4/traceloop/task/decorator.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:42:25.834193 traceloop_sdk-0.0.4/traceloop/tracing/__init__.py
+-rw-r--r--   0        0        0     1419 2023-08-02 14:03:30.448209 traceloop_sdk-0.0.4/traceloop/tracing/tracer.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:57:19.484179 traceloop_sdk-0.0.4/traceloop/workflow/__init__.py
+-rw-r--r--   0        0        0      644 2023-08-01 14:01:15.916149 traceloop_sdk-0.0.4/traceloop/workflow/decorator.py
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 traceloop_sdk-0.0.4/PKG-INFO
```

### Comparing `traceloop_sdk-0.0.3/traceloop/task/decorator.py` & `traceloop_sdk-0.0.4/traceloop/task/decorator.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.3/traceloop/tracing/tracer.py` & `traceloop_sdk-0.0.4/traceloop/tracing/tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 
 from opentelemetry import trace
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
-from opentelemetry.instrumentation.openai import OpenAIInstrumentor
+from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
-import opentelemetry.instrumentation.requests import RequestsInstrumentor
+
+from traceloop.instrumentation.openai import OpenAIInstrumentor
 
 TRACER_NAME = "traceloop.tracer"
 TRACELOOP_API_ENDPOINT = "https://api.traceloop.dev/v1/traces"
 
 
 class Tracer:
     __instance = None
```

### Comparing `traceloop_sdk-0.0.3/traceloop/workflow/decorator.py` & `traceloop_sdk-0.0.4/traceloop/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.3/PKG-INFO` & `traceloop_sdk-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: traceloop-sdk
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: openai (>=0.27.8,<0.28.0)
-Requires-Dist: opentelemetry-api (==1.18.0)
-Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0)
-Requires-Dist: opentelemetry-instrument-openai (==0.6.0)
-Requires-Dist: opentelemetry-instrumentation-requests (==0.39b0)
-Requires-Dist: opentelemetry-sdk (==1.18.0)
-Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: opentelemetry-api (>=1.19.0,<2.0.0)
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (>=1.19.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation-requests (>=0.40b0,<0.41)
+Requires-Dist: opentelemetry-sdk (>=1.19.0,<2.0.0)
 Description-Content-Type: text/markdown
```

