# Comparing `tmp/polywrap_http_plugin-0.1.0a9.tar.gz` & `tmp/polywrap_http_plugin-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_http_plugin-0.1.0a9.tar", max compression
+gzip compressed data, was "polywrap_http_plugin-0.1.0b2.tar", max compression
```

## Comparing `polywrap_http_plugin-0.1.0a9.tar` & `polywrap_http_plugin-0.1.0b2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1561 2023-07-02 08:14:03.632171 polywrap_http_plugin-0.1.0a9/README.md
--rw-r--r--   0        0        0     4896 2023-07-02 08:14:03.632171 polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-02 08:14:03.632171 polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/py.typed
--rw-r--r--   0        0        0      163 2023-07-02 08:14:22.036499 polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/wrap/__init__.py
--rw-r--r--   0        0        0     1247 2023-07-02 08:14:22.036499 polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/wrap/module.py
--rw-r--r--   0        0        0     1506 2023-07-02 08:14:22.036499 polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/wrap/types.py
--rw-r--r--   0        0        0     8589 2023-07-02 08:14:22.036499 polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/wrap/wrap_info.py
--rw-r--r--   0        0        0     1377 2023-07-02 08:14:03.632171 polywrap_http_plugin-0.1.0a9/pyproject.toml
--rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0a9/PKG-INFO
+-rw-r--r--   0        0        0     1561 2023-07-29 08:59:38.312160 polywrap_http_plugin-0.1.0b2/README.md
+-rw-r--r--   0        0        0     4896 2023-07-29 08:59:38.311447 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-29 08:59:38.310732 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/py.typed
+-rw-r--r--   0        0        0      163 2023-08-02 15:42:59.440377 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/__init__.py
+-rw-r--r--   0        0        0     1247 2023-08-02 15:42:59.440525 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/module.py
+-rw-r--r--   0        0        0     1506 2023-08-02 15:42:59.440646 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/types.py
+-rw-r--r--   0        0        0     8589 2023-08-02 15:42:59.440842 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1464 2023-08-02 15:42:42.713160 polywrap_http_plugin-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0b2/setup.py
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0b2/PKG-INFO
```

### Comparing `polywrap_http_plugin-0.1.0a9/README.md` & `polywrap_http_plugin-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/__init__.py` & `polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/wrap/module.py` & `polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/wrap/types.py` & `polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/types.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a9/polywrap_http_plugin/wrap/wrap_info.py` & `polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/wrap_info.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0a9/pyproject.toml` & `polywrap_http_plugin-0.1.0b2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,38 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-http-plugin"
-version = "0.1.0a9"
+version = "0.1.0b2"
 description = ""
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 include = ["polywrap_http_plugin/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-plugin = "0.1.0a35"
 httpx = "^0.23.3"
-polywrap-core = "0.1.0a35"
-polywrap-msgpack = "0.1.0a35"
-polywrap-manifest = "0.1.0a35"
+polywrap-plugin = "^0.1.0b2"
+polywrap-core = "^0.1.0b2"
+polywrap-msgpack = "^0.1.0b2"
+polywrap-manifest = "^0.1.0b2"
 
 [tool.poetry.group.dev.dependencies]
-polywrap-client = "0.1.0a35"
+polywrap-client = {path = "../../polywrap-client", develop = true}
+polywrap-uri-resolvers = {path = "../../polywrap-uri-resolvers", develop = true}
+polywrap-client-config-builder = {path = "../../polywrap-client-config-builder", develop = true}
 black = "^23.1.0"
 pytest = "^7.2.1"
-pytest-asyncio = "^0.20.3"
 isort = "^5.12.0"
 bandit = "^1.7.4"
 pyright = "^1.1.296"
 pylint = "^2.16.3"
-polywrap-uri-resolvers = "0.1.0a35"
-polywrap-client-config-builder = "0.1.0a35"
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 pytest-mock = "^3.10.0"
 pydocstyle = "^6.3.0"
 mocket = "^3.11.1"
 
 [tool.bandit]
@@ -47,15 +46,14 @@
 typeCheckingMode = "strict"
 reportShadowedImports = false
 exclude = [
     "**/wrap/"
 ]
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 testpaths = [
     "tests",
 ]
 
 [tool.pylint]
 disable = [
     "too-many-return-statements",
```

### Comparing `polywrap_http_plugin-0.1.0a9/PKG-INFO` & `polywrap_http_plugin-0.1.0b2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: polywrap-http-plugin
-Version: 0.1.0a9
+Version: 0.1.0b2
 Summary: 
 Author: Niraj
 Author-email: niraj@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
-Requires-Dist: polywrap-core (==0.1.0a35)
-Requires-Dist: polywrap-manifest (==0.1.0a35)
-Requires-Dist: polywrap-msgpack (==0.1.0a35)
-Requires-Dist: polywrap-plugin (==0.1.0a35)
+Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-plugin (>=0.1.0b2,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-http-plugin
 
 Http plugin currently supports two different methods `GET` and `POST`. Similar to calling axios, when defining request you need to specify a response type. Headers and query parameters may also be defined.
 
 ## Response Types
```

