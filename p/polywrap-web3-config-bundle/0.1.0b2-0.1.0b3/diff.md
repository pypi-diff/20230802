# Comparing `tmp/polywrap_web3_config_bundle-0.1.0b2.tar.gz` & `tmp/polywrap_web3_config_bundle-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_web3_config_bundle-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_web3_config_bundle-0.1.0b3.tar", max compression
```

## Comparing `polywrap_web3_config_bundle-0.1.0b2.tar` & `polywrap_web3_config_bundle-0.1.0b3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0       29 2023-07-29 08:59:38.302418 polywrap_web3_config_bundle-0.1.0b2/README.md
--rw-r--r--   0        0        0      125 2023-07-29 08:59:38.300641 polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/__init__.py
--rw-r--r--   0        0        0     2773 2023-07-29 10:35:18.362592 polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/bundle.py
--rw-r--r--   0        0        0      477 2023-07-29 08:59:38.300531 polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/config.py
--rw-r--r--   0        0        0        0 2023-07-29 08:59:38.301886 polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/py.typed
--rw-r--r--   0        0        0     1341 2023-08-02 16:00:52.667052 polywrap_web3_config_bundle-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 polywrap_web3_config_bundle-0.1.0b2/setup.py
--rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 polywrap_web3_config_bundle-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-08-02 16:06:36.147338 polywrap_web3_config_bundle-0.1.0b3/README.md
+-rw-r--r--   0        0        0      125 2023-08-02 16:06:36.147338 polywrap_web3_config_bundle-0.1.0b3/polywrap_web3_config_bundle/__init__.py
+-rw-r--r--   0        0        0     2773 2023-08-02 16:06:36.147338 polywrap_web3_config_bundle-0.1.0b3/polywrap_web3_config_bundle/bundle.py
+-rw-r--r--   0        0        0      477 2023-08-02 16:06:36.147338 polywrap_web3_config_bundle-0.1.0b3/polywrap_web3_config_bundle/config.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.147338 polywrap_web3_config_bundle-0.1.0b3/polywrap_web3_config_bundle/py.typed
+-rw-r--r--   0        0        0     1341 2023-08-02 16:21:04.938664 polywrap_web3_config_bundle-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 polywrap_web3_config_bundle-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/bundle.py` & `polywrap_web3_config_bundle-0.1.0b3/polywrap_web3_config_bundle/bundle.py`

 * *Files identical despite different names*

### Comparing `polywrap_web3_config_bundle-0.1.0b2/pyproject.toml` & `polywrap_web3_config_bundle-0.1.0b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-web3-config-bundle"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "Polywrap System Client Config Bundle"
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [
     { include = "polywrap_web3_config_bundle" },
 ]
 include = ["**/wrap.info", "**/wrap.wasm"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-core = "^0.1.0b2"
-polywrap-client-config-builder = "^0.1.0b2"
-polywrap-uri-resolvers = "^0.1.0b2"
-polywrap-manifest = "^0.1.0b2"
-polywrap-wasm = "^0.1.0b2"
-polywrap-ethereum-provider = "^0.1.0b2"
-polywrap-sys-config-bundle = "^0.1.0b2"
+polywrap-core = "^0.1.0b3"
+polywrap-client-config-builder = "^0.1.0b3"
+polywrap-uri-resolvers = "^0.1.0b3"
+polywrap-manifest = "^0.1.0b3"
+polywrap-wasm = "^0.1.0b3"
+polywrap-ethereum-provider = "^0.1.0b3"
+polywrap-sys-config-bundle = "^0.1.0b3"
 
 [tool.poetry.group.dev.dependencies]
 polywrap-client = {path = "../../polywrap-client", develop = true}
 pytest = "^7.1.2"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
```

### Comparing `polywrap_web3_config_bundle-0.1.0b2/PKG-INFO` & `polywrap_web3_config_bundle-0.1.0b3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: polywrap-web3-config-bundle
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
-Requires-Dist: polywrap-ethereum-provider (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-manifest (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-sys-config-bundle (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-uri-resolvers (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-wasm (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-client-config-builder (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-ethereum-provider (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-sys-config-bundle (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-uri-resolvers (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-wasm (>=0.1.0b3,<0.2.0)
 Description-Content-Type: text/markdown
 
 # polywrap-web3-config-bundle
```

