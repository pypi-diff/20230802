# Comparing `tmp/polywrap_plugin-0.1.0b2.tar.gz` & `tmp/polywrap_plugin-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_plugin-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_plugin-0.1.0b3.tar", max compression
```

## Comparing `polywrap_plugin-0.1.0b2.tar` & `polywrap_plugin-0.1.0b3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0      940 2023-06-19 11:17:54.183544 polywrap_plugin-0.1.0b2/README.md
--rw-r--r--   0        0        0      140 2023-04-10 13:52:54.322834 polywrap_plugin-0.1.0b2/polywrap_plugin/__init__.py
--rw-r--r--   0        0        0     2964 2023-06-15 11:56:46.974754 polywrap_plugin-0.1.0b2/polywrap_plugin/module.py
--rw-r--r--   0        0        0     1419 2023-06-15 11:56:46.976407 polywrap_plugin-0.1.0b2/polywrap_plugin/package.py
--rw-r--r--   0        0        0        0 2023-04-10 13:52:54.320363 polywrap_plugin-0.1.0b2/polywrap_plugin/py.typed
--rw-r--r--   0        0        0     3178 2023-06-15 11:56:46.975250 polywrap_plugin-0.1.0b2/polywrap_plugin/resolution_context_override_client.py
--rw-r--r--   0        0        0     3547 2023-06-15 11:56:46.975770 polywrap_plugin-0.1.0b2/polywrap_plugin/wrapper.py
--rw-r--r--   0        0        0     1127 2023-08-02 15:40:31.122280 polywrap_plugin-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0b2/setup.py
--rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0      940 2023-08-02 16:06:36.159338 polywrap_plugin-0.1.0b3/README.md
+-rw-r--r--   0        0        0      140 2023-08-02 16:06:36.163338 polywrap_plugin-0.1.0b3/polywrap_plugin/__init__.py
+-rw-r--r--   0        0        0     2964 2023-08-02 16:06:36.163338 polywrap_plugin-0.1.0b3/polywrap_plugin/module.py
+-rw-r--r--   0        0        0     1419 2023-08-02 16:06:36.163338 polywrap_plugin-0.1.0b3/polywrap_plugin/package.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.163338 polywrap_plugin-0.1.0b3/polywrap_plugin/py.typed
+-rw-r--r--   0        0        0     3178 2023-08-02 16:06:36.163338 polywrap_plugin-0.1.0b3/polywrap_plugin/resolution_context_override_client.py
+-rw-r--r--   0        0        0     3547 2023-08-02 16:06:36.163338 polywrap_plugin-0.1.0b3/polywrap_plugin/wrapper.py
+-rw-r--r--   0        0        0     1127 2023-08-02 16:12:36.772869 polywrap_plugin-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1443 1970-01-01 00:00:00.000000 polywrap_plugin-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_plugin-0.1.0b2/README.md` & `polywrap_plugin-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_plugin-0.1.0b2/polywrap_plugin/module.py` & `polywrap_plugin-0.1.0b3/polywrap_plugin/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_plugin-0.1.0b2/polywrap_plugin/package.py` & `polywrap_plugin-0.1.0b3/polywrap_plugin/package.py`

 * *Files identical despite different names*

### Comparing `polywrap_plugin-0.1.0b2/polywrap_plugin/resolution_context_override_client.py` & `polywrap_plugin-0.1.0b3/polywrap_plugin/resolution_context_override_client.py`

 * *Files identical despite different names*

### Comparing `polywrap_plugin-0.1.0b2/polywrap_plugin/wrapper.py` & `polywrap_plugin-0.1.0b3/polywrap_plugin/wrapper.py`

 * *Files identical despite different names*

### Comparing `polywrap_plugin-0.1.0b2/pyproject.toml` & `polywrap_plugin-0.1.0b3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-plugin"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "Plugin package"
 authors = ["Cesar <cesar@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-msgpack = "^0.1.0b2"
-polywrap-manifest = "^0.1.0b2"
-polywrap-core = "^0.1.0b2"
+polywrap-msgpack = "^0.1.0b3"
+polywrap-manifest = "^0.1.0b3"
+polywrap-core = "^0.1.0b3"
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
```

### Comparing `polywrap_plugin-0.1.0b2/PKG-INFO` & `polywrap_plugin-0.1.0b3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: polywrap-plugin
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Plugin package
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
 Description-Content-Type: text/markdown
 
 # polywrap-plugin
 
 Python implementation of the plugin wrapper runtime.
 
 ## Usage
```

