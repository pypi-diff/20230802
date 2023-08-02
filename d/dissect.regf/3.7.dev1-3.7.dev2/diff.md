# Comparing `tmp/dissect.regf-3.7.dev1.tar.gz` & `tmp/dissect.regf-3.7.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.regf-3.7.dev1.tar", last modified: Thu Jul 20 07:23:05 2023, max compression
+gzip compressed data, was "dissect.regf-3.7.dev2.tar", last modified: Wed Aug  2 13:33:50 2023, max compression
```

## Comparing `dissect.regf-3.7.dev1.tar` & `dissect.regf-3.7.dev2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:23:05.613091 dissect.regf-3.7.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-20 07:23:05.613091 dissect.regf-3.7.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:23:05.601091 dissect.regf-3.7.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:23:05.605091 dissect.regf-3.7.dev1/dissect/regf/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/dissect/regf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/dissect/regf/c_regf.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/dissect/regf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    16939 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/dissect/regf/regf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:23:05.605091 dissect.regf-3.7.dev1/dissect.regf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-07-20 07:23:05.000000 dissect.regf-3.7.dev1/dissect.regf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-20 07:23:05.000000 dissect.regf-3.7.dev1/dissect.regf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 07:23:05.000000 dissect.regf-3.7.dev1/dissect.regf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-20 07:23:05.000000 dissect.regf-3.7.dev1/dissect.regf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 07:23:05.000000 dissect.regf-3.7.dev1/dissect.regf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:23:05.609091 dissect.regf-3.7.dev1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/examples/walkhive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-07-20 07:22:51.000000 dissect.regf-3.7.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 07:23:05.613091 dissect.regf-3.7.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:23:05.609091 dissect.regf-3.7.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:23:05.609091 dissect.regf-3.7.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1969086 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/tests/data/SYSTEM.gz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 07:23:05.613091 dissect.regf-3.7.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/tests/test_regf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-20 07:22:37.000000 dissect.regf-3.7.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:50.753644 dissect.regf-3.7.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-08-02 13:33:50.753644 dissect.regf-3.7.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:50.741644 dissect.regf-3.7.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:50.749644 dissect.regf-3.7.dev2/dissect/regf/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/dissect/regf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/dissect/regf/c_regf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/dissect/regf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/dissect/regf/regf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:50.749644 dissect.regf-3.7.dev2/dissect.regf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3099 2023-08-02 13:33:50.000000 dissect.regf-3.7.dev2/dissect.regf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-02 13:33:50.000000 dissect.regf-3.7.dev2/dissect.regf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:33:50.000000 dissect.regf-3.7.dev2/dissect.regf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-02 13:33:50.000000 dissect.regf-3.7.dev2/dissect.regf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 13:33:50.000000 dissect.regf-3.7.dev2/dissect.regf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:50.749644 dissect.regf-3.7.dev2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/examples/walkhive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-08-02 13:33:40.000000 dissect.regf-3.7.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:33:50.757644 dissect.regf-3.7.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:50.749644 dissect.regf-3.7.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:50.753644 dissect.regf-3.7.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)  1969086 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/tests/data/SYSTEM.gz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:50.753644 dissect.regf-3.7.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/tests/test_regf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-02 13:33:35.000000 dissect.regf-3.7.dev2/tox.ini
```

### Comparing `dissect.regf-3.7.dev1/LICENSE` & `dissect.regf-3.7.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.7.dev1/PKG-INFO` & `dissect.regf-3.7.dev2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.regf
-Version: 3.7.dev1
+Version: 3.7.dev2
 Summary: A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.regf
 Project-URL: repository, https://github.com/fox-it/dissect.regf
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.regf-3.7.dev1/README.md` & `dissect.regf-3.7.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.7.dev1/dissect/regf/c_regf.py` & `dissect.regf-3.7.dev2/dissect/regf/c_regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.7.dev1/dissect/regf/regf.py` & `dissect.regf-3.7.dev2/dissect/regf/regf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 import struct
 import sys
 from functools import lru_cache
 from io import BytesIO
+from typing import Union
 
 from dissect.util.ts import wintimestamp
 
 from dissect.regf.c_regf import (
     REG_BINARY,
     REG_DWORD,
     REG_DWORD_BIG_ENDIAN,
@@ -318,64 +319,18 @@
                         data = b"".join(parts)
 
                         # assert(len(data) == data_size)
                         data = data[:data_size]
             self._data = data
         return self._data
 
-    def parse_value(self):
-        data = self.data
-
-        if self.kv.data_type in (REG_DWORD, REG_DWORD_BIG_ENDIAN):
-            if len(data) == 0:
-                return 0
-
-            if self.kv.data_type == REG_DWORD:
-                return c_regf.uint32(data[:4])
-            elif self.kv.data_type == REG_DWORD_BIG_ENDIAN:
-                return struct.unpack(">I", data[:4])[0]
-
-        if self.kv.data_type in (REG_SZ, REG_EXPAND_SZ):
-            return try_decode_sz(data)
-
-        if self.kv.data_type in (REG_BINARY, REG_NONE):
-            return data
-
-        if self.kv.data_type == REG_MULTI_SZ:
-            data_len = len(data)
-            data = BytesIO(data)
-
-            multi_string = []
-            while data.tell() < data_len:
-                string = read_null_terminated_wstring(data)
-                if string == "":
-                    break
-
-                multi_string.append(string)
-
-            return multi_string
-
-        if self.kv.data_type == REG_QWORD:
-            return c_regf.uint64(data) if len(data) else 0
-
-        if self.kv.data_type == REG_FULL_RESOURCE_DESCRIPTOR:
-            log.warning("Unimplemented REG_FULL_RESOURCE_DESCRIPTOR")
-            return data
-
-        if self.kv.data_type == REG_RESOURCE_REQUIREMENTS_LIST:
-            log.warning("Unimplemented REG_RESOURCE_REQUIREMENTS_LIST")
-            return data
-
-        log.warning("Data type 0x%x not supported", self.kv.data_type)
-        return data
-
     @property
     def value(self):
         if self._value is None:
-            self._value = self.parse_value()
+            self._value = parse_value(self.kv.data_type, self.data)
         return self._value
 
     def __repr__(self):
         return f"<KeyValue {self.name}={self.value!r}>"
 
 
 class ValueList:
@@ -528,14 +483,59 @@
     except UnicodeDecodeError:
         # Last ditch effort, decode the whole bytestring as if it were utf-16,
         # any decoding errors, which incase of utf-16 will be invalid utf-16
         # surrogates, will be ignored.
         return data.decode("utf-16-le", "ignore").strip("\x00")
 
 
+def parse_value(data_type: int, data: bytes) -> Union[int, str, list[str], bytes]:
+    if data_type in (REG_DWORD, REG_DWORD_BIG_ENDIAN):
+        if len(data) == 0:
+            return 0
+
+        if data_type == REG_DWORD:
+            return c_regf.uint32(data[:4])
+        elif data_type == REG_DWORD_BIG_ENDIAN:
+            return struct.unpack(">I", data[:4])[0]
+
+    if data_type == REG_QWORD:
+        return c_regf.uint64(data) if len(data) else 0
+
+    if data_type in (REG_SZ, REG_EXPAND_SZ):
+        return try_decode_sz(data)
+
+    if data_type in (REG_BINARY, REG_NONE):
+        return data
+
+    if data_type == REG_MULTI_SZ:
+        data_len = len(data)
+        data = BytesIO(data)
+
+        multi_string = []
+        while data.tell() < data_len:
+            string = read_null_terminated_wstring(data)
+            if string == "":
+                break
+
+            multi_string.append(string)
+
+        return multi_string
+
+    if data_type == REG_FULL_RESOURCE_DESCRIPTOR:
+        log.warning("Unimplemented REG_FULL_RESOURCE_DESCRIPTOR")
+        return data
+
+    if data_type == REG_RESOURCE_REQUIREMENTS_LIST:
+        log.warning("Unimplemented REG_RESOURCE_REQUIREMENTS_LIST")
+        return data
+
+    log.warning("Data type 0x%x not supported", data_type)
+    return data
+
+
 def read_null_terminated_wstring(stream, encoding="utf-16-le"):
     """Adapted function to read null terminated wide strings.
 
     The cstruct way raises EOFError when the end of the stream is reached.
     This is fine, but not what we want for this particular implementation.
     """
     wide_string = b""
```

### Comparing `dissect.regf-3.7.dev1/dissect.regf.egg-info/PKG-INFO` & `dissect.regf-3.7.dev2/dissect.regf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.regf
-Version: 3.7.dev1
+Version: 3.7.dev2
 Summary: A Dissect module implementing a parser for Windows registry file format, used to store application and OS configuration on Windows operating systems
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Affero General Public License v3
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.regf
 Project-URL: repository, https://github.com/fox-it/dissect.regf
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.regf-3.7.dev1/pyproject.toml` & `dissect.regf-3.7.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.7.dev1/tests/data/SYSTEM.gz` & `dissect.regf-3.7.dev2/tests/data/SYSTEM.gz`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.7.dev1/tests/docs/Makefile` & `dissect.regf-3.7.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.7.dev1/tests/docs/conf.py` & `dissect.regf-3.7.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.7.dev1/tests/test_regf.py` & `dissect.regf-3.7.dev2/tests/test_regf.py`

 * *Files identical despite different names*

### Comparing `dissect.regf-3.7.dev1/tox.ini` & `dissect.regf-3.7.dev2/tox.ini`

 * *Files identical despite different names*

