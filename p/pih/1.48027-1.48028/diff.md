# Comparing `tmp/pih-1.48027.tar.gz` & `tmp/pih-1.48028.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48027.tar", last modified: Wed Aug  2 06:34:26 2023, max compression
+gzip compressed data, was "pih-1.48028.tar", last modified: Wed Aug  2 07:05:51 2023, max compression
```

## Comparing `pih-1.48027.tar` & `pih-1.48028.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 06:34:26.621709 pih-1.48027/
--rw-rw-rw-   0        0        0      261 2023-08-02 06:34:26.621709 pih-1.48027/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 06:34:26.449792 pih-1.48027/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48027/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48027/pih/collection.py
--rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48027/pih/console_api.py
--rw-rw-rw-   0        0        0   111638 2023-08-02 05:09:57.000000 pih-1.48027/pih/const.py
--rw-rw-rw-   0        0        0   317651 2023-08-02 06:34:15.000000 pih-1.48027/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48027/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48027/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48027/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48027/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48027/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48027/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48027/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48027/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-02 06:34:26.590417 pih-1.48027/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-02 06:34:24.000000 pih-1.48027/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-02 06:34:25.000000 pih-1.48027/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 06:34:24.000000 pih-1.48027/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-02 06:34:25.000000 pih-1.48027/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-02 06:34:25.000000 pih-1.48027/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48027/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-02 06:34:26.621709 pih-1.48027/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 07:05:51.058216 pih-1.48028/
+-rw-rw-rw-   0        0        0      261 2023-08-02 07:05:51.964459 pih-1.48028/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 07:05:51.761334 pih-1.48028/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48028/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48028/pih/collection.py
+-rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48028/pih/console_api.py
+-rw-rw-rw-   0        0        0   111638 2023-08-02 05:09:57.000000 pih-1.48028/pih/const.py
+-rw-rw-rw-   0        0        0   317985 2023-08-02 07:04:46.000000 pih-1.48028/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48028/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48028/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48028/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48028/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48028/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48028/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48028/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48028/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:05:51.933206 pih-1.48028/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48028/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:05:51.980126 pih-1.48028/setup.cfg
```

### Comparing `pih-1.48027/pih/collection.py` & `pih-1.48028/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/console_api.py` & `pih-1.48028/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/const.py` & `pih-1.48028/pih/const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/pih.py` & `pih-1.48028/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -1643,15 +1643,15 @@
             
             @staticmethod
             def local() -> str:
                 return "1.48020"  
 
         @staticmethod
         def local() -> str:
-            return "1.48027"
+            return "1.48028"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
@@ -2490,14 +2490,19 @@
         SUPPORT_NAME_PREFIX: str = "_@@Support@@_"
         command_map: dict[str, ServiceDescription] | None = None
 
         class DATA_HOLDER:
             long_operation_listeners: list[Callable[[None], None]] = []
 
         @staticmethod
+        def check_on_host_chanchable(role_or_information: ServiceRoles | ServiceInformationBase) -> bool:
+            description: ServiceDescription = ServiceRoles.description(role_or_information)
+            return not description.host_changeable and StringTool.contains(PIH.OS.host(), description.host)
+
+        @staticmethod
         def call_listeners_on_long_operation() -> None:
             for listener in PIH.SERVICE.DATA_HOLDER.long_operation_listeners:
                 listener()
 
         @staticmethod
         def start_listen_for_long_operation(listener: Callable[[None], None]) -> None:
             PIH.SERVICE.DATA_HOLDER.long_operation_listeners.append(listener)
```

### Comparing `pih-1.48027/pih/rpc.py` & `pih-1.48028/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/rpcCommandCall_pb2.py` & `pih-1.48028/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48028/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/rpc_collection.py` & `pih-1.48028/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/rpc_const.py` & `pih-1.48028/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/service_example.py` & `pih-1.48028/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/tools.py` & `pih-1.48028/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih/widgets.py` & `pih-1.48028/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48027/pih_setup.py` & `pih-1.48028/pih_setup.py`

 * *Files identical despite different names*

