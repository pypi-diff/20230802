# Comparing `tmp/pulsar_sdk_py-0.1.1.tar.gz` & `tmp/pulsar_sdk_py-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulsar_sdk_py-0.1.1.tar", max compression
+gzip compressed data, was "pulsar_sdk_py-0.1.2.tar", max compression
```

## Comparing `pulsar_sdk_py-0.1.1.tar` & `pulsar_sdk_py-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-08-01 12:08:43.850947 pulsar_sdk_py-0.1.1/README.md
--rw-r--r--   0        0        0       34 2023-07-31 15:53:29.875987 pulsar_sdk_py-0.1.1/pulsar_sdk_py/__init__.py
--rw-r--r--   0        0        0     6326 2023-07-31 15:18:34.164193 pulsar_sdk_py-0.1.1/pulsar_sdk_py/enums.py
--rw-r--r--   0        0        0      140 2023-07-26 10:51:45.846061 pulsar_sdk_py-0.1.1/pulsar_sdk_py/exceptions.py
--rw-r--r--   0        0        0      634 2023-07-26 10:51:45.846131 pulsar_sdk_py-0.1.1/pulsar_sdk_py/helpers.py
--rw-r--r--   0        0        0    25958 2023-08-01 12:01:12.738885 pulsar_sdk_py-0.1.1/pulsar_sdk_py/pulsar_sdk.py
--rw-r--r--   0        0        0        0 2023-07-26 10:51:45.846396 pulsar_sdk_py-0.1.1/pulsar_sdk_py/schemas/__init__.py
--rw-r--r--   0        0        0    10286 2023-08-01 11:49:34.806474 pulsar_sdk_py-0.1.1/pulsar_sdk_py/schemas/schemas.py
--rw-r--r--   0        0        0     1283 2023-07-31 15:21:39.102392 pulsar_sdk_py-0.1.1/pulsar_sdk_py/schemas/serializer.py
--rw-r--r--   0        0        0      572 2023-08-01 12:03:10.879445 pulsar_sdk_py-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 pulsar_sdk_py-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-01 12:08:43.850947 pulsar_sdk_py-0.1.2/README.md
+-rw-r--r--   0        0        0       34 2023-07-31 15:53:29.875987 pulsar_sdk_py-0.1.2/pulsar_sdk_py/__init__.py
+-rw-r--r--   0        0        0     6326 2023-07-31 15:18:34.164193 pulsar_sdk_py-0.1.2/pulsar_sdk_py/enums.py
+-rw-r--r--   0        0        0      140 2023-07-26 10:51:45.846061 pulsar_sdk_py-0.1.2/pulsar_sdk_py/exceptions.py
+-rw-r--r--   0        0        0      634 2023-07-26 10:51:45.846131 pulsar_sdk_py-0.1.2/pulsar_sdk_py/helpers.py
+-rw-r--r--   0        0        0    25965 2023-08-01 12:11:48.834609 pulsar_sdk_py-0.1.2/pulsar_sdk_py/pulsar_sdk.py
+-rw-r--r--   0        0        0        0 2023-07-26 10:51:45.846396 pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/__init__.py
+-rw-r--r--   0        0        0    10286 2023-08-01 12:12:00.824832 pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/schemas.py
+-rw-r--r--   0        0        0     1283 2023-07-31 15:21:39.102392 pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/serializer.py
+-rw-r--r--   0        0        0      572 2023-08-02 17:59:50.429845 pulsar_sdk_py-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1556 1970-01-01 00:00:00.000000 pulsar_sdk_py-0.1.2/PKG-INFO
```

### Comparing `pulsar_sdk_py-0.1.1/README.md` & `pulsar_sdk_py-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-0.1.1/pulsar_sdk_py/enums.py` & `pulsar_sdk_py-0.1.2/pulsar_sdk_py/enums.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-0.1.1/pulsar_sdk_py/helpers.py` & `pulsar_sdk_py-0.1.2/pulsar_sdk_py/helpers.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-0.1.1/pulsar_sdk_py/pulsar_sdk.py` & `pulsar_sdk_py-0.1.2/pulsar_sdk_py/pulsar_sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,15 +408,15 @@
 
         def get_protocol(self, protocol_key: str) -> ProtocolData:
             response = self._RestClient__get_request_on_endpoint(
                 func_name="get_protocol", request_type="GET", protocol_key=protocol_key
             )
             return serialize_to_dataclass(response, ProtocolData)
 
-        def list_protocols(self, chain: ChainKeys = None) -> list[ProtocolData]:
+        def list_protocols(self, chain: ChainKeys | None = None) -> list[ProtocolData]:
             params_filtered = filter_non_empty_params(chain=chain)
             response = self._RestClient__get_request_on_endpoint(
                 func_name="list_protocols", request_type="GET", **params_filtered
             )
             return [serialize_to_dataclass(protocol, ProtocolData) for protocol in response]
 
         def get_number_protocols(self) -> int:
```

### Comparing `pulsar_sdk_py-0.1.1/pulsar_sdk_py/schemas/schemas.py` & `pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/schemas.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-0.1.1/pulsar_sdk_py/schemas/serializer.py` & `pulsar_sdk_py-0.1.2/pulsar_sdk_py/schemas/serializer.py`

 * *Files identical despite different names*

### Comparing `pulsar_sdk_py-0.1.1/pyproject.toml` & `pulsar_sdk_py-0.1.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pulsar-sdk-py"
-version = "0.1.1"
+version = "0.1.2"
 description = ""
 authors = [ "Pulsar <admin@pulsar.finance>",]
 readme = "README.md"
 packages = [
     {include = "pulsar_sdk_py"},
 ]
```

### Comparing `pulsar_sdk_py-0.1.1/PKG-INFO` & `pulsar_sdk_py-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulsar-sdk-py
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Pulsar
 Author-email: admin@pulsar.finance
 Requires-Python: >=3.11.0,<3.12.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
```

