# Comparing `tmp/pih-1.48028.tar.gz` & `tmp/pih-1.48029.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-1.48028.tar", last modified: Wed Aug  2 07:05:51 2023, max compression
+gzip compressed data, was "pih-1.48029.tar", last modified: Wed Aug  2 07:45:33 2023, max compression
```

## Comparing `pih-1.48028.tar` & `pih-1.48029.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:05:51.058216 pih-1.48028/
--rw-rw-rw-   0        0        0      261 2023-08-02 07:05:51.964459 pih-1.48028/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 07:05:51.761334 pih-1.48028/pih/
--rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48028/pih/__init__.py
--rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48028/pih/collection.py
--rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48028/pih/console_api.py
--rw-rw-rw-   0        0        0   111638 2023-08-02 05:09:57.000000 pih-1.48028/pih/const.py
--rw-rw-rw-   0        0        0   317985 2023-08-02 07:04:46.000000 pih-1.48028/pih/pih.py
--rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48028/pih/rpc.py
--rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48028/pih/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48028/pih/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48028/pih/rpc_collection.py
--rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48028/pih/rpc_const.py
--rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48028/pih/service_example.py
--rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48028/pih/tools.py
--rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48028/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:05:51.933206 pih-1.48028/pih.egg-info/
--rw-rw-rw-   0        0        0      261 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-02 07:05:50.000000 pih-1.48028/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48028/pih_setup.py
--rw-rw-rw-   0        0        0       42 2023-08-02 07:05:51.980126 pih-1.48028/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 07:45:33.855038 pih-1.48029/
+-rw-rw-rw-   0        0        0      261 2023-08-02 07:45:33.855038 pih-1.48029/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 07:45:33.261299 pih-1.48029/pih/
+-rw-rw-rw-   0        0        0      157 2022-12-03 14:38:35.000000 pih-1.48029/pih/__init__.py
+-rw-rw-rw-   0        0        0    20482 2023-07-25 14:36:49.000000 pih-1.48029/pih/collection.py
+-rw-rw-rw-   0        0        0    60753 2023-08-01 04:09:10.000000 pih-1.48029/pih/console_api.py
+-rw-rw-rw-   0        0        0   111167 2023-08-02 07:34:14.000000 pih-1.48029/pih/const.py
+-rw-rw-rw-   0        0        0   317983 2023-08-02 07:45:25.000000 pih-1.48029/pih/pih.py
+-rw-rw-rw-   0        0        0    24697 2023-07-28 13:13:08.000000 pih-1.48029/pih/rpc.py
+-rw-rw-rw-   0        0        0     1941 2022-07-31 10:55:18.000000 pih-1.48029/pih/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2465 2022-08-05 02:38:47.000000 pih-1.48029/pih/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0     2576 2023-07-31 23:11:58.000000 pih-1.48029/pih/rpc_collection.py
+-rw-rw-rw-   0        0        0     6453 2023-07-24 14:50:22.000000 pih-1.48029/pih/rpc_const.py
+-rw-rw-rw-   0        0        0      635 2023-06-11 13:35:46.000000 pih-1.48029/pih/service_example.py
+-rw-rw-rw-   0        0        0    38229 2023-08-01 02:41:41.000000 pih-1.48029/pih/tools.py
+-rw-rw-rw-   0        0        0     2280 2023-06-30 04:39:52.000000 pih-1.48029/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:45:33.823792 pih-1.48029/pih.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-08-02 07:45:31.000000 pih-1.48029/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2023-08-02 07:45:32.000000 pih-1.48029/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:45:31.000000 pih-1.48029/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2023-08-02 07:45:32.000000 pih-1.48029/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-02 07:45:32.000000 pih-1.48029/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2009 2023-08-01 00:47:12.000000 pih-1.48029/pih_setup.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:45:33.855038 pih-1.48029/setup.cfg
```

### Comparing `pih-1.48028/pih/collection.py` & `pih-1.48029/pih/collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/console_api.py` & `pih-1.48029/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/const.py` & `pih-1.48029/pih/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -1461,28 +1461,14 @@
             ServiceCommands.on_service_stops,
             ServiceCommands.get_service_information_table,
             ServiceCommands.heart_beat
         ],
         modules=["schedule", "lmdbm"]
     )
 
-    '''SERVICE_ADMIN: ServiceDescription = ServiceDescription(
-        name="ServiceAdmin",
-        description="Service admin",
-        host=CONST.HOST.DC1.NAME,
-        port=CONST.RPC.PORT(20),
-        host_changeable=False,
-        commands=[
-            ServiceCommands.on_service_starts,
-            ServiceCommands.on_service_stops,
-            ServiceCommands.get_service_information_table,
-            ServiceCommands.heart_beat
-        ]
-    )'''
-
     EVENT_AND_LOG: ServiceDescription = ServiceDescription(
                                             name="EventAndLog",
                                             description="Log and Event service",
                                             host=CONST.HOST.BACKUP_WORKER.NAME, 
                                             commands=[
                                                         ServiceCommands.send_log_message,
                                                         ServiceCommands.send_event
```

### Comparing `pih-1.48028/pih/pih.py` & `pih-1.48029/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,14 @@
 import urllib.parse
 
 from transliterate import translit
 
 pih_is_exists = importlib.util.find_spec("pih") is not None
 if not pih_is_exists:
     sys.path.append("//pih/facade")
-
 from pih.collection import  *
 from pih.tools import *
 from pih.const import *
 from pih.rpc_collection import *
 from pih.rpc import *
 from pih.rpc_const import *
 
@@ -1639,19 +1638,19 @@
 
     class VERSION:
 
         class MIO:
             
             @staticmethod
             def local() -> str:
-                return "1.48020"  
+                return "1.48022"  
 
         @staticmethod
         def local() -> str:
-            return "1.48028"
+            return "1.48029"
 
         @staticmethod
         def need_update() -> bool:
             return False
             #return importlib.util.find_spec(PIH.NAME) is not None and PIH.VERSION.local() < PIH.VERSION.remote()
     
     class INPUT_WAIT:
```

### Comparing `pih-1.48028/pih/rpc.py` & `pih-1.48029/pih/rpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/rpcCommandCall_pb2.py` & `pih-1.48029/pih/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/rpcCommandCall_pb2_grpc.py` & `pih-1.48029/pih/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/rpc_collection.py` & `pih-1.48029/pih/rpc_collection.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/rpc_const.py` & `pih-1.48029/pih/rpc_const.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/service_example.py` & `pih-1.48029/pih/service_example.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/tools.py` & `pih-1.48029/pih/tools.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih/widgets.py` & `pih-1.48029/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-1.48028/pih_setup.py` & `pih-1.48029/pih_setup.py`

 * *Files identical despite different names*

