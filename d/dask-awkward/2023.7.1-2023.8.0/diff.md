# Comparing `tmp/dask_awkward-2023.7.1.tar.gz` & `tmp/dask_awkward-2023.8.0.tar.gz`

## Comparing `dask_awkward-2023.7.1.tar` & `dask_awkward-2023.8.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/__init__.py
--rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/awkward.yaml
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/py.typed
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/sizeof.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/typing.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/utils.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/version.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/version.pyi
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/layers/__init__.py
--rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/layers/layers.py
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/__init__.py
--rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/_utils.py
--rw-r--r--   0        0        0    76062 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/core.py
--rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/describe.py
--rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/inspect.py
--rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/operations.py
--rw-r--r--   0        0        0    16591 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/optimize.py
--rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/reducers.py
--rw-r--r--   0        0        0    29197 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/structure.py
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/testutils.py
--rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/unproject_layout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/io/__init__.py
--rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/io/io.py
--rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/io/json.py
--rw-r--r--   0        0        0    14994 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/src/dask_awkward/lib/io/parquet.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/LICENSE
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/README.md
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/pyproject.toml
--rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dask_awkward-2023.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1758 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/__init__.py
+-rw-r--r--   0        0        0     1565 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/awkward.yaml
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/py.typed
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/sizeof.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/typing.py
+-rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/utils.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/version.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/version.pyi
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/layers/__init__.py
+-rw-r--r--   0        0        0    10109 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/layers/layers.py
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/__init__.py
+-rw-r--r--   0        0        0     1468 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/_utils.py
+-rw-r--r--   0        0        0    77173 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/core.py
+-rw-r--r--   0        0        0      513 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/describe.py
+-rw-r--r--   0        0        0     3607 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/inspect.py
+-rw-r--r--   0        0        0     1993 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/operations.py
+-rw-r--r--   0        0        0    16591 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/optimize.py
+-rw-r--r--   0        0        0    10948 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/reducers.py
+-rw-r--r--   0        0        0    30209 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/structure.py
+-rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/testutils.py
+-rw-r--r--   0        0        0    13999 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/unproject_layout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/io/__init__.py
+-rw-r--r--   0        0        0    17007 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/io/io.py
+-rw-r--r--   0        0        0    15217 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/io/json.py
+-rw-r--r--   0        0        0    15283 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/src/dask_awkward/lib/io/parquet.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/LICENSE
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/README.md
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/pyproject.toml
+-rw-r--r--   0        0        0     3183 2020-02-02 00:00:00.000000 dask_awkward-2023.8.0/PKG-INFO
```

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/awkward.yaml` & `dask_awkward-2023.8.0/src/dask_awkward/awkward.yaml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/typing.py` & `dask_awkward-2023.8.0/src/dask_awkward/typing.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/utils.py` & `dask_awkward-2023.8.0/src/dask_awkward/utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/layers/layers.py` & `dask_awkward-2023.8.0/src/dask_awkward/layers/layers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/__init__.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/_utils.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/_utils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/core.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -228,17 +228,17 @@
         label = "getitem"
         name = f"{label}-{token}"
         d = self.to_delayed(optimize_graph=True)
         task = {name: (operator.getitem, d.key, where)}
         hlg = HighLevelGraph.from_collections(name, task, dependencies=(d,))
         return Delayed(name, hlg)
 
-    def __getattr__(self, where: str) -> Any:
+    def __getattr__(self, attr: str) -> Any:
         d = self.to_delayed(optimize_graph=True)
-        return getattr(d, where)
+        return getattr(d, attr)
 
     @property
     def known_value(self) -> Any | None:
         return self._known_value
 
     def to_delayed(self, optimize_graph: bool = True) -> Delayed:
         """Convert Scalar collection into a Delayed collection.
@@ -557,46 +557,55 @@
             raise ValueError("rename= unsupported in dask-awkward")
         return Array(dsk, name, self._meta, divisions=self.divisions)
 
     def reset_meta(self) -> None:
         """Assign an empty typetracer array as the collection metadata."""
         self._meta = empty_typetracer()
 
-    def repartition(self, npartitions=None, divisions=None, rows_per_partition=None):
+    def repartition(
+        self,
+        npartitions: int | None = None,
+        divisions: tuple[int, ...] | None = None,
+        rows_per_partition: int | None = None,
+    ) -> Array:
         from dask_awkward.layers import AwkwardMaterializedLayer
         from dask_awkward.lib.structure import repartition_layer
 
         if sum(bool(_) for _ in [npartitions, divisions, rows_per_partition]) != 1:
             raise ValueError("Please specify exactly one of the inputs")
         if not self.known_divisions:
             self.eager_compute_divisions()
-        nrows = self.divisions[-1]
-        if npartitions:
+        nrows = self.defined_divisions[-1]
+        new_divisions: tuple[int, ...] = tuple()
+        if divisions:
+            new_divisions = divisions
+        elif npartitions:
             rows_per_partition = math.ceil(nrows / npartitions)
         if rows_per_partition:
-            divisions = list(range(0, nrows, rows_per_partition))
-            divisions.append(nrows)
+            new_divs = list(range(0, nrows, rows_per_partition))
+            new_divs.append(nrows)
+            new_divisions = tuple(new_divs)
 
         token = tokenize(self, divisions)
         key = f"repartition-{token}"
 
-        new_layer_raw = repartition_layer(self, key, divisions)
+        new_layer_raw = repartition_layer(self, key, new_divisions)
         new_layer = AwkwardMaterializedLayer(
             new_layer_raw,
             previous_layer_names=[self.name],
         )
         new_graph = HighLevelGraph.from_collections(
             key, new_layer, dependencies=(self,)
         )
         return new_array_object(
             new_graph,
             key,
             meta=self._meta,
             behavior=self.behavior,
-            divisions=divisions,
+            divisions=tuple(new_divisions),
         )
 
     def __len__(self) -> int:
         if not self.known_divisions:
             self.eager_compute_divisions()
         return self.divisions[-1]  # type: ignore
 
@@ -650,14 +659,17 @@
                     x
                     for x in fields
                     if _dir_pattern.match(x) and not keyword.iskeyword(x)
                 ]
             )
         )
 
+    def __reduce__(self):
+        return (Array, (self.dask, self.name, self._meta, self.divisions))
+
     @property
     def dask(self) -> HighLevelGraph:
         """High level task graph associated with the collection."""
         return self._dask
 
     @property
     def keys(self) -> list[Hashable]:
@@ -682,14 +694,20 @@
 
     @property
     def known_divisions(self) -> bool:
         """True if the divisions are known (absence of ``None`` in the tuple)."""
         return len(self.divisions) > 0 and None not in self.divisions
 
     @property
+    def defined_divisions(self) -> tuple[int, ...]:
+        if not self.known_divisions:
+            raise ValueError("defined_divisions only works when divisions are known.")
+        return self._divisions  # type: ignore
+
+    @property
     def npartitions(self) -> int:
         """Total number of partitions."""
         return len(self.divisions) - 1
 
     @property
     def layout(self) -> Content:
         """awkward Array layout associated with the eventual computed result."""
@@ -929,57 +947,59 @@
         sl: slice = where[0]
         rest = tuple(where[1:])
         step = sl.step or 1
         start = sl.start or 0
 
         if not self.known_divisions:
             self.eager_compute_divisions()
-        stop = sl.stop or self.divisions[-1]
-        start = start if start >= 0 else self.divisions[-1] + start
-        stop = stop if stop >= 0 else self.divisions[-1] + stop
+        stop = sl.stop or self.defined_divisions[-1]
+        start = start if start >= 0 else self.defined_divisions[-1] + start
+        stop = stop if stop >= 0 else self.defined_divisions[-1] + stop
         if step < 0:
             raise DaskAwkwardNotImplemented("negative step slice on zeroth dimension")
 
         # setup
         token = tokenize(self, where)
         name = f"getitem-{token}"
         remainder = 0
         outpart = 0
         divisions = [0]
         dask = {}
         # make low-level graph
         for i in range(self.npartitions):
-            if start > self.divisions[i + 1]:
+            if start > self.defined_divisions[i + 1]:
                 # first partition not yet found
                 continue
-            if stop < self.divisions[i] and dask:
+            if stop < self.defined_divisions[i] and dask:
                 # no more partitions with valid rows
                 # does **NOT** exit if there are no partitions yet, to make sure there is always
                 # at least one, needed to get metadata of empty output right
                 break
-            slice_start = max(start - self.divisions[i], 0 + remainder)
+            slice_start = max(start - self.defined_divisions[i], 0 + remainder)
             slice_end = min(
-                stop - self.divisions[i], self.divisions[i + 1] - self.divisions[i]
+                stop - self.defined_divisions[i],
+                self.defined_divisions[i + 1] - self.defined_divisions[i],
             )
             if (
                 slice_end == slice_start
-                and (self.divisions[i + 1] - self.divisions[i])
+                and (self.defined_divisions[i + 1] - self.defined_divisions[i])
                 and dask
             ):
                 # in case of zero-row last partition (if not only partition)
                 break
             dask[(name, outpart)] = (
                 _zero_getitem,
                 (self.name, i),
                 slice(slice_start, slice_end, step),
                 rest,
             )
             outpart += 1
             remainder = (
-                (self.divisions[i] + slice_start) - self.divisions[i + 1]
+                (self.defined_divisions[i] + slice_start)
+                - self.defined_divisions[i + 1]
             ) % step
             remainder = step - remainder if remainder < 0 else remainder
             nextdiv = math.ceil((slice_end - slice_start) / step)
             divisions.append(divisions[-1] + nextdiv)
 
         hlg = HighLevelGraph.from_collections(
             name,
@@ -1336,15 +1356,15 @@
         """
         out: Array = self.partitions[0].map_partitions(
             lambda x: x[:nrow], meta=self._meta
         )
         if compute:
             return out.compute()
         if self.known_divisions:
-            out._divisions = (0, min(nrow, self.divisions[1]))
+            out._divisions = (0, min(nrow, self.defined_divisions[1]))
         return out
 
 
 def _zero_getitem(arr: ak.Array, zeroth: slice, rest: tuple[slice, ...]) -> ak.Array:
     return arr.__getitem__((zeroth,) + rest)
 
 
@@ -1616,14 +1636,24 @@
     """
     token = token or tokenize(base_fn, *args, meta, **kwargs)
     label = hyphenize(label or funcname(base_fn))
     name = f"{label}-{token}"
     kwarg_flat_deps, kwarg_repacker = unpack_collections(kwargs, traverse=traverse)
     flat_deps, _ = unpack_collections(*args, *kwargs.values(), traverse=traverse)
 
+    if len(flat_deps) == 0:
+        message = (
+            "map_partitions expects at least one Dask collection instance, "
+            "you are passing non-Dask collections to dask-awkward code.\n"
+            "observed argument types:\n"
+        )
+        for arg in args:
+            message += f"- {type(arg)}"
+        raise TypeError(message)
+
     arg_flat_deps_expanded = []
     arg_repackers = []
     arg_lens_for_repackers = []
     for arg in args:
         this_arg_flat_deps, repacker = unpack_collections(arg, traverse=traverse)
         if (
             len(this_arg_flat_deps) > 0
```

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/describe.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/describe.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/inspect.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/inspect.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/operations.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/operations.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/optimize.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/optimize.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/reducers.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/reducers.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/structure.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 import builtins
 import warnings
 from collections.abc import Sequence
 from numbers import Number
 from typing import TYPE_CHECKING, Any
 
 import awkward as ak
-from dask.base import is_dask_collection
+import numpy as np
+from awkward._nplikes.typetracer import TypeTracerArray
+from dask.base import is_dask_collection, tokenize
+from dask.highlevelgraph import HighLevelGraph
 
+from dask_awkward.layers import AwkwardMaterializedLayer
 from dask_awkward.lib.core import (
     Array,
     PartitionCompatibility,
     map_partitions,
+    new_known_scalar,
+    new_scalar_object,
     partition_compatibility,
 )
 from dask_awkward.utils import (
     DaskAwkwardNotImplemented,
     IncompatiblePartitions,
     borrow_docstring,
 )
@@ -558,35 +564,57 @@
     #     neginf=neginf,
     #     highlevel=highlevel,
     #     behavior=behavior,
     # )
     raise DaskAwkwardNotImplemented("TODO")
 
 
+def _numaxis0(*integers):
+    return np.sum(np.array(integers))
+
+
 @borrow_docstring(ak.num)
 def num(
     array: Any,
     axis: int = 1,
     highlevel: bool = True,
     behavior: dict | None = None,
 ) -> Any:
     if not highlevel:
         raise ValueError("Only highlevel=True is supported")
-    if axis and axis != 0:
+    if axis == 0 or axis == -1 * array.ndim:
+        if array.known_divisions:
+            return new_known_scalar(array.defined_divisions[-1], label="num")
+
+        per_axis = map_partitions(
+            ak.num,
+            array,
+            axis=0,
+            meta=ak.Array(ak.Array([1, 1]).layout.to_typetracer(forget_length=True)),
+        )
+        name = f"numaxis0-{tokenize(array, axis)}"
+        keys = per_axis.__dask_keys__()
+        matlayer = AwkwardMaterializedLayer(
+            {(name, 0): (_numaxis0, *keys)}, previous_layer_names=[per_axis.name]
+        )
+        hlg = HighLevelGraph.from_collections(name, matlayer, dependencies=(per_axis,))
+        return new_scalar_object(
+            hlg,
+            name,
+            meta=TypeTracerArray._new(dtype=np.int64, shape=()),
+        )
+    else:
         return map_partitions(
             ak.num,
             array,
             axis=axis,
             highlevel=highlevel,
             behavior=behavior,
             output_divisions=1,
         )
-    if axis == 0:
-        return len(array)
-    raise DaskAwkwardNotImplemented("TODO")
 
 
 @borrow_docstring(ak.ones_like)
 def ones_like(
     array: Array,
     highlevel: bool = True,
     behavior: dict | None = None,
@@ -1112,18 +1140,18 @@
     data = [
         d[sl[0] : sl[1]] if sl is not None else d
         for d, sl in builtins.zip(data, slices)
     ]
     return ak.concatenate(data)
 
 
-def repartition_layer(arr: Array, key: str, divisions: list[int, ...]):
+def repartition_layer(arr: Array, key: str, divisions: tuple[int, ...]):
     layer = {}
 
-    indivs = arr.divisions
+    indivs = arr.defined_divisions
     i = 0
     for index, (start, end) in enumerate(builtins.zip(divisions[:-1], divisions[1:])):
         pp = []
         ss = []
         while indivs[i] <= start:
             i += 1
         j = i
```

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/testutils.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/testutils.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/unproject_layout.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/unproject_layout.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/io/io.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/io/io.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,16 +85,19 @@
     >>> a = ak.Array([[1, 2, 3], [4], [5, 6, 7, 8]])
     >>> c = dak.from_awkward(a, npartitions=3)
     >>> c.partitions[[0, 1]].compute()
     <Array [[1, 2, 3], [4]] type='2 * var * int64'>
 
     """
     nrows = len(source)
-    chunksize = int(math.ceil(nrows / npartitions))
-    locs = list(range(0, nrows, chunksize)) + [nrows]
+    if nrows == 0:
+        locs = [None, None]
+    else:
+        chunksize = int(math.ceil(nrows / npartitions))
+        locs = list(range(0, nrows, chunksize)) + [nrows]
     starts = locs[:-1]
     stops = locs[1:]
     meta = typetracer_array(source)
     return from_map(
         _FromAwkwardFn(source),
         starts,
         stops,
```

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/io/json.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/io/json.py`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/src/dask_awkward/lib/io/parquet.py` & `dask_awkward-2023.8.0/src/dask_awkward/lib/io/parquet.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 import itertools
 import logging
 import math
 import operator
 from typing import Any, Sequence
 
 import awkward as ak
-import fsspec
+import awkward.operations.ak_from_parquet as ak_from_parquet
+import awkward.operations.ak_to_arrow_table as ak_to_arrow_table
 from awkward.forms.form import Form
-from awkward.operations import ak_from_parquet, to_arrow_table
 from awkward.operations.ak_from_parquet import _load
 from dask.base import tokenize
 from dask.blockwise import BlockIndex
 from dask.highlevelgraph import HighLevelGraph
 from fsspec import AbstractFileSystem
-from fsspec.core import get_fs_token_paths
+from fsspec.core import get_fs_token_paths, url_to_fs
 
 from dask_awkward.lib.core import (
     Array,
     Scalar,
     map_partitions,
     new_scalar_object,
     typetracer_array,
@@ -32,27 +32,31 @@
 
 
 class _FromParquetFn:
     def __init__(
         self,
         *,
         fs: AbstractFileSystem,
-        schema: Any,
+        form: Any,
         listsep: str = "list.item",
         unnamed_root: bool = False,
         original_form: Form | None = None,
+        behavior: dict | None = None,
+        **kwargs: Any,
     ) -> None:
         self.fs = fs
-        self.schema = schema
+        self.form = form
         self.listsep = listsep
         self.unnamed_root = unnamed_root
-        self.columns = self.schema.columns(self.listsep)
+        self.columns = self.form.columns(self.listsep)
         if self.unnamed_root:
             self.columns = [f".{c}" for c in self.columns]
         self.original_form = original_form
+        self.behavior = behavior
+        self.kwargs = kwargs
 
     @abc.abstractmethod
     def __call__(self, source: Any) -> ak.Array:
         ...
 
     @abc.abstractmethod
     def project_columns(
@@ -61,213 +65,242 @@
         orignal_form: Form | None = None,
     ) -> _FromParquetFn:
         ...
 
     def __repr__(self) -> str:
         s = (
             "\nFromParquetFn(\n"
-            f"  schema={repr(self.schema)}\n"
+            f"  form={repr(self.form)}\n"
             f"  listsep={self.listsep}\n"
             f"  unnamed_root={self.unnamed_root}\n"
             f"  columns={self.columns}\n"
+            f"  behavior={self.behavior}\n"
         )
+        for key, val in self.kwargs.items():
+            s += f"  {key}={val}\n"
+        s = f"{s})"
         return s
 
     def __str__(self) -> str:
         return self.__repr__()
 
 
 class _FromParquetFileWiseFn(_FromParquetFn):
     def __init__(
         self,
         *,
         fs: AbstractFileSystem,
-        schema: Any,
+        form: Any,
         listsep: str = "list.item",
         unnamed_root: bool = False,
         original_form: Form | None = None,
+        behavior: dict | None = None,
+        **kwargs: Any,
     ) -> None:
         super().__init__(
             fs=fs,
-            schema=schema,
+            form=form,
             listsep=listsep,
             unnamed_root=unnamed_root,
             original_form=original_form,
+            behavior=behavior,
+            **kwargs,
         )
 
     def __call__(self, source: Any) -> Any:
-        array = _file_to_partition(
-            source,
-            self.fs,
-            self.columns,
-            self.schema,
+        array = _load(
+            [source],
+            parquet_columns=self.columns,
+            subrg=[None],
+            subform=self.form,
+            highlevel=True,
+            fs=self.fs,
+            behavior=self.behavior,
+            **self.kwargs,
         )
         return ak.Array(unproject_layout(self.original_form, array.layout))
 
     def project_columns(
         self,
         columns: Sequence[str] | None,
         original_form: Form | None = None,
     ) -> _FromParquetFileWiseFn:
         if columns is None:
             return self
-
-        new_schema = self.schema.select_columns(columns)
+        new_form = self.form.select_columns(columns)
         new = _FromParquetFileWiseFn(
             fs=self.fs,
-            schema=new_schema,
+            form=new_form,
             listsep=self.listsep,
             unnamed_root=self.unnamed_root,
             original_form=original_form,
+            behavior=self.behavior,
+            **self.kwargs,
         )
-
-        log.debug(f"project_columns received: {columns}")
-        log.debug(f"new schema is {repr(new_schema)}")
-        log.debug(f"new schema columns are: {new_schema.columns(self.listsep)}")
-        log.debug(new)
-
         return new
 
 
 class _FromParquetFragmentWiseFn(_FromParquetFn):
     def __init__(
         self,
         *,
         fs: AbstractFileSystem,
-        schema: Any,
+        form: Any,
         listsep: str = "list.item",
         unnamed_root: bool = False,
         original_form: Form | None = None,
+        behavior: dict | None = None,
+        **kwargs: Any,
     ) -> None:
         super().__init__(
             fs=fs,
-            schema=schema,
+            form=form,
             listsep=listsep,
             unnamed_root=unnamed_root,
             original_form=original_form,
+            behavior=behavior,
+            **kwargs,
         )
 
     def __call__(self, pair: Any) -> ak.Array:
         subrg, source = pair
         if isinstance(subrg, int):
             subrg = [[subrg]]
-        array = _file_to_partition(
-            source,
-            self.fs,
-            self.columns,
-            self.schema,
+        array = _load(
+            [source],
+            parquet_columns=self.columns,
             subrg=subrg,
+            subform=self.form,
+            highlevel=True,
+            fs=self.fs,
+            behavior=self.behavior,
+            **self.kwargs,
         )
+        # array = _file_to_partition(
+        #     source,
+        #     self.fs,
+        #     self.columns,
+        #     self.form,
+        #     subrg=subrg,
+        # )
         return ak.Array(unproject_layout(self.original_form, array.layout))
 
     def project_columns(
         self,
         columns: Sequence[str] | None,
         original_form: Form | None = None,
     ) -> _FromParquetFragmentWiseFn:
         if columns is None:
             return self
         return _FromParquetFragmentWiseFn(
             fs=self.fs,
-            schema=self.schema.select_columns(columns),
+            form=self.form.select_columns(columns),
             unnamed_root=self.unnamed_root,
             original_form=original_form,
+            behavior=self.behavior,
+            **self.kwargs,
         )
 
 
 def from_parquet(
-    path: Any,
-    storage_options: dict | None = None,
+    path: str | list[str],
+    *,
+    columns: str | list[str] | None = None,
+    storage_options: dict[str, Any] | None = None,
+    max_gap: int = 64_000,
+    max_block: int = 256_000_000,
+    footer_sample_size: int = 1_000_000,
+    generate_bitmasks: bool = False,
+    highlevel: bool = True,
+    behavior: dict | None = None,
     ignore_metadata: bool = True,
     scan_files: bool = False,
-    columns: Sequence[str] | None = None,
-    filters: Any | None = None,
-    split_row_groups: Any | None = None,
+    split_row_groups: bool = False,
 ) -> Array:
-    """Create an Array collection from a Parquet dataset.
+    if not highlevel:
+        raise ValueError("dask-awkward only supports highlevel=True")
 
-    Parameters
-    ----------
-    url : str
-        Location of data, including protocol (e.g. ``s3://``)
-    storage_options : dict
-        For creating filesystem (see ``fsspec`` documentation).
-    ignore_metadata : bool
-        Ignore parquet metadata associated with the input dataset (the
-        ``_metadata`` file).
-    scan_files : bool
-        TBD
-    columns : list[str], optional
-        Select columns to load
-    filters : list[list[tuple]], optional
-        Parquet-style filters for excluding row groups based on column statistics
-    split_row_groups: bool, optional
-        If True, each row group becomes a partition. If False, each
-        file becomes a partition. If None, the existence of a
-        ``_metadata`` file and ignore_metadata=False implies True,
-        else False.
-
-    Returns
-    -------
-    Array
-        Array collection from the parquet dataset.
-
-    """
-    fs, tok, paths = get_fs_token_paths(
-        path, mode="rb", storage_options=storage_options
+    fs, token, paths = get_fs_token_paths(
+        path,
+        mode="rb",
+        storage_options=storage_options,
     )
     label = "from-parquet"
     token = tokenize(
-        tok, paths, ignore_metadata, columns, filters, scan_files, split_row_groups
+        token,
+        paths,
+        columns,
+        max_gap,
+        max_block,
+        footer_sample_size,
+        generate_bitmasks,
+        behavior,
+        ignore_metadata,
+        scan_files,
+        split_row_groups,
     )
 
-    # same as ak_metadata_from_parquet
-    results = ak_from_parquet.metadata(
+    (
+        parquet_columns,
+        subform,
+        actual_paths,
+        fs,
+        subrg,
+        row_counts,
+        metadata,
+    ) = ak_from_parquet.metadata(
         path,
         storage_options,
         row_groups=None,
         columns=columns,
         ignore_metadata=ignore_metadata,
         scan_files=scan_files,
     )
-    parquet_columns, subform, actual_paths, fs, subrg, row_counts, metadata = results
 
     listsep = "list.item"
     unnamed_root = False
     for c in parquet_columns:
         if ".list.element." in c:
             listsep = "list.element"
             break
         if c.startswith("."):
             unnamed_root = True
 
     if split_row_groups is None:
         split_row_groups = row_counts is not None and len(row_counts) > 1
 
     meta = ak.Array(
-        subform.length_zero_array(highlevel=False).to_typetracer(forget_length=True)
+        subform.length_zero_array(highlevel=False).to_typetracer(forget_length=True),
+        behavior=behavior,
     )
 
     if split_row_groups is False or subrg is None:
         # file-wise
+
+        fn = _FromParquetFileWiseFn(
+            fs=fs,
+            form=subform,
+            listsep=listsep,
+            unnamed_root=unnamed_root,
+            max_gap=max_gap,
+            max_block=max_block,
+            footer_sample_size=footer_sample_size,
+            generate_bitmasks=generate_bitmasks,
+            behavior=behavior,
+        )
+
         return from_map(
-            _FromParquetFileWiseFn(
-                fs=fs,
-                schema=subform,
-                listsep=listsep,
-                unnamed_root=unnamed_root,
-            ),
+            fn,
             actual_paths,
             label=label,
             token=token,
             meta=typetracer_array(meta),
         )
     else:
         # row-group wise
-
         if set(subrg) == {None}:
             rgs_paths = {path: 0 for path in actual_paths}
             for i in range(metadata.num_row_groups):
                 fp = metadata.row_group(i).column(0).file_path
                 rgs_path = [p for p in rgs_paths if fp in p][
                     0
                 ]  # returns 1st if fp is empty
@@ -279,47 +312,37 @@
         divisions = [0] + list(
             itertools.accumulate([rg.num_rows for rg in rgs], operator.add)
         )
         pairs = []
 
         for isubrg, path in zip(subrg, actual_paths):
             pairs.extend([(irg, path) for irg in isubrg])
+
+        fn = _FromParquetFragmentWiseFn(
+            fs=fs,
+            form=subform,
+            listsep=listsep,
+            unnamed_root=unnamed_root,
+            max_gap=max_gap,
+            max_block=max_block,
+            footer_sample_size=footer_sample_size,
+            generate_bitmasks=generate_bitmasks,
+            behavior=behavior,
+        )
+
         return from_map(
-            _FromParquetFragmentWiseFn(
-                fs=fs,
-                schema=subform,
-                listsep=listsep,
-                unnamed_root=unnamed_root,
-            ),
+            fn,
             pairs,
             label=label,
             token=token,
             divisions=tuple(divisions),
             meta=typetracer_array(meta),
         )
 
 
-def _file_to_partition(path, fs, columns, schema, subrg=None):
-    """read a whole parquet file to awkward"""
-    return _load(
-        actual_paths=[path],
-        fs=fs,
-        parquet_columns=columns,
-        subrg=subrg or [None],
-        footer_sample_size=2**15,
-        max_gap=2**10,
-        max_block=2**22,
-        generate_bitmasks=False,
-        metadata=None,
-        highlevel=True,
-        subform=schema,
-        behavior=None,
-    )
-
-
 def _metadata_file_from_data_files(path_list, fs, out_path):
     """
     Aggregate _metadata and _common_metadata from data files
 
     Maybe only used in testing
 
     (similar to fastparquet's merge)
@@ -373,15 +396,15 @@
     return_metadata=False,  # whether making global _metadata
     compression=None,  # TBD
     head=False,  # is this the first piece
     # custom_metadata=None,
 ):
     import pyarrow.parquet as pq
 
-    t = to_arrow_table(
+    t = ak_to_arrow_table.to_arrow_table(
         data,
         list_to32=True,
         string_to32=True,
         bytestring_to32=True,
         categorical_as_dictionary=True,
         extensionarray=False,
     )
@@ -410,15 +433,15 @@
 class _ToParquetFn:
     def __init__(
         self,
         fs: AbstractFileSystem,
         path: Any,
         return_metadata: bool = False,
         compression: Any | None = None,
-        head: Any | None = None,
+        head: bool = False,
         npartitions: int | None = None,
         prefix: str | None = None,
     ):
         self.fs = fs
         self.path = path
         self.return_metadata = return_metadata
         self.compression = compression
@@ -480,15 +503,15 @@
     # TODO options we need:
     #  - compression per data type or per leaf column ("path.to.leaf": "zstd" format)
     #  - byte stream split for floats if compression is not None or lzma
     #  - partitioning
     #  - parquet 2 for full set of time and int types
     #  - v2 data page (for possible later fastparquet implementation)
     #  - dict encoding always off
-    fs, _ = fsspec.core.url_to_fs(path, **(storage_options or {}))
+    fs, _ = url_to_fs(path, **(storage_options or {}))
     name = f"write-parquet-{tokenize(fs, data, path)}"
 
     map_res = map_partitions(
         _ToParquetFn(fs, path=path, npartitions=data.npartitions, prefix=prefix),
         data,
         BlockIndex((data.npartitions,)),
         label="to-parquet",
```

### Comparing `dask_awkward-2023.7.1/.gitignore` & `dask_awkward-2023.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/LICENSE` & `dask_awkward-2023.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/README.md` & `dask_awkward-2023.8.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/pyproject.toml` & `dask_awkward-2023.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask_awkward-2023.7.1/PKG-INFO` & `dask_awkward-2023.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-awkward
-Version: 2023.7.1
+Version: 2023.8.0
 Summary: Awkward Array meets Dask
 Project-URL: Homepage, https://github.com/dask-contrib/dask-awkward
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-awkward/issues
 Author-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 Maintainer-email: Doug Davis <ddavis@ddavis.io>, Martin Durant <mdurant@anaconda.com>
 License: BSD-3-Clause
 License-File: LICENSE
```

