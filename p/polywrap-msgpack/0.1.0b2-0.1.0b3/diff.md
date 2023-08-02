# Comparing `tmp/polywrap_msgpack-0.1.0b2.tar.gz` & `tmp/polywrap_msgpack-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_msgpack-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_msgpack-0.1.0b3.tar", max compression
```

## Comparing `polywrap_msgpack-0.1.0b2.tar` & `polywrap_msgpack-0.1.0b3.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      704 2023-04-10 13:52:54.315489 polywrap_msgpack-0.1.0b2/README.md
--rw-r--r--   0        0        0      431 2023-06-15 11:56:46.973128 polywrap_msgpack-0.1.0b2/polywrap_msgpack/__init__.py
--rw-r--r--   0        0        0     2100 2023-06-15 11:56:46.970636 polywrap_msgpack-0.1.0b2/polywrap_msgpack/decoder.py
--rw-r--r--   0        0        0     2432 2023-06-15 11:56:46.974158 polywrap_msgpack-0.1.0b2/polywrap_msgpack/encoder.py
--rw-r--r--   0        0        0      781 2023-06-15 11:56:46.971165 polywrap_msgpack-0.1.0b2/polywrap_msgpack/errors.py
--rw-r--r--   0        0        0      316 2023-04-10 13:52:54.312333 polywrap_msgpack-0.1.0b2/polywrap_msgpack/extensions/__init__.py
--rw-r--r--   0        0        0     3126 2023-06-15 11:56:46.972978 polywrap_msgpack-0.1.0b2/polywrap_msgpack/extensions/generic_map.py
--rw-r--r--   0        0        0        0 2023-04-10 13:52:54.311842 polywrap_msgpack-0.1.0b2/polywrap_msgpack/py.typed
--rw-r--r--   0        0        0     2893 2023-06-15 11:56:46.974132 polywrap_msgpack-0.1.0b2/polywrap_msgpack/sanitize.py
--rw-r--r--   0        0        0     1205 2023-08-02 11:13:54.491151 polywrap_msgpack-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1396 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0b2/setup.py
--rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      704 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/README.md
+-rw-r--r--   0        0        0      431 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/polywrap_msgpack/__init__.py
+-rw-r--r--   0        0        0     2100 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/polywrap_msgpack/decoder.py
+-rw-r--r--   0        0        0     2432 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/polywrap_msgpack/encoder.py
+-rw-r--r--   0        0        0      781 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/polywrap_msgpack/errors.py
+-rw-r--r--   0        0        0      316 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/polywrap_msgpack/extensions/__init__.py
+-rw-r--r--   0        0        0     3126 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/polywrap_msgpack/extensions/generic_map.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/polywrap_msgpack/py.typed
+-rw-r--r--   0        0        0     2893 2023-08-02 16:06:36.159338 polywrap_msgpack-0.1.0b3/polywrap_msgpack/sanitize.py
+-rw-r--r--   0        0        0     1205 2023-08-02 16:07:05.249592 polywrap_msgpack-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1104 1970-01-01 00:00:00.000000 polywrap_msgpack-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_msgpack-0.1.0b2/README.md` & `polywrap_msgpack-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_msgpack-0.1.0b2/polywrap_msgpack/decoder.py` & `polywrap_msgpack-0.1.0b3/polywrap_msgpack/decoder.py`

 * *Files identical despite different names*

### Comparing `polywrap_msgpack-0.1.0b2/polywrap_msgpack/encoder.py` & `polywrap_msgpack-0.1.0b3/polywrap_msgpack/encoder.py`

 * *Files identical despite different names*

### Comparing `polywrap_msgpack-0.1.0b2/polywrap_msgpack/errors.py` & `polywrap_msgpack-0.1.0b3/polywrap_msgpack/errors.py`

 * *Files identical despite different names*

### Comparing `polywrap_msgpack-0.1.0b2/polywrap_msgpack/extensions/generic_map.py` & `polywrap_msgpack-0.1.0b3/polywrap_msgpack/extensions/generic_map.py`

 * *Files identical despite different names*

### Comparing `polywrap_msgpack-0.1.0b2/polywrap_msgpack/sanitize.py` & `polywrap_msgpack-0.1.0b3/polywrap_msgpack/sanitize.py`

 * *Files identical despite different names*

### Comparing `polywrap_msgpack-0.1.0b2/pyproject.toml` & `polywrap_msgpack-0.1.0b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-msgpack"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "WRAP msgpack encoding"
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 msgpack = "^1.0.4"
```

### Comparing `polywrap_msgpack-0.1.0b2/PKG-INFO` & `polywrap_msgpack-0.1.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polywrap-msgpack
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: WRAP msgpack encoding
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

