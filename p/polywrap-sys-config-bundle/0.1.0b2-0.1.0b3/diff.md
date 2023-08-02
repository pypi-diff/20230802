# Comparing `tmp/polywrap_sys_config_bundle-0.1.0b2.tar.gz` & `tmp/polywrap_sys_config_bundle-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_sys_config_bundle-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_sys_config_bundle-0.1.0b3.tar", max compression
```

## Comparing `polywrap_sys_config_bundle-0.1.0b2.tar` & `polywrap_sys_config_bundle-0.1.0b3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0       29 2023-07-29 08:59:38.298097 polywrap_sys_config_bundle-0.1.0b2/README.md
--rw-r--r--   0        0        0      161 2023-07-29 08:59:38.296355 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/__init__.py
--rw-r--r--   0        0        0     3705 2023-07-29 15:59:17.973262 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/bundle.py
--rw-r--r--   0        0        0      473 2023-07-29 08:59:38.296672 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/config.py
--rw-r--r--   0        0        0      481 2023-07-29 08:59:38.296826 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/__init__.py
--rw-r--r--   0        0        0     4785 2023-07-29 08:59:38.296959 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.info
--rw-r--r--   0        0        0   102231 2023-07-29 08:59:38.297480 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.wasm
--rw-r--r--   0        0        0     6217 2023-07-29 08:59:38.297313 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/http-resolver/wrap.info
--rw-r--r--   0        0        0   143271 2023-07-29 08:59:38.298530 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/http-resolver/wrap.wasm
--rw-r--r--   0        0        0     9034 2023-07-29 10:22:30.675191 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/ipfs-http-client/wrap.info
--rw-r--r--   0        0        0   150523 2023-07-29 10:22:30.677439 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/ipfs-http-client/wrap.wasm
--rw-r--r--   0        0        0     6954 2023-07-29 10:22:30.704787 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/ipfs-sync-resolver/wrap.info
--rwxr-xr-x   0        0        0   253658 2023-07-29 10:22:30.706543 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/ipfs-sync-resolver/wrap.wasm
--rw-r--r--   0        0        0        0 2023-07-29 08:59:38.297745 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/py.typed
--rw-r--r--   0        0        0      141 2023-07-29 08:59:38.298029 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/types/__init__.py
--rw-r--r--   0        0        0     1126 2023-07-29 08:59:38.298182 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/types/bundle_package.py
--rw-r--r--   0        0        0      607 2023-07-29 08:59:38.298420 polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/types/embedded_file_reader.py
--rw-r--r--   0        0        0     1375 2023-08-02 15:59:48.230298 polywrap_sys_config_bundle-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1263 1970-01-01 00:00:00.000000 polywrap_sys_config_bundle-0.1.0b2/setup.py
--rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 polywrap_sys_config_bundle-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-08-02 16:06:36.135338 polywrap_sys_config_bundle-0.1.0b3/README.md
+-rw-r--r--   0        0        0      161 2023-08-02 16:06:36.139338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/__init__.py
+-rw-r--r--   0        0        0     3705 2023-08-02 16:06:36.139338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/bundle.py
+-rw-r--r--   0        0        0      473 2023-08-02 16:06:36.139338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/config.py
+-rw-r--r--   0        0        0      481 2023-08-02 16:06:36.139338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/__init__.py
+-rw-r--r--   0        0        0     4785 2023-08-02 16:06:36.139338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.info
+-rw-r--r--   0        0        0   102231 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.wasm
+-rw-r--r--   0        0        0     6217 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/http-resolver/wrap.info
+-rw-r--r--   0        0        0   143271 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/http-resolver/wrap.wasm
+-rw-r--r--   0        0        0     9034 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/ipfs-http-client/wrap.info
+-rw-r--r--   0        0        0   150523 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/ipfs-http-client/wrap.wasm
+-rw-r--r--   0        0        0     6954 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/ipfs-sync-resolver/wrap.info
+-rwxr-xr-x   0        0        0   253658 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/ipfs-sync-resolver/wrap.wasm
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/py.typed
+-rw-r--r--   0        0        0      141 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/types/__init__.py
+-rw-r--r--   0        0        0     1126 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/types/bundle_package.py
+-rw-r--r--   0        0        0      607 2023-08-02 16:06:36.143338 polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/types/embedded_file_reader.py
+-rw-r--r--   0        0        0     1375 2023-08-02 16:20:01.311030 polywrap_sys_config_bundle-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0      792 1970-01-01 00:00:00.000000 polywrap_sys_config_bundle-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/bundle.py` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.info` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.info`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.wasm` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/file-system-resolver/wrap.wasm`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/http-resolver/wrap.info` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/http-resolver/wrap.info`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/http-resolver/wrap.wasm` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/http-resolver/wrap.wasm`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/ipfs-http-client/wrap.info` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/ipfs-http-client/wrap.info`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/ipfs-http-client/wrap.wasm` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/ipfs-http-client/wrap.wasm`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/ipfs-sync-resolver/wrap.info` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/ipfs-sync-resolver/wrap.info`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/embeds/ipfs-sync-resolver/wrap.wasm` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/embeds/ipfs-sync-resolver/wrap.wasm`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/types/bundle_package.py` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/types/bundle_package.py`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/polywrap_sys_config_bundle/types/embedded_file_reader.py` & `polywrap_sys_config_bundle-0.1.0b3/polywrap_sys_config_bundle/types/embedded_file_reader.py`

 * *Files identical despite different names*

### Comparing `polywrap_sys_config_bundle-0.1.0b2/pyproject.toml` & `polywrap_sys_config_bundle-0.1.0b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-sys-config-bundle"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "Polywrap System Client Config Bundle"
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [
     { include = "polywrap_sys_config_bundle" },
 ]
 include = ["**/wrap.info", "**/wrap.wasm"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-core = "^0.1.0b2"
-polywrap-client-config-builder = "^0.1.0b2"
-polywrap-uri-resolvers = "^0.1.0b2"
-polywrap-manifest = "^0.1.0b2"
-polywrap-wasm = "^0.1.0b2"
-polywrap-fs-plugin = "^0.1.0b2"
-polywrap-http-plugin = "^0.1.0b2"
+polywrap-core = "^0.1.0b3"
+polywrap-client-config-builder = "^0.1.0b3"
+polywrap-uri-resolvers = "^0.1.0b3"
+polywrap-manifest = "^0.1.0b3"
+polywrap-wasm = "^0.1.0b3"
+polywrap-fs-plugin = "^0.1.0b3"
+polywrap-http-plugin = "^0.1.0b3"
 
 [tool.poetry.group.dev.dependencies]
 polywrap-client = {path = "../../polywrap-client", develop = true}
 pytest = "^7.1.2"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
```

### Comparing `polywrap_sys_config_bundle-0.1.0b2/PKG-INFO` & `polywrap_sys_config_bundle-0.1.0b3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: polywrap-sys-config-bundle
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Polywrap System Client Config Bundle
 Author: Niraj
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-client-config-builder (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-fs-plugin (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-http-plugin (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-manifest (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-uri-resolvers (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-wasm (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-client-config-builder (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-fs-plugin (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-http-plugin (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-uri-resolvers (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-wasm (>=0.1.0b3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-sys-config-bundle
```

