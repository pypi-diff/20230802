# Comparing `tmp/discovery-core-0.4.0.tar.gz` & `tmp/discovery-core-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.4.0.tar", last modified: Wed Aug  2 16:52:17 2023, max compression
+gzip compressed data, was "discovery-core-0.4.1.tar", last modified: Wed Aug  2 16:53:42 2023, max compression
```

## Comparing `discovery-core-0.4.0.tar` & `discovery-core-0.4.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.069423 discovery-core-0.4.0/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.4.0/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.4.0/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-02 16:52:17.069629 discovery-core-0.4.0/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.4.0/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.051319 discovery-core-0.4.0/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-02 16:52:16.000000 discovery-core-0.4.0/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-02 16:52:16.000000 discovery-core-0.4.0/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-02 16:52:16.000000 discovery-core-0.4.0/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-02 16:52:16.000000 discovery-core-0.4.0/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.051704 discovery-core-0.4.0/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-08-02 16:45:52.000000 discovery-core-0.4.0/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.052874 discovery-core-0.4.0/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.0/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63432 2023-08-02 16:51:55.000000 discovery-core-0.4.0/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25922 2023-08-01 22:47:24.000000 discovery-core-0.4.0/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.055097 discovery-core-0.4.0/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.0/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.4.0/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.4.0/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.056306 discovery-core-0.4.0/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.0/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.4.0/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.059434 discovery-core-0.4.0/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.0/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.4.0/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.4.0/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.4.0/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-02 16:52:17.070278 discovery-core-0.4.0/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.4.0/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.060369 discovery-core-0.4.0/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.4.0/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.062096 discovery-core-0.4.0/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.0/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.4.0/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20699 2023-08-01 22:48:11.000000 discovery-core-0.4.0/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.064588 discovery-core-0.4.0/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.0/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.4.0/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.4.0/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.066607 discovery-core-0.4.0/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.0/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.4.0/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.4.0/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:52:17.068761 discovery-core-0.4.0/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.0/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.4.0/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.4.0/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.092922 discovery-core-0.4.1/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.4.1/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.4.1/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-02 16:53:42.093353 discovery-core-0.4.1/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.4.1/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.070923 discovery-core-0.4.1/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-02 16:53:41.000000 discovery-core-0.4.1/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-02 16:53:42.000000 discovery-core-0.4.1/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-02 16:53:41.000000 discovery-core-0.4.1/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-02 16:53:41.000000 discovery-core-0.4.1/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.071259 discovery-core-0.4.1/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-08-02 16:53:22.000000 discovery-core-0.4.1/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.073087 discovery-core-0.4.1/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63432 2023-08-02 16:51:55.000000 discovery-core-0.4.1/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25922 2023-08-01 22:47:24.000000 discovery-core-0.4.1/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.075191 discovery-core-0.4.1/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.4.1/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.4.1/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.076175 discovery-core-0.4.1/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.4.1/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.079167 discovery-core-0.4.1/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.4.1/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.4.1/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.4.1/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-02 16:53:42.094467 discovery-core-0.4.1/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.4.1/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.080159 discovery-core-0.4.1/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.4.1/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.082672 discovery-core-0.4.1/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.4.1/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20699 2023-08-01 22:48:11.000000 discovery-core-0.4.1/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.085876 discovery-core-0.4.1/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.4.1/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.4.1/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.088615 discovery-core-0.4.1/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.4.1/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.4.1/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:53:42.091931 discovery-core-0.4.1/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.4.1/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.4.1/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.4.1/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.4.0/LICENSE.txt` & `discovery-core-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/PKG-INFO` & `discovery-core-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.4.0/README.rst` & `discovery-core-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.4.1/discovery_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.4.0
+Version: 0.4.1
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.4.0/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.4.1/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/ds_core/components/abstract_component.py` & `discovery-core-0.4.1/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/ds_core/components/core_commons.py` & `discovery-core-0.4.1/ds_core/components/core_commons.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.4.1/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.4.1/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/ds_core/intent/abstract_intent.py` & `discovery-core-0.4.1/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/ds_core/properties/abstract_properties.py` & `discovery-core-0.4.1/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/ds_core/properties/decorator_patterns.py` & `discovery-core-0.4.1/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/ds_core/properties/property_manager.py` & `discovery-core-0.4.1/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/setup.py` & `discovery-core-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/test/components/abstract_component_test.py` & `discovery-core-0.4.1/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/test/components/commons_test.py` & `discovery-core-0.4.1/test/components/commons_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/test/handlers/connector_contract_test.py` & `discovery-core-0.4.1/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/test/handlers/handler_factory_test.py` & `discovery-core-0.4.1/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/test/intent/abstract_intent_test.py` & `discovery-core-0.4.1/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/test/intent/pyarrow_intent_model.py` & `discovery-core-0.4.1/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.4.1/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.4.0/test/properties/property_manager_test.py` & `discovery-core-0.4.1/test/properties/property_manager_test.py`

 * *Files identical despite different names*

