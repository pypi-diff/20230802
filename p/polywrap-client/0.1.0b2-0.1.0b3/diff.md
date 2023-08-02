# Comparing `tmp/polywrap_client-0.1.0b2.tar.gz` & `tmp/polywrap_client-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_client-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_client-0.1.0b3.tar", max compression
```

## Comparing `polywrap_client-0.1.0b2.tar` & `polywrap_client-0.1.0b3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1230 2023-06-19 11:17:54.181072 polywrap_client-0.1.0b2/README.md
--rw-r--r--   0        0        0       86 2023-04-10 13:52:54.291570 polywrap_client-0.1.0b2/polywrap_client/__init__.py
--rw-r--r--   0        0        0     8997 2023-07-29 18:37:27.847942 polywrap_client-0.1.0b2/polywrap_client/client.py
--rw-r--r--   0        0        0      929 2023-07-29 18:37:34.754411 polywrap_client-0.1.0b2/polywrap_client/errors.py
--rw-r--r--   0        0        0        0 2023-04-10 13:52:54.291832 polywrap_client-0.1.0b2/polywrap_client/py.typed
--rw-r--r--   0        0        0     1311 2023-08-02 15:56:35.128369 polywrap_client-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     1963 1970-01-01 00:00:00.000000 polywrap_client-0.1.0b2/setup.py
--rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 polywrap_client-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1230 2023-08-02 16:06:36.155338 polywrap_client-0.1.0b3/README.md
+-rw-r--r--   0        0        0       86 2023-08-02 16:06:36.155338 polywrap_client-0.1.0b3/polywrap_client/__init__.py
+-rw-r--r--   0        0        0     8997 2023-08-02 16:06:36.155338 polywrap_client-0.1.0b3/polywrap_client/client.py
+-rw-r--r--   0        0        0      929 2023-08-02 16:06:36.155338 polywrap_client-0.1.0b3/polywrap_client/errors.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.155338 polywrap_client-0.1.0b3/polywrap_client/py.typed
+-rw-r--r--   0        0        0     1311 2023-08-02 16:16:52.592246 polywrap_client-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 polywrap_client-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_client-0.1.0b2/README.md` & `polywrap_client-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_client-0.1.0b2/polywrap_client/client.py` & `polywrap_client-0.1.0b3/polywrap_client/client.py`

 * *Files identical despite different names*

### Comparing `polywrap_client-0.1.0b2/polywrap_client/errors.py` & `polywrap_client-0.1.0b3/polywrap_client/errors.py`

 * *Files identical despite different names*

### Comparing `polywrap_client-0.1.0b2/pyproject.toml` & `polywrap_client-0.1.0b3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-client"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-manifest = "^0.1.0b2"
-polywrap-msgpack = "^0.1.0b2"
-polywrap-core = "^0.1.0b2"
+polywrap-manifest = "^0.1.0b3"
+polywrap-msgpack = "^0.1.0b3"
+polywrap-core = "^0.1.0b3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 polywrap-plugin = {path = "../polywrap-plugin", develop = true}
 polywrap-client-config-builder = {path = "../polywrap-client-config-builder", develop = true}
 polywrap-test-cases = {path = "../polywrap-test-cases", develop = true}
 pylint = "^2.15.4"
```

### Comparing `polywrap_client-0.1.0b2/PKG-INFO` & `polywrap_client-0.1.0b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: polywrap-client
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
 Description-Content-Type: text/markdown
 
 # polywrap-client
 
 Python implementation of the polywrap client.
 
 ## Usage
```

