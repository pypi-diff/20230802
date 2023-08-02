# Comparing `tmp/polywrap_http_plugin-0.1.0b2.tar.gz` & `tmp/polywrap_http_plugin-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_http_plugin-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_http_plugin-0.1.0b3.tar", max compression
```

## Comparing `polywrap_http_plugin-0.1.0b2.tar` & `polywrap_http_plugin-0.1.0b3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1561 2023-07-29 08:59:38.312160 polywrap_http_plugin-0.1.0b2/README.md
--rw-r--r--   0        0        0     4896 2023-07-29 08:59:38.311447 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/__init__.py
--rw-r--r--   0        0        0        0 2023-07-29 08:59:38.310732 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/py.typed
--rw-r--r--   0        0        0      163 2023-08-02 15:42:59.440377 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/__init__.py
--rw-r--r--   0        0        0     1247 2023-08-02 15:42:59.440525 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/module.py
--rw-r--r--   0        0        0     1506 2023-08-02 15:42:59.440646 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/types.py
--rw-r--r--   0        0        0     8589 2023-08-02 15:42:59.440842 polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/wrap_info.py
--rw-r--r--   0        0        0     1464 2023-08-02 15:42:42.713160 polywrap_http_plugin-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     2393 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0b2/setup.py
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1561 2023-08-02 16:06:36.151338 polywrap_http_plugin-0.1.0b3/README.md
+-rw-r--r--   0        0        0     4896 2023-08-02 16:06:36.151338 polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.151338 polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/py.typed
+-rw-r--r--   0        0        0      163 2023-08-02 16:15:13.610258 polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/wrap/__init__.py
+-rw-r--r--   0        0        0     1247 2023-08-02 16:15:13.610258 polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/wrap/module.py
+-rw-r--r--   0        0        0     1506 2023-08-02 16:15:13.610258 polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/wrap/types.py
+-rw-r--r--   0        0        0     8589 2023-08-02 16:15:13.610258 polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1464 2023-08-02 16:14:46.228606 polywrap_http_plugin-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 polywrap_http_plugin-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_http_plugin-0.1.0b2/README.md` & `polywrap_http_plugin-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/__init__.py` & `polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/module.py` & `polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/wrap/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/types.py` & `polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/wrap/types.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0b2/polywrap_http_plugin/wrap/wrap_info.py` & `polywrap_http_plugin-0.1.0b3/polywrap_http_plugin/wrap/wrap_info.py`

 * *Files identical despite different names*

### Comparing `polywrap_http_plugin-0.1.0b2/pyproject.toml` & `polywrap_http_plugin-0.1.0b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-http-plugin"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = ""
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 include = ["polywrap_http_plugin/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 httpx = "^0.23.3"
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

### Comparing `polywrap_http_plugin-0.1.0b2/setup.py` & `polywrap_http_plugin-0.1.0b3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,66 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: polywrap-http-plugin
+Version: 0.1.0b3
+Summary: 
+Author: Niraj
+Author-email: niraj@polywrap.io
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.23.3,<0.24.0)
+Requires-Dist: polywrap-core (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-plugin (>=0.1.0b3,<0.2.0)
+Description-Content-Type: text/markdown
+
+# polywrap-http-plugin
+
+Http plugin currently supports two different methods `GET` and `POST`. Similar to calling axios, when defining request you need to specify a response type. Headers and query parameters may also be defined.
+
+## Response Types
+
+`TEXT` - The server will respond with text, the HTTP plugin will return the text as-is.
+
+`BINARY` - The server will respond with binary data (_bytes_), the HTTP plugin will encode as a **base64** string and return it.
+
+## GET request
+
+Below is sample invocation of the `GET` request with custom request headers and query parameters (`urlParams`).
+
+```python
+result = client.invoke(
+    uri="wrap://ens/http.polywrap.eth",
+    method="get",
+    args={
+        "url": "http://www.example.com/api",
+        "request": {
+            "responseType": "TEXT",
+            "urlParams": [{"key": "query", "value": "foo"}],
+            "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
+        },
+    },
+)
+```
+
+## POST request
+
+Below is sample invocation of the `POST` request with custom request headers and query parameters (`urlParams`). It is also possible to set request body as shown below.
+
+```python
+response = client.invoke(
+    uri="wrap://ens/http.polywrap.eth",
+    method="post",
+    args={
+        "url": "http://www.example.com/api",
+        "request": {
+            "responseType": "TEXT",
+            "urlParams": [{"key": "query", "value": "foo"}],
+            "headers": [{"key": "X-Request-Header", "value": "req-foo"}],
+            "body": "{data: 'test-request'}",
+        }
+    }
+)
+```
 
-packages = \
-['polywrap_http_plugin', 'polywrap_http_plugin.wrap']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['httpx>=0.23.3,<0.24.0',
- 'polywrap-core>=0.1.0b2,<0.2.0',
- 'polywrap-manifest>=0.1.0b2,<0.2.0',
- 'polywrap-msgpack>=0.1.0b2,<0.2.0',
- 'polywrap-plugin>=0.1.0b2,<0.2.0']
-
-setup_kwargs = {
-    'name': 'polywrap-http-plugin',
-    'version': '0.1.0b2',
-    'description': '',
-    'long_description': '# polywrap-http-plugin\n\nHttp plugin currently supports two different methods `GET` and `POST`. Similar to calling axios, when defining request you need to specify a response type. Headers and query parameters may also be defined.\n\n## Response Types\n\n`TEXT` - The server will respond with text, the HTTP plugin will return the text as-is.\n\n`BINARY` - The server will respond with binary data (_bytes_), the HTTP plugin will encode as a **base64** string and return it.\n\n## GET request\n\nBelow is sample invocation of the `GET` request with custom request headers and query parameters (`urlParams`).\n\n```python\nresult = client.invoke(\n    uri="wrap://ens/http.polywrap.eth",\n    method="get",\n    args={\n        "url": "http://www.example.com/api",\n        "request": {\n            "responseType": "TEXT",\n            "urlParams": [{"key": "query", "value": "foo"}],\n            "headers": [{"key": "X-Request-Header", "value": "req-foo"}],\n        },\n    },\n)\n```\n\n## POST request\n\nBelow is sample invocation of the `POST` request with custom request headers and query parameters (`urlParams`). It is also possible to set request body as shown below.\n\n```python\nresponse = client.invoke(\n    uri="wrap://ens/http.polywrap.eth",\n    method="post",\n    args={\n        "url": "http://www.example.com/api",\n        "request": {\n            "responseType": "TEXT",\n            "urlParams": [{"key": "query", "value": "foo"}],\n            "headers": [{"key": "X-Request-Header", "value": "req-foo"}],\n            "body": "{data: \'test-request\'}",\n        }\n    }\n)\n```\n',
-    'author': 'Niraj',
-    'author_email': 'niraj@polywrap.io',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

