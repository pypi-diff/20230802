# Comparing `tmp/aica_api-0.0.3.tar.gz` & `tmp/aica_api-0.0.4.tar.gz`

## Comparing `aica_api-0.0.3.tar` & `aica_api-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-0.0.3/src/aica_api/__init__.py
--rw-r--r--   0        0        0     9398 2020-02-02 00:00:00.000000 aica_api-0.0.3/src/aica_api/client.py
--rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 aica_api-0.0.3/src/aica_api/ws_client.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 aica_api-0.0.3/tests/test_api.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aica_api-0.0.3/tests/test_ws.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-0.0.3/.gitignore
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-0.0.3/LICENSE
--rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aica_api-0.0.3/README.md
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aica_api-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aica_api-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aica_api-0.0.4/src/aica_api/__init__.py
+-rw-r--r--   0        0        0     9408 2020-02-02 00:00:00.000000 aica_api-0.0.4/src/aica_api/client.py
+-rw-r--r--   0        0        0     6749 2020-02-02 00:00:00.000000 aica_api-0.0.4/src/aica_api/ws_client.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 aica_api-0.0.4/tests/test_api.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aica_api-0.0.4/tests/test_ws.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 aica_api-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 aica_api-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 aica_api-0.0.4/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 aica_api-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 aica_api-0.0.4/PKG-INFO
```

### Comparing `aica_api-0.0.3/src/aica_api/client.py` & `aica_api-0.0.4/src/aica_api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     def _ws_endpoint(self, endpoint=''):
         """
         Build the connection address for a given websocket endpoint.
 
         :param endpoint: The websocket endpoint
         :return: The constructed connection address
         """
-        return f'{self._ws_address}/v1/{endpoint}'
+        return f'{self._ws_address}/{endpoint}'
 
     def check(self) -> requests.Response:
         """
         Make a GET request to the default endpoint to verify connectivity.
         """
         return requests.get(self._endpoint())
 
@@ -201,24 +201,24 @@
         Wait until a component predicate is true.
 
         :param component: The name of the component
         :param predicate: The name of the predicate
         :param timeout: Timeout duration in seconds. If set to None, block indefinitely
         :return: False if the connection times out before the predicate is true
         """
-        component = f'/{component}'
+        component = f'{component}'
 
         def check_predicate(data):
             try:
-                if data[component][predicate]:
+                if data[component]["predicates"][predicate]:
                     return True
             except KeyError:
                 return False
 
-        ws = WebsocketSyncClient(self._ws_endpoint('predicates'))
+        ws = WebsocketSyncClient(self._ws_endpoint('components'))
         return ws.read_until(check_predicate, timeout=timeout)
 
     def wait_for_condition(self, condition, timeout=None):
         """
         Wait until a condition is true.
 
         :param condition: The name of the condition
```

### Comparing `aica_api-0.0.3/src/aica_api/ws_client.py` & `aica_api-0.0.4/src/aica_api/ws_client.py`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.3/LICENSE` & `aica_api-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.3/README.md` & `aica_api-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aica_api-0.0.3/pyproject.toml` & `aica_api-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "aica_api"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Enrico Eberhard", email="enrico@aica.tech" },
 ]
 description = "A client utility for the AICA API"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

### Comparing `aica_api-0.0.3/PKG-INFO` & `aica_api-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aica_api
-Version: 0.0.3
+Version: 0.0.4
 Summary: A client utility for the AICA API
 Project-URL: Homepage, https://github.com/aica-technology/api
 Project-URL: Bug Tracker, https://github.com/aica-technology/api/issues
 Author-email: Enrico Eberhard <enrico@aica.tech>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

