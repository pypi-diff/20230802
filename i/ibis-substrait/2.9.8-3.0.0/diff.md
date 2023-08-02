# Comparing `tmp/ibis-substrait-2.9.8.tar.gz` & `tmp/ibis_substrait-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ibis-substrait-2.9.8.tar", max compression
+gzip compressed data, was "ibis_substrait-3.0.0.tar", max compression
```

## Comparing `ibis-substrait-2.9.8.tar` & `ibis_substrait-3.0.0.tar`

### file list

```diff
@@ -1,43 +1,52 @@
--rw-r--r--   0        0        0    11345 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/LICENSE
--rw-r--r--   0        0        0      171 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/README.md
--rw-r--r--   0        0        0       22 2022-08-10 19:32:23.579247 ibis-substrait-2.9.8/ibis_substrait/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/__init__.py
--rw-r--r--   0        0        0     5925 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/core.py
--rw-r--r--   0        0        0    34687 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/decompile.py
--rw-r--r--   0        0        0     1004 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/mapping.py
--rw-r--r--   0        0        0    29928 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/compiler/translate.py
--rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/__init__.py
--rw-r--r--   0        0        0       24 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/__init__.pyi
--rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/__init__.py
--rw-r--r--   0        0        0       19 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/__init__.pyi
--rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/__init__.py
--rw-r--r--   0        0        0      228 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/__init__.pyi
--rw-r--r--   0        0        0    42349 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/algebra_pb2.py
--rw-r--r--   0        0        0   127324 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/algebra_pb2.pyi
--rw-r--r--   0        0        0     1596 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/capabilities_pb2.py
--rw-r--r--   0        0        0     3200 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/capabilities_pb2.pyi
--rw-r--r--   0        0        0        0 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/__init__.py
--rw-r--r--   0        0        0       29 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/__init__.pyi
--rw-r--r--   0        0        0     3225 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.py
--rw-r--r--   0        0        0     7467 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/extensions/extensions_pb2.pyi
--rw-r--r--   0        0        0     7968 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/function_pb2.py
--rw-r--r--   0        0        0    20854 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/function_pb2.pyi
--rw-r--r--   0        0        0     8723 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.py
--rw-r--r--   0        0        0    20409 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/parameterized_types_pb2.pyi
--rw-r--r--   0        0        0     1930 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/plan_pb2.py
--rw-r--r--   0        0        0     4328 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/plan_pb2.pyi
--rw-r--r--   0        0        0    10711 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.py
--rw-r--r--   0        0        0    26952 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_expressions_pb2.pyi
--rw-r--r--   0        0        0    11524 2022-08-10 19:30:56.340017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_pb2.py
--rw-r--r--   0        0        0    28613 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/proto/substrait/ibis/type_pb2.pyi
--rw-r--r--   0        0        0        0 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/__init__.py
--rw-r--r--   0        0        0        0 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/__init__.py
--rw-r--r--   0        0        0     4478 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/conftest.py
--rw-r--r--   0        0        0    10441 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_compiler.py
--rw-r--r--   0        0        0     8962 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_decompiler.py
--rw-r--r--   0        0        0    13822 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_literal.py
--rw-r--r--   0        0        0    23098 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_tpch.py
--rw-r--r--   0        0        0      175 2022-08-10 19:30:56.344017 ibis-substrait-2.9.8/ibis_substrait/tests/conftest.py
--rw-r--r--   0        0        0     2690 2022-08-10 19:32:25.615230 ibis-substrait-2.9.8/pyproject.toml
--rw-r--r--   0        0        0     1153 2022-08-10 19:32:26.480906 ibis-substrait-2.9.8/setup.py
--rw-r--r--   0        0        0     1187 2022-08-10 19:32:26.481247 ibis-substrait-2.9.8/PKG-INFO
+-rw-r--r--   0        0        0    11345 2023-08-02 17:26:51.268753 ibis_substrait-3.0.0/LICENSE
+-rw-r--r--   0        0        0      951 2023-08-02 17:26:51.268753 ibis_substrait-3.0.0/README.md
+-rw-r--r--   0        0        0      147 2023-08-02 17:27:55.613296 ibis_substrait-3.0.0/ibis_substrait/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 17:26:51.268753 ibis_substrait-3.0.0/ibis_substrait/compiler/__init__.py
+-rw-r--r--   0        0        0    10438 2023-08-02 17:26:51.268753 ibis_substrait-3.0.0/ibis_substrait/compiler/core.py
+-rw-r--r--   0        0        0     6176 2023-08-02 17:26:51.268753 ibis_substrait-3.0.0/ibis_substrait/compiler/mapping.py
+-rw-r--r--   0        0        0    44983 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/compiler/translate.py
+-rw-r--r--   0        0        0        0 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/__init__.py
+-rw-r--r--   0        0        0      149 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/extension_types.yaml
+-rw-r--r--   0        0        0      722 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_aggregate_approx.yaml
+-rw-r--r--   0        0        0      921 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_aggregate_generic.yaml
+-rw-r--r--   0        0        0    42855 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_arithmetic.yaml
+-rw-r--r--   0        0        0     4467 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_arithmetic_decimal.yaml
+-rw-r--r--   0        0        0     3252 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_boolean.yaml
+-rw-r--r--   0        0        0     4956 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_comparison.yaml
+-rw-r--r--   0        0        0     6238 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_datetime.yaml
+-rw-r--r--   0        0        0     4213 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_logarithmic.yaml
+-rw-r--r--   0        0        0    11507 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_rounding.yaml
+-rw-r--r--   0        0        0      733 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_set.yaml
+-rw-r--r--   0        0        0    47765 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/functions_string.yaml
+-rw-r--r--   0        0        0      683 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/type_variations.yaml
+-rw-r--r--   0        0        0     1302 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/extensions/unknown.yaml
+-rw-r--r--   0        0        0        0 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/__init__.py
+-rw-r--r--   0        0        0     4478 2023-08-02 17:26:51.272753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/conftest.py
+-rw-r--r--   0        0        0    28761 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h01/tpc_h01.json
+-rw-r--r--   0        0        0    33502 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h03/tpc_h03.json
+-rw-r--r--   0        0        0    25270 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h04/tpc_h04.json
+-rw-r--r--   0        0        0    49248 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h05/tpc_h05.json
+-rw-r--r--   0        0        0    16994 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h06/tpc_h06.json
+-rw-r--r--   0        0        0    61824 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h07/tpc_h07.json
+-rw-r--r--   0        0        0    56492 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h09/tpc_h09.json
+-rw-r--r--   0        0        0    56492 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h090/tpc_h090.json
+-rw-r--r--   0        0        0    57207 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h091/tpc_h091.json
+-rw-r--r--   0        0        0    40466 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h10/tpc_h10.json
+-rw-r--r--   0        0        0    21818 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h11/tpc_h11.json
+-rw-r--r--   0        0        0    35179 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h12/tpc_h12.json
+-rw-r--r--   0        0        0    16553 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h13/tpc_h13.json
+-rw-r--r--   0        0        0    24676 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h18/tpc_h18.json
+-rw-r--r--   0        0        0    87093 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h19/tpc_h19.json
+-rw-r--r--   0        0        0    11798 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h20/tpc_h20.json
+-rw-r--r--   0        0        0    79060 2023-08-02 17:26:51.276753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h21/tpc_h21.json
+-rw-r--r--   0        0        0    29124 2023-08-02 17:26:51.280753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/snapshots/test_tpch/test_compile/tpc_h22/tpc_h22.json
+-rw-r--r--   0        0        0    17335 2023-08-02 17:26:51.280753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/test_compiler.py
+-rw-r--r--   0        0        0     8764 2023-08-02 17:26:51.280753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/test_extensions.py
+-rw-r--r--   0        0        0    11005 2023-08-02 17:26:51.280753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/test_literal.py
+-rw-r--r--   0        0        0    20556 2023-08-02 17:26:51.280753 ibis_substrait-3.0.0/ibis_substrait/tests/compiler/test_tpch.py
+-rw-r--r--   0        0        0      175 2023-08-02 17:26:51.280753 ibis_substrait-3.0.0/ibis_substrait/tests/conftest.py
+-rw-r--r--   0        0        0     6086 2023-08-02 17:26:51.280753 ibis_substrait-3.0.0/ibis_substrait/tests/integration/test_pyarrow.py
+-rw-r--r--   0        0        0     4714 2023-08-02 17:27:58.453318 ibis_substrait-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3345 1970-01-01 00:00:00.000000 ibis_substrait-3.0.0/setup.py
+-rw-r--r--   0        0        0     1995 1970-01-01 00:00:00.000000 ibis_substrait-3.0.0/PKG-INFO
```

### Comparing `ibis-substrait-2.9.8/LICENSE` & `ibis_substrait-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.8/ibis_substrait/compiler/translate.py` & `ibis_substrait-3.0.0/ibis_substrait/compiler/translate.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,29 +7,46 @@
 
 import collections
 import collections.abc
 import datetime
 import decimal
 import functools
 import itertools
+import math
 import operator
 import uuid
-from typing import Any, Mapping, MutableMapping, Sequence, TypeVar
+from collections.abc import Iterable, Mapping, MutableMapping, Sequence
+from typing import Any, TypeVar, Union
 
 import ibis
 import ibis.expr.datatypes as dt
 import ibis.expr.operations as ops
 import ibis.expr.schema as sch
 import ibis.expr.types as ir
+import toolz
 from ibis import util
+from ibis.common.graph import toposort
 from packaging import version
+from substrait.gen.proto import algebra_pb2 as stalg
+from substrait.gen.proto import type_pb2 as stt
 
-from ..proto.substrait.ibis import algebra_pb2 as stalg
-from ..proto.substrait.ibis import type_pb2 as stt
-from .core import SubstraitCompiler, _get_fields
+from ibis_substrait.compiler.core import SubstraitCompiler, _get_fields
+from ibis_substrait.compiler.mapping import (
+    IBIS_SUBSTRAIT_OP_MAPPING,
+    _extension_mapping,
+)
+
+IBIS_GTE_5 = version.parse(ibis.__version__) >= version.parse("5.0.0")
+IBIS_GTE_6 = version.parse(ibis.__version__) >= version.parse("6.0.0")
+
+try:
+    from typing import TypeAlias
+except ImportError:
+    # Python <= 3.9
+    from typing_extensions import TypeAlias
 
 T = TypeVar("T")
 
 
 def _nullability(dtype: dt.DataType) -> stt.Type.Nullability.V:
     return (
         stt.Type.Nullability.NULLABILITY_NULLABLE
@@ -113,29 +130,57 @@
 def _timestamp(dtype: dt.Timestamp) -> stt.Type:
     nullability = _nullability(dtype)
     if dtype.timezone is not None:
         return stt.Type(timestamp_tz=stt.Type.TimestampTZ(nullability=nullability))
     return stt.Type(timestamp=stt.Type.Timestamp(nullability=nullability))
 
 
-@translate.register
-def _interval(dtype: dt.Interval) -> stt.Type:
-    unit = dtype.unit
-    nullability = _nullability(dtype)
+if IBIS_GTE_6:
 
-    if unit == "Y":
-        return stt.Type(interval_year=stt.Type.IntervalYear(nullability=nullability))
-    elif unit == "M":
-        return stt.Type(interval_year=stt.Type.IntervalYear(nullability=nullability))
-    elif unit == "D":
-        return stt.Type(interval_day=stt.Type.IntervalDay(nullability=nullability))
-    elif unit == "s":
-        return stt.Type(interval_day=stt.Type.IntervalDay(nullability=nullability))
+    @translate.register
+    def _interval(dtype: dt.Interval) -> stt.Type:
+        unit = dtype.unit.name
+        nullability = _nullability(dtype)
+
+        if unit == "YEAR":
+            return stt.Type(
+                interval_year=stt.Type.IntervalYear(nullability=nullability)
+            )
+        elif unit == "MONTH":
+            return stt.Type(
+                interval_year=stt.Type.IntervalYear(nullability=nullability)
+            )
+        elif unit == "DAY":
+            return stt.Type(interval_day=stt.Type.IntervalDay(nullability=nullability))
+        elif unit == "SECOND":
+            return stt.Type(interval_day=stt.Type.IntervalDay(nullability=nullability))
+
+        raise ValueError(f"unsupported substrait unit: {unit!r}")
+
+else:
+
+    @translate.register
+    def _interval(dtype: dt.Interval) -> stt.Type:
+        unit = dtype.unit
+        nullability = _nullability(dtype)
+
+        if unit == "Y":
+            return stt.Type(
+                interval_year=stt.Type.IntervalYear(nullability=nullability)
+            )
+        elif unit == "M":
+            return stt.Type(
+                interval_year=stt.Type.IntervalYear(nullability=nullability)
+            )
+        elif unit == "D":
+            return stt.Type(interval_day=stt.Type.IntervalDay(nullability=nullability))
+        elif unit == "s":
+            return stt.Type(interval_day=stt.Type.IntervalDay(nullability=nullability))
 
-    raise ValueError(f"unsupported substrait unit: {unit!r}")
+        raise ValueError(f"unsupported substrait unit: {unit!r}")
 
 
 @translate.register
 def _array(dtype: dt.Array) -> stt.Type:
     return stt.Type(
         list=stt.Type.List(
             type=translate(dtype.value_type),
@@ -195,34 +240,33 @@
         ),
     )
 
 
 @translate.register(ir.Expr)
 def _expr(
     expr: ir.Expr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
-    return translate(expr.op(), expr, compiler, **kwargs)
+    return translate(expr.op(), compiler=compiler, **kwargs)
 
 
 @translate.register(ops.Literal)
 def _literal(
     op: ops.Literal,
-    expr: ir.ScalarExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
-    dtype = expr.type()
-    value = op.value
-    if value is None:
+    if op.value is None:
         return stalg.Expression(
-            literal=stalg.Expression.Literal(null=translate(dtype, **kwargs))
+            literal=stalg.Expression.Literal(null=translate(op.output_dtype, **kwargs))  # type: ignore
         )
-    return stalg.Expression(literal=translate_literal(dtype, op.value))
+    return stalg.Expression(literal=translate_literal(op.output_dtype, op.value))  # type: ignore
 
 
 @functools.singledispatch
 def translate_literal(
     dtype: dt.DataType,
     op: object,
 ) -> stalg.Expression.Literal:
@@ -237,130 +281,127 @@
 
 
 @translate_literal.register
 def _literal_boolean(
     dtype: dt.Boolean,
     value: bool,
 ) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(boolean=value, nullable=True)
+    return stalg.Expression.Literal(boolean=value)
 
 
 @translate_literal.register
 def _literal_int8(_: dt.Int8, value: int) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(i8=value, nullable=True)
+    return stalg.Expression.Literal(i8=value)
 
 
 @translate_literal.register
 def _literal_int16(_: dt.Int16, value: int) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(i16=value, nullable=True)
+    return stalg.Expression.Literal(i16=value)
 
 
 @translate_literal.register
 def _literal_int32(_: dt.Int32, value: int) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(i32=value, nullable=True)
+    return stalg.Expression.Literal(i32=value)
 
 
 @translate_literal.register
 def _literal_int64(d_: dt.Int64, value: int) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(i64=value, nullable=True)
+    return stalg.Expression.Literal(i64=value)
 
 
 @translate_literal.register
 def _literal_float32(_: dt.Float32, value: float) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(fp32=value, nullable=True)
+    return stalg.Expression.Literal(fp32=value)
 
 
 @translate_literal.register
 def _literal_float64(_: dt.Float64, value: float) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(fp64=value, nullable=True)
+    return stalg.Expression.Literal(fp64=value)
 
 
 @translate_literal.register
 def _literal_decimal(
     dtype: dt.Decimal, value: decimal.Decimal
 ) -> stalg.Expression.Literal:
     raise NotImplementedError
 
 
 @translate_literal.register
 def _literal_string(_: dt.String, value: str) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(string=value, nullable=True)
+    return stalg.Expression.Literal(string=value)
 
 
 @translate_literal.register
 def _literal_binary(_: dt.Binary, value: bytes) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(binary=value, nullable=True)
+    return stalg.Expression.Literal(binary=value)
 
 
 @translate_literal.register
 def _literal_timestamp(
     dtype: dt.Timestamp,
     value: datetime.datetime,
 ) -> stalg.Expression.Literal:
     micros_since_epoch = int(value.timestamp() * 1e6)
     if dtype.timezone is not None:
-        return stalg.Expression.Literal(timestamp_tz=micros_since_epoch, nullable=True)
-    return stalg.Expression.Literal(timestamp=micros_since_epoch, nullable=True)
+        return stalg.Expression.Literal(timestamp_tz=micros_since_epoch)
+    return stalg.Expression.Literal(timestamp=micros_since_epoch)
 
 
 @translate_literal.register
 def _literal_struct(
     dtype: dt.Struct,
     mapping: collections.OrderedDict,
 ) -> stalg.Expression.Literal:
     return stalg.Expression.Literal(
         struct=stalg.Expression.Literal.Struct(
             fields=[
                 translate_literal(field_type, val)
                 for val, field_type in zip(mapping.values(), dtype.types)
             ]
-        ),
-        nullable=True,
+        )
     )
 
 
 @translate_literal.register
 def _literal_map(
     dtype: dt.Map,
     mapping: collections.abc.MutableMapping,
 ) -> stalg.Expression.Literal:
     if not mapping:
-        return stalg.Expression.Literal(empty_map=translate(dtype).map, nullable=True)
+        return stalg.Expression.Literal(empty_map=translate(dtype).map)
     return stalg.Expression.Literal(
         map=stalg.Expression.Literal.Map(
             key_values=[
                 stalg.Expression.Literal.Map.KeyValue(
                     key=translate_literal(dtype.key_type, key),
                     value=translate_literal(dtype.value_type, value),
                 )
                 for key, value in mapping.items()
             ],
-        ),
-        nullable=True,
+        )
     )
 
 
 @translate_literal.register
 def _literal_array(
     dtype: dt.Array,
     sequence: Sequence[T],
 ) -> stalg.Expression.Literal:
     if not sequence:
-        return stalg.Expression.Literal(empty_list=translate(dtype).list, nullable=True)
+        return stalg.Expression.Literal(empty_list=translate(dtype).list)
     return stalg.Expression.Literal(
         list=stalg.Expression.Literal.List(
             values=[translate_literal(dtype.value_type, value) for value in sequence],
-        ),
-        nullable=True,
+        )
     )
 
 
 @translate_literal.register(dt.UUID)
 def _literal_uuid(dtype: dt.UUID, value: str | uuid.UUID) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(uuid=uuid.UUID(hex=str(value)).bytes, nullable=True)
+    return stalg.Expression.Literal(uuid=uuid.UUID(hex=str(value)).bytes)
 
 
 _MINUTES_PER_HOUR = _SECONDS_PER_MINUTE = 60
 _MICROSECONDS_PER_SECOND = 1_000_000
 
 
 def _time_to_micros(value: datetime.time) -> int:
@@ -371,25 +412,25 @@
         + value.second * _MICROSECONDS_PER_SECOND
         + value.microsecond
     )
 
 
 @translate_literal.register
 def _literal_time(time: dt.Time, value: datetime.time) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(time=_time_to_micros(value), nullable=True)
+    return stalg.Expression.Literal(time=_time_to_micros(value))
 
 
 def _date_to_days(value: datetime.date) -> int:
     delta = value - datetime.datetime.utcfromtimestamp(0).date()
     return delta.days
 
 
 @translate_literal.register
 def _literal_date(date: dt.Date, value: datetime.date) -> stalg.Expression.Literal:
-    return stalg.Expression.Literal(date=_date_to_days(value), nullable=True)
+    return stalg.Expression.Literal(date=_date_to_days(value))
 
 
 @functools.singledispatch
 def translate_preceding(value: int | None) -> stalg.Expression.WindowFunction.Bound:
     raise NotImplementedError()
 
 
@@ -420,181 +461,243 @@
 @translate_following.register
 def _following_int(offset: int) -> stalg.Expression.WindowFunction.Bound:
     return stalg.Expression.WindowFunction.Bound(
         following=stalg.Expression.WindowFunction.Bound.Following(offset=offset)
     )
 
 
+if IBIS_GTE_5:
+
+    @translate_following.register
+    @translate_preceding.register
+    def _window_boundary(  # type: ignore
+        boundary: ops.window.WindowBoundary,
+    ) -> stalg.Expression.WindowFunction.Bound:
+        # new window boundary class in Ibis 5.x
+        if boundary.preceding:
+            return translate_preceding(boundary.value.value)
+        else:
+            return translate_following(boundary.value.value)
+
+
 def _translate_window_bounds(
     precedes: tuple[int, int] | int | None,
     follows: tuple[int, int] | int | None,
 ) -> tuple[
     stalg.Expression.WindowFunction.Bound,
     stalg.Expression.WindowFunction.Bound,
 ]:
     # all preceding or all following or one or the other
     preceding = util.promote_list(precedes)
     following = util.promote_list(follows)
 
+    # Change in behavior of `promote_list` in Ibis 4.x so we do this for now
+    preceding = [None] if precedes is None else preceding
+    following = [None] if follows is None else following
+
     if len(preceding) == 2:
-        if following:
+        if following and following != [None]:
             raise ValueError(
                 "`following` not allowed when window bounds are both preceding"
             )
 
         lower, upper = preceding
         return translate_preceding(lower), translate_preceding(upper)
 
     if len(preceding) != 1:
         raise ValueError(f"preceding must be length 1 or 2 got: {len(preceding)}")
 
     if len(following) == 2:
-        if preceding:
+        if preceding and preceding != [None]:
             raise ValueError(
                 "`preceding` not allowed when window bounds are both following"
             )
 
         lower, upper = following
         return translate_following(lower), translate_following(upper)
     elif len(following) != 1:
         raise ValueError(f"following must be length 1 or 2 got: {len(following)}")
 
     return translate_preceding(*preceding), translate_following(*following)
 
 
-if version.parse(ibis.__version__) >= version.parse("3.0.0"):
-
-    @translate.register(ops.Alias)
-    def alias_op(
-        op: ops.Alias,
-        expr: ir.ValueExpr,
-        compiler: SubstraitCompiler,
-        **kwargs: Any,
-    ) -> stalg.Expression:
-        # For an alias, dispatch on the underlying argument
-        return translate(op.arg.op(), op.arg, compiler, **kwargs)
+@translate.register(ops.Alias)
+def alias_op(
+    op: ops.Alias,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    # For an alias, dispatch on the underlying argument
+    return translate(op.arg, compiler=compiler, **kwargs)
 
 
-@translate.register(ops.ValueOp)
+@translate.register(ops.ValueOp)  # type: ignore
 def value_op(
-    op: ops.ValueOp,
-    expr: ir.ValueExpr,
+    op: ops.ValueOp,  # type: ignore
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
+    # Check if scalar function is valid for input dtype(s) and insert casts as needed to
+    # make sure inputs are correct.
+    op = _check_and_upcast(op)
     # given the details of `op` -> function id
     return stalg.Expression(
         scalar_function=stalg.Expression.ScalarFunction(
-            function_reference=compiler.function_id(expr),
-            output_type=translate(expr.type()),
+            function_reference=compiler.function_id(op),
+            output_type=translate(op.output_dtype),
             arguments=[
-                stalg.FunctionArgument(value=translate(arg, compiler, **kwargs))
+                stalg.FunctionArgument(
+                    value=translate(arg, compiler=compiler, **kwargs)
+                )
                 for arg in op.args
-                if isinstance(arg, ir.Expr)
+                if isinstance(arg, ops.Value)
             ],
         )
     )
 
 
-@translate.register(ops.WindowOp)
+@translate.register(ops.WindowOp)  # type: ignore
 def window_op(
-    op: ops.WindowOp,
-    expr: ir.ValueExpr,
+    op: ops.WindowOp,  # type: ignore
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
-    lower_bound, upper_bound = _translate_window_bounds(
-        op.window.preceding, op.window.following
-    )
+    if IBIS_GTE_5:
+        # Ibis >= 5.x
+        window_gb = op.frame.group_by
+        window_ob = op.frame.order_by
+        start = op.frame.start
+        end = op.frame.end
+        func = op.func
+        func_args = op.func.args
+    else:
+        window_gb = op.window._group_by
+        window_ob = op.window._order_by
+        start = op.window.preceding
+        end = op.window.following
+        func = op.expr
+        func_args = op.expr.args
+
+    lower_bound, upper_bound = _translate_window_bounds(start, end)
+
     return stalg.Expression(
         window_function=stalg.Expression.WindowFunction(
-            function_reference=compiler.function_id(op.expr),
-            partitions=[
-                translate(gb, compiler, **kwargs) for gb in op.window._group_by
-            ],
-            sorts=[translate(ob, compiler, **kwargs) for ob in op.window._order_by],
-            output_type=translate(expr.type()),
+            function_reference=compiler.function_id(func),
+            partitions=[translate(gb, compiler=compiler, **kwargs) for gb in window_gb],
+            sorts=[translate(ob, compiler=compiler, **kwargs) for ob in window_ob],
+            output_type=translate(op.output_dtype),
             phase=stalg.AggregationPhase.AGGREGATION_PHASE_INITIAL_TO_RESULT,
             arguments=[
-                stalg.FunctionArgument(value=translate(arg, compiler, **kwargs))
-                for arg in op.expr.op().args
-                if isinstance(arg, ir.Expr)
+                stalg.FunctionArgument(
+                    value=translate(arg, compiler=compiler, **kwargs)
+                )
+                for arg in func_args
+                if isinstance(arg, ops.Value)
             ],
             lower_bound=lower_bound,
             upper_bound=upper_bound,
         )
     )
 
 
 @translate.register(ops.Reduction)
 def _reduction(
     op: ops.Reduction,
-    expr: ir.ScalarExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.AggregateFunction:
     return stalg.AggregateFunction(
-        function_reference=compiler.function_id(expr),
-        arguments=[stalg.FunctionArgument(value=translate(op.arg, compiler, **kwargs))],
+        function_reference=compiler.function_id(op),
+        arguments=[
+            stalg.FunctionArgument(value=translate(op.arg, compiler=compiler, **kwargs))  # type: ignore
+        ],
         sorts=[],  # TODO: ibis doesn't support this yet
         phase=stalg.AggregationPhase.AGGREGATION_PHASE_INITIAL_TO_RESULT,
-        output_type=translate(expr.type()),
+        output_type=translate(op.output_dtype),
     )
 
 
 @translate.register(ops.Count)
+@translate.register(ops.CountStar)
 def _count(
     op: ops.Count,
-    expr: ir.ScalarExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.AggregateFunction:
-    translated_args = []
-    arg = op.arg
-    if not isinstance(arg, ir.TableExpr):
+    translated_args: list[stalg.FunctionArgument] = []
+    if not isinstance(op.arg, ops.TableNode):
         translated_args.append(
-            stalg.FunctionArgument(value=translate(arg, compiler, **kwargs))
+            stalg.FunctionArgument(value=translate(op.arg, compiler=compiler, **kwargs))
         )
     return stalg.AggregateFunction(
-        function_reference=compiler.function_id(expr),
+        function_reference=compiler.function_id(op),
         arguments=translated_args,
         sorts=[],  # TODO: ibis doesn't support this yet
         phase=stalg.AggregationPhase.AGGREGATION_PHASE_INITIAL_TO_RESULT,
-        output_type=translate(expr.type()),
+        output_type=translate(op.output_dtype),
+    )
+
+
+@translate.register(ops.StandardDev)
+@translate.register(ops.Variance)
+def _variance_base(
+    op: ops.StandardDev | ops.Variance,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.AggregateFunction:
+    translated_arg = stalg.FunctionArgument(
+        value=translate(op.arg, compiler=compiler, **kwargs)
+    )
+    translated_how = stalg.FunctionOption(
+        name="distribution", preference=["POPULATION" if op.how == "pop" else "SAMPLE"]
+    )
+    return stalg.AggregateFunction(
+        function_reference=compiler.function_id(op=op),
+        arguments=[translated_arg],
+        options=[translated_how],
+        sorts=[],  # TODO: ibis doesn't support this yet
+        phase=stalg.AggregationPhase.AGGREGATION_PHASE_INITIAL_TO_RESULT,
+        output_type=translate(op.output_dtype),
     )
 
 
 @translate.register(ops.SortKey)
 def sort_key(
     op: ops.SortKey,
-    expr: ir.SortExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.SortField:
     ordering = "ASC" if op.ascending else "DESC"
     return stalg.SortField(
-        expr=translate(op.expr, compiler, **kwargs),
+        expr=translate(op.expr, compiler=compiler, **kwargs),
         direction=getattr(
             stalg.SortField.SortDirection,
             f"SORT_DIRECTION_{ordering}_NULLS_FIRST",
         ),
     )
 
 
 @translate.register(ops.TableColumn)
 def table_column(
     op: ops.TableColumn,
-    expr: ir.ColumnExpr,
-    _: SubstraitCompiler,
     *,
+    compiler: SubstraitCompiler,
     child_rel_field_offsets: MutableMapping[ops.TableNode, int] | None = None,
+    **kwargs: Any,
 ) -> stalg.Expression:
-    schema = op.table.schema()
+    schema = op.table.schema
     relative_offset = schema._name_locs[op.name]
-    base_offset = (child_rel_field_offsets or {}).get(op.table.op(), 0)
+    base_offset = (child_rel_field_offsets or {}).get(op.table, 0)
     absolute_offset = base_offset + relative_offset
     return stalg.Expression(
         selection=stalg.Expression.FieldReference(
             root_reference=stalg.Expression.FieldReference.RootReference(),
             direct_reference=stalg.Expression.ReferenceSegment(
                 struct_field=stalg.Expression.ReferenceSegment.StructField(
                     field=absolute_offset,
@@ -603,23 +706,23 @@
         )
     )
 
 
 @translate.register(ops.StructField)
 def struct_field(
     op: ops.StructField,
-    _: ir.ColumnExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
     child = translate(op.arg, compiler=compiler, **kwargs)
     field_name = op.field
     # TODO: store names/types inverse mapping on datatypes.Struct for O(1)
     # access to field index
-    field_index = op.arg.type().names.index(field_name)
+    field_index = op.arg.output_dtype.names.index(field_name)
 
     struct_field = child.selection.direct_reference.struct_field
 
     # keep digging until we bottom out on the deepest child reference which
     # becomes the parent for the returned reference
     while struct_field.HasField("child"):
         struct_field = struct_field.child.struct_field
@@ -633,105 +736,144 @@
     )
 
     return child
 
 
 @translate.register(ops.UnboundTable)
 def unbound_table(
-    op: ops.UnboundTable, expr: ir.TableExpr, _: SubstraitCompiler, **kwargs: Any
+    op: ops.UnboundTable,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
 ) -> stalg.Rel:
     return stalg.Rel(
         read=stalg.ReadRel(
             # TODO: filter,
             # TODO: projection,
+            common=stalg.RelCommon(direct=stalg.RelCommon.Direct()),
             base_schema=translate(op.schema),
             named_table=stalg.ReadRel.NamedTable(names=[op.name]),
         )
     )
 
 
-def _get_child_relation_field_offsets(table: ir.TableExpr) -> dict[ops.TableNode, int]:
+def _get_child_relation_field_offsets(table: ops.TableNode) -> dict[ops.TableNode, int]:
     """Return the offset of each of table's fields.
 
     This function calculates the starting index of a relations fields, as if
     all relations were part of a single flat schema.
 
     Examples
     --------
     >>> import ibis
     >>> t1 = ibis.table(
     ...     [("a", "int64"), ("b", "string"), ("c", "array<int64>")],
     ...     name="t1",
     ... )
     >>> t2 = ibis.table([("d", "string"), ("e", "map<string, float64>")], name="t2")
     >>> expr = t1.join(t2, t1.b == t2.d)
-    >>> mapping = _get_child_relation_field_offsets(expr)
+    >>> mapping = _get_child_relation_field_offsets(expr.op())
     >>> mapping[t1.op()]  # the first relation is always zero
     0
     >>> mapping[t2.op()]  # first relation has 3 fields, so the second starts at 3
     3
     """
-    table_op = table.op()
-    if isinstance(table_op, ops.Join):
-        root_tables = [table_op.left.op(), table_op.right.op()]
-        accum = itertools.accumulate((len(t.schema) for t in root_tables), initial=0)
-        return dict(zip(root_tables, accum))
+    if isinstance(table, ops.Join):
+        # Descend into the left and right tables to grab offsets from nested joins
+        left_keys = _get_child_relation_field_offsets(table.left)
+        right_keys = _get_child_relation_field_offsets(table.right)
+        root_tables = [table.left, table.right]
+        accum = [0, len(root_tables[0].schema)]
+        return toolz.merge(left_keys, right_keys, dict(zip(root_tables, accum)))
     return {}
 
 
 @translate.register(ops.Selection)
 def selection(
     op: ops.Selection,
-    expr: ir.TableExpr,
+    *,
     compiler: SubstraitCompiler,
     child_rel_field_offsets: Mapping[ops.TableNode, int] | None = None,
     **kwargs: Any,
 ) -> stalg.Rel:
     assert (
         not child_rel_field_offsets
     ), "non-empty child_rel_field_offsets passed in to selection translation rule"
     child_rel_field_offsets = _get_child_relation_field_offsets(op.table)
     # source
     relation = translate(
         op.table,
-        compiler,
+        compiler=compiler,
         child_rel_field_offsets=child_rel_field_offsets,
         **kwargs,
     )
-
     # filter
     if op.predicates:
+        predicates = [pred.to_expr() for pred in op.predicates]
         relation = stalg.Rel(
             filter=stalg.FilterRel(
                 input=relation,
                 condition=translate(
-                    functools.reduce(operator.and_, op.predicates),
-                    compiler,
+                    functools.reduce(operator.and_, predicates),
+                    compiler=compiler,
                     child_rel_field_offsets=child_rel_field_offsets,
                     **kwargs,
                 ),
             )
         )
 
-    # projection
-    selections = [
-        col
-        for sel in op.selections
-        for col in (
-            sel.get_columns(sel.columns) if isinstance(sel, ir.TableExpr) else [sel]
-        )
-    ]
-    if op.selections:
+    if selections := _get_selections(op):
+        rels = [
+            (attr, getattr(relation, attr))
+            for attr in (
+                "aggregate",
+                "cross",
+                "extension_leaf",
+                "extension_multi",
+                "extension_single",
+                "fetch",
+                "filter",
+                "join",
+                "project",
+                "read",
+                "set",
+                "sort",
+            )
+        ]
+        for relname, rel in rels:
+            if relname == "aggregate" and rel.measures:
+                mapping_counter = itertools.count(
+                    len(rel.measures) + len(rel.groupings)
+                )
+                break
+            elif output_mapping := rel.common.emit.output_mapping:
+                mapping_counter = itertools.count(len(output_mapping))
+                break
+            elif not isinstance(op.table, ops.Join):
+                # If child table is join, we cannot reliably call schema due to
+                # potentially duplicate column names, so fallback to the orignal
+                # logic.
+                mapping_counter = itertools.count(len(op.table.schema))
+                break
+        else:
+            source_tables = _find_parent_tables(op)
+            mapping_counter = itertools.count(sum(len(t.schema) for t in source_tables))
+
         relation = stalg.Rel(
             project=stalg.ProjectRel(
                 input=relation,
+                common=stalg.RelCommon(
+                    emit=stalg.RelCommon.Emit(
+                        output_mapping=[next(mapping_counter) for _ in selections]
+                    )
+                ),
                 expressions=[
                     translate(
                         selection,
-                        compiler,
+                        compiler=compiler,
                         child_rel_field_offsets=child_rel_field_offsets,
                         **kwargs,
                     )
                     for selection in selections
                 ],
             )
         )
@@ -740,26 +882,53 @@
     if op.sort_keys:
         relation = stalg.Rel(
             sort=stalg.SortRel(
                 input=relation,
                 sorts=[
                     translate(
                         key,
-                        compiler,
+                        compiler=compiler,
                         child_rel_field_offsets=child_rel_field_offsets,
                         **kwargs,
                     )
                     for key in op.sort_keys
                 ],
             )
         )
 
     return relation
 
 
+def _get_selections(op: ops.Selection) -> Sequence[ir.Column]:
+    # projection / emit
+    selections = [
+        col
+        for sel in (x.to_expr() for x in op.selections)  # map ops to exprs
+        for col in (
+            map(sel.__getitem__, sel.columns)
+            if isinstance(sel, ir.TableExpr)  # type: ignore
+            else [sel]
+        )
+    ]
+
+    return selections
+
+
+def _find_parent_tables(op: ops.Selection) -> set[ops.PhysicalTable]:
+    # TODO: settle on a better source table definition than "PhysicalTable with
+    # a schema"
+    source_tables = {
+        t
+        for t in toposort(op).keys()
+        if isinstance(t, ops.PhysicalTable) and hasattr(t, "schema")
+    }
+
+    return source_tables
+
+
 @functools.singledispatch
 def _translate_join_type(op: ops.Join) -> stalg.JoinRel.JoinType.V:
     raise NotImplementedError(f"join type `{type(op).__name__}` not implemented")
 
 
 @_translate_join_type.register(ops.InnerJoin)
 def _translate_inner_join(_: ops.InnerJoin) -> stalg.JoinRel.JoinType.V:
@@ -790,45 +959,48 @@
 def _translate_anti_join(_: ops.LeftAntiJoin) -> stalg.JoinRel.JoinType.V:
     return stalg.JoinRel.JoinType.JOIN_TYPE_ANTI
 
 
 @translate.register(ops.Join)
 def join(
     op: ops.Join,
-    expr: ir.TableExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Rel:
     child_rel_field_offsets = kwargs.pop("child_rel_field_offsets", None)
+    child_rel_field_offsets = (
+        child_rel_field_offsets or _get_child_relation_field_offsets(op)
+    )
+    predicates = [pred.to_expr() for pred in op.predicates]
     return stalg.Rel(
         join=stalg.JoinRel(
-            left=translate(op.left, compiler, **kwargs),
-            right=translate(op.right, compiler, **kwargs),
+            left=translate(op.left, compiler=compiler, **kwargs),
+            right=translate(op.right, compiler=compiler, **kwargs),
             expression=translate(
-                functools.reduce(operator.and_, op.predicates),
-                compiler,
-                child_rel_field_offsets=child_rel_field_offsets
-                or _get_child_relation_field_offsets(expr),
+                functools.reduce(operator.and_, predicates),
+                compiler=compiler,
+                child_rel_field_offsets=child_rel_field_offsets,
                 **kwargs,
             ),
             type=_translate_join_type(op),
         )
     )
 
 
 @translate.register(ops.Limit)
 def limit(
     op: ops.Limit,
-    expr: ir.Expr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Rel:
     return stalg.Rel(
         fetch=stalg.FetchRel(
-            input=translate(op.table, compiler, **kwargs),
+            input=translate(op.table, compiler=compiler, **kwargs),
             offset=op.offset,
             count=op.n,
         )
     )
 
 
 @functools.singledispatch
@@ -854,142 +1026,459 @@
 def set_op_type_difference(op: ops.Difference) -> stalg.SetRel.SetOp.V:
     return stalg.SetRel.SetOp.SET_OP_MINUS_PRIMARY
 
 
 @translate.register(ops.SetOp)
 def set_op(
     op: ops.SetOp,
-    expr: ir.TableExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Rel:
     return stalg.Rel(
         set=stalg.SetRel(
             inputs=[
-                translate(op.left, compiler, **kwargs),
-                translate(op.right, compiler, **kwargs),
+                translate(op.left, compiler=compiler, **kwargs),
+                translate(op.right, compiler=compiler, **kwargs),
             ],
             op=translate_set_op_type(op),
         )
     )
 
 
 @translate.register(ops.Aggregation)
 def aggregation(
     op: ops.Aggregation,
-    expr: ir.TableExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Rel:
     if op.having:
         raise NotImplementedError("`having` not yet implemented")
 
-    table = op.table
-    predicates = op.predicates
+    table = op.table.to_expr()
+    predicates = [pred.to_expr() for pred in op.predicates]
     input = translate(
         table.filter(predicates) if predicates else table,
-        compiler,
+        compiler=compiler,
         **kwargs,
     )
 
     # TODO: we handle sorts before aggregation here but we shouldn't be
     #
     # sorts should be compiled after after aggregation, because that is
     # semantically where they belong, but due to ibis storing sort keys in the
     # aggregate class we have to sort first, so ibis will use the correct base
     # table when decompiling
     if op.sort_keys:
-        sorts = [translate(key, compiler, **kwargs) for key in op.sort_keys]
+        sorts = [translate(key, compiler=compiler, **kwargs) for key in op.sort_keys]
         input = stalg.Rel(sort=stalg.SortRel(input=input, sorts=sorts))
 
     aggregate = stalg.AggregateRel(
         input=input,
         groupings=[
             stalg.AggregateRel.Grouping(
-                grouping_expressions=[translate(by, compiler, **kwargs)]
+                grouping_expressions=[translate(by, compiler=compiler, **kwargs)]
             )
             for by in op.by
         ],
         measures=[
-            stalg.AggregateRel.Measure(measure=translate(metric, compiler, **kwargs))
+            stalg.AggregateRel.Measure(
+                measure=translate(metric, compiler=compiler, **kwargs)
+            )
             for metric in op.metrics
         ],
     )
 
     return stalg.Rel(aggregate=aggregate)
 
 
 @translate.register(ops.SimpleCase)
 @translate.register(ops.SearchedCase)
 def _simple_searched_case(
     op: ops.SimpleCase | ops.SearchedCase,
-    expr: ir.TableExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
     # the field names for an `if_then` are `if` and `else` which means we need
     # to pass those args in as a dictionary to not run afoul of SyntaxErrors`
     _ifs = []
     for case, result in zip(op.cases, op.results):
-        if_expr = case if not hasattr(op, "base") else op.base == case
+        if_expr = case if not hasattr(op, "base") else op.base.to_expr() == case
         _if = {
-            "if": translate(if_expr, compiler, **kwargs),
-            "then": translate(result, compiler, **kwargs),
+            "if": translate(if_expr, compiler=compiler, **kwargs),
+            "then": translate(result, compiler=compiler, **kwargs),
         }
         _ifs.append(stalg.Expression.IfThen.IfClause(**_if))
 
-    _else = {"else": translate(op.default, compiler, **kwargs)}
+    _else = {"else": translate(op.default, compiler=compiler, **kwargs)}
+
+    return stalg.Expression(if_then=stalg.Expression.IfThen(ifs=_ifs, **_else))
+
+
+@translate.register(ops.Where)
+def _where(
+    op: ops.Where,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    # the field names for an `if_then` are `if` and `else` which means we need
+    # to pass those args in as a dictionary to not run afoul of SyntaxErrors`
+    _if = {
+        "if": translate(op.bool_expr, compiler=compiler, **kwargs),
+        "then": translate(op.true_expr, compiler=compiler, **kwargs),
+    }
+    _else = {"else": translate(op.false_null_expr, compiler=compiler, **kwargs)}
+
+    _ifs = [stalg.Expression.IfThen.IfClause(**_if)]
 
     return stalg.Expression(if_then=stalg.Expression.IfThen(ifs=_ifs, **_else))
 
 
 @translate.register(ops.Contains)
 def _contains(
     op: ops.Contains,
-    expr: ir.TableExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
+    options = (
+        op.options
+        if isinstance(op.options, Iterable)
+        else ibis.util.promote_list(op.options)
+    )
     return stalg.Expression(
         singular_or_list=stalg.Expression.SingularOrList(
-            value=translate(op.value, compiler, **kwargs),
-            options=[translate(value, compiler, **kwargs) for value in op.options],
+            value=translate(op.value, compiler=compiler, **kwargs),
+            options=[
+                translate(value, compiler=compiler, **kwargs) for value in options
+            ],
         )
     )
 
 
 @translate.register(ops.Cast)
 def _cast(
     op: ops.Cast,
-    expr: ir.TableExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
     return stalg.Expression(
         cast=stalg.Expression.Cast(
-            type=translate(op.to), input=translate(op.arg, compiler, **kwargs)
+            type=translate(op.to),
+            input=translate(op.arg, compiler=compiler, **kwargs),
+            failure_behavior=stalg.Expression.Cast.FAILURE_BEHAVIOR_THROW_EXCEPTION,
         )
     )
 
 
 @translate.register(ops.ExtractDateField)
 def _extractdatefield(
     op: ops.ExtractDateField,
-    expr: ir.TableExpr,
+    *,
     compiler: SubstraitCompiler,
     **kwargs: Any,
 ) -> stalg.Expression:
     # e.g. "ExtractYear" -> "YEAR"
     span = type(op).__name__[len("Extract") :].upper()
     arguments = (
-        stalg.FunctionArgument(value=translate(arg, compiler, **kwargs))
+        stalg.FunctionArgument(value=translate(arg, compiler=compiler, **kwargs))
         for arg in op.args
-        if isinstance(arg, ir.Expr)
+        if isinstance(arg, ops.Value)
     )
-
     scalar_func = stalg.Expression.ScalarFunction(
-        function_reference=compiler.function_id(expr),
-        output_type=translate(expr.type()),
+        function_reference=compiler.function_id(op),
+        output_type=translate(op.output_dtype),
     )
-    scalar_func.arguments.add(enum=stalg.FunctionArgument.Enum(specified=span))
+    scalar_func.arguments.add(enum=span)
     scalar_func.arguments.extend(arguments)
     return stalg.Expression(scalar_function=scalar_func)
+
+
+@translate.register(ops.Log)
+def _log(
+    op: ops.Log,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    arg = stalg.FunctionArgument(value=translate(op.arg, compiler=compiler, **kwargs))
+    base = stalg.FunctionArgument(
+        value=translate(
+            op.base if op.base is not None else ibis.literal(math.e),
+            compiler=compiler,
+            **kwargs,
+        )
+    )
+
+    scalar_func = stalg.Expression.ScalarFunction(
+        function_reference=compiler.function_id(op),
+        output_type=translate(op.output_dtype),
+        arguments=[arg, base],
+    )
+    return stalg.Expression(scalar_function=scalar_func)
+
+
+@translate.register(ops.FloorDivide)
+def _floordivide(
+    op: ops.FloorDivide,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    left, right = op.left, op.right
+    return translate((left / right).floor(), compiler=compiler, **kwargs)
+
+
+@translate.register(ops.Clip)
+def _clip(
+    op: ops.Clip,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    arg, lower, upper = op.arg, op.lower, op.upper
+
+    if lower is not None and upper is not None:
+        return translate(
+            (arg >= lower).ifelse((arg <= upper).ifelse(arg, upper), lower),
+            compiler=compiler,
+            **kwargs,
+        )
+    elif lower is not None:
+        return translate(
+            (arg >= lower).ifelse(arg, lower),
+            compiler=compiler,
+            **kwargs,
+        )
+    elif upper is not None:
+        return translate(
+            (arg <= upper).ifelse(arg, upper),
+            compiler=compiler,
+            **kwargs,
+        )
+    raise AssertionError()
+
+
+@translate.register(ops.TableArrayView)
+def _table_array_view(
+    op: ops.TableArrayView,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    return translate(op.table, compiler=compiler, **kwargs)
+
+
+@translate.register(ops.SelfReference)
+def _self_reference(
+    op: ops.SelfReference,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    return translate(op.table, compiler=compiler, **kwargs)
+
+
+@translate.register(ops.ExistsSubquery)
+def _exists_subquery(
+    op: ops.ExistsSubquery,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    tuples = stalg.Rel(
+        filter=stalg.FilterRel(
+            input=translate(op.foreign_table, compiler=compiler),
+            condition=translate(
+                functools.reduce(ops.And, op.predicates),  # type: ignore
+                compiler=compiler,
+                **kwargs,
+            ),
+        )
+    )
+
+    return stalg.Expression(
+        subquery=stalg.Expression.Subquery(
+            set_predicate=stalg.Expression.Subquery.SetPredicate(
+                predicate_op=stalg.Expression.Subquery.SetPredicate.PREDICATE_OP_EXISTS,
+                tuples=tuples,
+            )
+        )
+    )
+
+
+@translate.register(ops.NotExistsSubquery)
+def _not_exists_subquery(
+    op: ops.NotExistsSubquery,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    assert compiler is not None
+    tuples = stalg.Rel(
+        filter=stalg.FilterRel(
+            input=translate(op.foreign_table, compiler=compiler),
+            condition=translate(
+                functools.reduce(ops.And, op.predicates),  # type: ignore
+                compiler=compiler,
+                **kwargs,
+            ),
+        )
+    )
+
+    return stalg.Expression(
+        scalar_function=stalg.Expression.ScalarFunction(
+            function_reference=compiler.function_id(ops.Not(op)),  # type: ignore
+            output_type=translate(op.output_dtype),
+            arguments=[
+                stalg.FunctionArgument(
+                    value=stalg.Expression(
+                        subquery=stalg.Expression.Subquery(
+                            set_predicate=stalg.Expression.Subquery.SetPredicate(
+                                predicate_op=stalg.Expression.Subquery.SetPredicate.PREDICATE_OP_EXISTS,
+                                tuples=tuples,
+                            )
+                        )
+                    )
+                )
+            ],
+        )
+    )
+
+
+@translate.register(ops.Floor)
+@translate.register(ops.Ceil)
+def _floor_ceil_cast(
+    op: ops.Floor,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    output_type = translate(op.output_dtype)
+    input = stalg.Expression(
+        scalar_function=stalg.Expression.ScalarFunction(
+            function_reference=compiler.function_id(op),
+            output_type=output_type,
+            arguments=[
+                stalg.FunctionArgument(
+                    value=translate(arg, compiler=compiler, **kwargs)
+                )
+                for arg in op.func_args  # type: ignore
+                if isinstance(arg, ops.Value)
+            ],
+        )
+    )
+    return stalg.Expression(
+        cast=stalg.Expression.Cast(
+            type=output_type,
+            input=input,
+            failure_behavior=stalg.Expression.Cast.FAILURE_BEHAVIOR_THROW_EXCEPTION,
+        )
+    )
+
+
+@translate.register(ops.ElementWiseVectorizedUDF)
+def _elementwise_udf(
+    op: ops.ElementWiseVectorizedUDF,
+    *,
+    compiler: SubstraitCompiler,
+    **kwargs: Any,
+) -> stalg.Expression:
+    if compiler.udf_uri is None:
+        raise ValueError(
+            """
+Cannot compile a Substrait plan that contains a UDF unless the
+compiler has a `udf_uri` attached.
+        """
+        )
+
+    # For referring to scalar function within plan use "{op_name}_{udf_name}"
+    # since op_name alone will collide with >1 UDF
+    udf_key = f"{type(op).__name__}_{op.func.__name__}"
+
+    # Explicitly register extension uri
+    extension_uri = compiler.register_extension_uri(compiler.udf_uri)
+
+    # Explicitly register extension function
+    try:
+        func_ext = compiler.function_extensions[udf_key]
+    except KeyError:
+        func_ext = compiler.function_extensions[
+            udf_key
+        ] = compiler.create_extension_function(extension_uri, op.func.__name__)
+
+    return stalg.Expression(
+        scalar_function=stalg.Expression.ScalarFunction(
+            function_reference=func_ext.function_anchor,
+            output_type=translate(op.return_type),
+            arguments=[
+                stalg.FunctionArgument(
+                    value=translate(arg, compiler=compiler, **kwargs)
+                )
+                for arg in op.func_args
+                if isinstance(arg, ops.Value)
+            ],
+        )
+    )
+
+
+def _check_and_upcast(op: ops.Node) -> ops.Node:
+    """Check that arguments to extension functions have consistent types."""
+    op_name = IBIS_SUBSTRAIT_OP_MAPPING[type(op).__name__]
+
+    anykey = ("any",) * len([arg for arg in op.args if arg is not None])
+
+    # First check if `any` is an option
+    function_extension = _extension_mapping[op_name].get(anykey)
+
+    # Otherwise, if the types don't match, cast up
+    if function_extension is None:
+        op = _upcast(op)
+
+    return op
+
+
+@functools.singledispatch
+def _upcast(op: ops.Node) -> Any:
+    return op
+
+
+@_upcast.register(ops.Binary)
+def _upcast_bin_op(op: ops.Binary) -> ops.Binary:
+    left, right = op.left.output_dtype, op.right.output_dtype
+
+    if left == right:
+        return op
+    elif dt.castable(left, right, upcast=True):
+        return type(op)(ops.Cast(op.left, to=right), op.right)  # type: ignore
+    elif dt.castable(right, left, upcast=True):
+        return type(op)(op.left, ops.Cast(op.right, to=left))  # type: ignore
+    else:
+        raise TypeError(
+            f"binop {type(op).__name__} called with incompatible types {left=} {right=}"
+        )
+
+
+string_op: TypeAlias = Union[
+    ops.Substring, ops.StrRight, ops.Repeat, ops.StringFind, ops.LPad, ops.RPad
+]
+
+
+@_upcast.register(ops.Substring)
+@_upcast.register(ops.StrRight)
+@_upcast.register(ops.Repeat)
+@_upcast.register(ops.StringFind)
+@_upcast.register(ops.LPad)
+@_upcast.register(ops.RPad)
+def _upcast_string_op(op: string_op) -> string_op:
+    # Substrait wants Int32 for all numeric args to string functions
+    casted_args = [
+        ops.Cast(newop, to=dt.Int32())  # type: ignore
+        if isinstance(newop.output_dtype, dt.SignedInteger)
+        else newop
+        for newop in op.args
+    ]
+    return type(op)(*casted_args)
```

### Comparing `ibis-substrait-2.9.8/ibis_substrait/tests/compiler/conftest.py` & `ibis_substrait-3.0.0/ibis_substrait/tests/compiler/conftest.py`

 * *Files identical despite different names*

### Comparing `ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_literal.py` & `ibis_substrait-3.0.0/ibis_substrait/tests/compiler/test_literal.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,19 +3,18 @@
 import uuid
 from collections import OrderedDict
 
 import ibis
 import ibis.expr.datatypes as dt
 import pytest
 import pytz
+from substrait.gen.proto import algebra_pb2 as stalg
+from substrait.gen.proto import type_pb2 as stt
 
-from ibis_substrait.compiler.decompile import decompile
 from ibis_substrait.compiler.translate import _date_to_days, _time_to_micros, translate
-from ibis_substrait.proto.substrait.ibis import algebra_pb2 as stalg
-from ibis_substrait.proto.substrait.ibis import type_pb2 as stt
 
 NULLABILITY_NULLABLE = stt.Type.Nullability.NULLABILITY_NULLABLE
 
 TIMESTAMP = datetime.datetime(
     year=2021,
     month=11,
     day=15,
@@ -34,39 +33,29 @@
 
 literal_cases = pytest.mark.parametrize(
     ("expr", "ir"),
     [
         # booleans
         pytest.param(
             ibis.literal(True),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    boolean=True, nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(boolean=True)),
             id="boolean_true",
         ),
         pytest.param(
             ibis.literal(False),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    boolean=False, nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(boolean=False)),
             id="boolean_false",
         ),
     ]
     + [
         # integers
         pytest.param(
             ibis.literal(value),
             stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    **{substrait_type: value}, nullable=NULLABILITY_NULLABLE
-                )
+                literal=stalg.Expression.Literal(**{substrait_type: value})
             ),
             id=f"{substrait_type}_{value_name}",
         )
         for ibis_type, substrait_type in [
             (dt.int8, "i8"),
             (dt.int16, "i16"),
             (dt.int32, "i32"),
@@ -74,114 +63,85 @@
         ]
         for value_name, value in ibis_type.bounds._asdict().items()
     ]
     + [
         # floating point
         pytest.param(
             ibis.literal(1.0, type="float64"),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    fp64=1.0, nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(fp64=1.0)),
             id="fp64",
         ),
         pytest.param(
             ibis.literal(2.0, type="float32"),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    fp32=2.0, nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(fp32=2.0)),
             id="fp32",
         ),
         # strings
         pytest.param(
             ibis.literal("foo"),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    string="foo", nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(string="foo")),
             id="string",
         ),
         pytest.param(
-            ibis.literal("⋃"),
+            ibis.literal("⋃"),  # noqa: RUF001
             stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    string="⋃", nullable=NULLABILITY_NULLABLE
-                )
+                literal=stalg.Expression.Literal(string="⋃")  # noqa: RUF001
             ),
             id="unicode_string",
         ),
         # binary
         pytest.param(
             ibis.literal(b"42", type="binary"),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    binary=b"42", nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(binary=b"42")),
             id="binary",
         ),
         # timestamp
         pytest.param(
             ibis.timestamp(TIMESTAMP),
             stalg.Expression(
                 literal=stalg.Expression.Literal(
-                    timestamp=int(MICROSECONDS_SINCE_EPOCH),
-                    nullable=NULLABILITY_NULLABLE,
+                    timestamp=int(MICROSECONDS_SINCE_EPOCH)
                 ),
             ),
             id="timestamp",
         ),
         pytest.param(
             ibis.timestamp(
                 datetime.datetime.fromtimestamp(TIMESTAMP.timestamp(), tz=pytz.utc),
                 timezone="UTC",
             ),
             stalg.Expression(
                 literal=stalg.Expression.Literal(
-                    timestamp_tz=int(MICROSECONDS_SINCE_EPOCH),
-                    nullable=NULLABILITY_NULLABLE,
+                    timestamp_tz=int(MICROSECONDS_SINCE_EPOCH)
                 ),
             ),
             id="timestamp_tz",
         ),
         # date
         pytest.param(
             ibis.date(DATE.isoformat()),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    date=DATE_DAYS, nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(date=DATE_DAYS)),
             id="date",
         ),
         # time
         pytest.param(
             ibis.time(TIME),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    time=TIME_MICROS, nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(time=TIME_MICROS)),
             id="time",
         ),
     ]
     + [
         # interval_year_to_month
         pytest.param(
             ibis.interval(**{key: value}),
             stalg.Expression(
                 literal=stalg.Expression.Literal(
                     interval_year_to_month=(
                         stalg.Expression.Literal.IntervalYearToMonth(**{key: value})
-                    ),
-                    nullable=NULLABILITY_NULLABLE,
+                    )
                 ),
             ),
             id=f"interval_year_to_month_{key}",
             marks=[pytest.mark.xfail(raises=NotImplementedError)],
         )
         for key, value in [("years", 84), ("months", 42)]
     ]
@@ -189,16 +149,15 @@
         # interval_day_to_second
         pytest.param(
             ibis.interval(**{key: value}),
             stalg.Expression(
                 literal=stalg.Expression.Literal(
                     interval_day_to_second=(
                         stalg.Expression.Literal.IntervalDayToSecond(**{key: value})
-                    ),
-                    nullable=NULLABILITY_NULLABLE,
+                    )
                 ),
             ),
             id=f"interval_day_to_second_{key}",
             marks=[pytest.mark.xfail(raises=NotImplementedError)],
         )
         for key, value in [("days", 84), ("seconds", 42)]
     ]
@@ -209,76 +168,57 @@
         # struct
         pytest.param(
             ibis.literal(OrderedDict(a=1.0, b=[2.0])),
             stalg.Expression(
                 literal=stalg.Expression.Literal(
                     struct=stalg.Expression.Literal.Struct(
                         fields=[
-                            stalg.Expression.Literal(
-                                fp64=1.0, nullable=NULLABILITY_NULLABLE
-                            ),
+                            stalg.Expression.Literal(fp64=1.0),
                             stalg.Expression.Literal(
                                 list=stalg.Expression.Literal.List(
-                                    values=[
-                                        stalg.Expression.Literal(
-                                            fp64=2.0, nullable=NULLABILITY_NULLABLE
-                                        )
-                                    ],
+                                    values=[stalg.Expression.Literal(fp64=2.0)],
                                 ),
-                                nullable=NULLABILITY_NULLABLE,
                             ),
                         ]
                     ),
-                    nullable=NULLABILITY_NULLABLE,
                 ),
             ),
             id="struct",
             marks=[pytest.mark.no_decompile],
         ),
         # map
         pytest.param(
             ibis.literal(dict(a=[], b=[2])),
             stalg.Expression(
                 literal=stalg.Expression.Literal(
                     map=stalg.Expression.Literal.Map(
                         key_values=[
                             stalg.Expression.Literal.Map.KeyValue(
-                                key=stalg.Expression.Literal(
-                                    string="a", nullable=NULLABILITY_NULLABLE
-                                ),
+                                key=stalg.Expression.Literal(string="a"),
                                 value=stalg.Expression.Literal(
                                     empty_list=stt.Type.List(
                                         type=stt.Type(
                                             i8=stt.Type.I8(
                                                 nullability=NULLABILITY_NULLABLE
                                             )
                                         ),
                                         nullability=NULLABILITY_NULLABLE,
                                     ),
-                                    nullable=NULLABILITY_NULLABLE,
                                 ),
                             ),
                             stalg.Expression.Literal.Map.KeyValue(
-                                key=stalg.Expression.Literal(
-                                    string="b", nullable=NULLABILITY_NULLABLE
-                                ),
+                                key=stalg.Expression.Literal(string="b"),
                                 value=stalg.Expression.Literal(
                                     list=stalg.Expression.Literal.List(
-                                        values=[
-                                            stalg.Expression.Literal(
-                                                i8=2, nullable=NULLABILITY_NULLABLE
-                                            )
-                                        ],
+                                        values=[stalg.Expression.Literal(i8=2)],
                                     ),
-                                    nullable=NULLABILITY_NULLABLE,
                                 ),
                             ),
                         ],
                     ),
-                    nullable=NULLABILITY_NULLABLE,
                 ),
             ),
             id="map",
         ),
         # empty map
         pytest.param(
             ibis.literal({}, type="map<string, int64>"),
@@ -289,38 +229,29 @@
                             string=stt.Type.String(nullability=NULLABILITY_NULLABLE)
                         ),
                         value=stt.Type(
                             i64=stt.Type.I64(nullability=NULLABILITY_NULLABLE)
                         ),
                         nullability=NULLABILITY_NULLABLE,
                     ),
-                    nullable=NULLABILITY_NULLABLE,
                 )
             ),
             id="empty_map",
         ),
     ]
     + [
         # uuid
         pytest.param(
             ibis.literal(UUID, type=dt.uuid),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    uuid=UUID.bytes, nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(uuid=UUID.bytes)),
             id="uuid_typed",
         ),
         pytest.param(
             ibis.literal(str(UUID), type=dt.uuid),
-            stalg.Expression(
-                literal=stalg.Expression.Literal(
-                    uuid=UUID.bytes, nullable=NULLABILITY_NULLABLE
-                )
-            ),
+            stalg.Expression(literal=stalg.Expression.Literal(uuid=UUID.bytes)),
             id="uuid_string",
         ),
     ]
     + [
         # null
         pytest.param(
             ibis.literal(None, type="float64"),
@@ -350,34 +281,29 @@
         # list
         pytest.param(
             ibis.literal(["a", "b"]),  # called Array in ibis
             stalg.Expression(
                 literal=stalg.Expression.Literal(
                     list=stalg.Expression.Literal.List(
                         values=[
-                            stalg.Expression.Literal(
-                                string="a", nullable=NULLABILITY_NULLABLE
-                            ),
-                            stalg.Expression.Literal(
-                                string="b", nullable=NULLABILITY_NULLABLE
-                            ),
+                            stalg.Expression.Literal(string="a"),
+                            stalg.Expression.Literal(string="b"),
                         ],
                     ),
-                    nullable=NULLABILITY_NULLABLE,
                 ),
             ),
             id="array",
         ),
     ],
 )
 
 
 @literal_cases
 def test_literal(compiler, expr, ir):
-    result = translate(expr, compiler)
+    result = translate(expr, compiler=compiler)
     assert result.SerializeToString() == ir.SerializeToString()
 
 
 @pytest.mark.xfail(
     raises=(ibis.common.exceptions.IbisTypeError, NotImplementedError),
     reason="Ibis doesn't allow decimal values through validation",
 )
@@ -388,22 +314,15 @@
     ir = stalg.Expression(
         literal=stalg.Expression.Literal(
             decimal=stalg.Expression.Literal.Decimal(
                 value=b"234.234", precision=6, scale=3
             )
         )
     )
-    result = translate(expr, compiler)
+    result = translate(expr, compiler=compiler)
     assert result.SerializeToString() == ir.SerializeToString()
 
 
 @pytest.mark.parametrize("value", [ibis.NA, ibis.literal(None)])
 def test_bare_null(compiler, value):
     with pytest.raises(NotImplementedError, match="untyped null literals"):
-        translate(value, compiler)
-
-
-@literal_cases
-def test_decompile(expr, ir):
-    value, dtype = decompile(ir.literal)
-    result = ibis.literal(value, type=dtype)
-    assert result.equals(expr)
+        translate(value, compiler=compiler)
```

### Comparing `ibis-substrait-2.9.8/ibis_substrait/tests/compiler/test_tpch.py` & `ibis_substrait-3.0.0/ibis_substrait/tests/compiler/test_tpch.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 from datetime import date
 
 import ibis
 import pytest
+from google.protobuf import json_format
 from packaging import version
 from pytest_lazyfixture import lazy_fixture
-from substrait_validator import Config, check_plan
 
-from ibis_substrait.compiler.decompile import decompile
+# changes in ops have led to one of the tpc queries ending up constructed
+# in a different order, so we snapshot query 9 with two versions of Ibis.
+ibis5 = pytest.mark.skipif(
+    version.parse(ibis.__version__) >= version.parse("5.0.0"),
+    reason="Field ordering difference btwn 4.x and 5.x",
+)
+ibis4 = pytest.mark.skipif(
+    version.parse(ibis.__version__) < version.parse("5.0.0"),
+    reason="Field ordering difference btwn 4.x and 5.x",
+)
 
 
 @pytest.fixture
 def tpc_h01(lineitem):
     return (
         lineitem.filter(lambda t: t.l_shipdate <= date(year=1998, month=9, day=2))
         .group_by(["l_returnflag", "l_linestatus"])
@@ -22,15 +31,15 @@
                 t.l_extendedprice * (1 - t.l_discount) * (1 + t.l_tax)
             ).sum(),
             avg_qty=lambda t: t.l_quantity.mean(),
             avg_price=lambda t: t.l_extendedprice.mean(),
             avg_disc=lambda t: t.l_discount.mean(),
             count_order=lambda t: t.count(),
         )
-        .sort_by(["l_returnflag", "l_linestatus"])
+        .order_by(["l_returnflag", "l_linestatus"])
     )
 
 
 @pytest.fixture
 def tpc_h02(
     part, supplier, partsupp, nation, region, REGION="EUROPE", SIZE=25, TYPE="BRASS"
 ):
@@ -70,15 +79,15 @@
             q.p_mfgr,
             q.s_address,
             q.s_phone,
             q.s_comment,
         ]
     )
 
-    return q.sort_by(
+    return q.order_by(
         [
             ibis.desc(q.s_acctbal),
             q.n_name,
             q.s_name,
             q.p_partkey,
         ]
     ).limit(100)
@@ -94,15 +103,15 @@
     q = customer.join(orders, customer.c_custkey == orders.o_custkey)
     q = q.join(lineitem, lineitem.l_orderkey == orders.o_orderkey)
     q = q.filter(
         [q.c_mktsegment == "BUILDING", q.o_orderdate < DATE, q.l_shipdate > DATE]
     )
     qg = q.group_by([q.l_orderkey, q.o_orderdate, q.o_shippriority])
     q = qg.aggregate(revenue=(q.l_extendedprice * (1 - q.l_discount)).sum())
-    q = q.sort_by([ibis.desc(q.revenue), q.o_orderdate])
+    q = q.order_by([ibis.desc(q.revenue), q.o_orderdate])
     q = q.limit(10)
 
     return q
 
 
 @pytest.fixture
 def tpc_h04(orders, lineitem):
@@ -114,15 +123,15 @@
             cond.any(),
             orders.o_orderdate >= "1993-07-01",
             orders.o_orderdate < "1993-10-01",
         ]
     )
     q = q.group_by([orders.o_orderpriority])
     q = q.aggregate(order_count=orders.count())
-    q = q.sort_by([orders.o_orderpriority])
+    q = q.order_by([orders.o_orderpriority])
     return q
 
 
 @pytest.fixture
 def tpc_h05(customer, orders, lineitem, supplier, nation, region):
     q = customer
     q = q.join(orders, customer.c_custkey == orders.o_custkey)
@@ -141,15 +150,15 @@
             q.o_orderdate >= "1994-01-01",
             q.o_orderdate < "1995-01-01",
         ]
     )
     revexpr = q.l_extendedprice * (1 - q.l_discount)
     gq = q.group_by([q.n_name])
     q = gq.aggregate(revenue=revexpr.sum())
-    q = q.sort_by([ibis.desc(q.revenue)])
+    q = q.order_by([ibis.desc(q.revenue)])
     return q
 
 
 @pytest.fixture
 def tpc_h06(lineitem):
     q = lineitem
     discount_min = round(0.06 - 0.01, 2)
@@ -193,15 +202,15 @@
             | ((q.cust_nation == "GERMANY") & (q.supp_nation == "FRANCE")),
             q.l_shipdate.between("1995-01-01", "1996-12-31"),
         ]
     )
 
     gq = q.group_by(["supp_nation", "cust_nation", "l_year"])
     q = gq.aggregate(revenue=q.volume.sum())
-    q = q.sort_by(["supp_nation", "cust_nation", "l_year"])
+    q = q.order_by(["supp_nation", "cust_nation", "l_year"])
 
     return q
 
 
 @pytest.fixture
 def tpc_h08(
     part,
@@ -242,21 +251,20 @@
     )
 
     q = q.mutate(
         nation_volume=ibis.case().when(q.nation == "BRAZIL", q.volume).else_(0).end()
     )
     gq = q.group_by([q.o_year])
     q = gq.aggregate(mkt_share=q.nation_volume.sum() / q.volume.sum())
-    q = q.sort_by([q.o_year])
+    q = q.order_by([q.o_year])
     return q
 
 
 @pytest.fixture
 def tpc_h09(part, supplier, lineitem, partsupp, orders, nation):
-
     q = lineitem
     q = q.join(supplier, supplier.s_suppkey == lineitem.l_suppkey)
     q = q.join(
         partsupp,
         (partsupp.ps_suppkey == lineitem.l_suppkey)
         & (partsupp.ps_partkey == lineitem.l_partkey),
     )
@@ -273,15 +281,15 @@
         q.p_name,
     ]
 
     q = q.filter([q.p_name.like("%GREEN%")])
 
     gq = q.group_by([q.nation, q.o_year])
     q = gq.aggregate(sum_profit=q.amount.sum())
-    q = q.sort_by([q.nation, ibis.desc(q.o_year)])
+    q = q.order_by([q.nation, ibis.desc(q.o_year)])
     return q
 
 
 @pytest.fixture
 def tpc_h10(customer, orders, lineitem, nation):
     q = customer
     q = q.join(orders, customer.c_custkey == orders.o_custkey)
@@ -304,15 +312,15 @@
             q.n_name,
             q.c_address,
             q.c_comment,
         ]
     )
     q = gq.aggregate(revenue=(q.l_extendedprice * (1 - q.l_discount)).sum())
 
-    q = q.sort_by(ibis.desc(q.revenue))
+    q = q.order_by(ibis.desc(q.revenue))
     return q.limit(20)
 
 
 @pytest.fixture
 def tpc_h11(partsupp, supplier, nation):
     q = partsupp
     q = q.join(supplier, partsupp.ps_suppkey == supplier.s_suppkey)
@@ -325,15 +333,15 @@
     innerq = innerq.join(nation, nation.n_nationkey == supplier.s_nationkey)
     innerq = innerq.filter([innerq.n_name == "GERMANY"])
     innerq = innerq.aggregate(total=(innerq.ps_supplycost * innerq.ps_availqty).sum())
 
     gq = q.group_by([q.ps_partkey])
     q = gq.aggregate(value=(q.ps_supplycost * q.ps_availqty).sum())
     q = q.filter([q.value > innerq.total * 0.0001])
-    q = q.sort_by(ibis.desc(q.value))
+    q = q.order_by(ibis.desc(q.value))
     return q
 
 
 @pytest.fixture
 def tpc_h12(orders, lineitem):
     q = orders
     q = q.join(lineitem, orders.o_orderkey == lineitem.l_orderkey)
@@ -361,15 +369,15 @@
             q.o_orderpriority.case()
             .when("1-URGENT", 0)
             .when("2-HIGH", 0)
             .else_(1)
             .end()
         ).sum(),
     )
-    q = q.sort_by(q.l_shipmode)
+    q = q.order_by(q.l_shipmode)
 
     return q
 
 
 @pytest.fixture
 def tpc_h13(customer, orders):
     innerq = customer
@@ -380,15 +388,15 @@
     )
     innergq = innerq.group_by([innerq.c_custkey])
     innerq = innergq.aggregate(c_count=innerq.o_orderkey.count())
 
     gq = innerq.group_by([innerq.c_count])
     q = gq.aggregate(custdist=innerq.count())
 
-    q = q.sort_by([ibis.desc(q.custdist), ibis.desc(q.c_count)])
+    q = q.order_by([ibis.desc(q.custdist), ibis.desc(q.c_count)])
     return q
 
 
 @pytest.fixture
 def tpc_h14(lineitem, part):
     q = lineitem
     q = q.join(part, lineitem.l_partkey == part.p_partkey)
@@ -411,15 +419,15 @@
     gqrev = qrev.group_by([lineitem.l_suppkey])
     qrev = gqrev.aggregate(
         total_revenue=(qrev.l_extendedprice * (1 - qrev.l_discount)).sum()
     )
 
     q = supplier.join(qrev, supplier.s_suppkey == qrev.l_suppkey)
     q = q.filter([q.total_revenue == qrev.total_revenue.max()])
-    q = q.sort_by([q.s_suppkey])
+    q = q.order_by([q.s_suppkey])
     q = q[q.s_suppkey, q.s_name, q.s_address, q.s_phone, q.total_revenue]
     return q
 
 
 @pytest.fixture
 def tpc_h16(partsupp, part, supplier):
     q = partsupp.join(part, part.p_partkey == partsupp.ps_partkey)
@@ -431,17 +439,17 @@
             ~q.ps_suppkey.isin(
                 supplier.filter(
                     [supplier.s_comment.like("%Customer%Complaints%")]
                 ).s_suppkey
             ),
         ]
     )
-    gq = q.groupby([q.p_brand, q.p_type, q.p_size])
+    gq = q.group_by([q.p_brand, q.p_type, q.p_size])
     q = gq.aggregate(supplier_cnt=q.ps_suppkey.nunique())
-    q = q.sort_by([ibis.desc(q.supplier_cnt), q.p_brand, q.p_type, q.p_size])
+    q = q.order_by([ibis.desc(q.supplier_cnt), q.p_brand, q.p_type, q.p_size])
     return q
 
 
 @pytest.fixture
 def tpc_h17(lineitem, part):
     q = lineitem.join(part, part.p_partkey == lineitem.l_partkey)
 
@@ -457,26 +465,28 @@
     )
     q = q.aggregate(avg_yearly=q.l_extendedprice.sum() / 7.0)
     return q
 
 
 @pytest.fixture
 def tpc_h18(customer, orders, lineitem):
-    subgq = lineitem.groupby([lineitem.l_orderkey])
+    subgq = lineitem.group_by([lineitem.l_orderkey])
     subq = subgq.aggregate(qty_sum=lineitem.l_quantity.sum())
     subq = subq.filter([subq.qty_sum > 300])
 
     q = customer
     q = q.join(orders, customer.c_custkey == orders.o_custkey)
     q = q.join(lineitem, orders.o_orderkey == lineitem.l_orderkey)
     q = q.filter([q.o_orderkey.isin(subq.l_orderkey)])
 
-    gq = q.groupby([q.c_name, q.c_custkey, q.o_orderkey, q.o_orderdate, q.o_totalprice])
+    gq = q.group_by(
+        [q.c_name, q.c_custkey, q.o_orderkey, q.o_orderdate, q.o_totalprice]
+    )
     q = gq.aggregate(sum_qty=q.l_quantity.sum())
-    q = q.sort_by([ibis.desc(q.o_totalprice), q.o_orderdate])
+    q = q.order_by([ibis.desc(q.o_totalprice), q.o_orderdate])
     return q.limit(100)
 
 
 @pytest.fixture
 def tpc_h19(lineitem, part):
     q = lineitem.join(part, part.p_partkey == lineitem.l_partkey)
 
@@ -538,15 +548,15 @@
         ]
     )
 
     q1 = q1.filter([q1.n_name == "CANADA", q1.s_suppkey.isin(q2.ps_suppkey)])
 
     q1 = q1[q1.s_name, q1.s_address]
 
-    return q1.sort_by(q1.s_name)
+    return q1.order_by(q1.s_name)
 
 
 @pytest.fixture
 def tpc_h21(supplier, lineitem, orders, nation):
     L2 = lineitem.view()
     L3 = lineitem.view()
 
@@ -577,15 +587,15 @@
                 ).any()
             ),
         ]
     )
 
     gq = q.group_by([q.s_name])
     q = gq.aggregate(numwait=q.count())
-    q = q.sort_by([ibis.desc(q.numwait), q.s_name])
+    q = q.order_by([ibis.desc(q.numwait), q.s_name])
     return q.limit(100)
 
 
 @pytest.fixture
 def tpc_h22(customer, orders):
     q = customer.filter(
         [
@@ -609,164 +619,80 @@
     custsale = custsale[
         customer.c_phone.substr(0, 2).name("cntrycode"), customer.c_acctbal
     ]
 
     gq = custsale.group_by(custsale.cntrycode)
     outerq = gq.aggregate(numcust=custsale.count(), totacctbal=custsale.c_acctbal.sum())
 
-    return outerq.sort_by(outerq.cntrycode)
-
-
-@pytest.mark.xfail(
-    version.parse("2.1.1") < version.parse(ibis.__version__) <= version.parse("3.0.2"),
-    reason="issue with unbounded decimal precision fixed on ibis-master",
-)
-def test_tpch1(tpc_h01, lineitem, compiler):
-    plan = compiler.compile(tpc_h01)
-    assert plan.SerializeToString()
-
-    (result,) = decompile(plan)
-    expected = (
-        lineitem.filter(lambda t: t.l_shipdate <= date(year=1998, month=9, day=2))
-        .group_by(["l_returnflag", "l_linestatus"])
-        .aggregate(
-            sum_qty=lambda t: t.l_quantity.sum(),
-            sum_base_price=lambda t: t.l_extendedprice.sum(),
-            sum_disc_price=lambda t: (t.l_extendedprice * (1 - t.l_discount)).sum(),
-            sum_charge=lambda t: (
-                t.l_extendedprice * (1 - t.l_discount) * (1 + t.l_tax)
-            ).sum(),
-            avg_qty=lambda t: t.l_quantity.mean(),
-            avg_price=lambda t: t.l_extendedprice.mean(),
-            avg_disc=lambda t: t.l_discount.mean(),
-            count_order=lambda t: t.count(),
-        )
-        .sort_by(["l_returnflag", "l_linestatus"])
-    )
-    assert result.equals(expected)
+    return outerq.order_by(outerq.cntrycode)
 
 
 TPC_H = [
     lazy_fixture("tpc_h01"),
     pytest.param(
         lazy_fixture("tpc_h02"),
         marks=pytest.mark.xfail(
-            raises=KeyError, reason="TableArrayView not implemented"
+            raises=AssertionError, reason="Correlated Subquery issues"
         ),
     ),
     lazy_fixture("tpc_h03"),
-    pytest.param(
-        lazy_fixture("tpc_h04"),
-        marks=pytest.mark.xfail(
-            raises=KeyError, reason="ExistsSubquery not implemented"
-        ),
-    ),
+    lazy_fixture("tpc_h04"),
     lazy_fixture("tpc_h05"),
     lazy_fixture("tpc_h06"),
-    pytest.param(
-        lazy_fixture("tpc_h07"),
-        marks=pytest.mark.xfail(
-            raises=NotImplementedError, reason="Self reference (view)"
-        ),
-    ),
+    lazy_fixture("tpc_h07"),
     pytest.param(
         lazy_fixture("tpc_h08"),
         marks=pytest.mark.xfail(
-            raises=NotImplementedError, reason="Self reference (view)"
+            raises=TypeError,
+            reason="Aggregates need to be handled differently than they are",
         ),
     ),
-    lazy_fixture("tpc_h09"),
+    pytest.param(lazy_fixture("tpc_h09"), marks=ibis5),
+    pytest.param(lazy_fixture("tpc_h09"), marks=ibis4),
     lazy_fixture("tpc_h10"),
     lazy_fixture("tpc_h11"),
     lazy_fixture("tpc_h12"),
     lazy_fixture("tpc_h13"),
     pytest.param(
         lazy_fixture("tpc_h14"),
         marks=pytest.mark.xfail(
             raises=TypeError,
-            reason="protobuf error resulting subquery (cannot merge Expression and AggregateFunction)",  # noqa
+            reason="protobuf error resulting subquery (cannot merge Expression and AggregateFunction)",
         ),
     ),
     pytest.param(
         lazy_fixture("tpc_h15"),
         marks=pytest.mark.xfail(
-            raises=KeyError, reason="TableArrayView not implemented"
+            raises=AssertionError, reason="Correlated Subquery issues"
         ),
     ),
     pytest.param(
         lazy_fixture("tpc_h16"),
         marks=pytest.mark.xfail(
-            raises=TypeError, reason="IntegerColumn is not iterable"
+            raises=ValueError, reason="countdistinct not handled correctly"
         ),
     ),
     pytest.param(
         lazy_fixture("tpc_h17"),
         marks=pytest.mark.xfail(
             raises=NotImplementedError,
             reason="ibis.expr.operations.relations.Aggregation",
         ),
     ),
-    pytest.param(
-        lazy_fixture("tpc_h18"),
-        marks=pytest.mark.xfail(
-            raises=TypeError, reason="IntegerColumn is not iterable"
-        ),
-    ),
+    lazy_fixture("tpc_h18"),
     lazy_fixture("tpc_h19"),
-    pytest.param(
-        lazy_fixture("tpc_h20"),
-        marks=pytest.mark.xfail(
-            raises=TypeError, reason="IntegerColumn is not iterable"
-        ),
-    ),
-    pytest.param(
-        lazy_fixture("tpc_h21"),
-        marks=pytest.mark.xfail(
-            raises=KeyError, reason="ExistsSubquery not implemented"
-        ),
-    ),
-    pytest.param(
-        lazy_fixture("tpc_h22"),
-        marks=pytest.mark.xfail(
-            raises=KeyError, reason="NotExistsSubquery not implemented"
-        ),
-    ),
+    lazy_fixture("tpc_h20"),
+    lazy_fixture("tpc_h21"),
+    lazy_fixture("tpc_h22"),
 ]
 
 
-@pytest.mark.skipif(
-    version.parse(ibis.__version__) <= version.parse("3.0.0"),
-    reason="TPC queries aren't formatted in an ibis 2.x compatible way",
-)
-@pytest.mark.parametrize(
-    "query",
-    TPC_H,
-)
-def test_compile(query, compiler):
-    _ = compiler.compile(query)
-
-
-@pytest.mark.skipif(
-    version.parse(ibis.__version__) <= version.parse("3.0.0"),
-    reason="TPC queries aren't formatted in an ibis 2.x compatible way",
-)
 @pytest.mark.parametrize(
     "query",
     TPC_H,
 )
-def test_compile_validate(query, compiler):
+def test_compile(query, compiler, snapshot, request):
     plan = compiler.compile(query)
 
-    c = Config()
-    # too few field names
-    c.override_diagnostic_level(4003, "error", "info")
-    # function def unavailable, cannot check validity of call
-    c.override_diagnostic_level(6003, "warning", "info")
-    # failed to resolve YAML: unknown url type
-    c.override_diagnostic_level(2002, "warning", "info")  # too few field names
-    # typecast validation rules are net yet implemented
-    c.override_diagnostic_level(1, "warning", "info")  # too few field names
-
-    # check_plan takes substrait Plans as arguments but because of namespacing,
-    # our plan is no longer strictly a substrait.plan_pb2.Plan.
-    # Workaround for now is to send in the bytes which it handles without issue.
-    assert check_plan(plan.SerializeToString(), config=c)
+    snapshot.assert_match(
+        json_format.MessageToJson(plan), f"{request.node.callspec.id}.json"
+    )
```

