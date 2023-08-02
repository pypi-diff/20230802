# Comparing `tmp/traceloop_sdk-0.0.1.tar.gz` & `tmp/traceloop_sdk-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceloop_sdk-0.0.1.tar", max compression
+gzip compressed data, was "traceloop_sdk-0.0.2.tar", max compression
```

## Comparing `traceloop_sdk-0.0.1.tar` & `traceloop_sdk-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0        0 2023-08-02 09:25:16.062473 traceloop_sdk-0.0.1/README.md
--rw-r--r--   0        0        0      477 2023-08-02 09:26:20.035292 traceloop_sdk-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-30 14:54:26.714515 traceloop_sdk-0.0.1/traceloop/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:29:56.846025 traceloop_sdk-0.0.1/traceloop/agent/__init__.py
--rw-r--r--   0        0        0      238 2023-08-01 13:49:46.129127 traceloop_sdk-0.0.1/traceloop/agent/decorator.py
--rw-r--r--   0        0        0        0 2023-08-01 13:30:02.778279 traceloop_sdk-0.0.1/traceloop/agent/tool/__init__.py
--rw-r--r--   0        0        0      236 2023-08-01 14:31:03.279362 traceloop_sdk-0.0.1/traceloop/agent/tool/decorator.py
--rw-r--r--   0        0        0      239 2023-08-01 13:41:08.608117 traceloop_sdk-0.0.1/traceloop/semconv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 15:13:41.585793 traceloop_sdk-0.0.1/traceloop/task/__init__.py
--rw-r--r--   0        0        0      729 2023-08-01 14:01:15.919064 traceloop_sdk-0.0.1/traceloop/task/decorator.py
--rw-r--r--   0        0        0        0 2023-07-30 15:42:25.834193 traceloop_sdk-0.0.1/traceloop/tracing/__init__.py
--rw-r--r--   0        0        0     1299 2023-08-01 14:51:28.099690 traceloop_sdk-0.0.1/traceloop/tracing/tracer.py
--rw-r--r--   0        0        0        0 2023-08-01 09:57:19.484179 traceloop_sdk-0.0.1/traceloop/workflow/__init__.py
--rw-r--r--   0        0        0      644 2023-08-01 14:01:15.916149 traceloop_sdk-0.0.1/traceloop/workflow/decorator.py
--rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 traceloop_sdk-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 09:25:16.062473 traceloop_sdk-0.0.2/README.md
+-rw-r--r--   0        0        0      550 2023-08-02 11:48:51.166183 traceloop_sdk-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-30 14:54:26.714515 traceloop_sdk-0.0.2/traceloop/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:29:56.846025 traceloop_sdk-0.0.2/traceloop/agent/__init__.py
+-rw-r--r--   0        0        0      238 2023-08-01 13:49:46.129127 traceloop_sdk-0.0.2/traceloop/agent/decorator.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:30:02.778279 traceloop_sdk-0.0.2/traceloop/agent/tool/__init__.py
+-rw-r--r--   0        0        0      236 2023-08-01 14:31:03.279362 traceloop_sdk-0.0.2/traceloop/agent/tool/decorator.py
+-rw-r--r--   0        0        0      239 2023-08-01 13:41:08.608117 traceloop_sdk-0.0.2/traceloop/semconv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:13:41.585793 traceloop_sdk-0.0.2/traceloop/task/__init__.py
+-rw-r--r--   0        0        0      729 2023-08-01 14:01:15.919064 traceloop_sdk-0.0.2/traceloop/task/decorator.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:42:25.834193 traceloop_sdk-0.0.2/traceloop/tracing/__init__.py
+-rw-r--r--   0        0        0     1298 2023-08-02 11:47:53.513752 traceloop_sdk-0.0.2/traceloop/tracing/tracer.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:57:19.484179 traceloop_sdk-0.0.2/traceloop/workflow/__init__.py
+-rw-r--r--   0        0        0      644 2023-08-01 14:01:15.916149 traceloop_sdk-0.0.2/traceloop/workflow/decorator.py
+-rw-r--r--   0        0        0      641 1970-01-01 00:00:00.000000 traceloop_sdk-0.0.2/PKG-INFO
```

### Comparing `traceloop_sdk-0.0.1/traceloop/task/decorator.py` & `traceloop_sdk-0.0.2/traceloop/task/decorator.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.1/traceloop/tracing/tracer.py` & `traceloop_sdk-0.0.2/traceloop/tracing/tracer.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 from opentelemetry import trace
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 from opentelemetry.instrumentation.openai import OpenAIInstrumentor
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
 
 TRACER_NAME = "traceloop.tracer"
-TRACELOOP_API_ENDPOINT = "https://api.traceloop.io/v1/traces"
+TRACELOOP_API_ENDPOINT = "https://api.traceloop.dev/v1/traces"
 
 
 class Tracer:
     __instance = None
 
     @staticmethod
     def init():
         api_key = os.getenv("TRACELOOP_API_KEY")
-        traceloop_api_endpoint = os.getenv("TRACELOOP_API_ENDPOINT") if os.getenv(
-            "TRACELOOP_API_ENDPOINT") else TRACELOOP_API_ENDPOINT
+        api_endpoint = os.getenv("TRACELOOP_API_ENDPOINT") or TRACELOOP_API_ENDPOINT
+        print(f"Initializing Tracer with API endpoint: {api_endpoint}")
         provider = TracerProvider()
         exporter = OTLPSpanExporter(
-            endpoint=TRACELOOP_API_ENDPOINT,
+            endpoint=api_endpoint,
             headers={
                 "Authorization": f"Bearer {api_key}",
             }
         )
         processor = BatchSpanProcessor(exporter)
         provider.add_span_processor(processor)
         trace.set_tracer_provider(provider)
```

### Comparing `traceloop_sdk-0.0.1/traceloop/workflow/decorator.py` & `traceloop_sdk-0.0.2/traceloop/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.1/PKG-INFO` & `traceloop_sdk-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceloop-sdk
-Version: 0.0.1
+Version: 0.0.2
 Summary: 
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

