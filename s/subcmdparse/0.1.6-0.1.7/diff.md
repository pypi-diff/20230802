# Comparing `tmp/subcmdparse-0.1.6.tar.gz` & `tmp/subcmdparse-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "subcmdparse-0.1.6.tar", last modified: Mon Jul 10 08:38:23 2023, max compression
+gzip compressed data, was "subcmdparse-0.1.7.tar", last modified: Wed Aug  2 06:08:38 2023, max compression
```

## Comparing `subcmdparse-0.1.6.tar` & `subcmdparse-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.159335 subcmdparse-0.1.6/
--rw-r--r--   0 dhkim      (501) staff       (20)      357 2023-07-10 08:38:23.158772 subcmdparse-0.1.6/PKG-INFO
--rw-r--r--   0 dhkim      (501) staff       (20)       60 2022-06-19 07:33:30.000000 subcmdparse-0.1.6/README.md
--rw-r--r--   0 dhkim      (501) staff       (20)       38 2023-07-10 08:38:23.159527 subcmdparse-0.1.6/setup.cfg
--rw-r--r--   0 dhkim      (501) staff       (20)     1219 2023-07-10 08:37:47.000000 subcmdparse-0.1.6/setup.py
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.150925 subcmdparse-0.1.6/src/
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.154292 subcmdparse-0.1.6/src/subcmdparse/
--rw-r--r--   0 dhkim      (501) staff       (20)       53 2022-06-19 07:33:30.000000 subcmdparse-0.1.6/src/subcmdparse/__init__.py
--rw-r--r--   0 dhkim      (501) staff       (20)     8407 2023-07-10 08:36:14.000000 subcmdparse-0.1.6/src/subcmdparse/subcmdparse.py
--rw-r--r--   0 dhkim      (501) staff       (20)      300 2022-06-19 07:33:30.000000 subcmdparse-0.1.6/src/subcmdparse/util.py
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.157361 subcmdparse-0.1.6/src/subcmdparse.egg-info/
--rw-r--r--   0 dhkim      (501) staff       (20)      357 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/PKG-INFO
--rw-r--r--   0 dhkim      (501) staff       (20)      320 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/SOURCES.txt
--rw-r--r--   0 dhkim      (501) staff       (20)        1 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/dependency_links.txt
--rw-r--r--   0 dhkim      (501) staff       (20)       14 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/requires.txt
--rw-r--r--   0 dhkim      (501) staff       (20)       12 2023-07-10 08:38:23.000000 subcmdparse-0.1.6/src/subcmdparse.egg-info/top_level.txt
-drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-07-10 08:38:23.157811 subcmdparse-0.1.6/tests/
--rw-r--r--   0 dhkim      (501) staff       (20)     7227 2022-06-19 07:33:30.000000 subcmdparse-0.1.6/tests/test_subcommand.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-08-02 06:08:38.866518 subcmdparse-0.1.7/
+-rw-r--r--   0 dhkim      (501) staff       (20)      357 2023-08-02 06:08:38.866215 subcmdparse-0.1.7/PKG-INFO
+-rw-r--r--   0 dhkim      (501) staff       (20)       60 2022-06-19 07:33:30.000000 subcmdparse-0.1.7/README.md
+-rw-r--r--   0 dhkim      (501) staff       (20)       38 2023-08-02 06:08:38.866680 subcmdparse-0.1.7/setup.cfg
+-rw-r--r--   0 dhkim      (501) staff       (20)     1219 2023-08-02 06:08:29.000000 subcmdparse-0.1.7/setup.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-08-02 06:08:38.858787 subcmdparse-0.1.7/src/
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-08-02 06:08:38.862696 subcmdparse-0.1.7/src/subcmdparse/
+-rw-r--r--   0 dhkim      (501) staff       (20)       53 2022-06-19 07:33:30.000000 subcmdparse-0.1.7/src/subcmdparse/__init__.py
+-rw-r--r--   0 dhkim      (501) staff       (20)     9238 2023-08-02 06:08:08.000000 subcmdparse-0.1.7/src/subcmdparse/subcmdparse.py
+-rw-r--r--   0 dhkim      (501) staff       (20)      300 2022-06-19 07:33:30.000000 subcmdparse-0.1.7/src/subcmdparse/util.py
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-08-02 06:08:38.865239 subcmdparse-0.1.7/src/subcmdparse.egg-info/
+-rw-r--r--   0 dhkim      (501) staff       (20)      357 2023-08-02 06:08:38.000000 subcmdparse-0.1.7/src/subcmdparse.egg-info/PKG-INFO
+-rw-r--r--   0 dhkim      (501) staff       (20)      320 2023-08-02 06:08:38.000000 subcmdparse-0.1.7/src/subcmdparse.egg-info/SOURCES.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)        1 2023-08-02 06:08:38.000000 subcmdparse-0.1.7/src/subcmdparse.egg-info/dependency_links.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)       14 2023-08-02 06:08:38.000000 subcmdparse-0.1.7/src/subcmdparse.egg-info/requires.txt
+-rw-r--r--   0 dhkim      (501) staff       (20)       12 2023-08-02 06:08:38.000000 subcmdparse-0.1.7/src/subcmdparse.egg-info/top_level.txt
+drwxr-xr-x   0 dhkim      (501) staff       (20)        0 2023-08-02 06:08:38.865636 subcmdparse-0.1.7/tests/
+-rw-r--r--   0 dhkim      (501) staff       (20)     7227 2022-06-19 07:33:30.000000 subcmdparse-0.1.7/tests/test_subcommand.py
```

### Comparing `subcmdparse-0.1.6/setup.py` & `subcmdparse-0.1.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="subcmdparse", # Replace with your own username
-    version="0.1.6",
+    version="0.1.7",
     author="Donghwi Kim",
     author_email="dhkim09@kaist.ac.kr",
     description="Subcommand extension for argparse package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dhkim09a/subcmdparse",
     packages=setuptools.find_packages(where='src'),
```

### Comparing `subcmdparse-0.1.6/src/subcmdparse/subcmdparse.py` & `subcmdparse-0.1.7/src/subcmdparse/subcmdparse.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 # PYTHON_ARGCOMPLETE_OK
 
 from __future__ import annotations
 
 import argparse
-from typing import Union, List
+from typing import Any, Optional, Union, List, Protocol, Callable, Type
 from gettext import gettext as _
 
 from .util import compile_shargs
 
 try:
     import argcomplete
 except ImportError:
     pass
 
 
+class _Subcommand_on_command(Protocol):
+    def __call__(self, args: object, unknown_args: Optional[object] = None) -> Any:
+        pass
+
+
+class _InternalSubcmdArgs(Protocol):
+    _func: _Subcommand_on_command
+    _allow_unknown_args: bool
+
+
 class TolerableSubParsersAction(argparse._SubParsersAction):
     @property
     def choices(self):
         return None
 
     @choices.setter
     def choices(self, val):
@@ -49,15 +59,15 @@
     #     # message = parser.format_help()
     #     message = parser.format_usage()
     #     if indent:
     #         lines = message.split('\n')
     #         message = '\n'.join([indent + line for line in lines])
     #     parser._print_message(message, file)
 
-    def __call__(self, parser, namespace, values, option_string=None):
+    def __call__(self, parser: SubcommandParser, namespace, values, option_string=None):
         # depth first search
         stack: list[tuple[SubcommandParser, int]] = []
         stack.append((parser, 0))
         while stack and (elm := stack.pop()):
             parser, level = elm
             # self.print_help(parser, indent='  ' * level)
             # self.print_help(parser)
@@ -66,24 +76,24 @@
                 to_push = [(subcmd.parser, level + 1) for subcmd in parser.subcommands]
                 to_push.reverse()
                 stack.extend(to_push)
         parser.exit()
 
 
 class SubcommandParser(argparse.ArgumentParser):
-    subparsers = None
-    subcommands: list = None
-    parent_shared_parsers: List[argparse.ArgumentParser] = None
-    shared_parser: argparse.ArgumentParser = None
+    subparsers: Optional[argparse._SubParsersAction] = None
+    subcommands: Optional[list[Subcommand]] = None
+    parent_shared_parsers: Optional[List[argparse.ArgumentParser]] = None
+    shared_parser: Optional[argparse.ArgumentParser] = None
 
     argcomplete: bool
     __allow_unknown_args: bool
     add_help_all: bool
 
-    __unknown_args: list = None
+    __unknown_args: Optional[list] = None
 
     @property
     def allow_unknown_args(self) -> bool:
         return self.__allow_unknown_args
 
     @allow_unknown_args.setter
     def allow_unknown_args(self, val: bool):
@@ -101,58 +111,66 @@
         default_prefix = '-' if '-' in self.prefix_chars else self.prefix_chars[0]
         if self.add_help:
             self.add_argument(
                 default_prefix*2+'usage'+default_prefix+'all',
                 action=_UsageAllAction, default=argparse.SUPPRESS,
                 help=_('show all subcommand usages recursively'))
 
-    def add_subcommands(self, *subcommands, title=None, required=True, help=None, metavar='SUBCOMMAND'):
+    def add_subcommands(self, *subcommands: Subcommand, title: Optional[str] = None, required: bool = True, help: Optional[str] = None, metavar: str = 'SUBCOMMAND'):
         if not self.subparsers:
+            kwargs = {}
+            if title:
+                kwargs['title'] = title
+            if self.allow_unknown_args:
+                kwargs['action'] = TolerableSubParsersAction
             self.subparsers = self.add_subparsers(
-                **{'title': title} if title else {},
                 required=required,
                 help=help,
                 metavar=metavar,
-                **{'action': TolerableSubParsersAction} if self.allow_unknown_args else {},
+                **kwargs,
             )
 
         if not self.subcommands:
             self.subcommands = []
 
         self.subcommands.extend(list(subcommands))
 
     def _register_subcommands(self):
         if not self.subcommands:
             return
+        
+        # self.subparsers must not be None after self.add_subcommands()
+        assert self.subparsers
+
         for subcommand in self.subcommands:
             if not isinstance(subcommand, Subcommand):
                 raise TypeError(str(subcommand.__class__) + 'is not Subcommand')
             subcommand._register(self.subparsers,
                                  parents=[*(self.parent_shared_parsers if self.parent_shared_parsers else []),
                                           *([self.shared_parser] if self.shared_parser else [])],
                                  )
 
     def try_argcomplete(self):
         if 'argcomplete' in globals():
             argcomplete.autocomplete(self)
         else:
             print('warning: install \'argcomplete\' package to enable bash autocomplete')
 
-    def parse_args(self, *args, **kwargs) -> any:
+    def parse_args(self, *args, **kwargs) -> _InternalSubcmdArgs:
         self._register_subcommands()
         if self.argcomplete:
             self.try_argcomplete()
         parsed_args, unknown_args = super().parse_known_args(*args, **kwargs)
         if unknown_args and not parsed_args._allow_unknown_args:
             msg = _('unrecognized arguments: %s')
             self.error(msg % ' '.join(unknown_args))
         self.__unknown_args = unknown_args
         return parsed_args
 
-    def exec_subcommands(self, parsed_args: object = None):
+    def exec_subcommands(self, parsed_args: Optional[_InternalSubcmdArgs] = None):
         if not parsed_args:
             parsed_args = self.parse_args()
 
         if parsed_args._allow_unknown_args:
             parsed_args._func(parsed_args, unknown_args=self.__unknown_args)
         else:
             parsed_args._func(parsed_args)
@@ -205,30 +223,31 @@
 
     def on_parser_init(self, parser: SubcommandParser):
         raise NotImplementedError
 
     def on_command(self, args, unknown_args=None):
         raise NotImplementedError
 
-    def _register(self, subparsers, parents: List[argparse.ArgumentParser] = None):
-        kwargs = {'help': self.help}
+    def _register(self, subparsers: argparse._SubParsersAction, parents: Optional[List[argparse.ArgumentParser]] = None):
+        kwargs: dict[str, Any] = {'help': self.help}
         if parents:
             kwargs['parents'] = parents
 
         self.parser = subparsers.add_parser(self.name, **kwargs)
         self.parser.__class__ = SubcommandParser
+        assert isinstance(self.parser, SubcommandParser)
         self.parser.parent_shared_parsers = parents
         self.on_parser_init(self.parser)
         self.parser._register_subcommands()
         self.parser.set_defaults(
             _func=self.on_command,
             _allow_unknown_args=self.parser.allow_unknown_args,
         )
 
-    def __init__(self, subparsers = None, name: str = None, help: str = '', dependency: Union[str, List[str]] = ''):
+    def __init__(self, subparsers: Optional[argparse._SubParsersAction] = None, name: Optional[str] = None, help: str = '', dependency: Union[str, List[str]] = ''):
         self.name = name if name else type(self).__name__.lower()
         self.help = help
         if subparsers:
             self._register(subparsers)
 
     @classmethod
     def exec(cls, *args, **kwargs):
```

### Comparing `subcmdparse-0.1.6/tests/test_subcommand.py` & `subcmdparse-0.1.7/tests/test_subcommand.py`

 * *Files identical despite different names*

