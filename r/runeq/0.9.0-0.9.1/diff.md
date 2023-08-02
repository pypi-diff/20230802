# Comparing `tmp/runeq-0.9.0.tar.gz` & `tmp/runeq-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runeq-0.9.0.tar", last modified: Thu Sep 29 14:46:47 2022, max compression
+gzip compressed data, was "runeq-0.9.1.tar", last modified: Tue Nov 22 12:38:53 2022, max compression
```

## Comparing `runeq-0.9.0.tar` & `runeq-0.9.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.497004 runeq-0.9.0/
--rw-r--r--   0 cranti     (501) wheel        (0)     1066 2022-09-29 14:46:14.000000 runeq-0.9.0/LICENSE
--rw-r--r--   0 cranti     (501) wheel        (0)     1672 2022-09-29 14:46:47.496703 runeq-0.9.0/PKG-INFO
--rw-r--r--   0 cranti     (501) wheel        (0)      971 2022-09-29 14:46:14.000000 runeq-0.9.0/README.md
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.483222 runeq-0.9.0/cli/
--rwxr-xr-x   0 cranti     (501) wheel        (0)     3633 2022-09-29 14:46:14.000000 runeq-0.9.0/cli/__init__.py
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.484195 runeq-0.9.0/runeq/
--rw-r--r--   0 cranti     (501) wheel        (0)      239 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/__init__.py
--rw-r--r--   0 cranti     (501) wheel        (0)     7267 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/config.py
--rw-r--r--   0 cranti     (501) wheel        (0)      743 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/errors.py
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.489266 runeq-0.9.0/runeq/resources/
--rw-r--r--   0 cranti     (501) wheel        (0)      573 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/resources/__init__.py
--rw-r--r--   0 cranti     (501) wheel        (0)     7229 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/resources/client.py
--rw-r--r--   0 cranti     (501) wheel        (0)     5414 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/resources/common.py
--rw-r--r--   0 cranti     (501) wheel        (0)     4767 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/resources/org.py
--rw-r--r--   0 cranti     (501) wheel        (0)    14560 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/resources/patient.py
--rw-r--r--   0 cranti     (501) wheel        (0)     7741 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/resources/stream.py
--rw-r--r--   0 cranti     (501) wheel        (0)    40485 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/resources/stream_metadata.py
--rw-r--r--   0 cranti     (501) wheel        (0)     2724 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/resources/user.py
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.490135 runeq-0.9.0/runeq/stream/
--rw-r--r--   0 cranti     (501) wheel        (0)       83 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/stream/__init__.py
--rw-r--r--   0 cranti     (501) wheel        (0)    15093 2022-09-29 14:46:14.000000 runeq-0.9.0/runeq/stream/v1.py
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.486411 runeq-0.9.0/runeq.egg-info/
--rw-r--r--   0 cranti     (501) wheel        (0)     1672 2022-09-29 14:46:47.000000 runeq-0.9.0/runeq.egg-info/PKG-INFO
--rw-r--r--   0 cranti     (501) wheel        (0)      865 2022-09-29 14:46:47.000000 runeq-0.9.0/runeq.egg-info/SOURCES.txt
--rw-r--r--   0 cranti     (501) wheel        (0)        1 2022-09-29 14:46:47.000000 runeq-0.9.0/runeq.egg-info/dependency_links.txt
--rw-r--r--   0 cranti     (501) wheel        (0)       34 2022-09-29 14:46:47.000000 runeq-0.9.0/runeq.egg-info/entry_points.txt
--rw-r--r--   0 cranti     (501) wheel        (0)       81 2022-09-29 14:46:47.000000 runeq-0.9.0/runeq.egg-info/requires.txt
--rw-r--r--   0 cranti     (501) wheel        (0)       16 2022-09-29 14:46:47.000000 runeq-0.9.0/runeq.egg-info/top_level.txt
--rw-r--r--   0 cranti     (501) wheel        (0)       38 2022-09-29 14:46:47.497084 runeq-0.9.0/setup.cfg
--rw-r--r--   0 cranti     (501) wheel        (0)     1190 2022-09-29 14:46:14.000000 runeq-0.9.0/setup.py
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.491093 runeq-0.9.0/tests/
--rw-r--r--   0 cranti     (501) wheel        (0)       33 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/__init__.py
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.495035 runeq-0.9.0/tests/resources/
--rw-r--r--   0 cranti     (501) wheel        (0)       31 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/resources/__init__.py
--rw-r--r--   0 cranti     (501) wheel        (0)     1319 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/resources/test_client.py
--rw-r--r--   0 cranti     (501) wheel        (0)     9406 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/resources/test_common.py
--rw-r--r--   0 cranti     (501) wheel        (0)     7526 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/resources/test_org.py
--rw-r--r--   0 cranti     (501) wheel        (0)    25183 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/resources/test_patient.py
--rw-r--r--   0 cranti     (501) wheel        (0)     9790 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/resources/test_stream.py
--rw-r--r--   0 cranti     (501) wheel        (0)    58283 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/resources/test_stream_metadata.py
--rw-r--r--   0 cranti     (501) wheel        (0)     3364 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/resources/test_user.py
-drwxr-xr-x   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:47.495913 runeq-0.9.0/tests/stream/
--rw-r--r--   0 cranti     (501) wheel        (0)        0 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/stream/__init__.py
--rw-r--r--   0 cranti     (501) wheel        (0)    16794 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/stream/test_v1.py
--rw-r--r--   0 cranti     (501) wheel        (0)     5028 2022-09-29 14:46:14.000000 runeq-0.9.0/tests/test_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.371748 runeq-0.9.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1066 2022-11-22 12:38:20.000000 runeq-0.9.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2015 2022-11-22 12:38:53.371748 runeq-0.9.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1314 2022-11-22 12:38:20.000000 runeq-0.9.1/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.315747 runeq-0.9.1/cli/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     3633 2022-11-22 12:38:20.000000 runeq-0.9.1/cli/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.315747 runeq-0.9.1/runeq/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7267 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      743 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/errors.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.331747 runeq-0.9.1/runeq/resources/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      573 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/resources/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7229 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/resources/client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5414 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/resources/common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4767 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/resources/org.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14560 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/resources/patient.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7741 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/resources/stream.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41040 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/resources/stream_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2724 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/resources/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.339747 runeq-0.9.1/runeq/stream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/stream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15093 2022-11-22 12:38:20.000000 runeq-0.9.1/runeq/stream/v1.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.319747 runeq-0.9.1/runeq.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2015 2022-11-22 12:38:53.000000 runeq-0.9.1/runeq.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      865 2022-11-22 12:38:53.000000 runeq-0.9.1/runeq.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2022-11-22 12:38:53.000000 runeq-0.9.1/runeq.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2022-11-22 12:38:53.000000 runeq-0.9.1/runeq.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       81 2022-11-22 12:38:53.000000 runeq-0.9.1/runeq.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2022-11-22 12:38:53.000000 runeq-0.9.1/runeq.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2022-11-22 12:38:53.371748 runeq-0.9.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1190 2022-11-22 12:38:20.000000 runeq-0.9.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.343747 runeq-0.9.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.367748 runeq-0.9.1/tests/resources/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       31 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/resources/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1319 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/resources/test_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9406 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/resources/test_common.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7526 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/resources/test_org.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25183 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/resources/test_patient.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9790 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/resources/test_stream.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61649 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/resources/test_stream_metadata.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3364 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/resources/test_user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:53.371748 runeq-0.9.1/tests/stream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/stream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16794 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/stream/test_v1.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5028 2022-11-22 12:38:20.000000 runeq-0.9.1/tests/test_config.py
```

### Comparing `runeq-0.9.0/LICENSE` & `runeq-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/PKG-INFO` & `runeq-0.9.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runeq
-Version: 0.9.0
+Version: 0.9.1
 Summary: Query data from Rune Labs APIs
 Home-page: https://github.com/rune-labs/runeq-python
 Author: Rune Labs
 Maintainer-email: support@runelabs.io
 Keywords: rune labs api query data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,7 +40,35 @@
 To install the library using pip:
 
     pip3 install runeq
 
 To install from source:
 
     python3 setup.py install
+
+## Development
+
+Initialize a virtual environment, with dev requirements installed:
+
+    make init
+
+Run tests:
+    
+    make test
+    # With coverage
+    make test-coverage
+
+Lint:
+
+    make lint
+
+Preview documentation:
+    
+    make -C docs preview
+
+Build PyPI artifact:
+
+    make build-dist
+
+Clean up ignored files/artifacts:
+
+    make clean
```

### Comparing `runeq-0.9.0/cli/__init__.py` & `runeq-0.9.1/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/config.py` & `runeq-0.9.1/runeq/config.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/errors.py` & `runeq-0.9.1/runeq/errors.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/resources/__init__.py` & `runeq-0.9.1/runeq/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/resources/client.py` & `runeq-0.9.1/runeq/resources/client.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/resources/common.py` & `runeq-0.9.1/runeq/resources/common.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/resources/org.py` & `runeq-0.9.1/runeq/resources/org.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/resources/patient.py` & `runeq-0.9.1/runeq/resources/patient.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/resources/stream.py` & `runeq-0.9.1/runeq/resources/stream.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/resources/stream_metadata.py` & `runeq-0.9.1/runeq/resources/stream_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from io import StringIO
 from typing import Callable, Iterable, Iterator, List, Optional, Type, Union
 
 import pandas as pd
 
 from .client import GraphClient, StreamClient, global_graph_client
 from .common import ItemBase, ItemSet
-from .patient import Device, Patient
+from .patient import Device, Patient, get_patient
 from .stream import get_stream_availability, get_stream_data
 from runeq.errors import RuneError
 
 
 class Dimension(ItemBase):
     """
     A dimension of a stream type. This is akin to a column in a table,
@@ -754,47 +754,53 @@
     stream_set = StreamMetadataSet()
 
     if type(stream_ids) is str:
         stream_ids = [stream_ids]
     else:
         stream_ids = list(stream_ids)
 
-    result = client.execute(
-        statement=query,
-        stream_ids=stream_ids,
-    )
+    # Query stream list in batches of <= 100 streams, since graph api cannot
+    # query for more than 100 streams at once.
+    stream_list_results = []
+    for start in range(0, len(stream_ids), 100):
+        result = client.execute(
+            statement=query,
+            stream_ids=stream_ids[start:start + 100],
+        )
+        stream_list_results.append(result)
 
     seen_stream_ids = set(stream_ids)
-    stream_list = result.get("streamListByIds", {})
-    for stream_attrs in stream_list.get("streams", []):
-        stream_type = _parse_stream_type(stream_attrs["streamType"])
-
-        del stream_attrs["streamType"]
-        norm_dev_id = Device.normalize_id(stream_attrs["device_id"])
-        stream_attrs["device_id"] = norm_dev_id
-
-        # Add query parameters to stream attributes
-        params = {}
-        if stream_attrs.get("parameters"):
-            for param in stream_attrs['parameters']:
-                stream_attrs[param["key"]] = param["value"]
-                params[param["key"]] = param["value"]
-            del stream_attrs['parameters']
-
-        stream = StreamMetadata(
-            stream_type=stream_type,
-            parameters=params,
-            **stream_attrs
-        )
-        stream_set.add(stream)
+    for result in stream_list_results:
+        stream_list = result.get("streamListByIds", {})
+        for stream_attrs in stream_list.get("streams", []):
+            stream_type = _parse_stream_type(stream_attrs["streamType"])
+
+            del stream_attrs["streamType"]
+            norm_dev_id = Device.normalize_id(stream_attrs["device_id"])
+            stream_attrs["device_id"] = norm_dev_id
+
+            # Add query parameters to stream attributes
+            params = {}
+            if stream_attrs.get("parameters"):
+                for param in stream_attrs['parameters']:
+                    stream_attrs[param["key"]] = param["value"]
+                    params[param["key"]] = param["value"]
+                del stream_attrs['parameters']
+
+            stream = StreamMetadata(
+                stream_type=stream_type,
+                parameters=params,
+                **stream_attrs
+            )
+            stream_set.add(stream)
 
-        try:
-            seen_stream_ids.remove(stream.id)
-        except KeyError:
-            pass
+            try:
+                seen_stream_ids.remove(stream.id)
+            except KeyError:
+                pass
 
     if len(seen_stream_ids) > 0:
         raise RuneError(
             f"1+ stream ID(s) not found: {','.join(seen_stream_ids)}"
         )
 
     if len(stream_set) == 1:
@@ -831,14 +837,17 @@
             API. Otherwise, the global GraphClient is used.
         **parameters: A
 
     """
     if not patient_id:
         raise ValueError("must provide a patient_id")
 
+    # Checks whether patient is accessible, otherwise raises NotFoundError.
+    get_patient(patient_id=patient_id, client=client)
+
     client = client or global_graph_client()
     query = '''
         query getStreamList($cursor: Cursor, $filters: StreamQueryFilters) {
             streamList(filters: $filters, cursor: $cursor) {
                 pageInfo {
                     endCursor
                 }
```

### Comparing `runeq-0.9.0/runeq/resources/user.py` & `runeq-0.9.1/runeq/resources/user.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq/stream/v1.py` & `runeq-0.9.1/runeq/stream/v1.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/runeq.egg-info/PKG-INFO` & `runeq-0.9.1/runeq.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runeq
-Version: 0.9.0
+Version: 0.9.1
 Summary: Query data from Rune Labs APIs
 Home-page: https://github.com/rune-labs/runeq-python
 Author: Rune Labs
 Maintainer-email: support@runelabs.io
 Keywords: rune labs api query data
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,7 +40,35 @@
 To install the library using pip:
 
     pip3 install runeq
 
 To install from source:
 
     python3 setup.py install
+
+## Development
+
+Initialize a virtual environment, with dev requirements installed:
+
+    make init
+
+Run tests:
+    
+    make test
+    # With coverage
+    make test-coverage
+
+Lint:
+
+    make lint
+
+Preview documentation:
+    
+    make -C docs preview
+
+Build PyPI artifact:
+
+    make build-dist
+
+Clean up ignored files/artifacts:
+
+    make clean
```

### Comparing `runeq-0.9.0/runeq.egg-info/SOURCES.txt` & `runeq-0.9.1/runeq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/setup.py` & `runeq-0.9.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = r.read()
 
 with open('requirements/common.txt', 'r') as r:
     install_requires = r.read().splitlines()
 
 setup(
     name=package_name,
-    version='0.9.0',
+    version='0.9.1',
     author='Rune Labs',
     maintainer_email='support@runelabs.io',
     description='Query data from Rune Labs APIs',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords='rune labs api query data',
     url='https://github.com/rune-labs/runeq-python',
```

### Comparing `runeq-0.9.0/tests/resources/test_client.py` & `runeq-0.9.1/tests/resources/test_client.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/tests/resources/test_common.py` & `runeq-0.9.1/tests/resources/test_common.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/tests/resources/test_org.py` & `runeq-0.9.1/tests/resources/test_org.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/tests/resources/test_patient.py` & `runeq-0.9.1/tests/resources/test_patient.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/tests/resources/test_stream.py` & `runeq-0.9.1/tests/resources/test_stream.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/tests/resources/test_stream_metadata.py` & `runeq-0.9.1/tests/resources/test_stream_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Tests for fetching stream metadata.
 
 """
+import copy
 import json
 from unittest import TestCase, mock
 
 from runeq.config import Config
 from runeq.resources.client import GraphClient, StreamClient
 from runeq.resources.stream_metadata import (
     Dimension, StreamMetadata, StreamMetadataSet, StreamType,
@@ -456,16 +457,112 @@
                     "max_time": 1648234860,
                     "id": "s2"
                 }
             ],
             streams.to_list(),
         )
 
+    def test_get_over_hundred_stream_metadata(self):
+        """
+        Test get stream metadata can query for >100 streams by batching
+        by requests of size <=100 streams.
+
+        """
+        self.mock_graph_client.execute = mock.Mock()
+
+        stream_resp = {
+            "created_at": 1655226140.508,
+            "algorithm": "a1",
+            "device_id": "patient-p1,device-d1",
+            "patient_id": "p1",
+            "streamType": {
+                "id": "duration",
+                "name": "Duration",
+                "description": "Duration over time.",
+                "shape": {
+                    "dimensions": [
+                        {
+                            "id": "time",
+                            "data_type": "timestamp",
+                            "quantity_name": "Time",
+                            "quantity_abbrev": "t",
+                            "unit_name": "Seconds",
+                            "unit_abbrev": "s"
+                        },
+                        {
+                            "id": "duration",
+                            "data_type": "sfloat",
+                            "quantity_name": "Duration",
+                            "quantity_abbrev": "Duration",
+                            "unit_name": "Seconds",
+                            "unit_abbrev": "s"
+                        }
+                    ]
+                }
+            },
+            "min_time": 1648231560,
+            "max_time": 1648234860
+        }
+
+        first_hundred_streams = []
+        for i in range(100):
+            resp = copy.deepcopy(stream_resp)
+            resp["id"] = str(i)
+            first_hundred_streams.append(resp)
+
+        next_fifty_streams = []
+        for i in range(100, 150):
+            resp = copy.deepcopy(stream_resp)
+            resp["id"] = str(i)
+            next_fifty_streams.append(resp)
+
+        self.mock_graph_client.execute.side_effect = [
+            {
+                "streamListByIds": {
+                    "pageInfo": {
+                        "endCursor": None
+                    },
+                    "streams": first_hundred_streams
+                }
+            },
+            {
+                "streamListByIds": {
+                    "pageInfo": {
+                        "endCursor": None
+                    },
+                    "streams": next_fifty_streams
+                }
+            },
+        ]
+
+        streams = get_stream_metadata(
+            stream_ids=[str(i) for i in range(150)],
+            client=self.mock_graph_client
+        )
 
-    def test_get_patient_streams_basic(self):
+        self.assertEqual(150, len(streams.to_list()))
+
+    @mock.patch("runeq.resources.stream_metadata.get_patient")
+    def test_get_patient_stream_metadata_no_access(self, get_patient):
+        """
+        Test get_patient_stream_metadata fails if the user doesn't have access
+        to the patient ID or if the patient doesn't exist.
+        """
+        get_patient.side_effect = Exception("NotFoundError")
+
+        with self.assertRaises(Exception) as context:
+            get_patient_stream_metadata(
+                patient_id='foo',
+                client=self.mock_graph_client
+            )
+
+        self.assertTrue('NotFoundError' in str(context.exception))
+
+    @mock.patch("runeq.resources.stream_metadata.get_patient")
+    def test_get_patient_streams_basic(self, _):
         """
         Test filtering streams by all parameters.
 
         """
         self.mock_graph_client.execute = mock.Mock()
         self.mock_graph_client.execute.side_effect = [
             {
@@ -635,16 +732,16 @@
                     "max_time": 1648234860,
                     "id": "s2"
                 }
             ],
             streams.to_list(),
         )
 
-
-    def test_get_patient_streams_paginated(self):
+    @mock.patch("runeq.resources.stream_metadata.get_patient")
+    def test_get_patient_streams_paginated(self, _):
         """
         Test filtering streams by all parameters, where the user has to
         page through streams.
 
         """
         self.mock_graph_client.execute = mock.Mock()
         self.mock_graph_client.execute.side_effect = [
```

### Comparing `runeq-0.9.0/tests/resources/test_user.py` & `runeq-0.9.1/tests/resources/test_user.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/tests/stream/test_v1.py` & `runeq-0.9.1/tests/stream/test_v1.py`

 * *Files identical despite different names*

### Comparing `runeq-0.9.0/tests/test_config.py` & `runeq-0.9.1/tests/test_config.py`

 * *Files identical despite different names*

