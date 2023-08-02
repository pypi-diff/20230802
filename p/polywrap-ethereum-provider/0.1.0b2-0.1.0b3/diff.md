# Comparing `tmp/polywrap_ethereum_provider-0.1.0b2.tar.gz` & `tmp/polywrap_ethereum_provider-0.1.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_ethereum_provider-0.1.0b2.tar", max compression
+gzip compressed data, was "polywrap_ethereum_provider-0.1.0b3.tar", max compression
```

## Comparing `polywrap_ethereum_provider-0.1.0b2.tar` & `polywrap_ethereum_provider-0.1.0b3.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1646 2023-07-29 08:59:38.305561 polywrap_ethereum_provider-0.1.0b2/README.md
--rw-r--r--   0        0        0     6610 2023-07-29 16:11:00.364857 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/__init__.py
--rw-r--r--   0        0        0     1813 2023-07-29 16:11:00.321347 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/connection.py
--rw-r--r--   0        0        0     2730 2023-07-29 16:11:00.331355 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/connections.py
--rw-r--r--   0        0        0     1452 2023-07-29 16:11:00.316852 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/networks.py
--rw-r--r--   0        0        0        0 2023-07-29 08:59:38.304579 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/py.typed
--rw-r--r--   0        0        0      163 2023-08-02 15:55:35.220977 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/__init__.py
--rw-r--r--   0        0        0     2481 2023-08-02 15:55:35.221148 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/module.py
--rw-r--r--   0        0        0      816 2023-08-02 15:55:35.221230 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/types.py
--rw-r--r--   0        0        0     7359 2023-08-02 15:55:35.221343 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/wrap_info.py
--rw-r--r--   0        0        0     1709 2023-08-02 15:55:12.706846 polywrap_ethereum_provider-0.1.0b2/pyproject.toml
--rw-r--r--   0        0        0     2526 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0b2/setup.py
--rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0b2/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-08-02 16:06:36.147338 polywrap_ethereum_provider-0.1.0b3/README.md
+-rw-r--r--   0        0        0     6610 2023-08-02 16:06:36.147338 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/__init__.py
+-rw-r--r--   0        0        0     1813 2023-08-02 16:06:36.147338 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/connection.py
+-rw-r--r--   0        0        0     2730 2023-08-02 16:06:36.147338 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/connections.py
+-rw-r--r--   0        0        0     1452 2023-08-02 16:06:36.147338 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/networks.py
+-rw-r--r--   0        0        0        0 2023-08-02 16:06:36.147338 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/py.typed
+-rw-r--r--   0        0        0      163 2023-08-02 16:16:22.090425 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/wrap/__init__.py
+-rw-r--r--   0        0        0     2481 2023-08-02 16:16:22.094425 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/wrap/module.py
+-rw-r--r--   0        0        0      816 2023-08-02 16:16:22.094425 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/wrap/types.py
+-rw-r--r--   0        0        0     7359 2023-08-02 16:16:22.094425 polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1709 2023-08-02 16:15:47.944340 polywrap_ethereum_provider-0.1.0b3/pyproject.toml
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0b3/PKG-INFO
```

### Comparing `polywrap_ethereum_provider-0.1.0b2/README.md` & `polywrap_ethereum_provider-0.1.0b3/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/__init__.py` & `polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/connection.py` & `polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/connection.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/connections.py` & `polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/connections.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/networks.py` & `polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/networks.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/module.py` & `polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/wrap/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/types.py` & `polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/wrap/types.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/wrap_info.py` & `polywrap_ethereum_provider-0.1.0b3/polywrap_ethereum_provider/wrap/wrap_info.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0b2/pyproject.toml` & `polywrap_ethereum_provider-0.1.0b3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-ethereum-provider"
-version = "0.1.0b2"
+version = "0.1.0b3"
 description = "Ethereum provider in python"
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [{include = "polywrap_ethereum_provider"}]
 include = ["polywrap_ethereum_provider/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 web3 = "6.1.0"
 eth_account = "0.8.0"
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
 eth-tester = "^0.8.0b3"
 pytest = "^7.1.2"
```

### Comparing `polywrap_ethereum_provider-0.1.0b2/PKG-INFO` & `polywrap_ethereum_provider-0.1.0b3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: polywrap-ethereum-provider
-Version: 0.1.0b2
+Version: 0.1.0b3
 Summary: Ethereum provider in python
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: eth_account (==0.8.0)
-Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-manifest (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-msgpack (>=0.1.0b2,<0.2.0)
-Requires-Dist: polywrap-plugin (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-core (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0b3,<0.2.0)
+Requires-Dist: polywrap-plugin (>=0.1.0b3,<0.2.0)
 Requires-Dist: web3 (==6.1.0)
 Description-Content-Type: text/markdown
 
 # polywrap-ethereum-plugin
 The Ethereum Provider plugin implements the `ethereum-provider-interface` @ [ens/wraps.eth:ethereum-provider@2.0.0](https://app.ens.domains/name/wraps.eth/details) (see [../../interface/polywrap.graphql](../../interface/polywrap.graphql)). It handles Ethereum wallet transaction signatures and sends JSON RPC requests for the Ethereum wrapper.
 
 ## Usage
```

