# Comparing `tmp/shshsh-1.0.3.tar.gz` & `tmp/shshsh-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shshsh-1.0.3.tar", max compression
+gzip compressed data, was "shshsh-1.0.4.tar", max compression
```

## Comparing `shshsh-1.0.3.tar` & `shshsh-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2420 2023-08-01 19:44:09.097627 shshsh-1.0.3/README.md
--rw-r--r--   0        0        0      345 2023-08-02 16:57:55.567845 shshsh-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      176 2023-08-01 18:14:56.490713 shshsh-1.0.3/shshsh/__init__.py
--rw-r--r--   0        0        0       52 2023-08-01 19:00:12.394172 shshsh-1.0.3/shshsh/global_vars.py
--rw-r--r--   0        0        0      449 2023-07-29 15:04:40.678142 shshsh-1.0.3/shshsh/pipe.py
--rw-r--r--   0        0        0     2656 2023-08-01 19:05:37.427520 shshsh-1.0.3/shshsh/quick.py
--rw-r--r--   0        0        0    14720 2023-08-02 16:53:09.951165 shshsh-1.0.3/shshsh/shell.py
--rw-r--r--   0        0        0     5748 2023-08-01 19:06:50.924190 shshsh-1.0.3/shshsh/streamer.py
--rw-r--r--   0        0        0      934 2023-08-01 19:23:06.874235 shshsh-1.0.3/shshsh/utils.py
--rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 shshsh-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2420 2023-08-01 19:44:09.097627 shshsh-1.0.4/README.md
+-rw-r--r--   0        0        0      345 2023-08-02 17:27:43.824595 shshsh-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-08-01 18:14:56.490713 shshsh-1.0.4/shshsh/__init__.py
+-rw-r--r--   0        0        0       52 2023-08-01 19:00:12.394172 shshsh-1.0.4/shshsh/global_vars.py
+-rw-r--r--   0        0        0      449 2023-07-29 15:04:40.678142 shshsh-1.0.4/shshsh/pipe.py
+-rw-r--r--   0        0        0     2656 2023-08-01 19:05:37.427520 shshsh-1.0.4/shshsh/quick.py
+-rw-r--r--   0        0        0    14720 2023-08-02 16:53:09.951165 shshsh-1.0.4/shshsh/shell.py
+-rw-r--r--   0        0        0     5748 2023-08-02 17:27:19.601260 shshsh-1.0.4/shshsh/streamer.py
+-rw-r--r--   0        0        0      934 2023-08-01 19:23:06.874235 shshsh-1.0.4/shshsh/utils.py
+-rw-r--r--   0        0        0     2878 1970-01-01 00:00:00.000000 shshsh-1.0.4/PKG-INFO
```

### Comparing `shshsh-1.0.3/README.md` & `shshsh-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `shshsh-1.0.3/shshsh/quick.py` & `shshsh-1.0.4/shshsh/quick.py`

 * *Files identical despite different names*

### Comparing `shshsh-1.0.3/shshsh/shell.py` & `shshsh-1.0.4/shshsh/shell.py`

 * *Files identical despite different names*

### Comparing `shshsh-1.0.3/shshsh/streamer.py` & `shshsh-1.0.4/shshsh/streamer.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,20 @@
     from .shell import Sh
 
 
 def bytes_streamer(stream: IO[bytes], sep: bytes = b"\n", chunk_size: int = 1024):
     chunk_data = b""
     while True:
         chunk_data += stream.read(chunk_size)
+        if not chunk_data:
+            return
         chunks = chunk_data.split(sep)
         for chunk in chunks[:-1]:
             yield chunk
         chunk_data = chunks[-1]
-        if not chunk_data:
-            return
 
 
 def str_streamer(stream: IO[bytes], sep: str = "\n", chunk_size: int = 1024):
     for chunk in bytes_streamer(stream, sep=sep.encode("utf8"), chunk_size=chunk_size):
         yield chunk.decode("utf8")
```

### Comparing `shshsh-1.0.3/shshsh/utils.py` & `shshsh-1.0.4/shshsh/utils.py`

 * *Files identical despite different names*

### Comparing `shshsh-1.0.3/PKG-INFO` & `shshsh-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shshsh
-Version: 1.0.3
+Version: 1.0.4
 Summary: bridge of python and shell
 Author: zqqqqz2000
 Author-email: zqqqqz2000@sina.cn
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

