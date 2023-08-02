# Comparing `tmp/springs-1.9.0.tar.gz` & `tmp/springs-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "springs-1.9.0.tar", last modified: Fri Dec  2 07:47:36 2022, max compression
+gzip compressed data, was "springs-1.9.1.tar", last modified: Sat Dec  3 05:42:16 2022, max compression
```

## Comparing `springs-1.9.0.tar` & `springs-1.9.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-12-02 07:47:36.759864 springs-1.9.0/
--rw-r--r--   0 lucas      (502) staff       (20)     1070 2022-03-07 20:55:39.000000 springs-1.9.0/LICENSE
--rw-r--r--   0 lucas      (502) staff       (20)     9348 2022-12-02 07:47:36.759625 springs-1.9.0/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)     8334 2022-09-16 04:34:18.000000 springs-1.9.0/README.md
--rw-r--r--   0 lucas      (502) staff       (20)     2337 2022-12-02 06:56:45.000000 springs-1.9.0/pyproject.toml
--rw-r--r--   0 lucas      (502) staff       (20)       38 2022-12-02 07:47:36.759909 springs-1.9.0/setup.cfg
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-12-02 07:47:36.755507 springs-1.9.0/src/
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-12-02 07:47:36.758572 springs-1.9.0/src/springs/
--rw-r--r--   0 lucas      (502) staff       (20)     1621 2022-12-02 06:39:40.000000 springs-1.9.0/src/springs/__init__.py
--rw-r--r--   0 lucas      (502) staff       (20)      244 2022-12-02 07:37:05.000000 springs-1.9.0/src/springs/__main__.py
--rw-r--r--   0 lucas      (502) staff       (20)    14924 2022-12-02 07:46:43.000000 springs-1.9.0/src/springs/commandline.py
--rw-r--r--   0 lucas      (502) staff       (20)    11253 2022-10-15 00:07:30.000000 springs-1.9.0/src/springs/core.py
--rw-r--r--   0 lucas      (502) staff       (20)     3083 2022-09-20 21:59:49.000000 springs-1.9.0/src/springs/flexyclasses.py
--rw-r--r--   0 lucas      (502) staff       (20)    17916 2022-10-19 00:27:14.000000 springs-1.9.0/src/springs/initialize.py
--rw-r--r--   0 lucas      (502) staff       (20)     6057 2022-11-02 19:26:25.000000 springs-1.9.0/src/springs/logging.py
--rw-r--r--   0 lucas      (502) staff       (20)     4315 2022-11-02 22:01:14.000000 springs-1.9.0/src/springs/memoizer.py
--rw-r--r--   0 lucas      (502) staff       (20)     3962 2022-12-02 07:37:19.000000 springs-1.9.0/src/springs/nicknames.py
--rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-04 06:00:03.000000 springs-1.9.0/src/springs/py.typed
--rw-r--r--   0 lucas      (502) staff       (20)     5324 2022-12-02 06:56:30.000000 springs-1.9.0/src/springs/resolvers.py
--rw-r--r--   0 lucas      (502) staff       (20)     8584 2022-12-02 07:45:40.000000 springs-1.9.0/src/springs/rich_utils.py
--rw-r--r--   0 lucas      (502) staff       (20)     2705 2022-12-02 07:45:48.000000 springs-1.9.0/src/springs/shortcuts.py
--rw-r--r--   0 lucas      (502) staff       (20)     5359 2022-10-19 01:45:48.000000 springs-1.9.0/src/springs/traversal.py
--rw-r--r--   0 lucas      (502) staff       (20)     7592 2022-12-02 06:25:03.000000 springs-1.9.0/src/springs/types_utils.py
--rw-r--r--   0 lucas      (502) staff       (20)     3929 2022-10-20 21:04:50.000000 springs-1.9.0/src/springs/utils.py
-drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-12-02 07:47:36.759388 springs-1.9.0/src/springs.egg-info/
--rw-r--r--   0 lucas      (502) staff       (20)     9348 2022-12-02 07:47:36.000000 springs-1.9.0/src/springs.egg-info/PKG-INFO
--rw-r--r--   0 lucas      (502) staff       (20)      597 2022-12-02 07:47:36.000000 springs-1.9.0/src/springs.egg-info/SOURCES.txt
--rw-r--r--   0 lucas      (502) staff       (20)        1 2022-12-02 07:47:36.000000 springs-1.9.0/src/springs.egg-info/dependency_links.txt
--rw-r--r--   0 lucas      (502) staff       (20)      296 2022-12-02 07:47:36.000000 springs-1.9.0/src/springs.egg-info/requires.txt
--rw-r--r--   0 lucas      (502) staff       (20)        8 2022-12-02 07:47:36.000000 springs-1.9.0/src/springs.egg-info/top_level.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-12-03 05:42:16.411812 springs-1.9.1/
+-rw-r--r--   0 lucas      (502) staff       (20)     1070 2022-03-07 20:55:39.000000 springs-1.9.1/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)     9348 2022-12-03 05:42:16.411606 springs-1.9.1/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     8334 2022-09-16 04:34:18.000000 springs-1.9.1/README.md
+-rw-r--r--   0 lucas      (502) staff       (20)     2337 2022-12-03 05:40:46.000000 springs-1.9.1/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2022-12-03 05:42:16.411859 springs-1.9.1/setup.cfg
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-12-03 05:42:16.403512 springs-1.9.1/src/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-12-03 05:42:16.410066 springs-1.9.1/src/springs/
+-rw-r--r--   0 lucas      (502) staff       (20)     1621 2022-12-03 05:30:40.000000 springs-1.9.1/src/springs/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      244 2022-12-02 07:37:05.000000 springs-1.9.1/src/springs/__main__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    15280 2022-12-03 05:40:39.000000 springs-1.9.1/src/springs/commandline.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11253 2022-10-15 00:07:30.000000 springs-1.9.1/src/springs/core.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3478 2022-12-03 05:40:40.000000 springs-1.9.1/src/springs/flexyclasses.py
+-rw-r--r--   0 lucas      (502) staff       (20)    17916 2022-10-19 00:27:14.000000 springs-1.9.1/src/springs/initialize.py
+-rw-r--r--   0 lucas      (502) staff       (20)     6057 2022-11-02 19:26:25.000000 springs-1.9.1/src/springs/logging.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4315 2022-11-02 22:01:14.000000 springs-1.9.1/src/springs/memoizer.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4184 2022-12-03 05:40:40.000000 springs-1.9.1/src/springs/nicknames.py
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2022-09-04 06:00:03.000000 springs-1.9.1/src/springs/py.typed
+-rw-r--r--   0 lucas      (502) staff       (20)     5324 2022-12-02 06:56:30.000000 springs-1.9.1/src/springs/resolvers.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8584 2022-12-02 07:45:40.000000 springs-1.9.1/src/springs/rich_utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2705 2022-12-02 07:45:48.000000 springs-1.9.1/src/springs/shortcuts.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5359 2022-10-19 01:45:48.000000 springs-1.9.1/src/springs/traversal.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7592 2022-12-02 06:25:03.000000 springs-1.9.1/src/springs/types_utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3929 2022-10-20 21:04:50.000000 springs-1.9.1/src/springs/utils.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2022-12-03 05:42:16.411347 springs-1.9.1/src/springs.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     9348 2022-12-03 05:42:16.000000 springs-1.9.1/src/springs.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)      597 2022-12-03 05:42:16.000000 springs-1.9.1/src/springs.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2022-12-03 05:42:16.000000 springs-1.9.1/src/springs.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)      296 2022-12-03 05:42:16.000000 springs-1.9.1/src/springs.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        8 2022-12-03 05:42:16.000000 springs-1.9.1/src/springs.egg-info/top_level.txt
```

### Comparing `springs-1.9.0/LICENSE` & `springs-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/PKG-INFO` & `springs-1.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: springs
-Version: 1.9.0
+Version: 1.9.1
 Summary: A set of utilities to create and manage typed configuration files effectively, built on top of OmegaConf.
 Author-email: Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://springs.soldaini.net
 Project-URL: Repository, https://github.com/soldni/Springs
 Project-URL: Bug Tracker, https://github.com/soldni/Springs/issues
 Keywords: configuration,yaml,json,command line,cli,omegaconf,structured,config
```

### Comparing `springs-1.9.0/README.md` & `springs-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/pyproject.toml` & `springs-1.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "springs"
-version = "1.9.0"
+version = "1.9.1"
 description = "A set of utilities to create and manage typed configuration files effectively, built on top of OmegaConf."
 authors = [
     {name = "Luca Soldaini", email = "luca@soldaini.net" }
 ]
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `springs-1.9.0/src/springs/__init__.py` & `springs-1.9.1/src/springs/__init__.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/commandline.py` & `springs-1.9.1/src/springs/commandline.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     from_file,
     from_none,
     from_options,
     merge,
     to_yaml,
     unsafe_merge,
 )
+from .flexyclasses import is_flexyclass
 from .logging import configure_logging
 from .nicknames import NicknameRegistry
 from .rich_utils import (
     RichArgumentParser,
     add_pretty_traceback,
     print_config_as_tree,
     print_table,
@@ -256,16 +257,25 @@
         # strip leading and trailing curly braces
         config_path_or_nickname = config_path_or_nickname[1:-1]
 
         # config file is to load from nicknames
         loaded_config = NicknameRegistry.get(
             name=config_path_or_nickname, raise_if_missing=True
         )
-        if not isinstance(loaded_config, (DictConfig, ListConfig)):
+
+        if is_dataclass(loaded_config):
             loaded_config = from_dataclass(loaded_config)
+        elif is_flexyclass(loaded_config):
+            loaded_config = loaded_config.to_dict_config()  # type: ignore
+        elif not isinstance(loaded_config, (DictConfig, ListConfig)):
+            raise ValueError(
+                f"Nickname '{config_path_or_nickname}' is not a "
+                "DictConfig or ListConfig."
+            )
+
     else:
         # config file is to load from file
         loaded_config = from_file(config_path_or_nickname)
 
     return loaded_config
```

### Comparing `springs-1.9.0/src/springs/core.py` & `springs-1.9.1/src/springs/core.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/flexyclasses.py` & `springs-1.9.1/src/springs/flexyclasses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from copy import deepcopy
 from dataclasses import MISSING as DT_MISSING
 from dataclasses import Field, field, fields, is_dataclass
 from typing import Any, Dict, Generic, Type, TypeVar
 
 from omegaconf import MISSING as OC_MISSING
+from omegaconf import DictConfig
 from typing_extensions import dataclass_transform
 
 from .utils import get_annotations
 
 C = TypeVar("C", bound=Any)
 
 
@@ -58,14 +59,21 @@
         # We completely change how the constructor works to allow users
         # to use flexyclasses in the same way they would use a dataclass.
         factory_dict: Dict[str, Any] = {}
         factory_dict = {**cls.defaults(), **kwargs}
         return field(default_factory=lambda: factory_dict)
 
     @classmethod
+    def to_dict_config(cls, **kwargs: Any) -> DictConfig:
+        """Convert the FlexyClass to an OmegaConf DictConfig object"""
+        from .core import from_dict
+
+        return from_dict({**cls.defaults(), **kwargs})
+
+    @classmethod
     def flexyclass(cls, target_cls: Type[C]) -> Type["FlexyClass"]:
         """Decorator to create a FlexyClass from a class"""
 
         if is_dataclass(target_cls):
             attributes_iterator = ((f.name, f) for f in fields(target_cls))
         else:
             attributes_iterator = (
@@ -85,7 +93,12 @@
         )
 
 
 @dataclass_transform()
 def flexyclass(cls: Type[C]) -> Type[FlexyClass[C]]:
     """Alias for FlexyClass.flexyclass"""
     return FlexyClass.flexyclass(cls)
+
+
+def is_flexyclass(obj: Any) -> bool:
+    """Check if an object is a FlexyClass"""
+    return isinstance(obj, FlexyClass)
```

### Comparing `springs-1.9.0/src/springs/initialize.py` & `springs-1.9.1/src/springs/initialize.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/logging.py` & `springs-1.9.1/src/springs/logging.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/memoizer.py` & `springs-1.9.1/src/springs/memoizer.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/nicknames.py` & `springs-1.9.1/src/springs/nicknames.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 from dataclasses import is_dataclass
+from inspect import isclass
 from pathlib import Path
 from typing import (
     Any,
     Callable,
     Dict,
     Literal,
     Optional,
     Sequence,
     Set,
     Tuple,
     Type,
     TypeVar,
     Union,
+    cast,
     overload,
 )
 
 from omegaconf import DictConfig, ListConfig
 
 from .core import from_file
+from .flexyclasses import FlexyClass
 from .logging import configure_logging
 
-RegistryValue = Union[Type[Any], DictConfig, ListConfig]
+RegistryValue = Union[Type[Any], Type[FlexyClass], DictConfig, ListConfig]
 
 T = TypeVar("T")
 M = TypeVar("M", bound=RegistryValue)
 
 LOGGER = configure_logging(__name__)
 
 
@@ -88,20 +91,24 @@
 
     @classmethod
     def add(cls, name: str) -> Callable[[Type[T]], Type[T]]:
         """Decorator to save a structured configuration with a nickname
         for easy reuse."""
 
         def add_to_registry(cls_: Type[T]) -> Type[T]:
-            if not is_dataclass(cls_):
+            if not (
+                is_dataclass(cls_)
+                or isclass(cls_)
+                and issubclass(cls_, FlexyClass)
+            ):
                 raise ValueError(f"{cls_} must be a dataclass")
 
             if name in cls.__registry__:
                 raise ValueError(f"{name} is already registered")
-            return cls._add(name, cls_)
+            return cast(Type[T], cls._add(name, cls_))
 
         return add_to_registry
 
     @overload
     @classmethod
     def get(
         cls, name: str, raise_if_missing: Literal[True] = True
```

### Comparing `springs-1.9.0/src/springs/resolvers.py` & `springs-1.9.1/src/springs/resolvers.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/rich_utils.py` & `springs-1.9.1/src/springs/rich_utils.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/shortcuts.py` & `springs-1.9.1/src/springs/shortcuts.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/traversal.py` & `springs-1.9.1/src/springs/traversal.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/types_utils.py` & `springs-1.9.1/src/springs/types_utils.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs/utils.py` & `springs-1.9.1/src/springs/utils.py`

 * *Files identical despite different names*

### Comparing `springs-1.9.0/src/springs.egg-info/PKG-INFO` & `springs-1.9.1/src/springs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: springs
-Version: 1.9.0
+Version: 1.9.1
 Summary: A set of utilities to create and manage typed configuration files effectively, built on top of OmegaConf.
 Author-email: Luca Soldaini <luca@soldaini.net>
 License: Apache-2.0
 Project-URL: Homepage, https://springs.soldaini.net
 Project-URL: Repository, https://github.com/soldni/Springs
 Project-URL: Bug Tracker, https://github.com/soldni/Springs/issues
 Keywords: configuration,yaml,json,command line,cli,omegaconf,structured,config
```

### Comparing `springs-1.9.0/src/springs.egg-info/SOURCES.txt` & `springs-1.9.1/src/springs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

