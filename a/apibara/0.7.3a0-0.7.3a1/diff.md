# Comparing `tmp/apibara-0.7.3a0.tar.gz` & `tmp/apibara-0.7.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apibara-0.7.3a0.tar", max compression
+gzip compressed data, was "apibara-0.7.3a1.tar", max compression
```

## Comparing `apibara-0.7.3a0.tar` & `apibara-0.7.3a1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.7.3a0/LICENSE.txt
--rw-r--r--   0        0        0     1685 2023-07-24 14:46:53.473584 apibara-0.7.3a0/README.rst
--rw-r--r--   0        0        0     1270 2023-08-01 21:06:19.587210 apibara-0.7.3a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-01 16:15:25.550565 apibara-0.7.3a0/src/apibara/__init__.py
--rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.7.3a0/src/apibara/cursor.py
--rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.7.3a0/src/apibara/indexer/__init__.py
--rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.7.3a0/src/apibara/indexer/configuration.py
--rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.7.3a0/src/apibara/indexer/indexer.py
--rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.7.3a0/src/apibara/indexer/info.py
--rw-r--r--   0        0        0    12063 2023-08-01 21:01:19.923132 apibara-0.7.3a0/src/apibara/indexer/runner.py
--rw-r--r--   0        0        0    10502 2023-06-08 12:55:13.026953 apibara-0.7.3a0/src/apibara/indexer/storage.py
--rw-r--r--   0        0        0      687 2023-07-24 14:46:53.473584 apibara-0.7.3a0/src/apibara/protocol/__init__.py
--rw-r--r--   0        0        0     4424 2023-08-01 19:15:18.318533 apibara-0.7.3a0/src/apibara/protocol/client.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/protocol/proto/__init__.py
--rw-r--r--   0        0        0     3450 2023-08-01 21:01:03.928913 apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2.py
--rw-r--r--   0        0        0     3608 2023-08-01 19:15:20.623565 apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2.pyi
--rw-r--r--   0        0        0     4147 2023-08-01 21:00:10.094174 apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2_grpc.py
--rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2_grpc.pyi
--rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/__init__.py
--rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/cursor.py
--rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/felt.py
--rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.7.3a0/src/apibara/starknet/filter.py
--rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/indexer.py
--rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/__init__.py
--rw-r--r--   0        0        0     8286 2023-08-01 21:01:03.955913 apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2.py
--rw-r--r--   0        0        0    12814 2023-08-01 21:00:10.076174 apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2_grpc.pyi
--rw-r--r--   0        0        0    12370 2023-08-01 21:01:03.974914 apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2.py
--rw-r--r--   0        0        0    20350 2023-08-01 21:00:10.084174 apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2_grpc.py
--rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
--rw-r--r--   0        0        0     1138 2023-08-01 21:01:03.911913 apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2.py
--rw-r--r--   0        0        0      732 2023-08-01 19:15:20.609564 apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2.pyi
--rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2_grpc.py
--rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2_grpc.pyi
--rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 apibara-0.7.3a0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-01-15 18:52:09.124336 apibara-0.7.3a1/LICENSE.txt
+-rw-r--r--   0        0        0     1685 2023-07-24 14:46:53.473584 apibara-0.7.3a1/README.rst
+-rw-r--r--   0        0        0     1270 2023-08-01 23:00:08.138832 apibara-0.7.3a1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-01 16:15:25.550565 apibara-0.7.3a1/src/apibara/__init__.py
+-rw-r--r--   0        0        0      514 2023-01-15 18:52:09.124336 apibara-0.7.3a1/src/apibara/cursor.py
+-rw-r--r--   0        0        0      160 2023-01-15 18:52:09.124336 apibara-0.7.3a1/src/apibara/indexer/__init__.py
+-rw-r--r--   0        0        0      375 2023-01-15 18:52:09.124336 apibara-0.7.3a1/src/apibara/indexer/configuration.py
+-rw-r--r--   0        0        0     2393 2023-03-16 21:14:54.127582 apibara-0.7.3a1/src/apibara/indexer/indexer.py
+-rw-r--r--   0        0        0     1026 2023-01-16 18:48:50.663792 apibara-0.7.3a1/src/apibara/indexer/info.py
+-rw-r--r--   0        0        0    12082 2023-08-01 22:55:03.643832 apibara-0.7.3a1/src/apibara/indexer/runner.py
+-rw-r--r--   0        0        0    10502 2023-06-08 12:55:13.026953 apibara-0.7.3a1/src/apibara/indexer/storage.py
+-rw-r--r--   0        0        0      687 2023-07-24 14:46:53.473584 apibara-0.7.3a1/src/apibara/protocol/__init__.py
+-rw-r--r--   0        0        0     4424 2023-08-01 19:15:18.318533 apibara-0.7.3a1/src/apibara/protocol/client.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/protocol/proto/__init__.py
+-rw-r--r--   0        0        0     3450 2023-08-01 21:01:03.928913 apibara-0.7.3a1/src/apibara/protocol/proto/stream_pb2.py
+-rw-r--r--   0        0        0     3608 2023-08-01 19:15:20.623565 apibara-0.7.3a1/src/apibara/protocol/proto/stream_pb2.pyi
+-rw-r--r--   0        0        0     4147 2023-08-01 21:00:10.094174 apibara-0.7.3a1/src/apibara/protocol/proto/stream_pb2_grpc.py
+-rw-r--r--   0        0        0      878 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/protocol/proto/stream_pb2_grpc.pyi
+-rw-r--r--   0        0        0      264 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/__init__.py
+-rw-r--r--   0        0        0     1038 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/cursor.py
+-rw-r--r--   0        0        0     1375 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/felt.py
+-rw-r--r--   0        0        0    14725 2023-03-16 21:14:54.127582 apibara-0.7.3a1/src/apibara/starknet/filter.py
+-rw-r--r--   0        0        0      404 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/indexer.py
+-rw-r--r--   0        0        0        0 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/proto/__init__.py
+-rw-r--r--   0        0        0     8286 2023-08-01 21:01:03.955913 apibara-0.7.3a1/src/apibara/starknet/proto/filter_pb2.py
+-rw-r--r--   0        0        0    12814 2023-08-01 21:00:10.076174 apibara-0.7.3a1/src/apibara/starknet/proto/filter_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/proto/filter_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/proto/filter_pb2_grpc.pyi
+-rw-r--r--   0        0        0    12370 2023-08-01 21:01:03.974914 apibara-0.7.3a1/src/apibara/starknet/proto/starknet_pb2.py
+-rw-r--r--   0        0        0    20350 2023-08-01 21:00:10.084174 apibara-0.7.3a1/src/apibara/starknet/proto/starknet_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/proto/starknet_pb2_grpc.py
+-rw-r--r--   0        0        0      100 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/proto/starknet_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1138 2023-08-01 21:01:03.911913 apibara-0.7.3a1/src/apibara/starknet/proto/types_pb2.py
+-rw-r--r--   0        0        0      732 2023-08-01 19:15:20.609564 apibara-0.7.3a1/src/apibara/starknet/proto/types_pb2.pyi
+-rw-r--r--   0        0        0      158 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/proto/types_pb2_grpc.py
+-rw-r--r--   0        0        0       76 2023-01-15 18:52:09.125336 apibara-0.7.3a1/src/apibara/starknet/proto/types_pb2_grpc.pyi
+-rw-r--r--   0        0        0     2753 1970-01-01 00:00:00.000000 apibara-0.7.3a1/PKG-INFO
```

### Comparing `apibara-0.7.3a0/LICENSE.txt` & `apibara-0.7.3a1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/README.rst` & `apibara-0.7.3a1/README.rst`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/pyproject.toml` & `apibara-0.7.3a1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apibara"
-version = "0.7.3a0"
+version = "0.7.3a1"
 description = "Apibara cliend SDK. Stream and transform on-chain data with Python."
 authors = ["Francesco Ceccon <francesco@apibara.com>"]
 license = "Apache-2.0"
 readme = "README.rst"
 homepage = "https://www.apibara.com"
 repository= "https://github.com/apibara/python-sdk"
 keywords = [
```

### Comparing `apibara-0.7.3a0/src/apibara/cursor.py` & `apibara-0.7.3a1/src/apibara/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/indexer/indexer.py` & `apibara-0.7.3a1/src/apibara/indexer/indexer.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/indexer/info.py` & `apibara-0.7.3a1/src/apibara/indexer/info.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/indexer/runner.py` & `apibara-0.7.3a1/src/apibara/indexer/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,15 +264,15 @@
                                 batch_size=1,
                             )
 
                 if not is_pending:
                     previous_end_cursor = message.data.end_cursor
 
                 if self._reconnect_to_avoid_disconnection is not None:
-                    if _blocks_before_reconnect <= 0:
+                    if _blocks_before_reconnect <= 0 and not is_pending:
                         _blocks_before_reconnect = (
                             self._reconnect_to_avoid_disconnection
                         )
                         await client.configure(
                             filter=config.filter.encode(),
                             finality=config.finality,
                             cursor=end_cursor,
```

### Comparing `apibara-0.7.3a0/src/apibara/indexer/storage.py` & `apibara-0.7.3a1/src/apibara/indexer/storage.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/protocol/__init__.py` & `apibara-0.7.3a1/src/apibara/protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/protocol/client.py` & `apibara-0.7.3a1/src/apibara/protocol/client.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2.py` & `apibara-0.7.3a1/src/apibara/protocol/proto/stream_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2.pyi` & `apibara-0.7.3a1/src/apibara/protocol/proto/stream_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2_grpc.py` & `apibara-0.7.3a1/src/apibara/protocol/proto/stream_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/protocol/proto/stream_pb2_grpc.pyi` & `apibara-0.7.3a1/src/apibara/protocol/proto/stream_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/cursor.py` & `apibara-0.7.3a1/src/apibara/starknet/cursor.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/felt.py` & `apibara-0.7.3a1/src/apibara/starknet/felt.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/filter.py` & `apibara-0.7.3a1/src/apibara/starknet/filter.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2.py` & `apibara-0.7.3a1/src/apibara/starknet/proto/filter_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/proto/filter_pb2.pyi` & `apibara-0.7.3a1/src/apibara/starknet/proto/filter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2.py` & `apibara-0.7.3a1/src/apibara/starknet/proto/starknet_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/proto/starknet_pb2.pyi` & `apibara-0.7.3a1/src/apibara/starknet/proto/starknet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2.py` & `apibara-0.7.3a1/src/apibara/starknet/proto/types_pb2.py`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/src/apibara/starknet/proto/types_pb2.pyi` & `apibara-0.7.3a1/src/apibara/starknet/proto/types_pb2.pyi`

 * *Files identical despite different names*

### Comparing `apibara-0.7.3a0/PKG-INFO` & `apibara-0.7.3a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apibara
-Version: 0.7.3a0
+Version: 0.7.3a1
 Summary: Apibara cliend SDK. Stream and transform on-chain data with Python.
 Home-page: https://www.apibara.com
 License: Apache-2.0
 Keywords: ethereum,web3,starknet
 Author: Francesco Ceccon
 Author-email: francesco@apibara.com
 Requires-Python: >=3.8,<3.11
```

