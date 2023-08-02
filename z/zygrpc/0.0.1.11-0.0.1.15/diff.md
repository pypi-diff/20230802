# Comparing `tmp/zygrpc-0.0.1.11.tar.gz` & `tmp/zygrpc-0.0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zygrpc-0.0.1.11.tar", last modified: Mon Nov 28 06:42:09 2022, max compression
+gzip compressed data, was "zygrpc-0.0.1.15.tar", last modified: Wed Aug  2 09:42:22 2023, max compression
```

## Comparing `zygrpc-0.0.1.11.tar` & `zygrpc-0.0.1.15.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 lixi      (1000) lixi      (1000)        0 2022-11-28 06:42:09.983602 zygrpc-0.0.1.11/
--rw-r--r--   0 lixi      (1000) lixi      (1000)     1072 2022-07-14 08:27:43.000000 zygrpc-0.0.1.11/LICENSE
--rw-r--r--   0 lixi      (1000) lixi      (1000)       79 2022-07-14 08:27:55.000000 zygrpc-0.0.1.11/MANIFEST.in
--rw-r--r--   0 lixi      (1000) lixi      (1000)     1982 2022-11-28 06:42:09.983602 zygrpc-0.0.1.11/PKG-INFO
--rw-r--r--   0 lixi      (1000) lixi      (1000)     1186 2022-07-14 08:27:55.000000 zygrpc-0.0.1.11/README.md
-drwxr-xr-x   0 lixi      (1000) lixi      (1000)        0 2022-11-28 06:42:09.983602 zygrpc-0.0.1.11/proto/
--rw-r--r--   0 lixi      (1000) lixi      (1000)     5007 2022-11-28 06:41:06.000000 zygrpc-0.0.1.11/proto/zhiyan_rpc_pb2.py
--rw-r--r--   0 lixi      (1000) lixi      (1000)     5814 2022-11-28 06:41:06.000000 zygrpc-0.0.1.11/proto/zhiyan_rpc_pb2_grpc.py
--rw-r--r--   0 lixi      (1000) lixi      (1000)     1151 2022-07-14 08:27:55.000000 zygrpc-0.0.1.11/pyproject.toml
--rw-r--r--   0 lixi      (1000) lixi      (1000)       35 2022-07-14 08:27:55.000000 zygrpc-0.0.1.11/requirements.txt
--rw-r--r--   0 lixi      (1000) lixi      (1000)       38 2022-11-28 06:42:09.983602 zygrpc-0.0.1.11/setup.cfg
-drwxr-xr-x   0 lixi      (1000) lixi      (1000)        0 2022-11-28 06:42:09.983602 zygrpc-0.0.1.11/zygrpc.egg-info/
--rw-r--r--   0 lixi      (1000) lixi      (1000)     1982 2022-11-28 06:42:09.000000 zygrpc-0.0.1.11/zygrpc.egg-info/PKG-INFO
--rw-r--r--   0 lixi      (1000) lixi      (1000)      311 2022-11-28 06:42:09.000000 zygrpc-0.0.1.11/zygrpc.egg-info/SOURCES.txt
--rw-r--r--   0 lixi      (1000) lixi      (1000)        1 2022-11-28 06:42:09.000000 zygrpc-0.0.1.11/zygrpc.egg-info/dependency_links.txt
--rw-r--r--   0 lixi      (1000) lixi      (1000)       29 2022-11-28 06:42:09.000000 zygrpc-0.0.1.11/zygrpc.egg-info/requires.txt
--rw-r--r--   0 lixi      (1000) lixi      (1000)       18 2022-11-28 06:42:09.000000 zygrpc-0.0.1.11/zygrpc.egg-info/top_level.txt
-drwxr-xr-x   0 lixi      (1000) lixi      (1000)        0 2022-11-28 06:42:09.983602 zygrpc-0.0.1.11/zygrpc_help/
--rw-r--r--   0 lixi      (1000) lixi      (1000)        0 2022-07-14 08:27:55.000000 zygrpc-0.0.1.11/zygrpc_help/__init__.py
--rw-r--r--   0 lixi      (1000) lixi      (1000)        8 2022-08-31 08:50:50.000000 zygrpc-0.0.1.11/zygrpc_help/version.txt
+drwxr-xr-x   0 lixi      (1000) lixi      (1000)        0 2023-08-02 09:42:22.524638 zygrpc-0.0.1.15/
+-rw-r--r--   0 lixi      (1000) lixi      (1000)     1072 2022-07-14 08:27:43.000000 zygrpc-0.0.1.15/LICENSE
+-rw-r--r--   0 lixi      (1000) lixi      (1000)       79 2022-07-14 08:27:55.000000 zygrpc-0.0.1.15/MANIFEST.in
+-rw-r--r--   0 lixi      (1000) lixi      (1000)     1982 2023-08-02 09:42:22.521304 zygrpc-0.0.1.15/PKG-INFO
+-rw-r--r--   0 lixi      (1000) lixi      (1000)     1186 2022-07-14 08:27:55.000000 zygrpc-0.0.1.15/README.md
+drwxr-xr-x   0 lixi      (1000) lixi      (1000)        0 2023-08-02 09:42:22.521304 zygrpc-0.0.1.15/proto/
+-rw-r--r--   0 lixi      (1000) lixi      (1000)     5007 2022-11-28 06:41:06.000000 zygrpc-0.0.1.15/proto/zhiyan_rpc_pb2.py
+-rw-r--r--   0 lixi      (1000) lixi      (1000)     5814 2022-11-28 06:41:06.000000 zygrpc-0.0.1.15/proto/zhiyan_rpc_pb2_grpc.py
+-rw-r--r--   0 lixi      (1000) lixi      (1000)     1151 2022-07-14 08:27:55.000000 zygrpc-0.0.1.15/pyproject.toml
+-rw-r--r--   0 lixi      (1000) lixi      (1000)       35 2022-07-14 08:27:55.000000 zygrpc-0.0.1.15/requirements.txt
+-rw-r--r--   0 lixi      (1000) lixi      (1000)       38 2023-08-02 09:42:22.524638 zygrpc-0.0.1.15/setup.cfg
+drwxr-xr-x   0 lixi      (1000) lixi      (1000)        0 2023-08-02 09:42:22.521304 zygrpc-0.0.1.15/zygrpc.egg-info/
+-rw-r--r--   0 lixi      (1000) lixi      (1000)     1982 2023-08-02 09:42:22.000000 zygrpc-0.0.1.15/zygrpc.egg-info/PKG-INFO
+-rw-r--r--   0 lixi      (1000) lixi      (1000)      311 2023-08-02 09:42:22.000000 zygrpc-0.0.1.15/zygrpc.egg-info/SOURCES.txt
+-rw-r--r--   0 lixi      (1000) lixi      (1000)        1 2023-08-02 09:42:22.000000 zygrpc-0.0.1.15/zygrpc.egg-info/dependency_links.txt
+-rw-r--r--   0 lixi      (1000) lixi      (1000)       29 2023-08-02 09:42:22.000000 zygrpc-0.0.1.15/zygrpc.egg-info/requires.txt
+-rw-r--r--   0 lixi      (1000) lixi      (1000)       18 2023-08-02 09:42:22.000000 zygrpc-0.0.1.15/zygrpc.egg-info/top_level.txt
+drwxr-xr-x   0 lixi      (1000) lixi      (1000)        0 2023-08-02 09:42:22.521304 zygrpc-0.0.1.15/zygrpc_help/
+-rw-r--r--   0 lixi      (1000) lixi      (1000)        0 2022-07-14 08:27:55.000000 zygrpc-0.0.1.15/zygrpc_help/__init__.py
+-rw-r--r--   0 lixi      (1000) lixi      (1000)        8 2023-06-05 02:03:43.000000 zygrpc-0.0.1.15/zygrpc_help/version.txt
```

### Comparing `zygrpc-0.0.1.11/LICENSE` & `zygrpc-0.0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `zygrpc-0.0.1.11/PKG-INFO` & `zygrpc-0.0.1.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zygrpc
-Version: 0.0.1.11
+Version: 0.0.1.15
 Summary: ZhiYan Python gRPC SDK
 Author-email: Chengdu Geek Camp <lq@cdgeekcamp.com>
 License: MIT
 Project-URL: Documentation, https://gitee.com/warp-drive-tech/libzygrpc
 Project-URL: Source, https://gitee.com/warp-drive-tech/libzygrpc
 Project-URL: Home-page, https://gitee.com/warp-drive-tech/libzygrpc
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `zygrpc-0.0.1.11/README.md` & `zygrpc-0.0.1.15/README.md`

 * *Files identical despite different names*

### Comparing `zygrpc-0.0.1.11/proto/zhiyan_rpc_pb2.py` & `zygrpc-0.0.1.15/proto/zhiyan_rpc_pb2.py`

 * *Files identical despite different names*

### Comparing `zygrpc-0.0.1.11/proto/zhiyan_rpc_pb2_grpc.py` & `zygrpc-0.0.1.15/proto/zhiyan_rpc_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `zygrpc-0.0.1.11/pyproject.toml` & `zygrpc-0.0.1.15/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zygrpc-0.0.1.11/zygrpc.egg-info/PKG-INFO` & `zygrpc-0.0.1.15/zygrpc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zygrpc
-Version: 0.0.1.11
+Version: 0.0.1.15
 Summary: ZhiYan Python gRPC SDK
 Author-email: Chengdu Geek Camp <lq@cdgeekcamp.com>
 License: MIT
 Project-URL: Documentation, https://gitee.com/warp-drive-tech/libzygrpc
 Project-URL: Source, https://gitee.com/warp-drive-tech/libzygrpc
 Project-URL: Home-page, https://gitee.com/warp-drive-tech/libzygrpc
 Classifier: Operating System :: POSIX :: Linux
```

