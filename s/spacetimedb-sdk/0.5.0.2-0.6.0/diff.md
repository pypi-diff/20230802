# Comparing `tmp/spacetimedb_sdk-0.5.0.2.tar.gz` & `tmp/spacetimedb_sdk-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetimedb_sdk-0.5.0.2.tar", last modified: Mon Jul 17 21:17:09 2023, max compression
+gzip compressed data, was "spacetimedb_sdk-0.6.0.tar", last modified: Wed Aug  2 21:18:42 2023, max compression
```

## Comparing `spacetimedb_sdk-0.5.0.2.tar` & `spacetimedb_sdk-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:09.609229 spacetimedb_sdk-0.5.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 21:17:09.609229 spacetimedb_sdk-0.5.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 21:17:09.609229 spacetimedb_sdk-0.5.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:09.605229 spacetimedb_sdk-0.5.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/gen_lazydocs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:09.605229 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/client_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/local_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetime_websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11292 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetimedb_async_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    24869 2023-07-17 21:16:55.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetimedb_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 21:17:09.609229 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-17 21:17:09.000000 spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:18:42.843876 spacetimedb_sdk-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-02 21:18:42.843876 spacetimedb_sdk-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 21:18:42.843876 spacetimedb_sdk-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:18:42.843876 spacetimedb_sdk-0.6.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/src/gen_lazydocs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:18:42.843876 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/client_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/spacetime_websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/spacetimedb_async_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24920 2023-08-02 21:18:31.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/spacetimedb_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 21:18:42.843876 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-08-02 21:18:42.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-08-02 21:18:42.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 21:18:42.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-02 21:18:42.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-02 21:18:42.000000 spacetimedb_sdk-0.6.0/src/spacetimedb_sdk.egg-info/top_level.txt
```

### Comparing `spacetimedb_sdk-0.5.0.2/pyproject.toml` & `spacetimedb_sdk-0.6.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools", "wheel", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spacetimedb_sdk"
 authors = [
-    {name = "Derek Brinkmann", email = "derek@clockworklabs.io"},
+    {name = "Clockwork Labs", email = "derek@clockworklabs.io"},
 ]
 
 dependencies = [
     "websocket-client",
     "configparser",
 ]
-version = "0.5.0.2"
+version = "0.6.0"
 readme = "README.md"
 
 # urls
 # Should describe where to find useful info for your project
 [project.urls]
 homepage = "https://spacetimedb.com"
 repository = "https://github.com/clockworklabs/spacetimedb-python-sdk"
```

### Comparing `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/client_cache.py` & `spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/client_cache.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/local_config.py` & `spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/local_config.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetime_websocket_client.py` & `spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/spacetime_websocket_client.py`

 * *Files identical despite different names*

### Comparing `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetimedb_async_client.py` & `spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/spacetimedb_async_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -294,14 +294,15 @@
         for event in self.prescheduled_events:
             self.schedule_event(event[0], event[1], *event[2])
 
     async def _timeout_task(self, timeout):
         await asyncio.sleep(timeout)
         self.event_queue.put_nowait(("timeout",))
 
+    # TODO: Replace this with a proper async queue
     async def _event(self):
         update_task = asyncio.create_task(self._periodic_update())
         try:
             result = await self.event_queue.get()
             update_task.cancel()
             return result
         except Exception as e:
```

### Comparing `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk/spacetimedb_client.py` & `spacetimedb_sdk-0.6.0/src/spacetimedb_sdk/spacetimedb_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,20 +43,23 @@
         Returns:
             Identity: The Identity object.
         """
         return Identity(data)
 
     # override to_string
     def __str__(self):
-        return self.data.decode("utf-8")
+        return self.data.hex()
 
     # override = operator
     def __eq__(self, other):
         return isinstance(other, Identity) and self.data == other.data
 
+    def __hash__(self):
+        return hash(self.data)
+
 
 class DbEvent:
     """
     Represents a database event.
 
     Attributes:
         table_name (str): The name of the table associated with the event.
@@ -228,15 +231,15 @@
         self.wsc = WebSocketClient(
             "v1.text.spacetimedb",
             on_connect=on_connect,
             on_error=on_error,
             on_close=on_disconnect,
             on_message=self._on_message,
         )
-        print("CONNECTING " + host + " " + address_or_name)
+        # print("CONNECTING " + host + " " + address_or_name)
         self.wsc.connect(
             auth_token,
             host,
             address_or_name,
             ssl_enabled,
         )
```

### Comparing `spacetimedb_sdk-0.5.0.2/src/spacetimedb_sdk.egg-info/SOURCES.txt` & `spacetimedb_sdk-0.6.0/src/spacetimedb_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

