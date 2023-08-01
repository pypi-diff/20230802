# Comparing `tmp/discovery-core-0.2.9.tar.gz` & `tmp/discovery-core-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discovery-core-0.2.9.tar", last modified: Mon Jul 17 17:56:23 2023, max compression
+gzip compressed data, was "discovery-core-0.3.0.tar", last modified: Tue Aug  1 22:51:22 2023, max compression
```

## Comparing `discovery-core-0.2.9.tar` & `discovery-core-0.3.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.454125 discovery-core-0.2.9/
--rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.2.9/LICENSE.txt
--rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.2.9/MANIFEST.in
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-17 17:56:23.454347 discovery-core-0.2.9/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.2.9/README.rst
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.430993 discovery-core-0.2.9/discovery_core.egg-info/
--rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-07-17 17:56:23.000000 discovery-core-0.2.9/discovery_core.egg-info/PKG-INFO
--rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-07-17 17:56:23.000000 discovery-core-0.2.9/discovery_core.egg-info/SOURCES.txt
--rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-07-17 17:56:23.000000 discovery-core-0.2.9/discovery_core.egg-info/dependency_links.txt
--rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-07-17 17:56:23.000000 discovery-core-0.2.9/discovery_core.egg-info/top_level.txt
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.431628 discovery-core-0.2.9/ds_core/
--rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-17 17:53:02.000000 discovery-core-0.2.9/ds_core/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.434335 discovery-core-0.2.9/ds_core/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/ds_core/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.2.9/ds_core/components/abstract_component.py
--rw-r--r--   0 doatridge   (503) staff       (20)    23605 2023-07-15 23:59:50.000000 discovery-core-0.2.9/ds_core/components/core_commons.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.437331 discovery-core-0.2.9/ds_core/handlers/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/ds_core/handlers/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.2.9/ds_core/handlers/abstract_handlers.py
--rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.2.9/ds_core/handlers/pyarrow_handlers.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.438143 discovery-core-0.2.9/ds_core/intent/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/ds_core/intent/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.2.9/ds_core/intent/abstract_intent.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.442822 discovery-core-0.2.9/ds_core/properties/
--rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/ds_core/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.2.9/ds_core/properties/abstract_properties.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.2.9/ds_core/properties/decorator_patterns.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.2.9/ds_core/properties/property_manager.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-07-17 17:56:23.455384 discovery-core-0.2.9/setup.cfg
--rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.2.9/setup.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.443722 discovery-core-0.2.9/test/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.2.9/test/__init__.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.445824 discovery-core-0.2.9/test/components/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/test/components/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    31492 2023-06-29 16:42:17.000000 discovery-core-0.2.9/test/components/abstract_component_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)    15078 2023-07-13 23:46:04.000000 discovery-core-0.2.9/test/components/commons_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.448047 discovery-core-0.2.9/test/handlers/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/test/handlers/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.2.9/test/handlers/connector_contract_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.2.9/test/handlers/handler_factory_test.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.450585 discovery-core-0.2.9/test/intent/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/test/intent/__init__.py
--rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.2.9/test/intent/abstract_intent_test.py
--rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.2.9/test/intent/pyarrow_intent_model.py
-drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-07-17 17:56:23.453255 discovery-core-0.2.9/test/properties/
--rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.2.9/test/properties/__init__.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.2.9/test/properties/abstract_properties_manager_test.py
--rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.2.9/test/properties/property_manager_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.731775 discovery-core-0.3.0/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     1087 2023-06-28 23:35:32.000000 discovery-core-0.3.0/LICENSE.txt
+-rwxr-xr-x   0 doatridge   (503) staff       (20)       65 2023-06-28 23:35:32.000000 discovery-core-0.3.0/MANIFEST.in
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-01 22:51:22.731956 discovery-core-0.3.0/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)    13130 2023-06-28 23:35:32.000000 discovery-core-0.3.0/README.rst
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.715785 discovery-core-0.3.0/discovery_core.egg-info/
+-rw-r--r--   0 doatridge   (503) staff       (20)    14094 2023-08-01 22:51:22.000000 discovery-core-0.3.0/discovery_core.egg-info/PKG-INFO
+-rw-r--r--   0 doatridge   (503) staff       (20)     1092 2023-08-01 22:51:22.000000 discovery-core-0.3.0/discovery_core.egg-info/SOURCES.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)        1 2023-08-01 22:51:22.000000 discovery-core-0.3.0/discovery_core.egg-info/dependency_links.txt
+-rw-r--r--   0 doatridge   (503) staff       (20)       13 2023-08-01 22:51:22.000000 discovery-core-0.3.0/discovery_core.egg-info/top_level.txt
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.716136 discovery-core-0.3.0/ds_core/
+-rw-r--r--   0 doatridge   (503) staff       (20)       73 2023-07-30 23:37:36.000000 discovery-core-0.3.0/ds_core/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.718060 discovery-core-0.3.0/ds_core/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/ds_core/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    63342 2023-06-29 23:15:54.000000 discovery-core-0.3.0/ds_core/components/abstract_component.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    25922 2023-08-01 22:47:24.000000 discovery-core-0.3.0/ds_core/components/core_commons.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.719643 discovery-core-0.3.0/ds_core/handlers/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/ds_core/handlers/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    15258 2023-05-02 21:09:52.000000 discovery-core-0.3.0/ds_core/handlers/abstract_handlers.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     8143 2023-07-17 17:55:59.000000 discovery-core-0.3.0/ds_core/handlers/pyarrow_handlers.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.720515 discovery-core-0.3.0/ds_core/intent/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/ds_core/intent/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    11255 2023-06-29 15:15:01.000000 discovery-core-0.3.0/ds_core/intent/abstract_intent.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.724017 discovery-core-0.3.0/ds_core/properties/
+-rwxr-xr-x   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/ds_core/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    65710 2023-06-29 23:15:54.000000 discovery-core-0.3.0/ds_core/properties/abstract_properties.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2996 2022-09-22 17:31:08.000000 discovery-core-0.3.0/ds_core/properties/decorator_patterns.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11271 2023-06-29 15:15:01.000000 discovery-core-0.3.0/ds_core/properties/property_manager.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)      110 2023-08-01 22:51:22.732548 discovery-core-0.3.0/setup.cfg
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     2085 2023-07-03 17:06:43.000000 discovery-core-0.3.0/setup.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.724740 discovery-core-0.3.0/test/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2023-06-29 15:06:28.000000 discovery-core-0.3.0/test/__init__.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.725717 discovery-core-0.3.0/test/components/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/test/components/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    31457 2023-08-01 20:07:50.000000 discovery-core-0.3.0/test/components/abstract_component_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    20699 2023-08-01 22:48:11.000000 discovery-core-0.3.0/test/components/commons_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.727141 discovery-core-0.3.0/test/handlers/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/test/handlers/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)    11054 2023-06-29 16:24:13.000000 discovery-core-0.3.0/test/handlers/connector_contract_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2560 2023-06-29 16:24:13.000000 discovery-core-0.3.0/test/handlers/handler_factory_test.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.728908 discovery-core-0.3.0/test/intent/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/test/intent/__init__.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     2899 2023-07-12 16:01:36.000000 discovery-core-0.3.0/test/intent/abstract_intent_test.py
+-rw-r--r--   0 doatridge   (503) staff       (20)     7100 2023-07-12 17:46:55.000000 discovery-core-0.3.0/test/intent/pyarrow_intent_model.py
+drwxr-xr-x   0 doatridge   (503) staff       (20)        0 2023-08-01 22:51:22.731154 discovery-core-0.3.0/test/properties/
+-rw-r--r--   0 doatridge   (503) staff       (20)        0 2022-01-11 19:24:12.000000 discovery-core-0.3.0/test/properties/__init__.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)    36169 2023-06-29 23:15:54.000000 discovery-core-0.3.0/test/properties/abstract_properties_manager_test.py
+-rwxr-xr-x   0 doatridge   (503) staff       (20)     9513 2023-06-29 16:47:52.000000 discovery-core-0.3.0/test/properties/property_manager_test.py
```

### Comparing `discovery-core-0.2.9/LICENSE.txt` & `discovery-core-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/PKG-INFO` & `discovery-core-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.9
+Version: 0.3.0
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.9/README.rst` & `discovery-core-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/discovery_core.egg-info/PKG-INFO` & `discovery-core-0.3.0/discovery_core.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discovery-core
-Version: 0.2.9
+Version: 0.3.0
 Summary: Augmented Intent Single Task Adaptive Components
 Home-page: http://github.com/gigas64/discovery-core
 Author: Gigas64
 Author-email: gigas64@opengrass.net
 License: BSD
 Keywords: Foundation SDK Machine learning AI component intent data science
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `discovery-core-0.2.9/discovery_core.egg-info/SOURCES.txt` & `discovery-core-0.3.0/discovery_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/ds_core/components/abstract_component.py` & `discovery-core-0.3.0/ds_core/components/abstract_component.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/ds_core/components/core_commons.py` & `discovery-core-0.3.0/ds_core/components/core_commons.py`

 * *Files 6% similar despite different names*

```diff
@@ -148,14 +148,27 @@
         if not isinstance(seq, list):
             raise ValueError("The sequence must be of type 'list'")
         if not isinstance(other, list):
             raise ValueError("The sequence must be of type 'list'")
         return list(set(seq).union(set(other)))
 
     @staticmethod
+    def list_dup(seq: list) -> list:
+        """ Useful utility method to return duplicates"""
+        if not isinstance(seq, list):
+            raise ValueError("The sequence must be of type 'list'")
+        seen = set()
+        # Note: assign seen add to a local variable as local variable are less costly to resolve than dynamic call
+        seen_add = seen.add
+        # adds all elements it doesn't know yet to seen and all other to return
+        seen_twice = set(x for x in seq if x in seen or seen_add(x))
+        # turn the set into a list (as requested)
+        return list(seen_twice)
+
+    @staticmethod
     def list_unique(seq: list) -> list:
         """ Useful utility method to retain the order of a list but removes duplicates"""
         if not isinstance(seq, list):
             raise ValueError("The sequence must be of type 'list'")
         seen = set()
         # Note: assign seen add to a local variable as local variable are less costly to resolve than dynamic call
         seen_add = seen.add
@@ -210,55 +223,65 @@
         precision = precision if isinstance(precision, int) else 5
         seq_min = min(seq)
         seq_range = max(seq) - seq_min
         n_range = (b - a)
         return [round((n_range * ((x - seq_min) / seq_range)) + a, precision) for x in seq]
 
     @staticmethod
-    def filter_headers(data: pa.Table, headers: [str, list]=None, d_type: pa.DataType=None, drop: bool=None,
-                       regex: [str, list]=None) -> list:
-        """ returns a list of headers based on the filter criteria
+    def filter_headers(data: pa.Table, headers: [str, list]=None, d_types: list=None, regex: [str, list]=None,
+                       drop: bool=None) -> list:
+        """ returns a list of headers based on the filter criteria. The order of filter is d_type, headers then regex.
 
         :param data: the Canonical data to get the column headers from
-        :param headers: a list of headers to drop or filter on type
-        :param d_type: a li
-        :param drop: to drop or not drop the selection
-        :param regex: a regular expression to search the headers
+        :param d_types: (optional) a list of pyarrow DataTypes of the columns headers
+        :param headers: (optional) a list of header strings to select from the columns headers
+        :param regex: (optional) a regular expression to search from the columns headers
+        :param drop: (optional) reverses the selection and drops the selected column headers
         :return: a filtered list of headers
 
         :raise: TypeError if any of the types are not as expected
         """
         if not isinstance(data, pa.Table):
             raise TypeError("The first function attribute must be a pa.Table")
         drop = drop if isinstance(drop, bool) else False
         headers = CoreCommons.list_formatter(headers)
         regex = '|'.join(CoreCommons.list_formatter(regex))
-
-        rtn_list = data.column_names
+        rtn_list = []
+        if d_types is not None and d_types:
+            for n in data.column_names:
+                c = data.column(n).combine_chunks()
+                for t in d_types:
+                    if c.type.equals(t):
+                        rtn_list.append(n)
+        else:
+            rtn_list = data.column_names
         if headers is not None and headers:
-            _ = pc.is_in(rtn_list, pa.array(headers))
-            rtn_list = pa.array(rtn_list).filter(_).to_pylist()
+            rtn_list = CoreCommons.list_intersect(rtn_list, headers)
         if regex is not None and regex:
             _ = pc.extract_regex(rtn_list, regex).is_valid()
             rtn_list = pa.array(rtn_list).filter(_).to_pylist()
         if drop:
             return CoreCommons.list_diff(data.column_names, rtn_list)
         return rtn_list
 
     @staticmethod
-    def filter_columns(data: pa.Table, headers=None, drop: bool=None, regex: [str, list]=None) -> pa.Table:
-        """ Returns a subset of columns based on the filter criteria
+    def filter_columns(data: pa.Table, headers=None, d_types: list=None, regex: [str, list]=None,
+                       drop: bool=None) -> pa.Table:
+        """ Returns a subset of columns based on the filter criteria. The order of filter is d_type, headers then regex.
 
         :param data: the Canonical data to get the column headers from
-        :param headers: a list of headers to drop or filter on type
-        :param drop: to drop or not drop the headers
-        :param regex: a regular expression to search the headers
+        :param d_types: (optional) a list of pyarrow DataTypes of the columns headers
+        :param headers: (optional) a list of header strings to select from the columns headers
+        :param regex: (optional) a regular expression to search from the columns headers
+        :param drop: (optional) reverses the selection and drops the selected column headers
+        :return: a filtered list of headers
         :return:
         """
-        return data.select(CoreCommons.filter_headers(data=data, headers=headers, drop=drop, regex=regex))
+        return data.select(CoreCommons.filter_headers(data=data, headers=headers, d_types=d_types, regex=regex,
+                                                      drop=drop))
 
     @staticmethod
     def table_append(t1: pa.Table, t2: pa.Table):
         """ appends all the columns in t2 to t1 """
         if not isinstance(t2, pa.Table):
             raise ValueError("As a minimum, the second value passed must be a PyArrow Table")
         if not isinstance(t1, pa.Table):
@@ -270,106 +293,121 @@
             t1 = t1.append_column(c, t2.column(c))
         return t1
 
     @staticmethod
     def table_flatten(t :pa.Table):
         """ flattens a table of lists and struct data types """
         working = True
-
+        row_count = t.num_rows
         while working:
             working = False
-            for idx in range(len(t.column_names)):
-                c = t.column_names[idx]
-                record = t.column(c).combine_chunks()
+            for c in t.column_names:
+                if c not in t.column_names:
+                    continue
+                record = t.column(c)
+                if isinstance(record, pa.ChunkedArray):
+                    record = record.combine_chunks()
                 if pa.types.is_list(record.type):
-                    for i in range(pc.min(pc.list_value_length(record)).as_py()):
-                        t = t.append_column(f'{c}.nest_list_{i}', pc.list_element(t.column(c), i).combine_chunks())
+                    total_max = pc.max(pc.list_value_length(record)).as_py()
+                    if total_max is None:
+                        total_max = 1
+                    record = pc.list_slice(record, start=0, stop=total_max, return_fixed_size_list=True)
+                    for i in range(total_max):
+                        try:
+                            t = t.append_column(f'{c}.nest_list_{i}', pc.list_element(record, i))
+                        except ArrowInvalid:
+                            break
                     t = t.drop_columns(c)
                     working = True
                 if pa.types.is_struct(record.type):
                     t = t.flatten()
                     working = True
+        # drop null columns
+        for n in t.column_names:
+            c = t.column(n)
+            if pa.types.is_boolean(c.type):
+                if not pc.all(c).as_py():
+                    t = t.drop_columns(n)
+            elif len(c.drop_null()) == 0:
+                t = t.drop_columns(n)
         return t
 
     @staticmethod
     def table_nest(t: pa.Table) -> list:
         """ turns a flattened table back to a nested pattern """
 
-        def add_leaf(tree, keys, value):
-            key = keys[0]
-            tree[key] = value if len(keys) == 1 else add_leaf(tree[key] if key in tree else {}, keys[1:], value)
-            return tree
-
-        def traverse(d, path=[]):
-            if isinstance(d, dict):
-                for (k, v) in d.items():
-                    yield from traverse(v, [*path, k])
-                else:
-                    yield [*path, d]
-
-        def set_list(struct, keys, tree):
-            for key in tuple(struct.keys()):
-                if isinstance(struct.get(key), dict) and len(struct.get(key)) > 0:
-                    keys.append(key)
-                    set_list(struct.get(key), keys, tree)
-                if str(key).startswith('nest_list_'):
-                    snippet = list([struct.get(key, {})])
-                    if snippet[0] == {}:
-                        continue
-                    branch = tree
-                    for k in keys[:-1]:
-                        branch = branch.get(k)
+        def add_leaf(b_tree, b_keys, b_value):
+            l_key = b_keys[0]
+            try:
+                b_tree[l_key] = b_value if len(b_keys) == 1 else add_leaf(b_tree[l_key] if l_key in b_tree else {}, b_keys[1:], b_value)
+            except TypeError as e:
+                b_tree[l_key].append(b_value)
+            except (AttributeError, KeyError):
+                pass
+            return b_tree
+
+        # def del_leaf(b_tree, b_keys):
+        #     l_key = b_keys[0]
+        #     try:
+        #         b_tree.pop(l_key) if len(b_keys) == 1 else del_leaf(b_tree[l_key] if l_key in b_tree else {}, b_keys[1:])
+        #     except (AttributeError, KeyError):
+        #         pass
+        #     return b_tree
+        #
+        # def traverse(d, path=[]):
+        #     if isinstance(d, dict):
+        #         for (k, v) in d.items():
+        #             yield from traverse(v, [*path, k])
+        #         else:
+        #             yield [*path, d]
+
+        def set_list(struct, l_keys, l_tree):
+            for l_branch in tuple(struct.keys()):
+                if struct.get(l_branch) is None:
+                    continue
+                # loop to the top of the tree and work back
+                if isinstance(struct.get(l_branch), dict) and len(struct.get(l_branch)) > 0:
+                    l_keys.append(l_branch)
+                    set_list(struct.get(l_branch), l_keys, l_tree)
+                    l_keys.pop()
+                # look for the nest list
+                if str(l_branch).startswith('nest_list_'):
                     snippet = list(struct.values())
-                    struct.clear()
-                    branch[keys[-1]] = snippet
-            if len(keys) > 0:
-                keys.pop()
-            return tree
+                    l_tree = add_leaf(l_tree, l_keys, snippet)
+            return l_tree
 
         document = []
         for idx in range(t.num_rows):
             tree = {}
             for c in t.column_names:
                 names = c.split('.')
-                # set the branch
-                n = names.pop()
-                branch = {n: t.column(c)[idx].as_py()}
-                _ = (next(traverse(branch)))
-                while names:
-                    n = names.pop()
-                    branch = {n: branch}
-                    _ = (next(traverse(branch)))
-                # branch is correct
-                leaf = branch
-                keys = []
-                sub_leaf = tree
-                while leaf:
-                    key = list(leaf.keys())[0]
-                    keys.append(key)
-                    if key not in sub_leaf.keys():
-                        leaf = leaf.get(key)
-                        break
-                    if tree.keys() is None:
-                        break
-                    leaf = leaf.get(key)
-                    sub_leaf = sub_leaf.get(key)
-                tree = add_leaf(tree, keys, leaf)
+                value = t.column(c)[idx].as_py()
+                if value is None:
+                    continue
+                tree = add_leaf(tree, names, t.column(c)[idx].as_py())
             tree = set_list(tree, [], tree)
             document.append(tree)
         return document
 
     @staticmethod
     def column_cast(a: pa.Array, ty: pa.DataType) -> pa.Array:
         """ attempt to cast a pyarrow array to the given type """
         try:
             return a.cast(ty)
         except (ArrowInvalid, ArrowTypeError, ArrowNotImplementedError):
             return a
 
     @staticmethod
+    def column_precision(a: pa.Array):
+        """returns the max precision in a numeric pyarrow array"""
+        if pa.types.is_floating(a.type) or pa.types.is_integer(a.type):
+            return max([CoreCommons.precision_scale(x)[1] for x in a.drop_null().to_pylist()])
+        raise ValueError(f"The array should be numeric, type '{a.type}' sent.")
+
+    @staticmethod
     def table_cast(t: pa.Table, cat_max: int=None):
         """ attempt to cast a pyarrow table columns to the given type """
         cat_max = cat_max if isinstance(cat_max, int) else 40
         rtn_tbl = None
         for n in t.column_names:
             c = t.combine_chunks().column(n)
             if pa.types.is_string(c.type):
```

### Comparing `discovery-core-0.2.9/ds_core/handlers/abstract_handlers.py` & `discovery-core-0.3.0/ds_core/handlers/abstract_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/ds_core/handlers/pyarrow_handlers.py` & `discovery-core-0.3.0/ds_core/handlers/pyarrow_handlers.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/ds_core/intent/abstract_intent.py` & `discovery-core-0.3.0/ds_core/intent/abstract_intent.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/ds_core/properties/abstract_properties.py` & `discovery-core-0.3.0/ds_core/properties/abstract_properties.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/ds_core/properties/decorator_patterns.py` & `discovery-core-0.3.0/ds_core/properties/decorator_patterns.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/ds_core/properties/property_manager.py` & `discovery-core-0.3.0/ds_core/properties/property_manager.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/setup.py` & `discovery-core-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/test/components/abstract_component_test.py` & `discovery-core-0.3.0/test/components/abstract_component_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 from datetime import datetime
 from pprint import pprint
 
 import pandas as pd
 
 from ds_core.components.abstract_component import AbstractComponent
 from ds_core.handlers.abstract_handlers import ConnectorContract
-from ds_core.intent.python_cleaners_intent import PyarrowCleanersIntentModel as ControlIntentModel
 from ds_core.properties.abstract_properties import AbstractPropertyManager
+from test.intent.pyarrow_intent_model import PyarrowIntentModel
 from ds_core.properties.property_manager import PropertyManager
 
 
 class ControlPropertyManager(AbstractPropertyManager):
 
     def __init__(self, task_name, creator: str=None):
         # set additional keys
@@ -25,15 +25,15 @@
 
 class ControlComponent(AbstractComponent):
 
     DEFAULT_MODULE = 'ds_core.handlers.pyarrow_handlers'
     DEFAULT_SOURCE_HANDLER = 'PyarrowSourceHandler'
     DEFAULT_PERSIST_HANDLER = 'PyarrowPersistHandler'
 
-    def __init__(self, property_manager: ControlPropertyManager, intent_model: ControlIntentModel,
+    def __init__(self, property_manager: ControlPropertyManager, intent_model: PyarrowIntentModel,
                  default_save=None, reset_templates: bool = None, template_path: str=None, template_module: str=None,
                  template_source_handler: str=None, template_persist_handler: str=None, align_connectors: bool = None):
         super().__init__(property_manager=property_manager, intent_model=intent_model, default_save=default_save,
                          reset_templates=reset_templates, template_path=template_path, template_module=template_module,
                          template_source_handler=template_source_handler,
                          template_persist_handler=template_persist_handler, align_connectors=align_connectors)
 
@@ -44,15 +44,15 @@
                  template_source_handler: str=None, template_persist_handler: str=None, align_connectors: bool=None,
                  default_save_intent: bool=None, default_intent_level: bool=None, order_next_available: bool=None,
                  default_replace_intent: bool=None, has_contract: bool=None):
         pm_file_type = pm_file_type if isinstance(pm_file_type, str) else 'parquet'
         pm_module = pm_module if isinstance(pm_module, str) else 'ds_core.handlers.pyarrow_handlers'
         pm_handler = pm_handler if isinstance(pm_handler, str) else 'PyarrowPersistHandler'
         _pm = ControlPropertyManager(task_name=task_name, creator=creator)
-        _intent_model = ControlIntentModel(property_manager=_pm, default_save_intent=default_save_intent,
+        _intent_model = PyarrowIntentModel(property_manager=_pm, default_save_intent=default_save_intent,
                                            default_intent_level=default_intent_level,
                                            order_next_available=order_next_available,
                                            default_replace_intent=default_replace_intent)
         super()._init_properties(property_manager=_pm, uri_pm_path=uri_pm_path, default_save=default_save,
                                  uri_pm_repo=uri_pm_repo, pm_file_type=pm_file_type, pm_module=pm_module,
                                  pm_handler=pm_handler, pm_kwargs=pm_kwargs, has_contract=has_contract)
         return cls(property_manager=_pm, intent_model=_intent_model, default_save=default_save,
```

### Comparing `discovery-core-0.2.9/test/handlers/connector_contract_test.py` & `discovery-core-0.3.0/test/handlers/connector_contract_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/test/handlers/handler_factory_test.py` & `discovery-core-0.3.0/test/handlers/handler_factory_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/test/intent/abstract_intent_test.py` & `discovery-core-0.3.0/test/intent/abstract_intent_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/test/intent/pyarrow_intent_model.py` & `discovery-core-0.3.0/test/intent/pyarrow_intent_model.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/test/properties/abstract_properties_manager_test.py` & `discovery-core-0.3.0/test/properties/abstract_properties_manager_test.py`

 * *Files identical despite different names*

### Comparing `discovery-core-0.2.9/test/properties/property_manager_test.py` & `discovery-core-0.3.0/test/properties/property_manager_test.py`

 * *Files identical despite different names*

