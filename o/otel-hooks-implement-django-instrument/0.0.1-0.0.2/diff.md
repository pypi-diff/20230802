# Comparing `tmp/otel_hooks_implement_django_instrument-0.0.1-py3-none-any.whl.zip` & `tmp/otel_hooks_implement_django_instrument-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 3836 bytes, number of entries: 11
+Zip file size: 3845 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx        0 b- defN 23-Aug-02 02:48 tracing/__init__.py
 -rw-rw-r--  2.0 unx      238 b- defN 23-Aug-02 02:48 tracing/decorators.py
 -rw-rw-r--  2.0 unx     1936 b- defN 23-Aug-02 02:48 tracing/hooks.py
--rw-rw-r--  2.0 unx      855 b- defN 23-Aug-02 03:13 tracing/implementation_otel_hooks.py
+-rw-rw-r--  2.0 unx      871 b- defN 23-Aug-02 03:33 tracing/implementation_otel_hooks.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Aug-02 02:48 tracing/utils.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-Aug-02 02:48 tracing/tracers/__init__.py
 -rw-rw-r--  2.0 unx      675 b- defN 23-Aug-02 02:48 tracing/tracers/jaeger.py
--rw-rw-r--  2.0 unx      950 b- defN 23-Aug-02 03:19 otel_hooks_implement_django_instrument-0.0.1.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Aug-02 03:19 otel_hooks_implement_django_instrument-0.0.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx        8 b- defN 23-Aug-02 03:19 otel_hooks_implement_django_instrument-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      967 b- defN 23-Aug-02 03:19 otel_hooks_implement_django_instrument-0.0.1.dist-info/RECORD
-11 files, 5721 bytes uncompressed, 2154 bytes compressed:  62.3%
+-rw-rw-r--  2.0 unx      950 b- defN 23-Aug-02 03:34 otel_hooks_implement_django_instrument-0.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Aug-02 03:34 otel_hooks_implement_django_instrument-0.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        8 b- defN 23-Aug-02 03:34 otel_hooks_implement_django_instrument-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      967 b- defN 23-Aug-02 03:34 otel_hooks_implement_django_instrument-0.0.2.dist-info/RECORD
+11 files, 5737 bytes uncompressed, 2163 bytes compressed:  62.3%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: tracing/tracers/__init__.py
 Comment: 
 
 Filename: tracing/tracers/jaeger.py
 Comment: 
 
-Filename: otel_hooks_implement_django_instrument-0.0.1.dist-info/METADATA
+Filename: otel_hooks_implement_django_instrument-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: otel_hooks_implement_django_instrument-0.0.1.dist-info/WHEEL
+Filename: otel_hooks_implement_django_instrument-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: otel_hooks_implement_django_instrument-0.0.1.dist-info/top_level.txt
+Filename: otel_hooks_implement_django_instrument-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: otel_hooks_implement_django_instrument-0.0.1.dist-info/RECORD
+Filename: otel_hooks_implement_django_instrument-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tracing/implementation_otel_hooks.py

```diff
@@ -1,13 +1,13 @@
 import logging
-from hooks import log_hook, name_callback, otel_request_hook, span_callback, otel_response_hook
+from tracing.hooks import log_hook, name_callback, otel_request_hook, span_callback, otel_response_hook
 from opentelemetry.instrumentation.django import DjangoInstrumentor
 from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from opentelemetry.instrumentation.logging import LoggingInstrumentor
-from tracers.jaeger import provider
+from tracing.tracers.jaeger import provider
 
 
 def implement():
     DjangoInstrumentor().instrument(
         tracer_provider=provider,
         request_hook=otel_request_hook,
         response_hook=otel_response_hook
```

## Comparing `otel_hooks_implement_django_instrument-0.0.1.dist-info/METADATA` & `otel_hooks_implement_django_instrument-0.0.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otel-hooks-implement-django-instrument
-Version: 0.0.1
+Version: 0.0.2
 Summary: Implement hooks for opentelemetry-instrument
 Home-page: UNKNOWN
 Author: Huy Nguyen Dinh
 Author-email: huyn27316@gmail.com
 Maintainer: Huy Nguyen Dinh
 Maintainer-email: huyn27316@gmail.com
 License: BSD
```

## Comparing `otel_hooks_implement_django_instrument-0.0.1.dist-info/RECORD` & `otel_hooks_implement_django_instrument-0.0.2.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 tracing/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tracing/decorators.py,sha256=5Fcoyx5BCJW-oCd0DkTSP7MkAh8Qt9-7_nShWREl_RI,238
 tracing/hooks.py,sha256=rKKawHs5H80qLqPdRFv15Za8nn58YXeAEDMZ7QGhEGI,1936
-tracing/implementation_otel_hooks.py,sha256=psFg9jFyVm5MheQlENN0E4AixAytrqh7I7pptPN4aSM,855
+tracing/implementation_otel_hooks.py,sha256=hd78lu1kMKupJWudTQFcubHlMtNPosQIXYdHD0TitYY,871
 tracing/utils.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tracing/tracers/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tracing/tracers/jaeger.py,sha256=IRn_eb3hJxacvp-GEf8NVimmoBR1uaRbI6JXYvRYVuU,675
-otel_hooks_implement_django_instrument-0.0.1.dist-info/METADATA,sha256=_5wPr0igiCT4uy9uGHmGt_LvFjIwum4t9TikobpMlaU,950
-otel_hooks_implement_django_instrument-0.0.1.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-otel_hooks_implement_django_instrument-0.0.1.dist-info/top_level.txt,sha256=a_PXcpVC6M1lHYEmd8LmQBu5NUflPrcU4wXQmpeGgxk,8
-otel_hooks_implement_django_instrument-0.0.1.dist-info/RECORD,,
+otel_hooks_implement_django_instrument-0.0.2.dist-info/METADATA,sha256=uNSgr0esFaf_e4MckTQ0zaAuQJ1jZAm6hmwUTnoAte8,950
+otel_hooks_implement_django_instrument-0.0.2.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+otel_hooks_implement_django_instrument-0.0.2.dist-info/top_level.txt,sha256=a_PXcpVC6M1lHYEmd8LmQBu5NUflPrcU4wXQmpeGgxk,8
+otel_hooks_implement_django_instrument-0.0.2.dist-info/RECORD,,
```

