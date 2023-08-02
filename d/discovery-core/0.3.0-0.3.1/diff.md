# Comparing `tmp/discovery-core-0.3.0.tar.gz` & `tmp/discovery-core-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.3.0.tar", last modified: Tue Aug  1 22:51:22 2023, max compression
+gzip compressed data, was "discovery-core-0.3.1.tar", last modified: Wed Aug  2 16:44:25 2023, max compression
```

## Comparing `discovery-core-0.3.0.tar` & `discovery-core-0.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.731775 discovery-core-0.3.0/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.3.0/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.3.0/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-01 22:51:22.731956 discovery-core-0.3.0/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.3.0/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.715785 discovery-core-0.3.0/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-01 22:51:22.000000 discovery-core-0.3.0/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-01 22:51:22.000000 discovery-core-0.3.0/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-01 22:51:22.000000 discovery-core-0.3.0/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-01 22:51:22.000000 discovery-core-0.3.0/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.716136 discovery-core-0.3.0/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-30 23:37:36.000000 discovery-core-0.3.0/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.718060 discovery-core-0.3.0/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.3.0/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    25922 2023-08-01 22:47:24.000000 discovery-core-0.3.0/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.719643 discovery-core-0.3.0/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.3.0/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.3.0/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.720515 discovery-core-0.3.0/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.3.0/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.724017 discovery-core-0.3.0/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.3.0/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.3.0/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.3.0/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-01 22:51:22.732548 discovery-core-0.3.0/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.3.0/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.724740 discovery-core-0.3.0/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.3.0/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.725717 discovery-core-0.3.0/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.3.0/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    20699 2023-08-01 22:48:11.000000 discovery-core-0.3.0/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.727141 discovery-core-0.3.0/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.3.0/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.3.0/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.728908 discovery-core-0.3.0/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.3.0/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.3.0/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.731154 discovery-core-0.3.0/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.3.0/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.3.0/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.497705 discovery-core-0.3.1/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.3.1/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.3.1/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-02 16:44:25.497928 discovery-core-0.3.1/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.3.1/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.479920 discovery-core-0.3.1/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-02 16:44:25.000000 discovery-core-0.3.1/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-02 16:44:25.000000 discovery-core-0.3.1/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-02 16:44:25.000000 discovery-core-0.3.1/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-02 16:44:25.000000 discovery-core-0.3.1/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.480345 discovery-core-0.3.1/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-08-01 22:52:05.000000 discovery-core-0.3.1/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.481474 discovery-core-0.3.1/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.1/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63367 2023-08-02 16:42:41.000000 discovery-core-0.3.1/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25922 2023-08-01 22:47:24.000000 discovery-core-0.3.1/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.484491 discovery-core-0.3.1/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.1/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.3.1/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.3.1/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.485591 discovery-core-0.3.1/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.1/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.3.1/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.488719 discovery-core-0.3.1/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.1/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.3.1/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.3.1/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.3.1/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-02 16:44:25.499033 discovery-core-0.3.1/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.3.1/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.489347 discovery-core-0.3.1/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.3.1/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.491141 discovery-core-0.3.1/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.1/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.3.1/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20699 2023-08-01 22:48:11.000000 discovery-core-0.3.1/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.493330 discovery-core-0.3.1/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.1/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.3.1/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.3.1/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.494973 discovery-core-0.3.1/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.1/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.3.1/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.3.1/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-02 16:44:25.497017 discovery-core-0.3.1/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.1/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.3.1/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.3.1/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.3.0/LICENSE.txt` & `discovery-core-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/PKG-INFO` & `discovery-core-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.3.0/README.rst` & `discovery-core-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.3.1/discovery_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.3.0
+Version: 0.3.1
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.3.0/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.3.1/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/ds_core/components/abstract_component.py` & `discovery-core-0.3.1/ds_core/components/abstract_component.py`

 * *Files 0% similar despite different names*

```diff
@@ -454,15 +454,15 @@
         template_aligned = template_aligned if isinstance(template_aligned, bool) else False
         _schema, _netloc, _path = ConnectorContract.parse_address_elements(uri=uri)
         _module_name, _, _handler = self._from_handler(schema=_schema)
         connector_contract = ConnectorContract(uri=uri, module_name=_module_name, handler=_handler,
                                                version=self.pm.version, **kwargs)
         self.add_connector_contract(connector_name=connector_name, connector_contract=connector_contract,
                                     template_aligned=template_aligned, save=save)
-        return
+        return self
 
     def add_connector_contract(self, connector_name: str, connector_contract: ConnectorContract,
                                template_aligned: bool=None, save: bool=None):
         """ Sets a named connector contract
 
         :param connector_name: the name or label to identify and reference the connector
         :param connector_contract: a Connector Contract for the properties persistence
@@ -471,42 +471,42 @@
         :return: if load is True, returns a Pandas.DataFrame else None
         """
         if self.pm.has_connector(connector_name):
             self.pm.remove_connector_contract(connector_name)
         self.pm.set_connector_contract(connector_name=connector_name, connector_contract=connector_contract,
                                        aligned=template_aligned)
         self.pm_persist(save)
-        return
+        return self
 
     def add_connector_source(self, connector_name: str, uri_file: str, save: bool=None, **kwargs):
         """ Adds a connector using settings from the self.pm.TEMPLATE_SOURCE template connector.
 
         :param connector_name: the name or label to identify and reference the connector
         :param uri_file: the name of the file to append to the end of the default path
         :param save: override of the default save action set at initialisation.
         :param kwargs: any kwargs to add to the default connector
         :return:
         """
         self.add_connector_from_template(connector_name=connector_name, uri_file=uri_file,
                                          template_name=self.pm.TEMPLATE_SOURCE, save=save, **kwargs)
-        return
+        return self
 
     def add_connector_persist(self, connector_name: str, uri_file: str, save: bool=None, **kwargs):
         """ Adds a connector using settings from the self.pm.TEMPLATE_PERSIST template connector.
         self.pm.TEMPLATE_PERSIST are added at initialisation
 
         :param connector_name: the name or label to identify and reference the connector
         :param uri_file: the name of the file to append to the end of the default path
         :param save: override of the default save action set at initialisation.
         :param kwargs: any kwargs to add to the default connector
         :return:
         """
         self.add_connector_from_template(connector_name=connector_name, uri_file=uri_file,
                                          template_name=self.pm.TEMPLATE_PERSIST, save=save, **kwargs)
-        return
+        return self
 
     def add_connector_from_template(self, connector_name: str, uri_file: str, template_name: str,  save: bool=None,
                                     **kwargs):
         """ Adds a connector using settings from a template connector. By default a self.TEMPLATE_SOURCE and
         self.TEMPLATE_PERSIST are added at initialisation
 
         :param connector_name: the name or label to identify and reference the connector
@@ -522,15 +522,15 @@
         if not isinstance(kwargs, dict):
             kwargs = {}
         template.raw_kwargs.update(kwargs)
         cc = ConnectorContract(uri=uri, module_name=template.raw_module_name, handler=template.raw_handler,
                                version=self.pm.version, **kwargs)
         self.add_connector_contract(connector_name=connector_name, connector_contract=cc, template_aligned=True,
                                     save=save)
-        return
+        return self
 
     def reset_template_connectors(self, save: bool=None):
         """ resets connector contracts with template path and handler where they are template aligned.
         (see `set_connector_aligned`)
 
         :param save: override of the default save action set at initialisation.
         """
```

### Comparing `discovery-core-0.3.0/ds_core/components/core_commons.py` & `discovery-core-0.3.1/ds_core/components/core_commons.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.3.1/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.3.1/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/ds_core/intent/abstract_intent.py` & `discovery-core-0.3.1/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/ds_core/properties/abstract_properties.py` & `discovery-core-0.3.1/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/ds_core/properties/decorator_patterns.py` & `discovery-core-0.3.1/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/ds_core/properties/property_manager.py` & `discovery-core-0.3.1/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/setup.py` & `discovery-core-0.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/test/components/abstract_component_test.py` & `discovery-core-0.3.1/test/components/abstract_component_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/test/components/commons_test.py` & `discovery-core-0.3.1/test/components/commons_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/test/handlers/connector_contract_test.py` & `discovery-core-0.3.1/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/test/handlers/handler_factory_test.py` & `discovery-core-0.3.1/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/test/intent/abstract_intent_test.py` & `discovery-core-0.3.1/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/test/intent/pyarrow_intent_model.py` & `discovery-core-0.3.1/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.3.1/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.3.0/test/properties/property_manager_test.py` & `discovery-core-0.3.1/test/properties/property_manager_test.py`

 * *Files identical despite different names*

