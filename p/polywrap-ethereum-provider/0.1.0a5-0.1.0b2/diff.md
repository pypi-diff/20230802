# Comparing `tmp/polywrap_ethereum_provider-0.1.0a5.tar.gz` & `tmp/polywrap_ethereum_provider-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polywrap_ethereum_provider-0.1.0a5.tar", max compression
+gzip compressed data, was "polywrap_ethereum_provider-0.1.0b2.tar", max compression
```

## Comparing `polywrap_ethereum_provider-0.1.0a5.tar` & `polywrap_ethereum_provider-0.1.0b2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1646 2023-06-28 18:49:26.192624 polywrap_ethereum_provider-0.1.0a5/README.md
--rw-r--r--   0        0        0     6661 2023-06-28 18:49:26.192624 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/__init__.py
--rw-r--r--   0        0        0     1789 2023-06-28 18:49:26.196624 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/connection.py
--rw-r--r--   0        0        0     2759 2023-06-28 18:49:26.196624 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/connections.py
--rw-r--r--   0        0        0     1451 2023-06-28 18:49:26.196624 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/networks.py
--rw-r--r--   0        0        0        0 2023-06-28 18:49:26.196624 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/py.typed
--rw-r--r--   0        0        0      163 2023-06-28 18:49:43.628651 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/wrap/__init__.py
--rw-r--r--   0        0        0     2481 2023-06-28 18:49:43.628651 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/wrap/module.py
--rw-r--r--   0        0        0      816 2023-06-28 18:49:43.628651 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/wrap/types.py
--rw-r--r--   0        0        0     7359 2023-06-28 18:49:43.628651 polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/wrap/wrap_info.py
--rw-r--r--   0        0        0     1629 2023-06-28 18:49:26.196624 polywrap_ethereum_provider-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0     2266 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0     1646 2023-07-29 08:59:38.305561 polywrap_ethereum_provider-0.1.0b2/README.md
+-rw-r--r--   0        0        0     6610 2023-07-29 16:11:00.364857 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/__init__.py
+-rw-r--r--   0        0        0     1813 2023-07-29 16:11:00.321347 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/connection.py
+-rw-r--r--   0        0        0     2730 2023-07-29 16:11:00.331355 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/connections.py
+-rw-r--r--   0        0        0     1452 2023-07-29 16:11:00.316852 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/networks.py
+-rw-r--r--   0        0        0        0 2023-07-29 08:59:38.304579 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/py.typed
+-rw-r--r--   0        0        0      163 2023-08-02 15:55:35.220977 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/__init__.py
+-rw-r--r--   0        0        0     2481 2023-08-02 15:55:35.221148 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/module.py
+-rw-r--r--   0        0        0      816 2023-08-02 15:55:35.221230 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/types.py
+-rw-r--r--   0        0        0     7359 2023-08-02 15:55:35.221343 polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/wrap_info.py
+-rw-r--r--   0        0        0     1709 2023-08-02 15:55:12.706846 polywrap_ethereum_provider-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2526 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0b2/setup.py
+-rw-r--r--   0        0        0     2290 1970-01-01 00:00:00.000000 polywrap_ethereum_provider-0.1.0b2/PKG-INFO
```

### Comparing `polywrap_ethereum_provider-0.1.0a5/README.md` & `polywrap_ethereum_provider-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/__init__.py` & `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     Module,
     manifest,
 )
 
 
 class EthereumProviderPlugin(Module[Connections]):
     """A Polywrap plugin for interacting with EVM networks."""
+
     def __init__(self, connections: Connections):
         super().__init__(connections)
         self.connections = connections
 
     def request(
         self,
         args: ArgsRequest,
@@ -75,17 +76,15 @@
         args: ArgsSignerAddress,
         client: InvokerClient,
         env: Optional[Any] = None,
     ) -> Optional[str]:
         """Get the ethereum address of the signer. Return null if signer is missing."""
         connection = self.connections.get_connection(args.get("connection"))
         if connection.has_signer():
-            return Account.from_key(
-                connection.signer
-            ).address
+            return Account.from_key(connection.signer).address
         return None
 
     def wait_for_transaction(
         self,
         args: ArgsWaitForTransaction,
         client: InvokerClient,
         env: Optional[Any] = None,
@@ -144,17 +143,15 @@
         Throws if signer is missing.\
         This method requires a wallet-based signer with a private key,\
         and is not needed for most use cases.\
         Typically, transactions are sent by `request` and signed by the wallet.
         """
         connection = self.connections.get_connection(args.get("connection"))
         tx_hash = keccak(args["rlp"])
-        account = Account.from_key(
-            connection.signer
-        )
+        account = Account.from_key(connection.signer)
         key_obj = account._key_obj  # type: ignore
         (v, r, s, eth_signature_bytes) = sign_message_hash(key_obj, tx_hash)  # type: ignore
         return HexBytes(cast(bytes, eth_signature_bytes)).hex()
 
     def _get_transaction_receipt(
         self,
         args: ArgsWaitForTransaction,
```

### Comparing `polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/connection.py` & `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     __slots__: Tuple[str, str] = ("_provider", "_signer")
 
     _provider: JSONBaseProvider
     _signer: Optional[str]  # Private key
 
     def __init__(self, provider: JSONBaseProvider | str, signer: Optional[str]):
         """Initialize a connection to an EVM network."""
-        self._provider = Web3.HTTPProvider(provider) if isinstance(provider, str) else provider
+        self._provider = (
+            Web3.HTTPProvider(provider) if isinstance(provider, str) else provider
+        )
         self._signer = signer
 
     @property
     def provider(self) -> JSONBaseProvider:
         """EVM network provider."""
         return self._provider
```

### Comparing `polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/connections.py` & `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/connections.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .connection import Connection
 from .networks import KnownNetwork
 from .wrap.types import Connection as SchemaConnection
 
 
 class Connections:
     """Defines a set of connections to EVM networks."""
+
     __slots__: Tuple[str, str, str] = ("connections", "default_network", "signer")
 
     connections: Dict[str, Connection]
     default_network: str
     signer: Optional[str]
 
     def __init__(
@@ -30,17 +31,15 @@
                     f"Default network: {default_network} not in connections"
                 )
             self.default_network = default_network
         elif "mainnet" in self.connections:
             self.default_network = "mainnet"
         else:
             self.default_network = "mainnet"
-            self.connections["mainnet"] = Connection.from_network(
-                KnownNetwork.mainnet
-            )
+            self.connections["mainnet"] = Connection.from_network(KnownNetwork.mainnet)
 
     def get_connection(self, connection: Optional[SchemaConnection]) -> Connection:
         """Get a connection from a connection object."""
         if not connection:
             return self.with_signer(self.connections[self.default_network])
 
         if connection.get("networkNameOrChainId"):
```

### Comparing `polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/networks.py` & `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from enum import IntEnum, unique
 from typing import List
 
 
 @unique
 class KnownNetwork(IntEnum):
     """Defines a list of known networks."""
+
     mainnet = 1, "1", "mainnet"
     goerli = 5, "5", "goerli"
     sepolia = 11155111, "11155111", "sepolia"
     celo_mainnet = 42220, "42220", "celo_mainnet"
     celo_alfajores = 44787, "44787", "celo_alfajores"
     avalanche_mainnet = 43114, "43114", "avalanche_mainnet"
     avalanche_fuji = 43113, "43113", "avalanche_fuji"
```

### Comparing `polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/wrap/module.py` & `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/module.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/wrap/types.py` & `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/types.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a5/polywrap_ethereum_provider/wrap/wrap_info.py` & `polywrap_ethereum_provider-0.1.0b2/polywrap_ethereum_provider/wrap/wrap_info.py`

 * *Files identical despite different names*

### Comparing `polywrap_ethereum_provider-0.1.0a5/pyproject.toml` & `polywrap_ethereum_provider-0.1.0b2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,59 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "polywrap-ethereum-provider"
-version = "0.1.0a5"
+version = "0.1.0b2"
 description = "Ethereum provider in python"
 authors = ["Cesar <cesar@polywrap.io>", "Niraj <niraj@polywrap.io>"]
 readme = "README.md"
 packages = [{include = "polywrap_ethereum_provider"}]
 include = ["polywrap_ethereum_provider/wrap/**/*"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 web3 = "6.1.0"
 eth_account = "0.8.0"
-polywrap-plugin = "0.1.0a35"
-polywrap-core = "0.1.0a35"
-polywrap-msgpack = "0.1.0a35"
-polywrap-manifest = "0.1.0a35"
+polywrap-plugin = "^0.1.0b2"
+polywrap-core = "^0.1.0b2"
+polywrap-msgpack = "^0.1.0b2"
+polywrap-manifest = "^0.1.0b2"
 
 [tool.poetry.group.dev.dependencies]
+polywrap-client = {path = "../../polywrap-client", develop = true}
+polywrap-uri-resolvers = {path = "../../polywrap-uri-resolvers", develop = true}
+polywrap-client-config-builder = {path = "../../polywrap-client-config-builder", develop = true}
 eth-tester = "^0.8.0b3"
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
-polywrap-client = "0.1.0a35"
-polywrap-client-config-builder = "0.1.0a35"
-polywrap-uri-resolvers = "^0.1.0a35"
 
 [tool.bandit]
 exclude_dirs = ["tests"]
 
 [tool.black]
 target-version = ["py310"]
-exclude = [
-    "polywrap_ethereum_provider/wrap"
-]
+exclude = "polywrap_ethereum_provider/wrap/*"
 
 [tool.pyright]
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

### Comparing `polywrap_ethereum_provider-0.1.0a5/PKG-INFO` & `polywrap_ethereum_provider-0.1.0b2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: polywrap-ethereum-provider
-Version: 0.1.0a5
+Version: 0.1.0b2
 Summary: Ethereum provider in python
 Author: Cesar
 Author-email: cesar@polywrap.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: eth_account (==0.8.0)
-Requires-Dist: polywrap-core (==0.1.0a35)
-Requires-Dist: polywrap-manifest (==0.1.0a35)
-Requires-Dist: polywrap-msgpack (==0.1.0a35)
-Requires-Dist: polywrap-plugin (==0.1.0a35)
+Requires-Dist: polywrap-core (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-manifest (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-msgpack (>=0.1.0b2,<0.2.0)
+Requires-Dist: polywrap-plugin (>=0.1.0b2,<0.2.0)
 Requires-Dist: web3 (==6.1.0)
 Description-Content-Type: text/markdown
 
 # polywrap-ethereum-plugin
 The Ethereum Provider plugin implements the `ethereum-provider-interface` @ [ens/wraps.eth:ethereum-provider@2.0.0](https://app.ens.domains/name/wraps.eth/details) (see [../../interface/polywrap.graphql](../../interface/polywrap.graphql)). It handles Ethereum wallet transaction signatures and sends JSON RPC requests for the Ethereum wrapper.
 
 ## Usage
```

