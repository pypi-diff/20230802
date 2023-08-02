# Comparing `tmp/ConfigFramework-4.0.1.tar.gz` & `tmp/ConfigFramework-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ConfigFramework-4.0.1.tar", last modified: Wed Aug  2 11:42:47 2023, max compression
+gzip compressed data, was "ConfigFramework-4.0.2.tar", last modified: Wed Aug  2 12:15:50 2023, max compression
```

## Comparing `ConfigFramework-4.0.1.tar` & `ConfigFramework-4.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.667655 ConfigFramework-4.0.1/ConfigFramework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 11:42:47.000000 ConfigFramework-4.0.1/ConfigFramework.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.667655 ConfigFramework-4.0.1/config_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.667655 ConfigFramework-4.0.1/config_framework/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/composite.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/dict.py
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/env.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/json_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/toml_full_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/toml_read_only.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/loaders/yaml.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.667655 ConfigFramework-4.0.1/config_framework/types/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/config_framework/types/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/abstract/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/custom_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/types/variable_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/config_framework/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/utils/loader_specific_deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/config_framework/utils/loader_specific_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:42:47.671655 ConfigFramework-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-02 11:42:27.000000 ConfigFramework-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/ConfigFramework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-02 12:15:50.000000 ConfigFramework-4.0.2/ConfigFramework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-08-02 12:15:50.000000 ConfigFramework-4.0.2/ConfigFramework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:15:50.000000 ConfigFramework-4.0.2/ConfigFramework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-08-02 12:15:50.000000 ConfigFramework-4.0.2/ConfigFramework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 12:15:50.000000 ConfigFramework-4.0.2/ConfigFramework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6143 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5171 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/config_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/config_framework/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/composite.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      860 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/json_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/toml_full_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/toml_read_only.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/loaders/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/config_framework/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/config_framework/types/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/types/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5522 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/types/abstract/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/types/custom_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9621 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/types/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/types/variable_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/config_framework/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/utils/loader_specific_deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/config_framework/utils/loader_specific_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:15:50.350354 ConfigFramework-4.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-08-02 12:15:33.000000 ConfigFramework-4.0.2/setup.py
```

### Comparing `ConfigFramework-4.0.1/ConfigFramework.egg-info/PKG-INFO` & `ConfigFramework-4.0.2/ConfigFramework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConfigFramework
-Version: 4.0.1
+Version: 4.0.2
 Summary: A small framework to build your flexible project configurations
 Home-page: https://github.com/Rud356/ConfigFramework
 Author: Rud356
 Author-email: Rud356 <rud356github@gmail.com>
 License: MIT License
 Keywords: config,configuration,config managment,configuration managment
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ConfigFramework-4.0.1/ConfigFramework.egg-info/SOURCES.txt` & `ConfigFramework-4.0.2/ConfigFramework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/LICENSE` & `ConfigFramework-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/PKG-INFO` & `ConfigFramework-4.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ConfigFramework
-Version: 4.0.1
+Version: 4.0.2
 Summary: A small framework to build your flexible project configurations
 Home-page: https://github.com/Rud356/ConfigFramework
 Author: Rud356
 Author-email: Rud356 <rud356github@gmail.com>
 License: MIT License
 Keywords: config,configuration,config managment,configuration managment
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ConfigFramework-4.0.1/README.md` & `ConfigFramework-4.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/loaders/composite.py` & `ConfigFramework-4.0.2/config_framework/loaders/composite.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/loaders/dict.py` & `ConfigFramework-4.0.2/config_framework/loaders/dict.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/loaders/env.py` & `ConfigFramework-4.0.2/config_framework/loaders/env.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/loaders/json.py` & `ConfigFramework-4.0.2/config_framework/loaders/json.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/loaders/json_string.py` & `ConfigFramework-4.0.2/config_framework/loaders/json_string.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/loaders/toml_full_features.py` & `ConfigFramework-4.0.2/config_framework/loaders/toml_full_features.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/loaders/toml_read_only.py` & `ConfigFramework-4.0.2/config_framework/loaders/toml_read_only.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/loaders/yaml.py` & `ConfigFramework-4.0.2/config_framework/loaders/yaml.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/types/abstract/loader.py` & `ConfigFramework-4.0.2/config_framework/types/abstract/loader.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/types/config.py` & `ConfigFramework-4.0.2/config_framework/types/config.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/types/variable.py` & `ConfigFramework-4.0.2/config_framework/types/variable.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/types/variable_key.py` & `ConfigFramework-4.0.2/config_framework/types/variable_key.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/utils/loader_specific_deserializer.py` & `ConfigFramework-4.0.2/config_framework/utils/loader_specific_deserializer.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/config_framework/utils/loader_specific_serializer.py` & `ConfigFramework-4.0.2/config_framework/utils/loader_specific_serializer.py`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/pyproject.toml` & `ConfigFramework-4.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ConfigFramework-4.0.1/setup.py` & `ConfigFramework-4.0.2/setup.py`

 * *Files identical despite different names*

