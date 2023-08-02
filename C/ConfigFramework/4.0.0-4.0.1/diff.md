# Comparing `tmp/ConfigFramework-4.0.0.tar.gz` & `tmp/ConfigFramework-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConfigFramework-4.0.0.tar", last modified: Tue Aug  1 19:26:14 2023, max compression
+gzip compressed data, was "ConfigFramework-4.0.1.tar", last modified: Wed Aug  2 11:42:47 2023, max compression
```

## Comparing `ConfigFramework-4.0.0.tar` & `ConfigFramework-4.0.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.514429 ConfigFramework-4.0.0/ConfigFramework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-01 19:26:14.000000 ConfigFramework-4.0.0/ConfigFramework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.514429 ConfigFramework-4.0.0/config_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.514429 ConfigFramework-4.0.0/config_framework/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/json_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/toml_full_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/toml_read_only.py
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/loaders/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.514429 ConfigFramework-4.0.0/config_framework/types/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/config_framework/types/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/abstract/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/custom_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/types/variable_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/config_framework/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/utils/loader_specific_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/config_framework/utils/loader_specific_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 19:26:14.518429 ConfigFramework-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-01 19:25:57.000000 ConfigFramework-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.667655 ConfigFramework-4.0.1/ConfigFramework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.667655 ConfigFramework-4.0.1/config_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.667655 ConfigFramework-4.0.1/config_framework/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/json_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/toml_full_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/toml_read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.667655 ConfigFramework-4.0.1/config_framework/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/config_framework/types/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/abstract/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/custom_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/variable_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/config_framework/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/utils/loader_specific_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/utils/loader_specific_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/setup.py
```

### Comparing `ConfigFramework-4.0.0/ConfigFramework.egg-info/PKG-INFO` & `ConfigFramework-4.0.1/ConfigFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConfigFramework
-Version: 4.0.0
+Version: 4.0.1
 Summary: A small framework to build your flexible project configurations
 Home-page: https://github.com/Rud356/ConfigFramework
 Author: Rud356
 Author-email: Rud356 <rud356github@gmail.com>
 License: MIT License
 Keywords: config,configuration,config managment,configuration managment
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ConfigFramework-4.0.0/ConfigFramework.egg-info/SOURCES.txt` & `ConfigFramework-4.0.1/ConfigFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/LICENSE` & `ConfigFramework-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/PKG-INFO` & `ConfigFramework-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConfigFramework
-Version: 4.0.0
+Version: 4.0.1
 Summary: A small framework to build your flexible project configurations
 Home-page: https://github.com/Rud356/ConfigFramework
 Author: Rud356
 Author-email: Rud356 <rud356github@gmail.com>
 License: MIT License
 Keywords: config,configuration,config managment,configuration managment
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ConfigFramework-4.0.0/README.md` & `ConfigFramework-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/config_framework/loaders/composite.py` & `ConfigFramework-4.0.1/config_framework/loaders/composite.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,21 @@
         self.loaders = loaders
 
     @classmethod
     def load(
         cls, *loaders: AbstractLoader,
         defaults: Optional[MutableMapping[str, Any]] = None
     ):
+        """
+        Initializes composite loader.
+
+        :param loaders: any number of different config sources that can be used for providing configuration.
+        :param defaults: default values.
+        :return: instance of composite loader.
+        """
         return cls(
             data=ChainMap(*loaders),
             defaults=defaults or {},
             loaders=loaders
         )
 
     def dump(self, include_defaults: bool = False) -> None:
```

### Comparing `ConfigFramework-4.0.0/config_framework/loaders/dict.py` & `ConfigFramework-4.0.1/config_framework/loaders/env.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from os import environ
 from typing import Optional, MutableMapping, Any
 
 from config_framework.types.abstract import AbstractLoader
 
 
-class Dict(AbstractLoader):
+class Environment(AbstractLoader):
     @classmethod
-    def load(
-        cls, data: MutableMapping[str, Any],
-        defaults: Optional[MutableMapping[str, Any]] = None
-    ):
-        return cls(data=data, defaults=defaults or {})
+    def load(cls, defaults: Optional[MutableMapping[str, Any]] = None):
+        """
+        Loads data from environment.
+
+        :param defaults: default values.
+        :return: instance of env loader.
+        """
+        return cls(data=dict(environ), defaults=defaults or {})
 
     def dump(self, include_defaults: bool = False) -> None:
         """
-        This method doesn't changes anything since dict is updated whenever
-        values are changed.
+        This method doesn't change env variables at all
+        because not many types, convert properly into string env variable
+        and can be loaded back.
 
         :param include_defaults: specifies if
             you want to have default variables to be dumped.
         :return: nothing.
         """
         pass
```

### Comparing `ConfigFramework-4.0.0/config_framework/loaders/json.py` & `ConfigFramework-4.0.1/config_framework/loaders/json.py`

 * *Files 18% similar despite different names*

```diff
@@ -31,14 +31,24 @@
     def load(
         cls, path: Union[PathLike, Path],
         defaults: Optional[MutableMapping[str, Any]] = None,
         encoding: str = "utf8",
         json_loader=json.load,
         json_dumper=partial(json.dump, ensure_ascii=False, indent=4),
     ):
+        """
+        Loads json file from path into loader.
+
+        :param path: where file with json is located.
+        :param defaults: default values.
+        :param encoding: which encoding does config file has (defaults to utf-8).
+        :param json_loader: function that loads json file.
+        :param json_dumper: function that dumps to json file.
+        :return: instance of json loader.
+        """
         with open(path, encoding=encoding) as data_f:
             data = json_loader(data_f)
 
         return cls(
             data=data, defaults=defaults or {},
             path=path, encoding=encoding,
             json_loader=json_loader, json_dumper=json_dumper
```

### Comparing `ConfigFramework-4.0.0/config_framework/loaders/json_string.py` & `ConfigFramework-4.0.1/config_framework/loaders/json_string.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,24 +26,34 @@
         cls,
         data_string: str,
         encoding: str = "utf8",
         defaults: Optional[MutableMapping[str, Any]] = None,
         json_loader=json.loads,
         json_dumper=partial(json.dumps, ensure_ascii=False, indent=4),
     ):
+        """
+        Loads json file from path into loader.
+
+        :param data_string: string with valid json formatted text.
+        :param defaults: default values.
+        :param encoding: which encoding does config file has (defaults to utf-8).
+        :param json_loader: function that loads json from string.
+        :param json_dumper: function that dumps to json string.
+        :return: instance of json string loader.
+        """
         data = json_loader(data_string)
 
         return cls(
             data=data, defaults=defaults or {}, encoding=encoding,
             json_loader=json_loader, json_dumper=json_dumper
         )
 
     def dump(self, include_defaults: bool = False) -> None:
         """
-        This method doesn't changes anything at all
+        This method doesn't change anything at all
         because strings are unchangeable.
 
         :param include_defaults: specifies if
             you want to have default variables to be dumped.
         :return: nothing.
         """
         pass
```

### Comparing `ConfigFramework-4.0.0/config_framework/loaders/toml_full_features.py` & `ConfigFramework-4.0.1/config_framework/loaders/toml_full_features.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,18 +33,16 @@
         encoding: str = "utf8",
     ):
         """
         Initializes loader for read only toml.
 
         :param path: path that is used to load config.
         :param defaults: default values.
-        :param loader_kwargs: used for specifying parameters, according to
-        tomls' documentation of `toml.load` function.
-        :param dumper_kwargs: used for specifying parameters, according to
-        tomls' documentation of `toml.dump` function.
+        :param loader_kwargs: used for specifying parameters, according to toml documentation of `toml.load` function.
+        :param dumper_kwargs: used for specifying parameters, according to toml documentation of `toml.dump` function.
         :param encoding: which encoding should be used for a file.
         :return: instance of TomlReadOnly class.
         """
         with open(path, encoding=encoding) as data_f:
             data = toml_loader_lib.load(data_f)
 
         if loader_kwargs is None:
```

### Comparing `ConfigFramework-4.0.0/config_framework/loaders/toml_read_only.py` & `ConfigFramework-4.0.1/config_framework/loaders/toml_read_only.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,18 +36,20 @@
         encoding: str = "utf8",
     ):
         """
         Initializes loader for read only toml.
 
         :param path: path that is used to load config.
         :param defaults: default values.
-        :param loader_kwargs: used for specifying parameters, according to
-        tomllibs' documentation of `tomllib.load` function.
+        :param loader_kwargs: used for specifying parameters, according to tomllib documentation of `tomllib.load`
+            function.
+
         :param dumper_kwargs: not used.
         :param encoding: which encoding should be used for a file.
+
         :return: instance of TomlReadOnly class.
         """
         with open(path, encoding=encoding, mode="b") as data_f:
             data = toml_loader_lib.load(data_f)
 
         if loader_kwargs is None:
             loader_kwargs = dict()
```

### Comparing `ConfigFramework-4.0.0/config_framework/loaders/yaml.py` & `ConfigFramework-4.0.1/config_framework/loaders/yaml.py`

 * *Files 14% similar despite different names*

```diff
@@ -39,14 +39,24 @@
     def load(
         cls, path: Union[PathLike, Path],
         defaults: Optional[MutableMapping[str, Any]] = None,
         encoding: str = "utf8",
         yaml_loader=partial(yaml.load, Loader=Loader),
         yaml_dumper=partial(yaml.dump, Dumper=Dumper),
     ):
+        """
+        Loads yaml from file.
+
+        :param path: where is yaml file to load data from.
+        :param defaults: default values for config.
+        :param encoding: which encoding does config file has (defaults to utf-8).
+        :param yaml_loader: function that is used for loading data from file.
+        :param yaml_dumper: function that is used for saving data to file.
+        :return: instance of yaml loader.
+        """
         with open(path, encoding=encoding) as data_f:
             data = yaml_loader(data_f)
 
         return cls(
             data=data, defaults=defaults or {},
             path=path, encoding=encoding,
             yaml_loader=yaml_loader,
```

### Comparing `ConfigFramework-4.0.0/config_framework/types/abstract/loader.py` & `ConfigFramework-4.0.1/config_framework/types/abstract/loader.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/config_framework/types/config.py` & `ConfigFramework-4.0.1/config_framework/types/config.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/config_framework/types/variable.py` & `ConfigFramework-4.0.1/config_framework/types/variable.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/config_framework/types/variable_key.py` & `ConfigFramework-4.0.1/config_framework/types/variable_key.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/config_framework/utils/loader_specific_deserializer.py` & `ConfigFramework-4.0.1/config_framework/utils/loader_specific_deserializer.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/config_framework/utils/loader_specific_serializer.py` & `ConfigFramework-4.0.1/config_framework/utils/loader_specific_serializer.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/pyproject.toml` & `ConfigFramework-4.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.0/setup.py` & `ConfigFramework-4.0.1/setup.py`

 * *Files identical despite different names*

