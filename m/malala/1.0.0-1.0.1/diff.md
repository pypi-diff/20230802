# Comparing `tmp/malala-1.0.0.tar.gz` & `tmp/malala-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "malala-1.0.0.tar", last modified: Tue Aug  1 19:48:40 2023, max compression
+gzip compressed data, was "malala-1.0.1.tar", last modified: Wed Aug  2 18:16:41 2023, max compression
```

## Comparing `malala-1.0.0.tar` & `malala-1.0.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.428255 malala-1.0.0/
--rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 19:48:40.428143 malala-1.0.0/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-01 02:16:10.000000 malala-1.0.0/README.md
--rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-01 19:48:40.428290 malala-1.0.0/setup.cfg
--rw-r--r--   0 jmf        (501) staff       (20)      466 2023-08-01 19:47:59.000000 malala-1.0.0/setup.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.425506 malala-1.0.0/src/
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.426154 malala-1.0.0/src/malala/
--rw-r--r--   0 jmf        (501) staff       (20)       69 2023-08-01 19:41:47.000000 malala-1.0.0/src/malala/__init__.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.426931 malala-1.0.0/src/malala/constants/
--rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-01 02:23:15.000000 malala-1.0.0/src/malala/constants/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)       75 2023-08-01 01:09:45.000000 malala-1.0.0/src/malala/constants/sockets.py
--rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-01 00:55:04.000000 malala-1.0.0/src/malala/constants/time.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.427146 malala-1.0.0/src/malala/logger/
--rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:55:01.000000 malala-1.0.0/src/malala/logger/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-01 00:43:31.000000 malala-1.0.0/src/malala/logger/logging.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.427759 malala-1.0.0/src/malala/sockets/
--rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-01 01:16:34.000000 malala-1.0.0/src/malala/sockets/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-01 01:15:29.000000 malala-1.0.0/src/malala/sockets/tcp_socket.py
--rw-r--r--   0 jmf        (501) staff       (20)     1189 2023-08-01 19:41:49.000000 malala-1.0.0/src/malala/sockets/transport.py
--rw-r--r--   0 jmf        (501) staff       (20)      735 2023-08-01 19:26:05.000000 malala-1.0.0/src/malala/sockets/unix_socket.py
--rw-r--r--   0 jmf        (501) staff       (20)     1835 2023-08-01 19:26:27.000000 malala-1.0.0/src/malala/sockets/websocket.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.428003 malala-1.0.0/src/malala/tasks/
--rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-01 01:18:20.000000 malala-1.0.0/src/malala/tasks/__init__.py
--rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-01 01:17:48.000000 malala-1.0.0/src/malala/tasks/tasks.py
-drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-01 19:48:40.426608 malala-1.0.0/src/malala.egg-info/
--rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-01 19:48:40.000000 malala-1.0.0/src/malala.egg-info/PKG-INFO
--rw-r--r--   0 jmf        (501) staff       (20)      547 2023-08-01 19:48:40.000000 malala-1.0.0/src/malala.egg-info/SOURCES.txt
--rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-01 19:48:40.000000 malala-1.0.0/src/malala.egg-info/dependency_links.txt
--rw-r--r--   0 jmf        (501) staff       (20)        7 2023-08-01 19:48:40.000000 malala-1.0.0/src/malala.egg-info/top_level.txt
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-02 18:16:41.224680 malala-1.0.1/
+-rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-02 18:16:41.224543 malala-1.0.1/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      116 2023-08-02 18:06:35.000000 malala-1.0.1/README.md
+-rw-r--r--   0 jmf        (501) staff       (20)       38 2023-08-02 18:16:41.224719 malala-1.0.1/setup.cfg
+-rw-r--r--   0 jmf        (501) staff       (20)      466 2023-08-02 18:15:50.000000 malala-1.0.1/setup.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-02 18:16:41.221814 malala-1.0.1/src/
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-02 18:16:41.222534 malala-1.0.1/src/malala/
+-rw-r--r--   0 jmf        (501) staff       (20)       69 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/__init__.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-02 18:16:41.223338 malala-1.0.1/src/malala/constants/
+-rw-r--r--   0 jmf        (501) staff       (20)       43 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/constants/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)       58 2023-08-02 18:11:59.000000 malala-1.0.1/src/malala/constants/sockets.py
+-rw-r--r--   0 jmf        (501) staff       (20)       42 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/constants/time.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-02 18:16:41.223552 malala-1.0.1/src/malala/logger/
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/logger/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)        0 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/logger/logging.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-02 18:16:41.224159 malala-1.0.1/src/malala/sockets/
+-rw-r--r--   0 jmf        (501) staff       (20)      102 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/sockets/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      562 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/sockets/tcp_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1153 2023-08-02 18:12:40.000000 malala-1.0.1/src/malala/sockets/transport.py
+-rw-r--r--   0 jmf        (501) staff       (20)      735 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/sockets/unix_socket.py
+-rw-r--r--   0 jmf        (501) staff       (20)     1835 2023-08-02 18:13:35.000000 malala-1.0.1/src/malala/sockets/websocket.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-02 18:16:41.224388 malala-1.0.1/src/malala/tasks/
+-rw-r--r--   0 jmf        (501) staff       (20)       31 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/tasks/__init__.py
+-rw-r--r--   0 jmf        (501) staff       (20)      665 2023-08-02 18:06:35.000000 malala-1.0.1/src/malala/tasks/tasks.py
+drwxr-xr-x   0 jmf        (501) staff       (20)        0 2023-08-02 18:16:41.222993 malala-1.0.1/src/malala.egg-info/
+-rw-r--r--   0 jmf        (501) staff       (20)      208 2023-08-02 18:16:41.000000 malala-1.0.1/src/malala.egg-info/PKG-INFO
+-rw-r--r--   0 jmf        (501) staff       (20)      547 2023-08-02 18:16:41.000000 malala-1.0.1/src/malala.egg-info/SOURCES.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        1 2023-08-02 18:16:41.000000 malala-1.0.1/src/malala.egg-info/dependency_links.txt
+-rw-r--r--   0 jmf        (501) staff       (20)        7 2023-08-02 18:16:41.000000 malala-1.0.1/src/malala.egg-info/top_level.txt
```

### Comparing `malala-1.0.0/src/malala/sockets/tcp_socket.py` & `malala-1.0.1/src/malala/sockets/tcp_socket.py`

 * *Files identical despite different names*

### Comparing `malala-1.0.0/src/malala/sockets/transport.py` & `malala-1.0.1/src/malala/sockets/transport.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import json
 from asyncio import StreamReader, StreamWriter
 from typing import AsyncGenerator
-from ..constants.sockets import B_DELIM, S_DELIM
+from ..constants.sockets import DELIM
 
 
 class Transport:
     @staticmethod
     async def recv_bytes(reader: StreamReader) -> AsyncGenerator[bytes, None]:
         async for _bytes in reader:
-            yield _bytes
+            yield _bytes[0:len(_bytes)-1]
 
     @staticmethod
     async def recv_str(reader: StreamReader) -> AsyncGenerator[str, None]:
         async for _bytes in reader:
-            yield _bytes.decode().split(S_DELIM)[0]
+            yield _bytes.decode()
 
     @staticmethod
     async def recv_json(reader: StreamReader) -> AsyncGenerator[dict, None]:
         async for _bytes in reader:
-            yield json.loads(_bytes.decode().split(S_DELIM)[0])
+            yield json.loads(_bytes.decode())
 
     @staticmethod
     async def send_bytes(_bytes: bytes, writer: StreamWriter) -> None:
-        writer.write(_bytes + B_DELIM)
+        writer.write(_bytes + DELIM)
         await writer.drain()
 
     @staticmethod
     async def send_str(_str: str, writer: StreamWriter) -> None:
-        writer.write(_str.encode() + B_DELIM)
+        writer.write(_str.encode() + DELIM)
         await writer.drain()
 
     @staticmethod
     async def send_json(_json: dict, writer: StreamWriter) -> None:
-        writer.write(json.dumps(_json).encode() + B_DELIM)
+        writer.write(json.dumps(_json).encode() + DELIM)
         await writer.drain()
```

### Comparing `malala-1.0.0/src/malala/sockets/unix_socket.py` & `malala-1.0.1/src/malala/sockets/unix_socket.py`

 * *Files identical despite different names*

### Comparing `malala-1.0.0/src/malala/sockets/websocket.py` & `malala-1.0.1/src/malala/sockets/websocket.py`

 * *Files identical despite different names*

### Comparing `malala-1.0.0/src/malala/tasks/tasks.py` & `malala-1.0.1/src/malala/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `malala-1.0.0/src/malala.egg-info/SOURCES.txt` & `malala-1.0.1/src/malala.egg-info/SOURCES.txt`

 * *Files identical despite different names*

