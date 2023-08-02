# Comparing `tmp/sophia_doc-0.1.5.tar.gz` & `tmp/sophia_doc-0.1.6.tar.gz`

## Comparing `sophia_doc-0.1.5.tar` & `sophia_doc-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/.DS_Store
--rw-r--r--   0        0        0    15605 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/__init__.py
--rw-r--r--   0        0        0     3621 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/py.typed
--rw-r--r--   0        0        0     4915 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/utils.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/builders/__init__.py
--rw-r--r--   0        0        0    16335 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/sophia_doc/builders/markdown.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/LICENSE
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/README.md
--rw-r--r--   0        0        0     2840 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 sophia_doc-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/sophia_doc/.DS_Store
+-rw-r--r--   0        0        0    13298 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/sophia_doc/__init__.py
+-rw-r--r--   0        0        0     4399 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/sophia_doc/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/sophia_doc/py.typed
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/sophia_doc/utils.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/sophia_doc/builders/__init__.py
+-rw-r--r--   0        0        0    16344 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/sophia_doc/builders/markdown.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/LICENSE
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/README.md
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 sophia_doc-0.1.6/PKG-INFO
```

### Comparing `sophia_doc-0.1.5/sophia_doc/.DS_Store` & `sophia_doc-0.1.6/sophia_doc/.DS_Store`

 * *Files identical despite different names*

### Comparing `sophia_doc-0.1.5/sophia_doc/__init__.py` & `sophia_doc-0.1.6/sophia_doc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,126 +19,37 @@
 import traceback
 import types
 import warnings
 from enum import Enum
 from functools import cached_property
 from typing import Any, Generic, NamedTuple, TypeVar, Union
 
+from typing_extensions import override
+
 from sophia_doc.utils import import_module
 
 _T = TypeVar("_T")
 
 
-def _find_class(func: Any) -> type | None:
-    # cut from pydoc
-    cls = sys.modules.get(func.__module__)
-    if cls is None:
-        return None
-    for name in func.__qualname__.split(".")[:-1]:
-        cls = getattr(cls, name)
-    if not inspect.isclass(cls):
-        return None
-    return cls
-
-
-def _find_doc(obj: Any) -> str | None:
-    # cut from pydoc
-    if inspect.ismethod(obj):
-        name = obj.__func__.__name__  # type: ignore
-        self = obj.__self__
-        if (
-            inspect.isclass(self)
-            and getattr(self, name, None).__func__ is obj.__func__  # type: ignore
-        ):
-            # class method
-            cls = self
-        else:
-            cls = self.__class__
-    elif inspect.isfunction(obj):
-        name = obj.__name__
-        cls = _find_class(obj)
-        if cls is None or getattr(cls, name) is not obj:
-            return None
-    elif inspect.isbuiltin(obj):
-        name = obj.__name__
-        self = obj.__self__
-        if inspect.isclass(self) and self.__qualname__ + "." + name == obj.__qualname__:
-            # class method
-            cls = self
-        else:
-            cls = self.__class__
-    # Should be tested before isdatadescriptor().
-    elif isinstance(obj, property):
-        func = obj.fget
-        name = func.__name__  # type: ignore
-        cls = _find_class(func)
-        if cls is None or getattr(cls, name) is not obj:
-            return None
-    elif inspect.ismethoddescriptor(obj) or inspect.isdatadescriptor(obj):
-        name = obj.__name__  # type: ignore
-        cls = obj.__objclass__  # type: ignore
-        if getattr(cls, name) is not obj:
-            return None
-        if inspect.ismemberdescriptor(obj):
-            slots = getattr(cls, "__slots__", None)
-            if isinstance(slots, dict) and name in slots:
-                return slots[name]
-    else:
-        return None
-    for base in cls.__mro__:  # type: ignore
-        try:
-            doc = _get_own_doc(getattr(base, name))
-        except AttributeError:
-            continue
-        if doc is not None:
-            return doc
-    return None
-
+def getdoc(obj: Any) -> str:
+    """Get the documentation string for an object if it is not inherited from its class.
 
-def _get_own_doc(obj: Any) -> str | None:
-    """Get the documentation string for an object if it is not inherited from its class."""
-    # cut from pydoc
+    All tabs are expanded to space. To clean up docstrings that are
+    indented to line up with blocks of code, any whitespace than can be
+    uniformly removed from the second line onwards is removed.
+    """
     try:
         doc = object.__getattribute__(obj, "__doc__")
-        if doc is None:
-            return None
-        if obj is not type:
+        if doc is not None and obj is not type:
             typedoc = type(obj).__doc__
             if isinstance(typedoc, str) and typedoc == doc:
-                return None
+                return ""
     except AttributeError:
-        return None
-    else:
-        return doc
-
-
-def _getdoc(obj: Any):
-    """Get the documentation string for an object.
-
-    All tabs are expanded to space. To clean up docstrings that are
-    indented to line up with blocks of code, any whitespace than can be
-    uniformly removed from the second line onwards is removed.
-    """
-    # cut from pydoc
-    doc = _get_own_doc(obj)
-    if doc is None:
-        try:
-            doc = _find_doc(obj)
-        except (AttributeError, TypeError):
-            return None
-    if not isinstance(doc, str):
-        return None
-    return inspect.cleandoc(doc)
-
-
-def getdoc(obj: Any) -> str:
-    """Get the docstring string or comments for an object."""
-    # cut from pydoc
-    result = _getdoc(obj) or inspect.getcomments(obj)
-    return result or ""
+        pass
+    return inspect.getdoc(obj) or ""
 
 
 def isdata(obj: object) -> bool:
     """Check if an object is of a type that probably means it's data."""
     # cut from pydoc
     return not (
         inspect.ismodule(obj)
@@ -146,15 +57,15 @@
         or inspect.isroutine(obj)
         or inspect.isframe(obj)
         or inspect.istraceback(obj)
         or inspect.iscode(obj)
     )
 
 
-def is_visible_name(name: str, _all: list | None = None) -> bool:
+def is_visible_name(name: str, _all: list[str] | None = None) -> bool:
     """Decide whether to show documentation on a variable.
 
     Args:
         name: The variable name.
         _all: __all__ list of a module.
 
     Returns:
@@ -189,15 +100,15 @@
 
     __slots__ = ("obj", "name", "module", "_qualname")
     obj: _T
     name: str
     module: ModuleNode
     _qualname: str
 
-    def __init__(self, obj: _T, name: str, qualname: str, module: ModuleNode):
+    def __init__(self, obj: _T, name: str, qualname: str, module: ModuleNode) -> None:
         """Init DocNode."""
         self.obj = obj
         self.name = name
         self._qualname = qualname
         self.module = module
 
     @cached_property
@@ -214,18 +125,20 @@
     def annotations(self) -> dict[str, Any]:
         """Annotations of this object."""
         return get_annotations(self.obj)
 
     @cached_property
     def docstring(self) -> str:
         """Docstring of this object."""
-        return getdoc(self.obj)
+        return getdoc(self.obj) or inspect.getcomments(self.obj) or ""
 
     @staticmethod
-    def from_obj(obj: Any, name: str, qualname: str, module: ModuleNode) -> DocNode:
+    def from_obj(
+        obj: Any, name: str, qualname: str, module: ModuleNode
+    ) -> DocNode[Any]:
         """Returns an object of DocNode's subclass.
 
         Args:
             obj: An object.
             name: The name of the object.
             qualname: The qualname of the object.
             module: The module of the object.
@@ -235,53 +148,54 @@
         """
         try:
             if inspect.ismodule(obj):
                 return ModuleNode(obj)
             if inspect.isclass(obj):
                 return ClassNode(obj, name, qualname, module)
             if inspect.isroutine(obj):
-                return FunctionNode(obj, name, qualname, module)  # type: ignore
+                return FunctionNode(obj, name, qualname, module)
         except AttributeError:
             pass
         if isdata(obj):
             return DataNode(obj, name, qualname, module)
         return OtherNode(obj, name, qualname, module)
 
-    def __repr__(self):
+    @override
+    def __repr__(self) -> str:
         """Return the repr of this DocNode."""
         return (
             f"{self.__class__.__name__}:{self.name} "
             f"obj:{self.obj} docstring:{self.docstring}"
         )
 
 
 class ModuleNode(DocNode[types.ModuleType]):
     """The class of module node."""
 
-    def __init__(self, obj: types.ModuleType):
+    def __init__(self, obj: types.ModuleType) -> None:
         """Init ModuleNode."""
         super().__init__(obj, obj.__name__, "", self)
 
     @cached_property
-    def attributes(self) -> list[DocNode]:
+    def attributes(self) -> list[DocNode[Any]]:
         """A list of attributes of this module."""
         _all = getattr(self.obj, "__all__", None)
-        attributes = []
+        attributes: list[DocNode[Any]] = []
         for key, value in list(getattr(self.obj, "__dict__", {}).items()):
             if (inspect.getmodule(value) or self.obj) is self.obj and is_visible_name(
                 key, _all
             ):
                 attributes.append(self.from_obj(value, key, key, self))
         return attributes
 
     @cached_property
     def submodules(self) -> list[ModuleNode]:
         """A list of submodules of this module."""
-        submodules = []
-        submodule_names = set()
+        submodules: list[ModuleNode] = []
+        submodule_names: set[str] = set()
         if self.is_package:
             for _importer, modname, _ispkg in pkgutil.iter_modules(self.obj.__path__):
                 if not is_visible_name(modname):
                     continue
                 try:
                     submodule_names.add(modname)
                     module = import_module(self.name + "." + modname)
@@ -341,33 +255,33 @@
 
     @cached_property
     def functions(self) -> list[FunctionNode]:
         """A list of function objects in this module's attributes."""
         return [i for i in self.attributes if isinstance(i, FunctionNode)]
 
     @cached_property
-    def data(self) -> list[DataNode]:
+    def data(self) -> list[DataNode[Any]]:
         """A list of data objects in module's this attributes."""
         return [i for i in self.attributes if isinstance(i, DataNode)]
 
 
 class ClassNode(DocNode[type]):
     """The class of class node."""
 
     class Attribute(NamedTuple):
         """The attribute of a class."""
 
         name: str
         kind: str
-        node: DocNode
+        node: DocNode[Any]
 
     @cached_property
     def attributes(self) -> list[ClassNode.Attribute]:
         """A list of attributes of this class."""
-        attributes = []
+        attributes: list[ClassNode.Attribute] = []
         for name in filter(is_visible_name, dir(self.obj)):
             if isinstance(self.obj, Enum) and name == "__init__":
                 continue
 
             if (
                 name != "__init__"
                 and name not in self.obj.__dict__
@@ -390,15 +304,15 @@
                 if name in getattr(self.obj, "__slots__", []):
                     continue
                 kind = "data descriptor"
             else:
                 kind = "data"
 
             # get original function from class method or static method
-            if kind == "class method" or kind == "static method":
+            if isinstance(value, (staticmethod, classmethod)):
                 value = value.__func__  # type: ignore
 
             # functools.cached_property needs special handling
             if isinstance(value, cached_property):
                 kind = "cached property"
                 node = DataNode(value, name, self.qualname + "." + name, self.module)
             else:
@@ -435,15 +349,24 @@
     @cached_property
     def is_abstract(self) -> bool:
         """Returns True if this class is an abstract class."""
         return inspect.isabstract(self.obj)
 
 
 class FunctionNode(
-    DocNode[Union[types.FunctionType, types.MethodType, types.MethodDescriptorType]]
+    DocNode[
+        Union[
+            types.FunctionType,
+            types.MethodType,
+            types.BuiltinFunctionType,
+            types.WrapperDescriptorType,
+            types.MethodDescriptorType,
+            types.ClassMethodDescriptorType,
+        ]
+    ]
 ):
     """The class of function node."""
 
     @cached_property
     def signature(self) -> inspect.Signature | None:
         """Signature of this function."""
         try:
@@ -465,15 +388,15 @@
             return True
         if inspect.isbuiltin(self.obj):
             _self = getattr(self.obj, "__self__", None)
             return not (inspect.ismodule(_self) or (_self is None))
         return False
 
     @cached_property
-    def is_lambda_func(self):
+    def is_lambda_func(self) -> bool:
         """Returns True if this function is a lambda function."""
         return self.realname == "<lambda>"
 
 
 class DataNode(DocNode[_T]):
     """The class of data node."""
```

### Comparing `sophia_doc-0.1.5/sophia_doc/__main__.py` & `sophia_doc-0.1.6/sophia_doc/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,47 @@
 """The Sophia-doc Command-line interface."""
+from __future__ import annotations
+
 import argparse
 import sys
 
 from docstring_parser import DocstringStyle
 
 from sophia_doc import ModuleNode
 from sophia_doc.builders.markdown import MarkdownBuilder
 from sophia_doc.utils import import_module
 
 if sys.version_info >= (3, 9):
     from argparse import BooleanOptionalAction
 else:
     from argparse import Action
+    from typing import Any, Callable, Iterable, Sequence, TypeVar
+
+    from typing_extensions import override
+
+    _T = TypeVar("_T")
 
     class BooleanOptionalAction(Action):
         def __init__(
             self,
-            option_strings,
-            dest,
-            default=None,
-            type=None,
-            choices=None,
-            required=False,
-            help=None,
-            metavar=None,
-        ):
-            _option_strings = []
+            option_strings: Sequence[str],
+            dest: str,
+            default: _T | str | None = None,
+            type: Callable[[str], _T] | Any | None = None,
+            choices: Iterable[_T] | None = None,
+            required: bool = False,
+            help: str | None = None,
+            metavar: str | tuple[str, ...] | None = None,
+        ) -> None:
+            _option_strings: list[str] = []
             for option_string in option_strings:
                 _option_strings.append(option_string)
 
                 if option_string.startswith("--"):
-                    option_string = "--no-" + option_string[2:]
+                    option_string = "--no-" + option_string[2:]  # noqa: PLW2901
                     _option_strings.append(option_string)
 
             if help is not None and default is not None:
                 help += " (default: %(default)s)"
 
             super().__init__(
                 option_strings=_option_strings,
@@ -44,19 +51,30 @@
                 type=type,
                 choices=choices,
                 required=required,
                 help=help,
                 metavar=metavar,
             )
 
-        def __call__(self, parser, namespace, values, option_string=None):
-            if option_string in self.option_strings:
-                setattr(namespace, self.dest, not option_string.startswith("--no-"))  # type: ignore
+        @override
+        def __call__(
+            self,
+            _parser: Any,
+            namespace: Any,
+            _values: str | Sequence[Any] | None,
+            option_string: str | None = None,
+        ) -> None:
+            if option_string is not None and option_string in self.option_strings:
+                setattr(
+                    namespace,
+                    self.dest,
+                    not option_string.startswith("--no-"),
+                )
 
-        def format_usage(self):
+        def format_usage(self) -> str:
             return " | ".join(self.option_strings)
 
 
 parser = argparse.ArgumentParser(
     description="Sophia_doc is a python package to automatically "
     "generate API documents for Python modules",
     formatter_class=argparse.ArgumentDefaultsHelpFormatter,
@@ -66,14 +84,21 @@
     "-o",
     "--output-dir",
     type=str,
     default="doc",
     help="The directory to write document.",
 )
 parser.add_argument(
+    "-f",
+    "--format",
+    type=str,
+    default="markdown",
+    help="File format of document.",
+)
+parser.add_argument(
     "--docstring-style",
     type=str,
     default="auto",
     help="Docstring style the python module used.",
 )
 parser.add_argument(
     "--ignore-data",
@@ -107,17 +132,18 @@
     "--init-file-name",
     type=str,
     default="index.md",
     help="The name of Markdown file from __init__.py, index.md by default.",
 )
 
 
-def cli():
+def cli() -> None:
     """The Sophia-doc Command-line interface."""
     args = parser.parse_args()
+    assert args.format == "markdown"
     MarkdownBuilder(
         ModuleNode(import_module(args.module)),
         docstring_style=getattr(DocstringStyle, args.docstring_style.upper()),
         anchor_extend=args.anchor_extend,
         ignore_data=args.ignore_data,
     ).write(
         args.output_dir,
```

### Comparing `sophia_doc-0.1.5/sophia_doc/utils.py` & `sophia_doc-0.1.6/sophia_doc/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,19 +26,19 @@
             warnings.filterwarnings("ignore", category=ImportWarning)
             return importlib.import_module(modname)
     except KeyboardInterrupt:
         # Dot not catch KeyboardInterrupt.
         # Catch KeyboardInterrupt may prevent user kill python
         # when the module took a too long time to import.
         raise
-    except BaseException as exc:
+    except BaseException as exc:  # noqa: BLE001
         raise ImportError(exc, traceback.format_exc()) from exc
 
 
-def format_annotation(annotation: Any, base_module: ModuleType | None = None) -> str:
+def format_annotation(annotation: Any, base_module: str | None = None) -> str:
     """Format the annotation.
 
     Args:
         annotation: The annotation object to be formatted.
         base_module: A module which the object from.
 
     Returns:
@@ -46,17 +46,17 @@
     """
     if annotation is inspect.Signature.empty:
         return ""
     if isinstance(annotation, str):
         return annotation
     # use regex delete 'ForwardRef' from annotation
     return re.sub(
-        r"\bForwardRef\((?P<quot>[\'\"])(?P<string>.*?)(?P=quot)\)",  # type: ignore
-        r"\g<string>",  # type: ignore
-        inspect.formatannotation(annotation, base_module),  # type: ignore
+        r"\bForwardRef\((?P<quot>[\'\"])(?P<string>.*?)(?P=quot)\)",
+        r"\g<string>",
+        inspect.formatannotation(annotation, base_module),
     )
 
 
 def format_parameter(parameter: inspect.Parameter, type_comments: bool = False) -> str:
     """Format inspect.Parameter object, type comments is optional.
 
     Cut from inspect.Parameter.__str__().
@@ -100,15 +100,15 @@
 
     Returns:
         The formatted string.
     """
     if type_comments:
         return str(signature)
 
-    result = []
+    result: list[str] = []
     render_pos_only_separator = False
     render_kw_only_separator = True
     for param in signature.parameters.values():
         formatted = format_parameter(param, type_comments=type_comments)
 
         kind = param.kind
```

### Comparing `sophia_doc-0.1.5/sophia_doc/builders/__init__.py` & `sophia_doc-0.1.6/sophia_doc/builders/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Builder is class to build ModuleNode to target formats."""
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from pathlib import Path
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 from docstring_parser import Docstring, DocstringStyle, parse
 
 if TYPE_CHECKING:
     from sophia_doc import DocNode, ModuleNode
 
 
@@ -25,29 +25,29 @@
     docstring_style: DocstringStyle
 
     def __init__(
         self,
         module: ModuleNode,
         *,
         docstring_style: DocstringStyle = DocstringStyle.AUTO,
-    ):
+    ) -> None:
         """Init Builder.
 
         Args:
             module: The Module Node to build.
             docstring_style: The docstring style. Defaults to DocstringStyle.AUTO.
         """
         self.module = module
         self.docstring_style = docstring_style
 
     def _new_builder(self, module: ModuleNode) -> Builder:
         """Get a new instance of Builder class, is used in write method."""
         return self.__class__(module, docstring_style=self.docstring_style)
 
-    def get_docstring(self, obj: DocNode) -> Docstring:
+    def get_docstring(self, obj: DocNode[Any]) -> Docstring:
         """Get the Docstring object of a DocNode object.
 
         Args:
             obj: A DocNode object.
 
         Returns:
             A Docstring object.
@@ -56,30 +56,30 @@
 
     @abstractmethod
     def text(self) -> str:
         """Get string of current module documentation."""
         raise NotImplementedError
 
     @abstractmethod
-    def get_path(self, **kwargs) -> Path:
+    def get_path(self, **kwargs: Any) -> Path:
         """Get the path to write file."""
         raise NotImplementedError
 
-    def write(self, output_dir: str, *, overwrite: bool = False, **kwargs) -> None:
+    def write(self, output_dir: str, *, overwrite: bool = False, **kwargs: Any) -> None:
         """Write file to output dir.
 
         Args:
             output_dir: The output directory.
             overwrite: If true will overwrite any file in output directory,
                 otherwise raise an Exception when file already exists.
             **kwargs: Other args.
         """
         filepath = Path(output_dir).resolve() / self.get_path(**kwargs)
         filepath.parent.mkdir(parents=True, exist_ok=True)
         if not self.module.is_namespace:
             filepath.touch(exist_ok=overwrite)
-            with open(filepath, "w", encoding="utf-8") as f:
+            with filepath.open("w", encoding="utf-8") as f:
                 f.write(self.text())
         for submodule in self.module.submodules:
             self._new_builder(submodule).write(
                 output_dir, overwrite=overwrite, **kwargs
             )
```

### Comparing `sophia_doc-0.1.5/sophia_doc/builders/markdown.py` & `sophia_doc-0.1.6/sophia_doc/builders/markdown.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """The Markdown Builder."""
 from __future__ import annotations
 
 import inspect
 import warnings
 from pathlib import Path
 from textwrap import indent
+from typing import Any
 
 from docstring_parser import Docstring, DocstringParam, DocstringStyle
+from typing_extensions import override
 
 from sophia_doc import ClassNode, DataNode, DocNode, FunctionNode, ModuleNode
 from sophia_doc.builders import Builder
 from sophia_doc.utils import format_annotation, format_signature
 
 
 def get_description(docstring: Docstring) -> list[str]:
@@ -37,17 +39,17 @@
         name: Parameter name.
         annotation: Parameter annotation.
         description: Parameter description.
 
     Returns:
         Formatted string of parameter.
     """
-    result = f"- {Markdown.bold(name)}"
+    result = f"- {Markdown.bold(Markdown.escape(name))}"
     if annotation:
-        result += f" ({Markdown.italic(annotation)})"
+        result += f" ({Markdown.italic(Markdown.escape(annotation))})"
     if description:
         result += f" - {description}"
     return result
 
 
 def parser_docstring_param(param: DocstringParam) -> str:
     """Get formatted string of parameter from a DocstringParam object.
@@ -61,22 +63,32 @@
     return parser_param(param.arg_name, param.type_name, param.description)
 
 
 class Markdown:
     """Markdown format."""
 
     @staticmethod
+    def escape(text: str) -> str:
+        """Escape Markdown control characters."""
+        new_text = ""
+        for c in text:
+            if c in "*#\\()[]<>_`":
+                new_text += "\\"
+            new_text += c
+        return new_text
+
+    @staticmethod
     def indent(text: str, level: int = 1) -> str:
         """Indent."""
         return indent(text, prefix=" " * (level * 2))
 
     @staticmethod
     def italic(text: str) -> str:
         """Italic."""
-        return f"*{text}*"
+        return f"_{text}_"
 
     @staticmethod
     def bold(text: str) -> str:
         """Bold."""
         return f"**{text}**"
 
     @staticmethod
@@ -105,295 +117,283 @@
     def __init__(
         self,
         module: ModuleNode,
         *,
         docstring_style: DocstringStyle = DocstringStyle.AUTO,
         anchor_extend: bool = False,
         ignore_data: bool = False,
-    ):
+    ) -> None:
         """Init Markdown Builder."""
         super().__init__(module, docstring_style=docstring_style)
         self.anchor_extend = anchor_extend
         self.ignore_data = ignore_data
 
+    @override
     def _new_builder(self, module: ModuleNode) -> Builder:
         return self.__class__(
             module,
             docstring_style=self.docstring_style,
             anchor_extend=self.anchor_extend,
             ignore_data=self.ignore_data,
         )
 
+    @override
     def get_path(
         self,
         exclude_module_name: bool = False,
         init_file_name: str = "index.md",
-        **kwargs,  # noqa: ARG002
+        **_kwagrs: Any,
     ) -> Path:
         """Get the path to write file.
 
         Args:
             exclude_module_name: If true will write file to path
                 which exclude module name, like change output path
                 form `./doc/sophia_doc/index.md` to `./doc/index.md`.
             init_file_name: The name of Markdown file
                 from __init__.py, `index.md` by default.
-            **kwargs: Other args.
         """
         if exclude_module_name:
             path = Path(*self.module.name.split(".")[1:])
         else:
             path = Path(*self.module.name.split(".")[0:])
         return (
             path / init_file_name if self.module.is_package else path.with_suffix(".md")
         )
 
+    @override
     def text(self) -> str:
         """Get string of current module documentation."""
         result: list[str] = []
         result.append(Markdown.title(self.module.name, 1))
 
         docstring = self.get_docstring(self.module)
         result.extend(get_description(docstring))
 
         result.extend(self.build_doc(node) for node in self.module.attributes)
 
-        return self._build_str(result).replace("<", r"\<").replace(">", r"\>")
+        return self._build_str(result) + "\n"
 
     @staticmethod
     def _build_str(str_list: list[str]) -> str:
         return "\n\n".join(filter(lambda x: x, str_list))
 
-    def build_doc(self, node: DocNode, *, level: int = 1, **kwargs) -> str:
+    def build_doc(self, node: DocNode[Any], *, level: int = 1, **kwargs: Any) -> str:
         """Build markdown string from a DocNode.
 
         Args:
             node: A DocNode.
             level: The title level.
             **kwargs: Other args.
 
         Returns:
             A markdown string.
         """
         if isinstance(node, ClassNode):
-            return self.build_class(node, level=level)
+            return self.build_class(node, level=level, **kwargs)
         if isinstance(node, FunctionNode):
             return self.build_function(node, level=level, **kwargs)
         if isinstance(node, DataNode):
             return self.build_data(node, level=level, **kwargs)
         raise ValueError
 
-    def _extend_title(self, title: str, node: DocNode) -> str:
-        return title + " {#" + node.qualname + "}" if self.anchor_extend else title
+    def _extend_title(self, title: str, node: DocNode[Any]) -> str:
+        return (
+            title + " {#" + Markdown.escape(node.qualname) + "}"
+            if self.anchor_extend
+            else title
+        )
 
-    def build_class(self, node: ClassNode, *, level: int = 1) -> str:
+    def build_class(self, node: ClassNode, *, level: int = 1, **_kwagrs: Any) -> str:
         """Build markdown string from a ClassNode.
 
         Args:
             node: A ClassNode.
             level: The title level.
 
         Returns:
             A markdown string.
         """
-        _kind = []
+        _kind: list[str] = []
         if node.is_abstract:
             _kind.append("abstract")
         if isinstance(node.obj, Exception):
             _kind.append("exception")
         else:
             _kind.append("class")
-        _kind = " ".join(_kind)
-
-        init = None
-        for attr in node.attributes:
-            if attr.name == "__init__":
-                assert isinstance(attr.node, FunctionNode)
-                init = attr.node
+        kind = " ".join(_kind)
 
         result: list[str] = []
         title = Markdown.title(
-            Markdown.italic(_kind) + " " + Markdown.inline_code(node.name), level + 1
+            Markdown.italic(kind) + " " + Markdown.inline_code(node.name), level + 1
         )
-        if init and init.signature:
-            title += format_signature(init.signature)
-        else:
-            warnings.warn(
-                f"Can not get __init__ method signature of class {node.name}",
-                stacklevel=1,
-            )
         result.append(self._extend_title(title, node))
 
         result.append("Bases: " + ", ".join(map(Markdown.inline_code, node.bases)))
 
         docstring = self.get_docstring(node)
         result.extend(get_description(docstring))
 
-        if init and init.signature:
-            result.extend(
-                self._build_argument(
-                    init, self.get_docstring(init), ignore_first_arg=True
-                )
-            )
-
         if docstring.params or node.annotations:
             result.append("- **Attributes**")
 
-            parma_dict: dict[str, tuple[inspect.Parameter, DocstringParam | None]] = {}
+            parma_dict: dict[
+                str, tuple[inspect.Parameter | None, DocstringParam | None]
+            ] = {}
             if node.annotations:
                 parma_dict = {
                     key: (annotation, None)
                     for key, annotation in node.annotations.items()
                     if not key.startswith("_")
                 }
 
             if docstring.params:
                 for param_doc in docstring.params:
                     annotation, _ = parma_dict.get(param_doc.arg_name, (None, None))
                     if param_doc.type_name is None and annotation:
                         param_doc.type_name = format_annotation(
-                            annotation, base_module=node.module.obj
+                            annotation, base_module=node.module.name
                         )
-                    parma_dict[param_doc.arg_name] = (  # type:ignore
-                        annotation,
-                        param_doc,
-                    )
+                    parma_dict[param_doc.arg_name] = (annotation, param_doc)
 
             for name, (annotation, param_doc) in parma_dict.items():
                 if param_doc is None:
                     result.append(
                         Markdown.indent(
                             parser_param(
                                 name,
-                                format_annotation(
-                                    annotation, base_module=node.module.obj
+                                annotation
+                                and format_annotation(
+                                    annotation, base_module=node.module.name
                                 ),
                                 None,
                             )
                         )
                     )
                 else:
                     result.append(Markdown.indent(parser_docstring_param(param_doc)))
 
         if docstring.examples:
             result.append("- **Examples**")
             result.append(Markdown.indent(docstring.examples[0].description or ""))
 
-        for name, kind, node_ in node.attributes:
-            if name == "__init__":
-                continue
+        for _name, kind, node_ in node.attributes:
             result.append(
                 self.build_doc(
                     node_,
                     level=level + 1,
                     kind=kind,
-                    ignore_first_arg=kind == "method" or kind == "class method",
+                    ignore_first_arg=kind in {"method", "class method"},
                 )
             )
 
         return self._build_str(result)
 
     @staticmethod
     def _build_argument(
         node: FunctionNode, docstring: Docstring, *, ignore_first_arg: bool = False
     ) -> list[str]:
-        result = []
+        result: list[str] = []
         if docstring.params or (node.signature and node.signature.parameters):
-            parma_dict: dict[str, tuple[inspect.Parameter, DocstringParam | None]] = {}
+            parma_dict: dict[
+                str, tuple[inspect.Parameter | None, DocstringParam | None]
+            ] = {}
             if node.signature and node.signature.parameters:
-                for key, param in node.signature.parameters.items():
+                for _key, param in node.signature.parameters.items():
+                    key = _key
                     if param.kind == param.VAR_POSITIONAL:
-                        key = "*" + key  # noqa: PLW2901
+                        key = "*" + key
                     elif param.kind == param.VAR_KEYWORD:
-                        key = "**" + key  # noqa: PLW2901
+                        key = "**" + key
                     parma_dict[key] = (param, None)
 
             if docstring.params:
                 for param_doc in docstring.params:
-                    if param_doc.arg_name not in parma_dict and (
-                        node.signature and node.signature.parameters
+                    if (
+                        param_doc.arg_name not in parma_dict
+                        and node.signature
+                        and node.signature.parameters
                     ):
                         warnings.warn(
-                            f'The argument "{param_doc.arg_name}" '
+                            f'The argument "{param_doc.arg_name}" of {node.qualname}'
                             f"can not find in function signature.",
                             stacklevel=1,
                         )
                     param, _ = parma_dict.get(param_doc.arg_name, (None, None))
                     if param_doc.type_name is None and param:
                         param_doc.type_name = format_annotation(
-                            param.annotation, base_module=node.module.obj
+                            param.annotation, base_module=node.module.name
                         )
-                    parma_dict[param_doc.arg_name] = (param, param_doc)  # type:ignore
+                    parma_dict[param_doc.arg_name] = (param, param_doc)
 
             if ignore_first_arg and parma_dict:
-                parma_dict.pop(list(parma_dict.keys())[0])
+                parma_dict.pop(next(iter(parma_dict.keys())))
 
             if parma_dict:
                 result.append("- **Arguments**")
 
             for param, param_doc in parma_dict.values():
-                if param_doc is None:
+                if param_doc is not None:
+                    result.append(Markdown.indent(parser_docstring_param(param_doc)))
+                elif param is not None:
                     result.append(
                         Markdown.indent(
                             parser_param(
                                 param.name,
                                 format_annotation(
-                                    param.annotation, base_module=node.module.obj
+                                    param.annotation, base_module=node.module.name
                                 ),
                                 None,
                             )
                         )
                     )
-                else:
-                    result.append(Markdown.indent(parser_docstring_param(param_doc)))
 
         return result
 
     def build_function(
         self,
         node: FunctionNode,
         *,
         level: int = 1,
         kind: str = "function",
         ignore_first_arg: bool = False,
-        **kwargs,  # noqa: ARG002
+        **_kwagrs: Any,
     ) -> str:
         """Build markdown string from a FunctionNode.
 
         Args:
             node: A FunctionNode.
             level: The title level.
             kind: The function kind, like 'function', 'method', 'class method'.
             ignore_first_arg: If True the first argument of the function
                 will be ignored.
-            **kwargs: Other args.
 
         Returns:
             A markdown string.
         """
         if not node.signature:
             warnings.warn(
                 f"The {node.qualname} ({node.obj}) not have signature, ignored.",
                 stacklevel=1,
             )
             return ""
 
-        _kind = []
+        _kind: list[str] = []
         if node.is_async:
             _kind.append("async")
         if node.is_lambda_func:
             _kind.append("lambda")
         _kind.append(kind)
-        _kind = " ".join(_kind)
+        kind = " ".join(_kind)
 
         result: list[str] = []
         result.append(
             self._extend_title(
                 Markdown.title(
-                    Markdown.italic(_kind)
+                    Markdown.italic(kind)
                     + " "
                     + Markdown.inline_code(
                         f"{node.name}{format_signature(node.signature)}"
                     ),
                     level + 1,
                 ),
                 node,
@@ -403,70 +403,75 @@
         docstring = self.get_docstring(node)
         result.extend(get_description(docstring))
 
         result.extend(
             self._build_argument(node, docstring, ignore_first_arg=ignore_first_arg)
         )
 
-        if docstring.returns or (
-            node.signature
-            and node.signature.return_annotation is not inspect.Signature.empty
+        if (
+            docstring.returns is not None
+            or node.signature.return_annotation is not inspect.Signature.empty
         ):
             result.append("- **Returns**")
 
             type_name = ""
-            if docstring.returns is not None and docstring.returns.type_name:
-                type_name = docstring.returns.type_name
-            elif (
-                node.signature is not None
-                and node.signature.return_annotation is not inspect.Signature.empty
+            if (
+                docstring.returns is not None
+                and docstring.returns.type_name is not None
             ):
+                type_name = docstring.returns.type_name
+            elif node.signature.return_annotation is not inspect.Signature.empty:
                 type_name = format_annotation(
-                    node.signature.return_annotation, base_module=node.module.obj
+                    node.signature.return_annotation, base_module=node.module.name
                 )
 
             if type_name:
-                result.append(Markdown.indent(f"Type: {Markdown.italic(type_name)}"))
+                result.append(
+                    Markdown.indent(
+                        f"Type: {Markdown.italic(Markdown.escape(type_name))}"
+                    )
+                )
 
             if docstring.returns and docstring.returns.description:
                 result.append(Markdown.indent(docstring.returns.description))
 
         if docstring.raises:
             result.append("- **Raises**")
             result.extend(
                 Markdown.indent(
                     "- {type_name} - {description}".format(
-                        type_name=Markdown.bold(raise_doc.type_name or ""),
+                        type_name=Markdown.bold(
+                            Markdown.escape(raise_doc.type_name or "")
+                        ),
                         description=raise_doc.description,
                     )
                 )
                 for raise_doc in docstring.raises
             )
 
         if docstring.examples:
             result.append("- **Examples**")
             result.append(Markdown.indent(docstring.examples[0].description or ""))
 
         return self._build_str(result)
 
     def build_data(
         self,
-        node: DataNode,
+        node: DataNode[Any],
         *,
         level: int = 1,
         kind: str = "data",
-        **kwargs,  # noqa: ARG002
+        **_kwagrs: Any,
     ) -> str:
         """Build markdown string from a DataNode.
 
         Args:
             node: A DataNode.
             level: The title level.
             kind: The function kind, like 'data', 'property'.
-            **kwargs: Other args.
 
         Returns:
             A markdown string.
         """
         if self.ignore_data and kind == "data":
             return ""
 
@@ -481,16 +486,18 @@
             )
         )
 
         if "property" in kind and node.annotations.get("return", None):
             result.append(
                 "Type: {type_name}".format(
                     type_name=Markdown.italic(
-                        format_annotation(
-                            node.annotations["return"], base_module=node.module.obj
+                        Markdown.escape(
+                            format_annotation(
+                                node.annotations["return"], base_module=node.module.name
+                            )
                         )
                     )
                 )
             )
 
         docstring = self.get_docstring(node)
         result.extend(get_description(docstring))
```

### Comparing `sophia_doc-0.1.5/.gitignore` & `sophia_doc-0.1.6/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -156,7 +156,11 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 .idea/
+
+docs/
+tests/
+main.py
```

### Comparing `sophia_doc-0.1.5/LICENSE` & `sophia_doc-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sophia_doc-0.1.5/README.md` & `sophia_doc-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `sophia_doc-0.1.5/PKG-INFO` & `sophia_doc-0.1.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sophia-doc
-Version: 0.1.5
+Version: 0.1.6
 Summary: A python package to automatically generate API documents for Python modules.
 Project-URL: Homepage, https://github.com/st1020/sophia-doc
 Project-URL: Source, https://github.com/st1020/sophia-doc
 Author-email: st1020 <stone_1020@qq.com>
 License: MIT
 License-File: LICENSE
 Keywords: doc,documentation,markdown,pydoc,sophia-doc
@@ -16,14 +16,15 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: Markup
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
 Requires-Dist: docstring-parser>=0.15
+Requires-Dist: typing-extensions>=4.7.1
 Description-Content-Type: text/markdown
 
 # Sophia-doc
 
 **A python package to automatically generate API documents for Python modules.**
 
 ## Introduction
```

