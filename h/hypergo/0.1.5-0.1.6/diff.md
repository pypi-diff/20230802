# Comparing `tmp/hypergo-0.1.5.tar.gz` & `tmp/hypergo-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypergo-0.1.5.tar", last modified: Tue Aug  1 18:13:56 2023, max compression
+gzip compressed data, was "hypergo-0.1.6.tar", last modified: Wed Aug  2 13:12:01 2023, max compression
```

## Comparing `hypergo-0.1.5.tar` & `hypergo-0.1.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.580047 hypergo-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.568047 hypergo-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.572047 hypergo-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-01 18:13:44.000000 hypergo-0.1.5/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-01 18:13:44.000000 hypergo-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-01 18:13:44.000000 hypergo-0.1.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-01 18:13:44.000000 hypergo-0.1.5/BACKLOG.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:44.000000 hypergo-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 18:13:56.580047 hypergo-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-01 18:13:44.000000 hypergo-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-01 18:13:44.000000 hypergo-0.1.5/RELEASE_NOTES.md
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-01 18:13:44.000000 hypergo-0.1.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.576047 hypergo-0.1.5/hypergo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/azure_service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/azure_service_bus_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/hypergo_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/hypergo_click.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/hypergo_cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/key_value_store.py
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/message.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/service_bus_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/stdio_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-01 18:13:44.000000 hypergo-0.1.5/hypergo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.576047 hypergo-0.1.5/hypergo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-01 18:13:56.000000 hypergo-0.1.5/hypergo.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-08-01 18:13:44.000000 hypergo-0.1.5/lint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-01 18:13:44.000000 hypergo-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-01 18:13:56.580047 hypergo-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-01 18:13:44.000000 hypergo-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 18:13:56.580047 hypergo-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test.json
--rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_dynamic_input_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_dynamic_routing_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_local_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-01 18:13:44.000000 hypergo-0.1.5/tests/test_utility_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:12:01.766395 hypergo-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:12:01.758396 hypergo-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:12:01.762395 hypergo-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-02 13:11:51.000000 hypergo-0.1.6/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-08-02 13:11:51.000000 hypergo-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-08-02 13:11:51.000000 hypergo-0.1.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     5867 2023-08-02 13:11:51.000000 hypergo-0.1.6/BACKLOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:11:51.000000 hypergo-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-02 13:12:01.766395 hypergo-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-02 13:11:51.000000 hypergo-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12636 2023-08-02 13:11:51.000000 hypergo-0.1.6/RELEASE_NOTES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-02 13:11:51.000000 hypergo-0.1.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:12:01.762395 hypergo-0.1.6/hypergo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/azure_service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/azure_service_bus_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6122 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/hypergo_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/hypergo_click.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/hypergo_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/service_bus_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/stdio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-08-02 13:11:51.000000 hypergo-0.1.6/hypergo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:12:01.762395 hypergo-0.1.6/hypergo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-08-02 13:12:01.000000 hypergo-0.1.6/hypergo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-08-02 13:12:01.000000 hypergo-0.1.6/hypergo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:12:01.000000 hypergo-0.1.6/hypergo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-02 13:12:01.000000 hypergo-0.1.6/hypergo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-02 13:12:01.000000 hypergo-0.1.6/hypergo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 13:12:01.000000 hypergo-0.1.6/hypergo.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2830 2023-08-02 13:11:51.000000 hypergo-0.1.6/lint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 13:11:51.000000 hypergo-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-08-02 13:12:01.766395 hypergo-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-08-02 13:11:51.000000 hypergo-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:12:01.766395 hypergo-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6992 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5173 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test_dynamic_input_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test_dynamic_routing_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test_local_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test_message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4034 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-08-02 13:11:51.000000 hypergo-0.1.6/tests/test_utility_serialization.py
```

### Comparing `hypergo-0.1.5/.github/workflows/python-publish.yml` & `hypergo-0.1.6/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/.gitignore` & `hypergo-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/BACKLOG.md` & `hypergo-0.1.6/BACKLOG.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/RELEASE_NOTES.md` & `hypergo-0.1.6/RELEASE_NOTES.md`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/azure_service_bus_connection.py` & `hypergo-0.1.6/hypergo/azure_service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/config.py` & `hypergo-0.1.6/hypergo/config.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/executor.py` & `hypergo-0.1.6/hypergo/executor.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/graph.py` & `hypergo-0.1.6/hypergo/graph.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/hypergo_cli.py` & `hypergo-0.1.6/hypergo/hypergo_cli.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/hypergo_click.py` & `hypergo-0.1.6/hypergo/hypergo_click.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/hypergo_cmd.py` & `hypergo-0.1.6/hypergo/hypergo_cmd.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/local_storage.py` & `hypergo-0.1.6/hypergo/local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/message.py` & `hypergo-0.1.6/hypergo/message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/service_bus_connection.py` & `hypergo-0.1.6/hypergo/service_bus_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/stdio_connection.py` & `hypergo-0.1.6/hypergo/stdio_connection.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/storage.py` & `hypergo-0.1.6/hypergo/storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/transform.py` & `hypergo-0.1.6/hypergo/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,11 +53,11 @@
 
             for result in func(self, the_data):
                 out_message = cast(JsonDict, result)
                 if "pass_by_reference" in output_operations:
                     str_result = Utility.stringify(out_message)
                     out_storage_key = Utility.hash(str_result)
                     storage.save(out_storage_key, str_result)
-                    out_message = {"storagekey": out_storage_key}
+                    out_message = {"body": {}, "routing": out_message['routingkey'], "storagekey": out_storage_key}
                 yield out_message
 
         return wrapped_func
```

### Comparing `hypergo-0.1.5/hypergo/utility.py` & `hypergo-0.1.6/hypergo/utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo/version.py` & `hypergo-0.1.6/hypergo/version.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/hypergo.egg-info/SOURCES.txt` & `hypergo-0.1.6/hypergo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/lint.sh` & `hypergo-0.1.6/lint.sh`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/setup.py` & `hypergo-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test.json` & `hypergo-0.1.6/tests/test.json`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test.yaml` & `hypergo-0.1.6/tests/test.yaml`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test_dynamic_input_bindings.py` & `hypergo-0.1.6/tests/test_dynamic_input_bindings.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test_dynamic_routing_key.py` & `hypergo-0.1.6/tests/test_dynamic_routing_key.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test_local_storage.py` & `hypergo-0.1.6/tests/test_local_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test_message.py` & `hypergo-0.1.6/tests/test_message.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test_storage.py` & `hypergo-0.1.6/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test_utility.py` & `hypergo-0.1.6/tests/test_utility.py`

 * *Files identical despite different names*

### Comparing `hypergo-0.1.5/tests/test_utility_serialization.py` & `hypergo-0.1.6/tests/test_utility_serialization.py`

 * *Files identical despite different names*

