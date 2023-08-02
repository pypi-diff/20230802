# Comparing `tmp/polywrap_client-0.1.0a4.tar.gz` & `tmp/polywrap_client-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_client-0.1.0a4.tar", max compression
+gzip compressed data, was "polywrap_client-0.1.0b2.tar", max compression
```

## Comparing `polywrap_client-0.1.0a4.tar` & `polywrap_client-0.1.0b2.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0        4 2023-02-24 13:52:49.839099 polywrap_client-0.1.0a4/README.md
--rw-r--r--   0        0        0       22 2023-02-24 13:52:49.843099 polywrap_client-0.1.0a4/polywrap_client/__init__.py
--rw-r--r--   0        0        0     5313 2023-02-24 13:52:49.843099 polywrap_client-0.1.0a4/polywrap_client/client.py
--rw-r--r--   0        0        0     1283 2023-02-24 14:00:34.812101 polywrap_client-0.1.0a4/pyproject.toml
--rw-r--r--   0        0        0      863 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a4/setup.py
--rw-r--r--   0        0        0      769 1970-01-01 00:00:00.000000 polywrap_client-0.1.0a4/PKG-INFO
+-rw-r--r--   0        0        0     1230 2023-06-19 11:17:54.181072 polywrap_client-0.1.0b2/README.md
+-rw-r--r--   0        0        0       86 2023-04-10 13:52:54.291570 polywrap_client-0.1.0b2/polywrap_client/__init__.py
+-rw-r--r--   0        0        0     8997 2023-07-29 18:37:27.847942 polywrap_client-0.1.0b2/polywrap_client/client.py
+-rw-r--r--   0        0        0      929 2023-07-29 18:37:34.754411 polywrap_client-0.1.0b2/polywrap_client/errors.py
+-rw-r--r--   0        0        0        0 2023-04-10 13:52:54.291832 polywrap_client-0.1.0b2/polywrap_client/py.typed
+-rw-r--r--   0        0        0     1311 2023-08-02 15:56:35.128369 polywrap_client-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     1963 1970-01-01 00:00:00.000000 polywrap_client-0.1.0b2/setup.py
+-rw-r--r--   0        0        0     1719 1970-01-01 00:00:00.000000 polywrap_client-0.1.0b2/PKG-INFO
```

### Comparing `polywrap_client-0.1.0a4/pyproject.toml` & `polywrap_client-0.1.0b2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,63 +1,60 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-client"
-version = "0.1.0a4"
+version = "0.1.0b2"
 description = ""
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-wasmtime = "^1.0.1"
-unsync = "^1.4.0"
-polywrap-core = "0.1.0a4"
-polywrap-msgpack = "0.1.0a4"
-polywrap-manifest = "0.1.0a4"
-polywrap-result = "0.1.0a4"
-polywrap-uri-resolvers = "0.1.0a4"
-result = "^0.8.0"
-pysha3 = "^1.0.2"
-pycryptodome = "^3.14.1"
+polywrap-manifest = "^0.1.0b2"
+polywrap-msgpack = "^0.1.0b2"
+polywrap-core = "^0.1.0b2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
-pytest-asyncio = "^0.19.0"
+polywrap-plugin = {path = "../polywrap-plugin", develop = true}
+polywrap-client-config-builder = {path = "../polywrap-client-config-builder", develop = true}
+polywrap-test-cases = {path = "../polywrap-test-cases", develop = true}
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
 pydocstyle = "^6.1.1"
-polywrap-plugin = { path = "../polywrap-plugin", develop = true }
+
+[tool.poetry.group.test.dependencies]
+pysha3 = "^1.0.2"
+pycryptodome = "^3.17"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportShadowedImports = false
 
 [tool.pytest.ini_options]
-asyncio_mode = "auto"
 testpaths = [
     "tests"
 ]
 
 [tool.pylint]
 disable = [
-    "too-many-return-statements",
+    "too-many-arguments",
 ]
 ignore = [
     "tests/"
 ]
 
 [tool.isort]
 profile = "black"
```

