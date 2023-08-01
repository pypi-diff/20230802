# Comparing `tmp/skeletonkey-0.1.2.tar.gz` & `tmp/skeletonkey-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skeletonkey-0.1.2.tar", last modified: Fri Jun 23 21:42:25 2023, max compression
+gzip compressed data, was "skeletonkey-0.1.3.tar", last modified: Tue Aug  1 22:12:10 2023, max compression
```

## Comparing `skeletonkey-0.1.2.tar` & `skeletonkey-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 21:42:25.239363 skeletonkey-0.1.2/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.2/LICENSE
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-06-23 21:42:25.219362 skeletonkey-0.1.2/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.2/README.md
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-06-23 21:42:25.251364 skeletonkey-0.1.2/setup.cfg
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      758 2023-06-23 21:40:28.000000 skeletonkey-0.1.2/setup.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 21:42:24.711337 skeletonkey-0.1.2/skeletonkey/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      562 2023-05-01 04:36:26.000000 skeletonkey-0.1.2/skeletonkey/__init__.py
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)    10442 2023-06-23 19:57:18.000000 skeletonkey-0.1.2/skeletonkey/config.py
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4691 2023-06-23 21:37:29.000000 skeletonkey-0.1.2/skeletonkey/core.py
-drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-06-23 21:42:25.123357 skeletonkey-0.1.2/skeletonkey.egg-info/
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-06-23 21:42:22.000000 skeletonkey-0.1.2/skeletonkey.egg-info/PKG-INFO
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      266 2023-06-23 21:42:23.000000 skeletonkey-0.1.2/skeletonkey.egg-info/SOURCES.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-06-23 21:42:22.000000 skeletonkey-0.1.2/skeletonkey.egg-info/dependency_links.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       14 2023-06-23 21:42:22.000000 skeletonkey-0.1.2/skeletonkey.egg-info/requires.txt
--rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-06-23 21:42:22.000000 skeletonkey-0.1.2/skeletonkey.egg-info/top_level.txt
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-01 22:12:10.302878 skeletonkey-0.1.3/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     1071 2023-05-01 03:35:36.000000 skeletonkey-0.1.3/LICENSE
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-08-01 22:12:10.290877 skeletonkey-0.1.3/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     3814 2023-05-01 05:00:51.000000 skeletonkey-0.1.3/README.md
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       38 2023-08-01 22:12:10.322878 skeletonkey-0.1.3/setup.cfg
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      758 2023-08-01 22:12:04.000000 skeletonkey-0.1.3/setup.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-01 22:12:09.830856 skeletonkey-0.1.3/skeletonkey/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      598 2023-08-01 22:00:42.000000 skeletonkey-0.1.3/skeletonkey/__init__.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)    11332 2023-08-01 22:00:42.000000 skeletonkey-0.1.3/skeletonkey/config.py
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     6133 2023-08-01 22:00:42.000000 skeletonkey-0.1.3/skeletonkey/core.py
+drwxr-xr-x   0 sizemol  (77241) grp.csci.Faculty (71145)        0 2023-08-01 22:12:10.214873 skeletonkey-0.1.3/skeletonkey.egg-info/
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)     4304 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/PKG-INFO
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)      266 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/SOURCES.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)        1 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/dependency_links.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       14 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/requires.txt
+-rw-r--r--   0 sizemol  (77241) grp.csci.Faculty (71145)       12 2023-08-01 22:12:07.000000 skeletonkey-0.1.3/skeletonkey.egg-info/top_level.txt
```

### Comparing `skeletonkey-0.1.2/LICENSE` & `skeletonkey-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.2/PKG-INFO` & `skeletonkey-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.1.2
+Version: 0.1.3
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `skeletonkey-0.1.2/README.md` & `skeletonkey-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `skeletonkey-0.1.2/setup.py` & `skeletonkey-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="skeletonkey",
-    version="0.1.2",
+    version="0.1.3",
     description="A bare-bones configuration managment tool.",
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sizemore0125/skeletonkey",
     author="Logan Sizemore",
     author_email="sizemore0125@gmail.com",
```

### Comparing `skeletonkey-0.1.2/skeletonkey/__init__.py` & `skeletonkey-0.1.3/skeletonkey/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,11 +6,11 @@
 and an instantiate funtion that can dynamically instantiate classes with their configurations. 
 It facilitates the management of complex configurations for applications using YAML files and enables 
 the dynamic loading of classes and their arguments at runtime.
 """
 
 __version__ = "0.0.11"
 
-from .core import unlock, instantiate
+from .core import unlock, instantiate, instantiate_all
 
 # Names to import with wildcard import
-__all__ = ["unlock", "instantiate"]
+__all__ = ["unlock", "instantiate", "instantiate_all"]
```

### Comparing `skeletonkey-0.1.2/skeletonkey/config.py` & `skeletonkey-0.1.3/skeletonkey/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 This code provides a set of utility functions to handle YAML configurations. 
 It facilitates the management of complex configurations for applications using YAML 
 files and enables the dynamic loading of classes and their arguments at runtime.
 """
 
 import argparse
-import inspect
 import os
 from typing import List
 
 import yaml
 
 
 def find_yaml_path(file_path: str) -> str:
@@ -55,15 +54,15 @@
         dict: A dictionary representing the YAML content.
     """
     path = find_yaml_path(path)
     with open(os.path.expanduser(path), "r") as handle:
         return yaml.safe_load(handle)
 
 
-def dict_to_path(dictionary: dict, parent_key="", sep="/") -> List[str]:
+def dict_to_path(dictionary: dict, parent_key="") -> List[str]:
     """
     Flatten a nested dictionary into a single-level dictionary by concatenating
     nested keys using a specified separator.
 
     Args:
         dictionary (dict): The nested dictionary to be flattened.
         parent_key (str): The initial parent key, default is an empty string.
@@ -168,15 +167,15 @@
     default_yaml = add_yaml_extension(default_yaml)
     default_config_path = os.path.join(config_path, default_yaml)
     default_config = open_yaml(default_config_path)
     return default_config
 
 
 def load_yaml_config(
-    config_path: str, config_name: str, default_keyword: str = "defaults"
+    config_path: str, config_name: str, default_keyword: str = "defaults", collection_keyword: str = "keyring"
 ) -> dict:
     """
     Load a YAML configuration file and update it with default configurations.
 
     Args:
         config_path (str): The file path to the YAML configuration file.
         config_name (str): The name of the YAML configuration file.
@@ -216,14 +215,28 @@
                     config.update(
                         (key, value)
                         for key, value in default_config.items()
                         if key not in config
                     )
         del config[default_keyword]
 
+    if collection_keyword in config:
+        collections_dict = config[collection_keyword]
+        for collection_key in collections_dict.keys():
+
+            if collection_key in config:
+                return ValueError("You cannot have a collection with the same name as an argument.")
+
+            collection_dict = collections_dict[collection_key]
+            config[collection_key] = {}
+            for subconfig_key in collection_dict.keys():
+                subconfig = get_default_args_from_path(config_path, collection_dict[subconfig_key])
+                config[collection_key].update({subconfig_key : subconfig})
+        del config[collection_keyword]
+    
     return config
 
 
 def add_args_from_dict(
     arg_parser: argparse.ArgumentParser, config: dict, prefix=""
 ) -> None:
     """
@@ -237,18 +250,23 @@
                        the arguments and their default values.
         prefix (str, optional): The prefix string for nested keys. Defaults to ''.
     """
     for key, value in config.items():
         if isinstance(value, dict):
             add_args_from_dict(arg_parser, value, f"{prefix}{key}.")
         else:
-            if key.startswith("$") and key[1:] in os.environ:
-                env_var = os.environ[key[1:]]
+            if key.startswith("$"):
+                if key[1:] in os.environ:
+                    value = os.environ[key[1:]]
                 arg_parser.add_argument(
-                    f"--{prefix}{key[1:]}", default=env_var, type=type(env_var)
+                    f"--{prefix}{key[1:]}", default=value, type=type(value)
+                )
+            elif key.startswith("?"):
+                arg_parser.add_argument(
+                    f"--{prefix}{key[1:]}", default=value, action='store_true'
                 )
             else:
                 arg_parser.add_argument(
                     f"--{prefix}{key}", default=value, type=type(value)
                 )
```

### Comparing `skeletonkey-0.1.2/skeletonkey.egg-info/PKG-INFO` & `skeletonkey-0.1.3/skeletonkey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skeletonkey
-Version: 0.1.2
+Version: 0.1.3
 Summary: A bare-bones configuration managment tool.
 Home-page: https://github.com/sizemore0125/skeletonkey
 Author: Logan Sizemore
 Author-email: sizemore0125@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

