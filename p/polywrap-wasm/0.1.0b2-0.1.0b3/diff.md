# Comparing `tmp/polywrap_wasm-0.1.0b2.tar.gz` & `tmp/polywrap_wasm-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_wasm-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_wasm-0.1.0b3.tar", max compression
```

## Comparing `polywrap_wasm-0.1.0b2.tar` & `polywrap_wasm-0.1.0b3.tar`

### file list

```diff
@@ -1,40 +1,39 @@
--rw-r--r--   0        0        0      872 2023-06-19 11:17:54.183806 polywrap_wasm-0.1.0b2/README.md
--rw-r--r--   0        0        0      182 2023-06-15 11:56:47.045912 polywrap_wasm-0.1.0b2/polywrap_wasm/__init__.py
--rw-r--r--   0        0        0     3699 2023-06-15 11:56:47.040006 polywrap_wasm-0.1.0b2/polywrap_wasm/buffer.py
--rw-r--r--   0        0        0      282 2023-06-15 11:56:47.040220 polywrap_wasm-0.1.0b2/polywrap_wasm/constants.py
--rw-r--r--   0        0        0      491 2023-06-26 13:04:45.471009 polywrap_wasm-0.1.0b2/polywrap_wasm/errors.py
--rw-r--r--   0        0        0     1693 2023-06-15 11:56:47.042772 polywrap_wasm-0.1.0b2/polywrap_wasm/exports.py
--rw-r--r--   0        0        0       85 2023-04-10 13:52:54.342282 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/__init__.py
--rw-r--r--   0        0        0     1854 2023-06-27 11:43:01.070420 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/abort.py
--rw-r--r--   0        0        0      604 2023-06-15 11:56:47.043435 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/debug.py
--rw-r--r--   0        0        0      940 2023-06-15 11:56:47.044618 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/env.py
--rw-r--r--   0        0        0     3046 2023-06-27 11:43:01.070891 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/get_implementations.py
--rw-r--r--   0        0        0     2372 2023-06-15 11:56:47.046320 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/invoke.py
--rw-r--r--   0        0        0     5182 2023-06-18 17:25:19.893387 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/subinvoke.py
--rw-r--r--   0        0        0      111 2023-04-10 13:52:54.345487 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/types/__init__.py
--rw-r--r--   0        0        0     1657 2023-06-15 11:56:47.055639 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/types/base_wrap_imports.py
--rw-r--r--   0        0        0     1626 2023-06-15 11:56:47.049717 polywrap_wasm-0.1.0b2/polywrap_wasm/imports/wrap_imports.py
--rw-r--r--   0        0        0     1637 2023-06-15 11:56:47.057278 polywrap_wasm-0.1.0b2/polywrap_wasm/inmemory_file_reader.py
--rw-r--r--   0        0        0     1162 2023-06-15 11:56:47.052015 polywrap_wasm-0.1.0b2/polywrap_wasm/instance.py
--rw-r--r--   0        0        0      100 2023-04-10 13:52:54.347457 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/__init__.py
--rw-r--r--   0        0        0     1143 2023-04-10 13:52:54.347682 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/abort.py
--rw-r--r--   0        0        0      865 2023-04-10 13:52:54.348659 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/debug.py
--rw-r--r--   0        0        0      813 2023-04-10 13:52:54.348843 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/env.py
--rw-r--r--   0        0        0     2646 2023-04-10 13:52:54.349116 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/get_implementations.py
--rw-r--r--   0        0        0     1864 2023-04-10 13:52:54.349279 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/invoke.py
--rw-r--r--   0        0        0     3466 2023-04-10 13:52:54.349752 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/subinvoke.py
--rw-r--r--   0        0        0     4502 2023-04-10 13:52:54.350091 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/subinvoke_implementation.py
--rw-r--r--   0        0        0      104 2023-04-10 13:52:54.352417 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/types/__init__.py
--rw-r--r--   0        0        0      309 2023-04-10 13:52:54.350469 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/types/base_wrap_linker.py
--rw-r--r--   0        0        0     1580 2023-06-15 11:56:47.054477 polywrap_wasm-0.1.0b2/polywrap_wasm/linker/wrap_linker.py
--rw-r--r--   0        0        0     1848 2023-06-15 11:56:47.060660 polywrap_wasm-0.1.0b2/polywrap_wasm/memory.py
--rw-r--r--   0        0        0        0 2023-04-10 13:52:54.350025 polywrap_wasm-0.1.0b2/polywrap_wasm/py.typed
--rw-r--r--   0        0        0      180 2023-06-15 11:56:47.053763 polywrap_wasm-0.1.0b2/polywrap_wasm/types/__init__.py
--rw-r--r--   0        0        0      766 2023-06-15 11:56:47.055264 polywrap_wasm-0.1.0b2/polywrap_wasm/types/invoke_result.py
--rw-r--r--   0        0        0      996 2023-06-15 11:56:47.056140 polywrap_wasm-0.1.0b2/polywrap_wasm/types/state.py
--rw-r--r--   0        0        0      902 2023-06-15 11:56:47.057043 polywrap_wasm-0.1.0b2/polywrap_wasm/types/wasm_invoke_options.py
--rw-r--r--   0        0        0     3529 2023-06-15 11:56:47.058526 polywrap_wasm-0.1.0b2/polywrap_wasm/wasm_package.py
--rw-r--r--   0        0        0     5642 2023-06-28 12:32:43.083415 polywrap_wasm-0.1.0b2/polywrap_wasm/wasm_wrapper.py
--rw-r--r--   0        0        0     1138 2023-08-02 15:39:28.464749 polywrap_wasm-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1746 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0b2/setup.py
--rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      872 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/README.md
+-rw-r--r--   0        0        0      182 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/__init__.py
+-rw-r--r--   0        0        0     3699 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/buffer.py
+-rw-r--r--   0        0        0      282 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/constants.py
+-rw-r--r--   0        0        0      491 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/errors.py
+-rw-r--r--   0        0        0     1693 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/exports.py
+-rw-r--r--   0        0        0       85 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/__init__.py
+-rw-r--r--   0        0        0     1854 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/abort.py
+-rw-r--r--   0        0        0      604 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/debug.py
+-rw-r--r--   0        0        0      940 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/env.py
+-rw-r--r--   0        0        0     3046 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/get_implementations.py
+-rw-r--r--   0        0        0     2372 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/invoke.py
+-rw-r--r--   0        0        0     5182 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/subinvoke.py
+-rw-r--r--   0        0        0      111 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/types/__init__.py
+-rw-r--r--   0        0        0     1657 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/types/base_wrap_imports.py
+-rw-r--r--   0        0        0     1626 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/imports/wrap_imports.py
+-rw-r--r--   0        0        0     1637 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/inmemory_file_reader.py
+-rw-r--r--   0        0        0     1162 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/instance.py
+-rw-r--r--   0        0        0      100 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/__init__.py
+-rw-r--r--   0        0        0     1143 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/abort.py
+-rw-r--r--   0        0        0      865 2023-08-02 16:06:36.167338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/debug.py
+-rw-r--r--   0        0        0      813 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/env.py
+-rw-r--r--   0        0        0     2646 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/get_implementations.py
+-rw-r--r--   0        0        0     1864 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/invoke.py
+-rw-r--r--   0        0        0     3466 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/subinvoke.py
+-rw-r--r--   0        0        0     4502 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/subinvoke_implementation.py
+-rw-r--r--   0        0        0      104 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/types/__init__.py
+-rw-r--r--   0        0        0      309 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/types/base_wrap_linker.py
+-rw-r--r--   0        0        0     1580 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/linker/wrap_linker.py
+-rw-r--r--   0        0        0     1848 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/memory.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/py.typed
+-rw-r--r--   0        0        0      180 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/types/__init__.py
+-rw-r--r--   0        0        0      766 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/types/invoke_result.py
+-rw-r--r--   0        0        0      996 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/types/state.py
+-rw-r--r--   0        0        0      902 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/types/wasm_invoke_options.py
+-rw-r--r--   0        0        0     3529 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/wasm_package.py
+-rw-r--r--   0        0        0     5642 2023-08-02 16:06:36.171338 polywrap_wasm-0.1.0b3/polywrap_wasm/wasm_wrapper.py
+-rw-r--r--   0        0        0     1138 2023-08-02 16:11:35.413385 polywrap_wasm-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 polywrap_wasm-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_wasm-0.1.0b2/README.md` & `polywrap_wasm-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/buffer.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/buffer.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/exports.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/exports.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/imports/abort.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/imports/abort.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/imports/debug.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/imports/debug.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/imports/env.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/imports/env.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/imports/get_implementations.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/imports/get_implementations.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/imports/invoke.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/imports/invoke.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/imports/subinvoke.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/imports/subinvoke.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/imports/types/base_wrap_imports.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/imports/types/base_wrap_imports.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/imports/wrap_imports.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/imports/wrap_imports.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/inmemory_file_reader.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/inmemory_file_reader.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/instance.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/instance.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/linker/abort.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/linker/abort.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/linker/debug.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/linker/debug.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/linker/env.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/linker/env.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/linker/get_implementations.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/linker/get_implementations.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/linker/invoke.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/linker/invoke.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/linker/subinvoke.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/linker/subinvoke.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/linker/subinvoke_implementation.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/linker/subinvoke_implementation.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/linker/wrap_linker.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/linker/wrap_linker.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/memory.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/memory.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/types/invoke_result.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/types/invoke_result.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/types/state.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/types/state.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/types/wasm_invoke_options.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/types/wasm_invoke_options.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/wasm_package.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/wasm_package.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/polywrap_wasm/wasm_wrapper.py` & `polywrap_wasm-0.1.0b3/polywrap_wasm/wasm_wrapper.py`

 * *Files identical despite different names*

### Comparing `polywrap_wasm-0.1.0b2/pyproject.toml` & `polywrap_wasm-0.1.0b3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-wasm"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 wasmtime = "^9.0.0"
-polywrap-msgpack = "^0.1.0b2"
-polywrap-manifest = "^0.1.0b2"
-polywrap-core = "^0.1.0b2"
+polywrap-msgpack = "^0.1.0b3"
+polywrap-manifest = "^0.1.0b3"
+polywrap-core = "^0.1.0b3"
 
 [tool.poetry.group.dev.dependencies]
 pycln = "^2.1.3"
 pytest = "^7.1.2"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
```

### Comparing `polywrap_wasm-0.1.0b2/PKG-INFO` & `polywrap_wasm-0.1.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: polywrap-wasm
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: 
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-manifest (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-msgpack (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0b3,<0.2.0)
 Requires-Dist: wasmtime (>=9.0.0,<10.0.0)
 Description-Content-Type: text/markdown
 
 # polywrap-wasm
 
 Python implementation of the Wasm wrapper runtime.
```

