# Comparing `tmp/traceloop_sdk-0.0.4.tar.gz` & `tmp/traceloop_sdk-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "traceloop_sdk-0.0.4.tar", max compression
+gzip compressed data, was "traceloop_sdk-0.0.5.tar", max compression
```

## Comparing `traceloop_sdk-0.0.4.tar` & `traceloop_sdk-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-08-02 09:25:16.062473 traceloop_sdk-0.0.4/README.md
--rw-r--r--   0        0        0      562 2023-08-02 14:04:11.214099 traceloop_sdk-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-02 13:35:06.247470 traceloop_sdk-0.0.4/traceloop/__init__.py
--rw-r--r--   0        0        0        0 2023-08-01 13:29:56.846025 traceloop_sdk-0.0.4/traceloop/agent/__init__.py
--rw-r--r--   0        0        0      238 2023-08-01 13:49:46.129127 traceloop_sdk-0.0.4/traceloop/agent/decorator.py
--rw-r--r--   0        0        0        0 2023-08-01 13:30:02.778279 traceloop_sdk-0.0.4/traceloop/agent/tool/__init__.py
--rw-r--r--   0        0        0      236 2023-08-01 14:31:03.279362 traceloop_sdk-0.0.4/traceloop/agent/tool/decorator.py
--rw-r--r--   0        0        0        0 2023-08-02 13:18:36.291777 traceloop_sdk-0.0.4/traceloop/instrumentation/__init__.py
--rw-r--r--   0        0        0    11253 2023-08-02 13:37:44.238046 traceloop_sdk-0.0.4/traceloop/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0       37 2023-08-02 13:35:46.090364 traceloop_sdk-0.0.4/traceloop/instrumentation/openai/package.py
--rw-r--r--   0        0        0      239 2023-08-01 13:41:08.608117 traceloop_sdk-0.0.4/traceloop/semconv/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 15:13:41.585793 traceloop_sdk-0.0.4/traceloop/task/__init__.py
--rw-r--r--   0        0        0      729 2023-08-01 14:01:15.919064 traceloop_sdk-0.0.4/traceloop/task/decorator.py
--rw-r--r--   0        0        0        0 2023-07-30 15:42:25.834193 traceloop_sdk-0.0.4/traceloop/tracing/__init__.py
--rw-r--r--   0        0        0     1419 2023-08-02 14:03:30.448209 traceloop_sdk-0.0.4/traceloop/tracing/tracer.py
--rw-r--r--   0        0        0        0 2023-08-01 09:57:19.484179 traceloop_sdk-0.0.4/traceloop/workflow/__init__.py
--rw-r--r--   0        0        0      644 2023-08-01 14:01:15.916149 traceloop_sdk-0.0.4/traceloop/workflow/decorator.py
--rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 traceloop_sdk-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-02 09:25:16.062473 traceloop_sdk-0.0.5/README.md
+-rw-r--r--   0        0        0      562 2023-08-02 14:21:32.936165 traceloop_sdk-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 13:35:06.247470 traceloop_sdk-0.0.5/traceloop/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:29:56.846025 traceloop_sdk-0.0.5/traceloop/agent/__init__.py
+-rw-r--r--   0        0        0      238 2023-08-01 13:49:46.129127 traceloop_sdk-0.0.5/traceloop/agent/decorator.py
+-rw-r--r--   0        0        0        0 2023-08-01 13:30:02.778279 traceloop_sdk-0.0.5/traceloop/agent/tool/__init__.py
+-rw-r--r--   0        0        0      236 2023-08-01 14:31:03.279362 traceloop_sdk-0.0.5/traceloop/agent/tool/decorator.py
+-rw-r--r--   0        0        0        0 2023-08-02 13:18:36.291777 traceloop_sdk-0.0.5/traceloop/instrumentation/__init__.py
+-rw-r--r--   0        0        0    11253 2023-08-02 13:37:44.238046 traceloop_sdk-0.0.5/traceloop/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0       37 2023-08-02 13:35:46.090364 traceloop_sdk-0.0.5/traceloop/instrumentation/openai/package.py
+-rw-r--r--   0        0        0      239 2023-08-01 13:41:08.608117 traceloop_sdk-0.0.5/traceloop/semconv/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:13:41.585793 traceloop_sdk-0.0.5/traceloop/task/__init__.py
+-rw-r--r--   0        0        0      729 2023-08-01 14:01:15.919064 traceloop_sdk-0.0.5/traceloop/task/decorator.py
+-rw-r--r--   0        0        0        0 2023-07-30 15:42:25.834193 traceloop_sdk-0.0.5/traceloop/tracing/__init__.py
+-rw-r--r--   0        0        0     1508 2023-08-02 14:21:19.769574 traceloop_sdk-0.0.5/traceloop/tracing/tracer.py
+-rw-r--r--   0        0        0        0 2023-08-01 09:57:19.484179 traceloop_sdk-0.0.5/traceloop/workflow/__init__.py
+-rw-r--r--   0        0        0      644 2023-08-01 14:01:15.916149 traceloop_sdk-0.0.5/traceloop/workflow/decorator.py
+-rw-r--r--   0        0        0      676 1970-01-01 00:00:00.000000 traceloop_sdk-0.0.5/PKG-INFO
```

### Comparing `traceloop_sdk-0.0.4/pyproject.toml` & `traceloop_sdk-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "traceloop-sdk"
-version = "0.0.4"
+version = "0.0.5"
 description = ""
 authors = ["Gal Kleinman <gal@traceloop.com>", "Nir Gazit <nir@traceloop.com>", "Tomer Friedman <tomer@traceloop.com>"]
 readme = "README.md"
 packages = [{include = "traceloop"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `traceloop_sdk-0.0.4/traceloop/instrumentation/openai/__init__.py` & `traceloop_sdk-0.0.5/traceloop/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.4/traceloop/task/decorator.py` & `traceloop_sdk-0.0.5/traceloop/task/decorator.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.4/traceloop/tracing/tracer.py` & `traceloop_sdk-0.0.5/traceloop/tracing/tracer.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,17 @@
                 "Authorization": f"Bearer {api_key}",
             }
         )
         processor = BatchSpanProcessor(exporter)
         provider.add_span_processor(processor)
         trace.set_tracer_provider(provider)
         Tracer.__instance = trace.get_tracer(TRACER_NAME)
+
+        os.environ["OTEL_PYTHON_REQUESTS_EXCLUDED_URLS"] = "https://api.openai.com/.*"
+
         OpenAIInstrumentor().instrument()
         RequestsInstrumentor().instrument()
 
     @staticmethod
     def instance():
         if Tracer.__instance is None:
             raise Exception("Tracer is not initialized")
```

### Comparing `traceloop_sdk-0.0.4/traceloop/workflow/decorator.py` & `traceloop_sdk-0.0.5/traceloop/workflow/decorator.py`

 * *Files identical despite different names*

### Comparing `traceloop_sdk-0.0.4/PKG-INFO` & `traceloop_sdk-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: traceloop-sdk
-Version: 0.0.4
+Version: 0.0.5
 Summary: 
 Author: Gal Kleinman
 Author-email: gal@traceloop.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

