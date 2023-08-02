# Comparing `tmp/polywrap_web3_config_bundle-0.1.0a2.tar.gz` & `tmp/polywrap_web3_config_bundle-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_web3_config_bundle-0.1.0a2.tar", max compression
+gzip compressed data, was "polywrap_web3_config_bundle-0.1.0b2.tar", max compression
```

## Comparing `polywrap_web3_config_bundle-0.1.0a2.tar` & `polywrap_web3_config_bundle-0.1.0b2.tar`

### file list

```diff
@@ -1,13 +1,8 @@
--rw-r--r--   0        0        0       96 2023-06-24 18:15:22.294239 polywrap_web3_config_bundle-0.1.0a2/README.md
--rw-r--r--   0        0        0      125 2023-06-26 07:15:11.711839 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/__init__.py
--rw-r--r--   0        0        0     3728 2023-06-28 19:06:29.105946 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/bundle.py
--rw-r--r--   0        0        0      477 2023-06-26 07:13:33.455620 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/config.py
--rw-r--r--   0        0        0      505 2023-06-28 19:22:40.888826 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/embeds/__init__.py
--rw-r--r--   0        0        0     9034 2023-06-24 18:45:48.235758 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/embeds/ipfs-http-client/wrap.info
--rw-r--r--   0        0        0   150523 2023-06-24 18:45:48.238769 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/embeds/ipfs-http-client/wrap.wasm
--rw-r--r--   0        0        0     6954 2023-06-25 07:01:49.516775 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/embeds/ipfs-sync-resolver/wrap.info
--rwxr-xr-x   0        0        0   253658 2023-06-25 07:01:49.518407 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/embeds/ipfs-sync-resolver/wrap.wasm
--rw-r--r--   0        0        0        0 2023-06-24 18:15:22.307878 polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/py.typed
--rw-r--r--   0        0        0     1385 2023-07-02 09:01:28.431242 polywrap_web3_config_bundle-0.1.0a2/pyproject.toml
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 polywrap_web3_config_bundle-0.1.0a2/setup.py
--rw-r--r--   0        0        0      874 1970-01-01 00:00:00.000000 polywrap_web3_config_bundle-0.1.0a2/PKG-INFO
+-rw-r--r--   0        0        0       29 2023-07-29 08:59:38.302418 polywrap_web3_config_bundle-0.1.0b2/README.md
+-rw-r--r--   0        0        0      125 2023-07-29 08:59:38.300641 polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/__init__.py
+-rw-r--r--   0        0        0     2773 2023-07-29 10:35:18.362592 polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/bundle.py
+-rw-r--r--   0        0        0      477 2023-07-29 08:59:38.300531 polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/config.py
+-rw-r--r--   0        0        0        0 2023-07-29 08:59:38.301886 polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/py.typed
+-rw-r--r--   0        0        0     1341 2023-08-02 16:00:52.667052 polywrap_web3_config_bundle-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0      955 1970-01-01 00:00:00.000000 polywrap_web3_config_bundle-0.1.0b2/setup.py
+-rw-r--r--   0        0        0      807 1970-01-01 00:00:00.000000 polywrap_web3_config_bundle-0.1.0b2/PKG-INFO
```

### Comparing `polywrap_web3_config_bundle-0.1.0a2/polywrap_web3_config_bundle/bundle.py` & `polywrap_web3_config_bundle-0.1.0b2/polywrap_web3_config_bundle/bundle.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,68 +5,40 @@
 from polywrap_ethereum_provider import ethereum_provider_plugin
 from polywrap_ethereum_provider.connection import Connection
 from polywrap_ethereum_provider.connections import Connections
 from polywrap_ethereum_provider.networks import KnownNetwork
 from polywrap_sys_config_bundle import BundlePackage, sys_bundle
 from polywrap_uri_resolvers import ExtendableUriResolver
 
-from .embeds import get_embedded_wrap
-
 ethreum_provider_package = ethereum_provider_plugin(
     Connections(
         connections={
             "mainnet": Connection.from_network(KnownNetwork.mainnet, None),
             "goerli": Connection.from_network(KnownNetwork.goerli, None),
         },
         default_network="mainnet",
     )
 )
 
-ipfs_providers = [
-    "https://ipfs.wrappers.io",
-    "https://ipfs.io",
-]
-
-
 web3_bundle: Dict[str, BundlePackage] = {
     "http": sys_bundle["http"],
+    "ipfs_http_client": sys_bundle["ipfs_http_client"],
+    "ipfs_resolver": sys_bundle["ipfs_resolver"],
     "ethreum_provider": BundlePackage(
         uri=Uri.from_str("plugin/ethereum-provider@2.0.0"),
         package=ethreum_provider_package,
         implements=[
             Uri.from_str("ens/wraps.eth:ethereum-provider@2.0.0"),
             Uri.from_str("ens/wraps.eth:ethereum-provider@1.1.0"),
         ],
         redirects_from=[
             Uri.from_str("ens/wraps.eth:ethereum-provider@2.0.0"),
             Uri.from_str("ens/wraps.eth:ethereum-provider@1.1.0"),
         ],
     ),
-    "ipfs_http_client": BundlePackage(
-        uri=Uri.from_str("embed/ipfs-http-client@1.0.0"),
-        package=get_embedded_wrap("ipfs-http-client"),
-        implements=[Uri.from_str("ens/wraps.eth:ipfs-http-client@1.0.0")],
-        redirects_from=[Uri.from_str("ens/wraps.eth:ipfs-http-client@1.0.0")],
-    ),
-    "ipfs_resolver": BundlePackage(
-        uri=Uri.from_str("embed/sync-ipfs-uri-resolver-ext@1.0.1"),
-        package=get_embedded_wrap("ipfs-sync-resolver"),
-        implements=[
-            Uri.from_str("ens/wraps.eth:sync-ipfs-uri-resolver-ext@1.0.1"),
-            *ExtendableUriResolver.DEFAULT_EXT_INTERFACE_URIS,
-        ],
-        redirects_from=[
-            Uri.from_str("ens/wraps.eth:sync-ipfs-uri-resolver-ext@1.0.1"),
-        ],
-        env={
-            "provider": ipfs_providers[0],
-            "fallbackProviders": ipfs_providers[1:],
-            "retries": {"tryResolveUri": 2, "getFile": 2},
-        },
-    ),
     "ens_text_record_resolver": BundlePackage(
         uri=Uri.from_str("ipfs/QmXcHWtKkfrFmcczdMSXH7udsSyV3UJeoWzkaUqGBm1oYs"),
         implements=[
             Uri.from_str("ens/wraps.eth:ens-text-record-uri-resolver-ext@1.0.1"),
             *ExtendableUriResolver.DEFAULT_EXT_INTERFACE_URIS,
         ],
         redirects_from=[
```

### Comparing `polywrap_web3_config_bundle-0.1.0a2/pyproject.toml` & `polywrap_web3_config_bundle-0.1.0b2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,60 +1,56 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-web3-config-bundle"
-version = "0.1.0a2"
+version = "0.1.0b2"
 description = "Polywrap System Client Config Bundle"
 authors = ["Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [
     { include = "polywrap_web3_config_bundle" },
 ]
 include = ["**/wrap.info", "**/wrap.wasm"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-polywrap-core = "^0.1.0a2"
-polywrap-client-config-builder = "^0.1.0a2"
-polywrap-uri-resolvers = "^0.1.0a2"
-polywrap-manifest = "^0.1.0a2"
-polywrap-wasm = "^0.1.0a2"
-polywrap-ethereum-provider = "^0.1.0a2"
-polywrap-sys-config-bundle = "^0.1.0a2"
+polywrap-core = "^0.1.0b2"
+polywrap-client-config-builder = "^0.1.0b2"
+polywrap-uri-resolvers = "^0.1.0b2"
+polywrap-manifest = "^0.1.0b2"
+polywrap-wasm = "^0.1.0b2"
+polywrap-ethereum-provider = "^0.1.0b2"
+polywrap-sys-config-bundle = "^0.1.0b2"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+polywrap-client = {path = "../../polywrap-client", develop = true}
 pytest = "^7.1.2"
-pytest-asyncio = "^0.19.0"
 pylint = "^2.15.4"
 black = "^22.10.0"
 bandit = { version = "^1.7.4", extras = ["toml"]}
 tox = "^3.26.0"
 tox-poetry = "^0.4.1"
 isort = "^5.10.1"
 pyright = "^1.1.275"
 pydocstyle = "^6.1.1"
 
-[tool.poetry.group.dev.dependencies]
-polywrap-client = "^0.1.0a35"
-
 [tool.bandit]
 exclude_dirs = ["tests"]
 skips = ["B310"]
 
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
 ]
```

### Comparing `polywrap_web3_config_bundle-0.1.0a2/setup.py` & `polywrap_web3_config_bundle-0.1.0b2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['polywrap_web3_config_bundle', 'polywrap_web3_config_bundle.embeds']
+['polywrap_web3_config_bundle']
 
 package_data = \
-{'': ['*'],
- 'polywrap_web3_config_bundle.embeds': ['ipfs-http-client/*',
-                                        'ipfs-sync-resolver/*']}
+{'': ['*']}
 
 install_requires = \
-['polywrap-client-config-builder>=0.1.0a2,<0.2.0',
- 'polywrap-core>=0.1.0a2,<0.2.0',
- 'polywrap-ethereum-provider>=0.1.0a2,<0.2.0',
- 'polywrap-manifest>=0.1.0a2,<0.2.0',
- 'polywrap-sys-config-bundle>=0.1.0a2,<0.2.0',
- 'polywrap-uri-resolvers>=0.1.0a2,<0.2.0',
- 'polywrap-wasm>=0.1.0a2,<0.2.0']
+['polywrap-client-config-builder>=0.1.0b2,<0.2.0',
+ 'polywrap-core>=0.1.0b2,<0.2.0',
+ 'polywrap-ethereum-provider>=0.1.0b2,<0.2.0',
+ 'polywrap-manifest>=0.1.0b2,<0.2.0',
+ 'polywrap-sys-config-bundle>=0.1.0b2,<0.2.0',
+ 'polywrap-uri-resolvers>=0.1.0b2,<0.2.0',
+ 'polywrap-wasm>=0.1.0b2,<0.2.0']
 
 setup_kwargs = {
     'name': 'polywrap-web3-config-bundle',
-    'version': '0.1.0a2',
+    'version': '0.1.0b2',
     'description': 'Polywrap System Client Config Bundle',
-    'long_description': '# polywrap-test-cases\n\nThis package allows fetching wrap test-cases from the wrap-test-harness.\n',
+    'long_description': '# polywrap-web3-config-bundle',
     'author': 'Niraj',
     'author_email': 'niraj@polywrap.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

