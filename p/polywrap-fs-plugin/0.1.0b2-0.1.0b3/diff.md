# Comparing `tmp/polywrap_fs_plugin-0.1.0b2.tar.gz` & `tmp/polywrap_fs_plugin-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_fs_plugin-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_fs_plugin-0.1.0b3.tar", max compression
```

## Comparing `polywrap_fs_plugin-0.1.0b2.tar` & `polywrap_fs_plugin-0.1.0b3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1002 2023-07-29 08:59:38.308066 polywrap_fs_plugin-0.1.0b2/README.md
--rw-r--r--   0        0        0     3768 2023-07-29 16:10:14.336638 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:59:38.307747 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/py.typed
--rw-r--r--   0        0        0      163 2023-08-02 15:42:01.043847 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/__init__.py
--rw-r--r--   0        0        0     2771 2023-08-02 15:42:01.043985 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/module.py
--rw-r--r--   0        0        0     1186 2023-08-02 15:42:01.044066 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/types.py
--rw-r--r--   0        0        0     7225 2023-08-02 15:42:01.044177 polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/wrap_info.py
--rw-r--r--   0        0        0     1511 2023-08-02 15:41:49.405508 polywrap_fs_plugin-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1788 1970-01-01 00:00:00.000000 polywrap_fs_plugin-0.1.0b2/setup.py
--rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 polywrap_fs_plugin-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1002 2023-08-02 16:06:36.147338 polywrap_fs_plugin-0.1.0b3/README.md
+-rw-r--r--   0        0        0     3768 2023-08-02 16:06:36.147338 polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.147338 polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/py.typed
+-rw-r--r--   0        0        0      163 2023-08-02 16:14:15.814751 polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/wrap/__init__.py
+-rw-r--r--   0        0        0     2771 2023-08-02 16:14:15.814751 polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/wrap/module.py
+-rw-r--r--   0        0        0     1186 2023-08-02 16:14:15.814751 polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/wrap/types.py
+-rw-r--r--   0        0        0     7225 2023-08-02 16:14:15.814751 polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1511 2023-08-02 16:13:41.992593 polywrap_fs_plugin-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1544 1970-01-01 00:00:00.000000 polywrap_fs_plugin-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_fs_plugin-0.1.0b2/README.md` & `polywrap_fs_plugin-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/__init__.py` & `polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/module.py` & `polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/wrap/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/types.py` & `polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/wrap/types.py`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0b2/polywrap_fs_plugin/wrap/wrap_info.py` & `polywrap_fs_plugin-0.1.0b3/polywrap_fs_plugin/wrap/wrap_info.py`

 * *Files identical despite different names*

### Comparing `polywrap_fs_plugin-0.1.0b2/pyproject.toml` & `polywrap_fs_plugin-0.1.0b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-fs-plugin"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = ""
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [{include = "polywrap_fs_plugin"}]
 include = ["polywrap_fs_plugin/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-plugin = "^0.1.0b2"
-polywrap-core = "^0.1.0b2"
-polywrap-msgpack = "^0.1.0b2"
-polywrap-manifest = "^0.1.0b2"
+polywrap-plugin = "^0.1.0b3"
+polywrap-core = "^0.1.0b3"
+polywrap-msgpack = "^0.1.0b3"
+polywrap-manifest = "^0.1.0b3"
 
 [tool.poetry.group.dev.dependencies]
 polywrap-client = {path = "../../polywrap-client", develop = true}
 polywrap-uri-resolvers = {path = "../../polywrap-uri-resolvers", develop = true}
 polywrap-client-config-builder = {path = "../../polywrap-client-config-builder", develop = true}
 black = "^23.1.0"
 pytest = "^7.2.1"
```

### Comparing `polywrap_fs_plugin-0.1.0b2/PKG-INFO` & `polywrap_fs_plugin-0.1.0b3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: polywrap-fs-plugin
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: 
 Author: Niraj
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-manifest (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-msgpack (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-plugin (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-plugin (>=0.1.0b3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-fs-plugin
 
 The Filesystem plugin enables wraps running within the Polywrap client to interact with the local filesystem.
 
 ## Interface
```

