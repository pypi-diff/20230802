# Comparing `tmp/impunity-1.0.2.tar.gz` & `tmp/impunity-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impunity-1.0.2.tar", max compression
+gzip compressed data, was "impunity-1.0.3.tar", max compression
```

## Comparing `impunity-1.0.2.tar` & `impunity-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1086 2023-03-03 23:02:21.617620 impunity-1.0.2/license.txt
--rw-r--r--   0        0        0     1363 2023-07-24 12:50:28.083889 impunity-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       54 2022-12-14 22:12:52.000000 impunity-1.0.2/src/impunity/__init__.py
--rw-r--r--   0        0        0      520 2023-05-03 12:48:13.573198 impunity-1.0.2/src/impunity/exception.py
--rw-r--r--   0        0        0        0 2023-02-08 08:48:46.044417 impunity-1.0.2/src/impunity/py.typed
--rw-r--r--   0        0        0      859 2023-06-20 12:24:15.987401 impunity-1.0.2/src/impunity/quantityNode.py
--rw-r--r--   0        0        0    38823 2023-07-24 12:47:46.611310 impunity-1.0.2/src/impunity/visitor.py
--rw-r--r--   0        0        0     9530 2023-07-20 13:23:10.648860 impunity-1.0.2/src/impunity/wrapper.py
--rw-r--r--   0        0        0      662 1970-01-01 00:00:00.000000 impunity-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     3675 2023-08-02 19:56:25.905117 impunity-1.0.3/README.md
+-rw-r--r--   0        0        0     1086 2023-08-02 19:56:25.909117 impunity-1.0.3/license.txt
+-rw-r--r--   0        0        0     1687 2023-08-02 19:56:25.909117 impunity-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       54 2023-08-02 19:56:25.909117 impunity-1.0.3/src/impunity/__init__.py
+-rw-r--r--   0        0        0      520 2023-08-02 19:56:25.909117 impunity-1.0.3/src/impunity/exception.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:56:25.909117 impunity-1.0.3/src/impunity/py.typed
+-rw-r--r--   0        0        0      573 2023-08-02 19:56:25.909117 impunity-1.0.3/src/impunity/quantityNode.py
+-rw-r--r--   0        0        0    40339 2023-08-02 19:56:25.913117 impunity-1.0.3/src/impunity/visitor.py
+-rw-r--r--   0        0        0     9573 2023-08-02 19:56:25.913117 impunity-1.0.3/src/impunity/wrapper.py
+-rw-r--r--   0        0        0     4372 1970-01-01 00:00:00.000000 impunity-1.0.3/PKG-INFO
```

### Comparing `impunity-1.0.2/license.txt` & `impunity-1.0.3/license.txt`

 * *Files identical despite different names*

### Comparing `impunity-1.0.2/src/impunity/exception.py` & `impunity-1.0.3/src/impunity/exception.py`

 * *Files identical despite different names*

### Comparing `impunity-1.0.2/src/impunity/quantityNode.py` & `impunity-1.0.3/src/impunity/quantityNode.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,23 @@
-import ast
-import sys
-from typing import Optional, TypeVar, overload
+from __future__ import annotations
 
-if sys.version_info >= (3, 9):
-    from _collections_abc import Sequence
-else:
-    from typing import Sequence
+import ast
+from typing import Optional, TypeVar
 
 Unit = Optional[str]
-N = TypeVar("N", bound=Optional[ast.expr], covariant=True)
+N = TypeVar("N", bound=ast.expr, covariant=True)
 
 
 class QuantityNode:
 
     """Node object with a unit attribute.
 
     Attributes:
         node : TypeVar("N", bound=Optional[ast.expr], covariant=True)
             Any type of expression found within an ast.
         unit : Optional[str]
             Optional string representing a UoM.
     """
 
-    @overload
-    def __init__(self, node: N, unit: Optional[Unit] = None) -> None:
-        ...
-
-    @overload
-    def __init__(self, node: N, unit: Optional[Sequence[Unit]] = None) -> None:
-        ...
-
-    def __init__(self, node, unit=None) -> None:
+    def __init__(self, node: None | N, unit: None | Unit = None) -> None:
         self.node = node
         self.unit = unit
```

### Comparing `impunity-1.0.2/src/impunity/visitor.py` & `impunity-1.0.3/src/impunity/visitor.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,146 +3,172 @@
 import ast
 import inspect
 import logging
 import sys
 import types
 import typing
 from math import isclose
-from typing import Any, Dict, Optional, Union, cast
-
-if sys.version_info >= (3, 9):
-    from _collections_abc import Callable, Sequence
-else:
-    from collections import Callable
-    from typing import Sequence
+from typing import (
+    Any,
+    Callable,
+    ClassVar,
+    Dict,
+    Optional,
+    Union,
+    cast,
+    overload,
+)
 
 import pint
 from pint import UnitRegistry
-
-if sys.version_info >= (3, 10):
-    # TBH Annotated from 3.9, TypeGuard from 3.10
-    from typing import Annotated, TypeGuard
-else:
-    from typing_extensions import Annotated, TypeGuard
+from typing_extensions import Annotated, Protocol, TypedDict, TypeGuard
 
 from .quantityNode import QuantityNode, Unit
 
-annotation_node = Union[ast.Subscript, ast.Name, ast.Constant]
-
+# annotation_node = Union[ast.Subscript, ast.Name, ast.Constant]
 
-# class annot_type(Annotated[int, "spam"]):
-#     """Class to access __metadata__ from Annotated variables"""
 
-#     def __init__(self, *args, **kw):
-#         super(annot_type, self).__init__(*args, **kw)
-#         self.__metadata__ = getattr(super(), "__metadata__")
+class HasMetadata(Protocol):
+    __metadata__: tuple[str, ...]
 
-annot_type = type(Annotated[int, "spam"])
 
+def is_annotated(hint: Any) -> TypeGuard[HasMetadata]:
+    """Determines whether the annotation is of type Annotated"""
+    return isinstance(hint, type(Annotated[int, "spam"]))
 
-logging.basicConfig(
-    level=logging.WARNING,
-    format="%(asctime)s [%(levelname)s] %(message)s",
-    handlers=[
-        # Creates a file "todays_date.py" with warnings
-        logging.StreamHandler(sys.stdout),
-    ],
-)
 
 _log = logging.getLogger(__name__)
 
 
-class VarDict(dict):
-    def __missing__(self, key):
-        _log.warning(
-            f"The variable {key} is not annotated. "
-            + "Defaulted to dimensionless"
-        )
+class VarDict(Dict[str, Any]):
+    def __missing__(self, key: str) -> None:
+        msg = f"Variable {key} is not annotated. Fallback to dimensionless"
+        _log.info(msg)
         return None
 
 
-def get_annotation_unit(
-    node: annotation_node | ast.expr,
-) -> Optional[str]:
-    """
-    Return a UoM from an AST Node. Return None if the node is not compatible.
-
-    :param node: Node with an annotation
-    :type node: ast.expr with annotation
-    :return: Optional str of the UoM
-    :rtype: Optional[str]
-    """
+class PrefixSuffix(TypedDict):
+    prefix: str
+    suffix: str
+
+
+def split_attribute(node: ast.Attribute) -> PrefixSuffix:
+    """Transform the AST of a.b.c in {'prefix': 'a.b', 'suffix': 'c'}."""
+
+    assert isinstance(node, ast.Attribute)
+    suffix = node.attr
+    attr = node.value
+    prefix = ""
+    while isinstance(attr, ast.Attribute):
+        prefix = "." + attr.attr + prefix
+        attr = attr.value
+    if isinstance(attr, ast.Name):
+        prefix = attr.id + prefix
 
-    unit = None
-    if isinstance(node, ast.Constant):
-        unit = node.value
-    elif isinstance(node, ast.Subscript):
-        if isinstance(node.slice, ast.Index):
-            if isinstance(node.slice.value, ast.Tuple):  # type: ignore
-                unit_node = node.slice.value.elts[1]  # type: ignore
-        elif isinstance(node.slice, ast.Tuple):
-            unit_node = node.slice.elts[1]
-        if isinstance(unit_node, ast.Constant):
-            unit = unit_node.value
-
-    return unit
-
-
-def is_annotated(
-    hint: Any, annot_type=annot_type
-) -> TypeGuard[annot_type]:  # type: ignore
-    """Determines whether the annotation is of type Annotated"""
-    return (type(hint) is annot_type) and hasattr(hint, "__metadata__")
+    return dict(prefix=prefix, suffix=suffix)
 
 
 class Visitor(ast.NodeTransformer):
 
     """Impunity AST visitor class checking for Annotations
     to transform the code if necessary
 
     Attributes:
-        impunity_func : dict[str, Callable]
+        impunity_func : dict[tuple[str, str], Callable]
             Dictionnary of Callables to keep track of functions
             tracked by impunity
         ureg : pint.UnitRegistry
             Unit Registry from Pint to manage UoMs.
     """
 
-    impunity_func: dict[str, Callable] = {}
+    # tuple[module_name, function_name]
+    impunity_func: ClassVar[dict[tuple[str, str], Callable[..., Any]]] = {}
+    impunity_funcdef: ClassVar[dict[str, ast.FunctionDef]] = {}
     ureg = UnitRegistry()
+    current_module: str = ""
 
-    def __init__(self, fun) -> None:
+    def __init__(self, fun: Callable[..., Any]) -> None:
         """
         Constructs all the necessary attributes for the visitor using the
         attributes of the fun Callable.
 
         Parameters
         ----------
             fun : Callable[..., Any]
                 Callable checked by impunity
         """
 
         self.nested_flag = False
         x: Dict[str, str] = {}
         self.vars = VarDict(x)
+        Visitor.current_module = fun.__module__
 
         # For class decorators
         if isinstance(fun, type):
             method_list = [
                 getattr(fun, func)
                 for func in dir(fun)
                 if callable(getattr(fun, func)) and not func.startswith("__")
             ]
-            self.add_func(fun.__init__)  # type: ignore
+            if (
+                init := fun.__init__  # type: ignore
+            ).__class__.__name__ != "wrapper_descriptor":
+                # meaning: does the class have a __init__
+                # (otherwise, it's an empty slot)
+                self.add_func(init)
             for function in method_list:
                 self.add_func(function)
             self.class_attr: Dict[str, Unit] = {}
         else:
             self.add_func(fun)
 
+    def fun_header(self, node: ast.AST) -> str:
+        lineno = getattr(node, "lineno", 0)
+        # coloffset = getattr(node, "coloffset", 0)
+        firstlineno = getattr(self.fun.__code__, "co_firstlineno", 0)
+        filename = getattr(self.fun.__code__, "co_filename")
+        return f"{filename}::{self.fun.__name__}:{firstlineno + lineno - 1} "
+
+    def get_annotation_unit(self, node: ast.expr) -> Optional[str]:
+        """
+        Return a UoM from an AST Node.
+        Return None if the node is not compatible.
+
+        :param node: Node with an annotation
+        :type node: ast.expr with annotation
+        :return: Optional str of the UoM
+        :rtype: Optional[str]
+        """
+
+        unit = None
+
+        if isinstance(node, ast.Constant):
+            unit = node.value
+
+        elif isinstance(node, ast.Attribute):
+            res = split_attribute(node)
+            module = self.fun_globals.get(res["prefix"], None)
+            if module is not None:
+                handle = getattr(module, res["suffix"], None)
+                if is_annotated(handle):
+                    unit = handle.__metadata__[0]
+                if isinstance(handle, str):
+                    unit = handle
+
+        elif isinstance(node, ast.Subscript):
+            if isinstance(node.slice, ast.Index):
+                if isinstance(node.slice.value, ast.Tuple):
+                    unit_node = node.slice.value.elts[1]
+            elif isinstance(node.slice, ast.Tuple):
+                unit_node = node.slice.elts[1]
+            if isinstance(unit_node, ast.Constant):
+                unit = unit_node.value
+
+        return unit
+
     def visit(self, root: ast.AST) -> ast.AST:
         """
         Initiate the visit of the root AST. Returns a checked ast.AST
         eventually modified to keep UoM coherence.
 
         Args:
             root : ast.AST
@@ -155,22 +181,60 @@
                 child.parent = node  # type: ignore
         method = "visit_" + root.__class__.__name__
         visitor = getattr(self, method, self.generic_visit)
         new_node = visitor(root)
         return new_node
 
     @classmethod
-    def add_func(cls, fun):
+    def add_func(cls, fun: Callable[..., Any] | ast.FunctionDef) -> None:
         """Add function to the impunity function dictionnary"""
         if isinstance(fun, ast.FunctionDef):
-            cls.impunity_func[fun.name] = fun
+            cls.impunity_funcdef[fun.name] = fun
         else:
-            cls.impunity_func[fun.__name__] = fun
+            cls.impunity_func[fun.__module__, fun.__name__] = fun
+
+    @overload
+    def get_func(self, name: str, module: None) -> None | ast.FunctionDef:
+        ...
+
+    @overload
+    def get_func(self, name: str, module: str) -> None | Callable[..., Any]:
+        ...
+
+    def get_func(
+        self, name: str, module: None | str = None
+    ) -> None | ast.FunctionDef | Callable[..., Any]:
+        result: None | ast.FunctionDef | Callable[..., Any] = None
+
+        if module is None:
+            # Check if nested function
+            result = self.impunity_funcdef.get(name, None)
+            if result is None:
+                # If not nested, check if in globals
+                fun = self.fun_globals.get(name, None)
+                if fun is not None:
+                    # if in globals, check if impunified
+                    result = self.impunity_func.get(
+                        (fun.__module__, name), None
+                    )
+            return result
 
-    def node_convert(self, expected_unit, received_unit, received_node):
+        result = self.impunity_func.get((module, name), None)
+        if result is None:
+            m = self.fun_globals.get(module, None)
+            if m is not None:
+                result = self.impunity_func.get((m.__name__, name), None)
+        return result
+
+    def node_convert(
+        self,
+        expected_unit: Optional[str],
+        received_unit: Optional[str],
+        received_node: ast.expr,
+    ) -> ast.expr:
         """check if the expected and the received units are coherents with
         each other by using the Pint library. Modify the received node
         accordingly and returns it.
 
         Parameters:
             - expected_unit : str
                 expected Unit of Measure string
@@ -189,47 +253,41 @@
             and "dimensionless"
             not in (
                 received_unit,
                 expected_unit,
             )
             and received_unit is not None
         ):
-            if pint.Unit(received_unit).is_compatible_with(
-                pint.Unit(expected_unit)
-            ):
+            received_pint_unit = pint.Unit(received_unit)  # type: ignore
+            expected_pint_unit = pint.Unit(expected_unit)  # type: ignore
+            if received_pint_unit.is_compatible_with(expected_pint_unit):
                 Q_ = self.ureg.Quantity
-                r0 = Q_(0, received_unit)
-                r1 = Q_(1, received_unit)
-                r10 = Q_(10, received_unit)
+                r0 = Q_(0, received_unit)  # type: ignore
+                r1 = Q_(1, received_unit)  # type: ignore
+                r10 = Q_(10, received_unit)  # type: ignore
 
                 e0 = r0.to(expected_unit)
                 e1 = r1.to(expected_unit)
                 e10 = r10.to(expected_unit)
 
                 if r0.m == e0.m:
-                    conv_value = (
-                        pint.Unit(expected_unit)
-                        .from_(pint.Unit(received_unit))
-                        .m
-                    )
+                    conv_value = expected_pint_unit.from_(received_pint_unit).m
 
                     if conv_value == 1:
                         new_node = received_node
                     else:
                         new_node = ast.BinOp(
                             received_node,
                             ast.Mult(),
                             ast.Constant(conv_value),
                         )
 
                 elif (e1.m - e0.m) == 1:
                     conv_value = (
-                        pint.Unit(expected_unit)
-                        .from_(pint.Unit(received_unit))
-                        .m
+                        expected_pint_unit.from_(received_pint_unit).m
                     ) - 1
 
                     # if conv_value == 0:
                     #     new_node = received_node
                     # else:
                     new_node = ast.BinOp(
                         received_node,
@@ -248,100 +306,91 @@
                         ast.Constant(e0.m),
                     )
                 else:
                     new_node = received_node  # log
 
             else:
                 _log.warning(
-                    f"In function {self.fun.__module__}/"
-                    + f"{self.fun.__name__}: "
+                    self.fun_header(received_node)
                     + f"Expected unit {expected_unit} "
                     + f"but received incompatible unit {received_unit}."
                 )
                 new_node = received_node
         else:
             new_node = received_node
         return new_node
 
-    @classmethod
-    def func_flush(cls):
-        return
-
-    @classmethod
-    def get_annotations(cls, name) -> Optional[Dict[str, Any]]:
+    def get_annotations(
+        self, name: str, module: None | str = None
+    ) -> Optional[Dict[str, Any]]:
         """Get annotations of a function found in the impunity_func class dict.
         Returns None if the function is not annotated.
 
         Parameters:
             - name : str
                 name of the function for which annotations are required
 
         Returns:
             - Optional dict of annotations
         """
 
-        if (fun := cls.impunity_func.get(name)) is not None:
-            annotations = getattr(fun, "__annotations__", None)
-            if annotations:
-                globals = list(cls.impunity_func.values())[-1].__globals__
-                locals = fun.__globals__
+        if (fun := self.get_func(name, module)) is not None:
+            if annotations := getattr(fun, "__annotations__", None):
+                globals = list(self.impunity_func.values())[-1].__globals__
+                locals = fun.__globals__  # type: ignore
                 annotations = {
                     k: v
                     if not isinstance(v, str)
                     else eval(v, globals, locals)
                     for k, v in annotations.items()
                 }
-                return cast(Dict, annotations)
+                return cast(Dict[str, Any], annotations)
         elif callable(name):
-            annotations = getattr(name, "__annotations__", None)
-            if annotations:
-                globals = list(cls.impunity_func.values())[-1].__globals__
-                locals = fun.__globals__  # type: ignore
+            if annotations := getattr(name, "__annotations__", None):
+                globals = list(self.impunity_func.values())[-1].__globals__
+                locals = name.__globals__  # type: ignore
                 annotations = {
                     k: v
                     if not isinstance(v, str)
                     else eval(v, globals, locals)
                     for k, v in annotations.items()
                 }
-                return cast(Dict, annotations)
+                return cast(Dict[str, Any], annotations)
 
         return None
 
-    @classmethod
-    def get_func(cls, name):
-        """getter function for the class dict"""
-        return cls.impunity_func.get(name)
-
     def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
         """Method called by the visitor if the visited node is
         function defintion. Is usually the root node in impunity
 
         Args:
             node (ast.FunctionDef): Visited Function Definition
 
         """
-        if not self.nested_flag:
-            self.func_flush()
+        # if not self.nested_flag:  # TODO
+        #     self.func_flush()
         # check for impunity decorator:
         if node.decorator_list:
             for decorator in node.decorator_list:
                 if isinstance(decorator, ast.Call) and isinstance(
                     decorator.func, ast.Name
                 ):
                     if decorator.func.id == "impunity":
                         for kw in decorator.keywords:
                             if hasattr(kw, "value"):
                                 if (
                                     kw.arg == "ignore"
                                     and kw.value.value  # type: ignore
                                 ):
-                                    self.impunity_func.pop(node.name, False)
+                                    self.impunity_func.pop(
+                                        (self.current_module, node.name), False
+                                    )
                                     return node
 
-        if (fun := self.get_func(node.name)) is not None:
+        if (fun := self.get_func(node.name, self.current_module)) is not None:
             self.nested_flag = True
             self.fun = fun
             self.fun_globals = fun.__globals__
             if getattr(self, "class_attr", False):
                 self.vars.update(self.class_attr)
         elif self.nested_flag:
             self.add_func(node)
@@ -351,44 +400,44 @@
         # Adding all annotations from own module
         annotations = getattr(
             sys.modules[self.fun.__module__], "__annotations__", None
         )
         if annotations is not None:
             for name, anno in annotations.items():
                 if is_annotated(anno):
-                    self.vars[name] = anno.__metadata__[0]  # type: ignore
+                    self.vars[name] = anno.__metadata__[0]
                 if isinstance(anno, str):
                     self.vars[name] = anno
 
         # Adding all annotations from imported modules
         for _, val in self.fun_globals.items():
             if isinstance(val, types.ModuleType):
-                annotations = getattr(val, "__annotations__", None)
-                if annotations is not None:
-                    for name, anno in annotations.items():
-                        if is_annotated(anno):
-                            x = anno.__metadata__[0]  # type: ignore
-                            self.vars[name] = x
-                        if isinstance(anno, str):
-                            self.vars[name] = anno
+                annotations = getattr(val, "__annotations__", {})
+                for name, anno in annotations.items():
+                    if is_annotated(anno):
+                        x = anno.__metadata__[0]
+                        self.vars[name] = x
+                    if isinstance(anno, str):
+                        self.vars[name] = anno
 
         # from function signature
         for arg in node.args.args:
             if arg.annotation is not None:
-                anno_unit = get_annotation_unit(arg.annotation)
+                anno_unit = self.get_annotation_unit(arg.annotation)
                 if anno_unit is not None and anno_unit in self.ureg:
                     self.vars[arg.arg] = anno_unit
                 else:
                     self.vars[arg.arg] = None
-                    _log.warning(
-                        f"In function {self.fun.__module__}/"
-                        + f"{self.fun.__name__}: "
-                        + "Signature of annotated functions must be "
-                        + "of type string or typing.Annotated"
-                    )
+                    # Removing this warning: not all parameters have to be
+                    # physical quantities
+                    # _log.warning(
+                    #     self.fun_header(node)
+                    #     + "Signature of annotated functions must be "
+                    #     + "of type string or typing.Annotated"
+                    # )
 
         # Check units in the return node
         node = cast(ast.FunctionDef, self.generic_visit(node))
         return node
 
     def get_node_unit(self, node: Optional[ast.expr]) -> QuantityNode:
         """Method to induce the unit of a node through recursive
@@ -410,42 +459,43 @@
         if isinstance(node, ast.Subscript):
             return QuantityNode(node, self.get_node_unit(node.value).unit)
         elif isinstance(node, ast.Tuple):
             elems = list(map(self.get_node_unit, node.elts))
             if len(elems) == 1:
                 return QuantityNode(elems[0].node, elems[0].unit)
             else:
+                # TODO Sequence[Unit] should we clean?
                 return QuantityNode(
                     ast.Tuple([elem.node for elem in elems], ctx=node.ctx),
-                    cast(Sequence[Unit], [elem.unit for elem in elems]),
+                    [elem.unit for elem in elems],  # type: ignore
                 )
         elif isinstance(node, ast.List):
             _log.warning(
-                f"In function {self.fun.__module__}"
-                + f"/{self.fun.__name__}"
-                + ": List not supported by impunity. "
-                + "Please use numpy arrays."
+                self.fun_header(node)
+                + "lists are not supported by impunity (but numpy arrays are)"
             )
             return QuantityNode(node, "dimensionless")
 
         elif isinstance(node, ast.Set):
+            # TODO Sequence[Unit] should we clean?
             elems = list(map(self.get_node_unit, node.elts))
             return QuantityNode(
                 ast.Set([elem.node for elem in elems]),
-                cast(Sequence[Unit], [elem.unit for elem in elems]),
+                [elem.unit for elem in elems],  # type: ignore
             )
 
         elif isinstance(node, ast.Dict):
             if not node.keys:
                 return QuantityNode(node, None)
             else:
+                # TODO Sequence[Unit] should we clean?
                 elems = list(map(self.get_node_unit, node.values))
                 return QuantityNode(
                     ast.Dict(zip(node.keys, [elem.node for elem in elems])),
-                    cast(Sequence[Unit], [elem.unit for elem in elems]),
+                    [elem.unit for elem in elems],  # type: ignore
                 )
         elif isinstance(node, ast.Name):
             return QuantityNode(node, self.vars[node.id])
 
         elif isinstance(node, ast.BinOp) and isinstance(
             node.op, (ast.Add, ast.Sub)
         ):
@@ -476,17 +526,17 @@
                 )
                 return QuantityNode(
                     ast.copy_location(new_node, node), left.unit
                 )
 
             else:
                 _log.warning(
-                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                    self.fun_header(node)
                     + f"Type {left.unit} and {right.unit} "
-                    + "are not compatible. Defaulted to dimensionless"
+                    + "are not compatible. Fallback to dimensionless"
                 )
                 return QuantityNode(node, "dimensionless")
 
         elif isinstance(node, ast.BinOp) and isinstance(
             node.op, (ast.Mult, ast.Div)
         ):
             left = self.get_node_unit(node.left)
@@ -496,18 +546,18 @@
                 new_node = ast.BinOp(left.node, node.op, right.node)
                 return QuantityNode(
                     ast.copy_location(new_node, node),
                     left.unit if left.unit is not None else right.unit,
                 )
 
             if is_annotated(left.unit):
-                left.unit = left.unit.__metadata__[0]  # type: ignore
+                left.unit = left.unit.__metadata__[0]
 
             if is_annotated(right.unit):
-                right.unit = right.unit.__metadata__[0]  # type: ignore
+                right.unit = right.unit.__metadata__[0]
 
             if pint.Unit(left.unit).is_compatible_with(  # type: ignore
                 pint.Unit(right.unit)  # type: ignore
             ):
                 conv_value = (
                     pint.Unit(left.unit)  # type: ignore
                     .from_(pint.Unit(right.unit))  # type: ignore
@@ -544,26 +594,26 @@
                 new_node = ast.BinOp(left.node, node.op, right.node)
                 return QuantityNode(
                     ast.copy_location(new_node, node),
                     left.unit if left.unit is not None else None,
                 )
 
             if is_annotated(left.unit):
-                left.unit = left.unit.__metadata__[0]  # type: ignore
+                left.unit = left.unit.__metadata__[0]
 
             if is_annotated(right.unit):
-                right.unit = right.unit.__metadata__[0]  # type: ignore
+                right.unit = right.unit.__metadata__[0]
 
             if left.unit == "dimensionless":
                 new_node = ast.BinOp(left.node, node.op, right.node)
                 return QuantityNode(new_node, "dimensionless")
 
             if right.unit is not None:
                 _log.warning(
-                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                    self.fun_header(node)
                     + "The exponent cannot be evaluated statically or is "
                     + "not dimensionless."
                 )
 
                 return QuantityNode(node, None)
 
             elif isinstance(right.node, ast.Constant):
@@ -595,68 +645,68 @@
                     elif isinstance(right.node.op, ast.Sub):
                         unit = (
                             f"({left.unit})^({pow_left.value}"
                             + f"-{pow_right.value})"
                         )
                     else:
                         _log.warning(
-                            f"In function {self.fun.__module__}"
-                            + f"/{self.fun.__name__}: "
-                            + "The exponent cannot be "
-                            + "evaluated statically or is "
-                            + "not dimensionless."
+                            self.fun_header(node)
+                            + "The exponent cannot be statically evaluated or "
+                            + "is not dimensionless."
                         )
                         new_node = ast.BinOp(left.node, node.op, right.node)
                         return QuantityNode(new_node, None)
                 new_node = ast.BinOp(left.node, node.op, right.node)
                 return QuantityNode(new_node, unit)
 
             else:
                 _log.warning(
-                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                    + "The exponent cannot be evaluated statically or is "
-                    + "not dimensionless."
+                    self.fun_header(node)
+                    + "The exponent cannot be statically evaluated or "
+                    + "is not dimensionless."
                 )
                 new_node = ast.BinOp(left.node, node.op, right.node)
                 return QuantityNode(new_node, None)
 
         elif isinstance(node, ast.BinOp):
             _log.warning(
-                f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                + "Binary Operation not supported yet."
+                self.fun_header(node) + "Binary Operation not supported yet."
             )
             return QuantityNode(node, None)
 
         elif isinstance(node, ast.IfExp):
             body = self.get_node_unit(node.body)
             orelse = self.get_node_unit(node.orelse)
 
             new_node = ast.IfExp(
                 test=node.test, body=body.node, orelse=orelse.node
             )
 
             if body.unit != orelse.unit:
                 _log.warning(
-                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                    self.fun_header(node)
                     + "Ternary operator with mixed units."
                 )
                 return QuantityNode(ast.copy_location(new_node, node), None)
             else:
                 return QuantityNode(
                     ast.copy_location(new_node, node), body.unit
                 )
 
         elif isinstance(node, ast.Call):
             node = self.generic_visit(node)  # type: ignore
             if isinstance(node.func, ast.Name):
-                id = node.func.id
+                id_ = node.func.id
+                module = None
             elif isinstance(node.func, ast.Attribute):
-                id = node.func.attr
+                res = split_attribute(node.func)
+                id_ = res["suffix"]
+                module = res["prefix"]
 
-            signature = self.get_annotations(id)
+            signature = self.get_annotations(id_, module)
 
             new_args = []
             offset = 0
 
             # if not a known impunity function or no return signature
             if (
                 signature is None
@@ -669,35 +719,35 @@
                 return_signature = list(signature.items())[-1]
 
                 for i, arg in enumerate(node.args):
                     expected = fun_signature[i + offset][1]
                     if fun_signature[i][0] == "self":
                         offset = 1
                     if is_annotated(expected):
-                        expected = expected.__metadata__[0]  # type: ignore
+                        expected = expected.__metadata__[0]
 
                     msg = (
-                        f"In function {self.fun.__module__}"
-                        + f"/{self.fun.__name__}: "
-                        + f"Function {id} expected unit "
+                        self.fun_header(node)
+                        + f"Function {id_} expected unit "
                         + f"{expected} but received unitless quantity"
                     )
 
                     if (received := self.get_node_unit(arg)).unit is None:
                         if expected is not inspect._empty:
                             _log.warning(msg)
                         new_args.append(arg)
                         continue
 
                     received.unit = (
-                        received.unit.__metadata__[0]  # type: ignore
+                        received.unit.__metadata__[0]
                         if is_annotated(received.unit)
                         else received.unit
                     )
 
+                    assert received.node is not None
                     new_arg = self.node_convert(
                         expected, received.unit, received.node
                     )
                     new_args.append(new_arg)
 
             new_node = (
                 node
@@ -706,15 +756,15 @@
                     func=node.func,
                     args=new_args,
                     keywords=node.keywords,
                 )
             )
 
             return_unit = (
-                return_signature[1].__metadata__[0]  # type: ignore
+                return_signature[1].__metadata__[0]
                 if is_annotated(return_signature[1])
                 else return_signature[1]
             )
 
             return QuantityNode(ast.copy_location(new_node, node), return_unit)
 
         elif isinstance(node, ast.Attribute):
@@ -734,65 +784,62 @@
             node (ast.Call): input node
 
         """
 
         if isinstance(node.func, ast.Name):
             fun_id = node.func.id
         elif isinstance(node.func, ast.Attribute):
-            attr = node.func
-            fun_id = ""
-            while isinstance(attr, ast.Attribute):
-                fun_id = "." + attr.attr + fun_id  # type: ignore
-                attr = attr.value  # type: ignore
-            if isinstance(attr, ast.Name):
-                fun_id = attr.id + fun_id  # type: ignore
+            res = split_attribute(node.func)
+            fun_id = res["prefix"] + "." + res["suffix"]
 
         if fun_id in __builtins__.keys():  # type: ignore
             node = self.generic_visit(node)  # type: ignore
             return node
 
         # parameters = inspect.getfullargspec(self.fun_globals[
         # node.func.id])
-        signature = self.get_annotations(fun_id)  # type: ignore
+        signature = self.get_annotations(fun_id)
 
         new_args: list[ast.BinOp | ast.expr] = []
         new_keywords: list[ast.BinOp | ast.expr] = []
         if node.args or node.keywords:
             if signature:
                 fun_signature = list(signature.items())[:-1]
             else:
                 return node
             for i, arg in enumerate(node.args):
                 if (received := self.get_node_unit(arg)).unit != (
                     expected := fun_signature[i][1]
                 ):
                     if is_annotated(expected):
-                        expected = expected.__metadata__[0]  # type: ignore
+                        expected = expected.__metadata__[0]
+                    assert received.node is not None
                     new_arg = self.node_convert(
                         expected, received.unit, received.node
                     )
                     new_args.append(new_arg)
                 else:
                     new_args.append(arg)
 
             for keyword in node.keywords:
                 if keyword.arg:
                     if (received := self.get_node_unit(keyword.value)) != (
                         expected := signature[keyword.arg]
                     ):
                         if is_annotated(expected):
-                            x = expected.__metadata__[0]  # type: ignore
+                            x = expected.__metadata__[0]
                             expected = x
                         if not (
                             isinstance(expected, str)
                             and isinstance(received.unit, str)
                         ):
                             # TODO To avoid annoying typing for now
                             return node
 
+                        assert received.node is not None
                         new_value = self.node_convert(
                             expected, received.unit, received.node
                         )
 
                         new_keyword = cast(
                             ast.expr,
                             ast.keyword(
@@ -823,16 +870,15 @@
             node (ast.AnnAssign): input node
 
         """
 
         value = self.get_node_unit(node.value)
 
         if value.node is None:
-            expected = cast(annotation_node, node.annotation)
-            expected_unit = get_annotation_unit(expected)
+            expected_unit = self.get_annotation_unit(node.annotation)
             self.vars[node.target.id] = expected_unit  # type: ignore
             return node
 
         if value.node != node.value:
             new_node = ast.AnnAssign(
                 target=node.target,
                 annotation=node.annotation,
@@ -841,55 +887,52 @@
             )
 
             node = ast.copy_location(new_node, node)
 
         if value.unit is None:
             new_node = node
 
-        elif (received := value).unit != (
-            expected := cast(annotation_node, node.annotation)
-        ):
-            expected_unit = get_annotation_unit(expected)
-            if is_annotated(received.unit):
-                received.unit = received.unit.__metadata__[0]  # type: ignore
+        else:
+            expected_unit = self.get_annotation_unit(node.annotation)
+            if is_annotated(value.unit):
+                value.unit = value.unit.__metadata__[0]
 
+            assert value.node is not None
             new_value = self.node_convert(
-                expected_unit, received.unit, received.node
+                expected_unit, value.unit, value.node
             )
             new_node = ast.AnnAssign(
                 target=node.target,
                 annotation=node.annotation,
                 value=new_value,
                 simple=node.simple,
             )
 
         if isinstance(node.target, ast.Attribute):
             if isinstance(node.target.value, ast.Name):
                 if node.target.value.id == "self":
                     self.class_attr[node.target.attr] = value.unit
         else:
             if isinstance(node.target, ast.Name):
-                annotation = get_annotation_unit(
-                    cast(annotation_node, node.annotation)
-                )
+                annotation = self.get_annotation_unit(node.annotation)
                 self.vars[node.target.id] = annotation
 
         return ast.copy_location(new_node, node)
 
     def visit_BinOp(self, node: ast.BinOp) -> ast.BinOp:
         """Method called by the visitor if the visited node is an
         Binary Operation node.
         Checks the units in the node and returns it eventually modified.
 
         Args:
             node (ast.BinOp): input node
 
         """
 
-        return self.get_node_unit(node).node
+        return self.get_node_unit(node).node  # type: ignore
 
     def visit_For(self, node: ast.For) -> ast.For:
         """Method called by the visitor if the visited node is a for loop node.
         Checks the units in the node and returns it eventually modified.
 
         Args:
             node (ast.For): input node
@@ -958,17 +1001,15 @@
             type_comment=f"unit: {value.unit}",
         )
 
         for target in node.targets:
             if isinstance(target, ast.Tuple):
                 received = (
                     [
-                        arg.__metadata__[0]  # type: ignore
-                        if is_annotated(arg)
-                        else arg
+                        arg.__metadata__[0] if is_annotated(arg) else arg
                         for arg in value.unit.__args__
                     ]
                     if hasattr(value.unit, "__args__")
                     else value.unit
                 )
                 for i, elem in enumerate(target.elts):
                     if isinstance(elem, ast.Name):
@@ -976,14 +1017,15 @@
                             self.vars[elem.id] = received[i].__forward_arg__
                         else:
                             self.vars[elem.id] = received[i]
 
             elif isinstance(target, ast.Name):
                 if target.id in self.vars:
                     expected = self.vars[target.id]
+                    assert value.node is not None
                     new_value = self.node_convert(
                         expected, value.unit, value.node
                     )
                     new_node = ast.Assign(
                         targets=node.targets,
                         value=new_value,
                     )
@@ -1001,74 +1043,76 @@
         Return node.
         Checks the units in the node and returns it eventually modified.
 
         Args:
             node (ast.Return): input node
 
         """
+
         for frameinfo in inspect.stack():
             if frameinfo.function == "visit_FunctionDef":
                 fun = frameinfo.frame.f_locals["node"].name
                 break
-        return_annotation = self.get_annotations(fun)
+
+        return_annotation = self.get_annotations(fun, self.current_module)
         received = self.get_node_unit(node.value)
 
         if received.node != node.value:
             new_node = ast.Return(value=received.node)
             node = ast.copy_location(new_node, node)
 
-        if return_annotation is inspect._empty or return_annotation is None:
-            _log.warning(
-                f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                + "Some return annotations are missing"
-            )
-            new_node = node
-            return ast.copy_location(new_node, node)
+        if isinstance(return_annotation, dict):
+            ret = return_annotation.get("return", None)
+            if ret is None:
+                _log.info(
+                    self.fun_header(node)
+                    + "Some return annotations are missing"
+                )
+                new_node = node
+                return ast.copy_location(new_node, node)
 
-        if isinstance(return_annotation, Dict):
-            if is_annotated(return_annotation["return"]):
-                ret = return_annotation["return"]
-                if len(ret.__args__) > 1:  # type: ignore
-                    expected = [
-                        x.__metadata__[0]  # type: ignore
-                        if is_annotated(x)
-                        else x
-                        for x in ret.__args__  # type: ignore
-                    ]
-                else:
-                    expected = ret.__metadata__[0]  # type: ignore
-            else:  # string annotations
-                expected = return_annotation["return"]
-        else:
-            _log.warning(
-                f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                "Type of the return annotation not supported yet"
+            if is_annotated(ret):
+                # if len(ret.__args__) > 1:
+                #    expected = [
+                #        x.__metadata__[0] if is_annotated(x) else x
+                #        for x in ret.__args__
+                #    ]
+                # else:
+                expected = ret.__metadata__[0]
+            elif not isinstance(expected := ret, str):
+                # if string annotations, keep going, otherwise stop
+                new_node = node
+                return ast.copy_location(new_node, node)
+        else:  # is None
+            _log.info(
+                self.fun_header(node) + "Some return annotations are missing"
             )
             new_node = node
             return ast.copy_location(new_node, node)
 
         if is_annotated(received.unit):
-            received.unit = received.unit.__metadata__[0]  # type: ignore
+            received.unit = received.unit.__metadata__[0]
 
         if isinstance(expected, list):
             if isinstance(received.unit, list):
                 new_node = node
             else:
                 _log.warning(
-                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                    "Expected more than one return value"
+                    self.fun_header(node)
+                    + "Expected more than one return value"
                 )
                 new_node = node
         else:
             if isinstance(received.unit, list):
                 _log.warning(
-                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                    "Expected more than one return value"
+                    self.fun_header(node)
+                    + "Expected more than one return value"
                 )
                 new_node = node
             else:
+                assert received.node is not None
                 new_value = self.node_convert(
                     expected, received.unit, received.node
                 )
                 new_node = ast.Return(value=new_value)
 
         return ast.copy_location(new_node, node)
```

### Comparing `impunity-1.0.2/src/impunity/wrapper.py` & `impunity-1.0.3/src/impunity/wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,22 +107,24 @@
     with the necessary unit conversions added, will be saved to
     the specified file.
 
     These rewritten functions can be further utilized in your codebase,
     allowing you to work with coherent units seamlessly.
     """
 
-    def deco_f(fun: Callable[..., Any]):
+    def deco_f(fun: F) -> F:
         if ignore:
             return fun
 
         # dedent for nested methods
         fun_tree = ast.parse(textwrap.dedent(inspect.getsource(fun)))
 
         visitor = Visitor(fun)
+        if "forward" in fun.__name__:
+            pass
         fun_tree = visitor.visit(fun_tree)  # type: ignore
 
         # get the string of the transformed function
         f_str = astor.to_source(fun_tree)
         if not rewrite:
             return fun
```

