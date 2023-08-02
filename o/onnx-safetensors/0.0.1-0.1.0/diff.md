# Comparing `tmp/onnx-safetensors-0.0.1.tar.gz` & `tmp/onnx-safetensors-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onnx-safetensors-0.0.1.tar", last modified: Tue Aug  1 23:58:48 2023, max compression
+gzip compressed data, was "onnx-safetensors-0.1.0.tar", last modified: Wed Aug  2 16:10:17 2023, max compression
```

## Comparing `onnx-safetensors-0.0.1.tar` & `onnx-safetensors-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:58:48.466755 onnx-safetensors-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-01 23:58:39.000000 onnx-safetensors-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-01 23:58:48.466755 onnx-safetensors-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-01 23:58:39.000000 onnx-safetensors-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:58:48.466755 onnx-safetensors-0.0.1/onnx_safetensors/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-08-01 23:58:39.000000 onnx-safetensors-0.0.1/onnx_safetensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-08-01 23:58:39.000000 onnx-safetensors-0.0.1/onnx_safetensors/_external_data_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-08-01 23:58:39.000000 onnx-safetensors-0.0.1/onnx_safetensors/_safetensors_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-08-01 23:58:39.000000 onnx-safetensors-0.0.1/onnx_safetensors/_safetensors_io_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:58:48.466755 onnx-safetensors-0.0.1/onnx_safetensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-08-01 23:58:48.000000 onnx-safetensors-0.0.1/onnx_safetensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-08-01 23:58:48.000000 onnx-safetensors-0.0.1/onnx_safetensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:58:48.000000 onnx-safetensors-0.0.1/onnx_safetensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-01 23:58:48.000000 onnx-safetensors-0.0.1/onnx_safetensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 23:58:48.000000 onnx-safetensors-0.0.1/onnx_safetensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-08-01 23:58:39.000000 onnx-safetensors-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 23:58:48.466755 onnx-safetensors-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/onnx_safetensors/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/onnx_safetensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6406 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/onnx_safetensors/_safetensors_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/onnx_safetensors/_safetensors_io_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/onnx_safetensors/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 16:10:17.000000 onnx-safetensors-0.1.0/onnx_safetensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-02 16:10:06.000000 onnx-safetensors-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 16:10:17.699046 onnx-safetensors-0.1.0/setup.cfg
```

### Comparing `onnx-safetensors-0.0.1/LICENSE` & `onnx-safetensors-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onnx-safetensors-0.0.1/PKG-INFO` & `onnx-safetensors-0.1.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: onnx-safetensors
-Version: 0.0.1
-Summary: ONNX extension for saving to and loading from safetensors
+Version: 0.1.0
+Summary: Use safetensors with ONNX
 Author-email: Justin Chu <justinchuby@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `onnx-safetensors-0.0.1/onnx_safetensors/_external_data_helper.py` & `onnx-safetensors-0.1.0/onnx_safetensors/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,82 +1,123 @@
 # Copyright (c) ONNX Project Contributors
 #
 # SPDX-License-Identifier: Apache-2.0
+"""Utilities for iterating on ONNX models."""
 
 from __future__ import annotations
 
+__all__ = [
+    "get_all_tensors",
+    "get_attribute_tensors",
+    "get_initializer_tensors",
+    "set_external_data_flag",
+    "apply_tensor_dict",
+]
+
 import itertools
-from typing import Callable, Iterable
+from typing import TYPE_CHECKING, Callable, Iterable, Mapping
 
 import onnx
 
+if TYPE_CHECKING:
+    import numpy as np
+
 
 def _recursive_attribute_processor(
     attribute: onnx.AttributeProto,
     func: Callable[[onnx.GraphProto], Iterable[onnx.TensorProto]],
 ) -> Iterable[onnx.TensorProto]:
     """Create an iterator through processing ONNX model attributes with functor."""
     if attribute.type == onnx.AttributeProto.GRAPH:
         yield from func(attribute.g)
     if attribute.type == onnx.AttributeProto.GRAPHS:
         for graph in attribute.graphs:
             yield from func(graph)
 
 
-def _get_initializer_tensors_from_graph(
-    model_proto_graph: onnx.GraphProto,
+def get_initializer_tensors(
+    proto: onnx.ModelProto | onnx.GraphProto,
 ) -> Iterable[onnx.TensorProto]:
-    """Create an iterator of initializer tensors from ONNX model graph."""
-    yield from model_proto_graph.initializer
-    for node in model_proto_graph.node:
+    """Create an iterator of initializer tensors from ONNX ModelProto or GraphProto."""
+    if isinstance(proto, onnx.ModelProto):
+        graph = proto.graph
+    else:
+        graph = proto
+    yield from graph.initializer
+    for node in graph.node:
         for attribute in node.attribute:
             yield from _recursive_attribute_processor(
-                attribute, _get_initializer_tensors_from_graph
+                attribute, get_initializer_tensors
             )
 
 
-def get_initializer_tensors(
-    model_proto: onnx.ModelProto,
-) -> Iterable[onnx.TensorProto]:
-    """Create an iterator of initializer tensors from ONNX model."""
-    yield from _get_initializer_tensors_from_graph(model_proto.graph)
-
-
-def _get_attribute_tensors_from_graph(
-    model_proto_graph: onnx.GraphProto,
+def get_attribute_tensors(
+    proto: onnx.ModelProto | onnx.GraphProto,
 ) -> Iterable[onnx.TensorProto]:
-    """Create an iterator of tensors from node attributes of an ONNX model graph."""
-    for node in model_proto_graph.node:
+    """Create an iterator of tensors from node attributes of an ONNX ModelProto or GraphProto."""
+    if isinstance(proto, onnx.ModelProto):
+        graph = proto.graph
+    else:
+        graph = proto
+    for node in graph.node:
         for attribute in node.attribute:
             if attribute.HasField("t"):
                 yield attribute.t
             yield from attribute.tensors
-            yield from _recursive_attribute_processor(
-                attribute, _get_attribute_tensors_from_graph
-            )
+            yield from _recursive_attribute_processor(attribute, get_attribute_tensors)
 
 
-def _get_attribute_tensors(
-    model_proto: onnx.ModelProto,
+def get_all_tensors(
+    proto: onnx.ModelProto | onnx.GraphProto,
 ) -> Iterable[onnx.TensorProto]:
-    """Create an iterator of tensors from node attributes of an ONNX model."""
-    yield from _get_attribute_tensors_from_graph(model_proto.graph)
-
-
-def get_all_tensors(model_proto: onnx.ModelProto) -> Iterable[onnx.TensorProto]:
     """Scan an ONNX model for all tensors and return as an iterator."""
     return itertools.chain(
-        get_initializer_tensors(model_proto),
-        _get_attribute_tensors(model_proto),
+        get_initializer_tensors(proto),
+        get_attribute_tensors(proto),
     )
 
 
 def set_external_data_flag(tensor: onnx.TensorProto, flag: bool) -> None:
     """Set or unset the external data flag of a tensor."""
     # We do not need the metadata about external data
     del tensor.external_data[:]
     if flag:
         # After loading raw_data from external_data, change the state of tensors
         tensor.data_location = onnx.TensorProto.EXTERNAL
     else:
         tensor.data_location = onnx.TensorProto.DEFAULT
-    return
+
+
+def clear_raw_data(tensor: onnx.TensorProto):
+    """Clear raw_data of a tensor."""
+    if tensor.HasField("raw_data"):
+        tensor.ClearField("raw_data")
+
+
+def apply_tensor_dict(
+    tensor_protos: Iterable[onnx.TensorProto], tensor_dict: Mapping[str, np.ndarray]
+) -> set[str]:
+    """Apply a dictionary of external data to a list of `TensorProto`s.
+
+    Args:
+        tensor_protos: All tensors in ONNX model to apply external data to.
+        tensor_dict: Dictionary of external data to apply to ONNX model.
+
+    Returns:
+        Names of tensors that were applied.
+    """
+    applied = set()
+    for tensor in tensor_protos:
+        name = tensor.name
+        if (external_tensor := tensor_dict.get(name)) is None:
+            continue
+        place_holder = onnx.helper.make_tensor(
+            name,
+            tensor.data_type,
+            tensor.dims,
+            vals=external_tensor,
+        )
+        tensor.raw_data = place_holder.raw_data
+        set_external_data_flag(tensor, False)
+        applied.add(name)
+
+    return applied
```

### Comparing `onnx-safetensors-0.0.1/onnx_safetensors.egg-info/PKG-INFO` & `onnx-safetensors-0.1.0/onnx_safetensors.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: onnx-safetensors
-Version: 0.0.1
-Summary: ONNX extension for saving to and loading from safetensors
+Version: 0.1.0
+Summary: Use safetensors with ONNX
 Author-email: Justin Chu <justinchuby@users.noreply.github.com>
 License: MIT License
         
         Copyright (c) 2023 Justin Chu
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `onnx-safetensors-0.0.1/pyproject.toml` & `onnx-safetensors-0.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "onnx-safetensors"
 dynamic = ["version"]
-description = "ONNX extension for saving to and loading from safetensors"
+description = "Use safetensors with ONNX"
 keywords = []
 authors = [
   { name = "Justin Chu", email = "justinchuby@users.noreply.github.com" },
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 license = { file = "LICENSE" }
@@ -26,15 +26,14 @@
   "Programming Language :: Python :: 3.11",
   "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
   "numpy",
   "onnx>=1.14",
   "safetensors",
-  "typing_extensions",
 ]
 
 [project.urls]
 Documentation = "https://github.com/justinchuby/onnx-safetensors#readme"
 Issues = "https://github.com/justinchuby/onnx-safetensors/issues"
 Source = "https://github.com/justinchuby/onnx-safetensors"
 
@@ -78,14 +77,15 @@
     "TID252", # Disallow relative imports
     "UP", # pyupgrade
     "W", # pycodestyle
     "YTT", # flake8-2020
 ]
 ignore = [
     "E501", # Line length. Not enforced because black will handle formatting
+    "PLR0913", # Too many arguments
 ]
 
 [tool.ruff.flake8-tidy-imports]
 # Disallow all relative imports.
 ban-relative-imports = "all"
 
 [tool.ruff.pydocstyle]
```

