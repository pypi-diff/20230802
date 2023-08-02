# Comparing `tmp/vertex_protocol-1.1.5.tar.gz` & `tmp/vertex_protocol-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vertex_protocol-1.1.5.tar", max compression
+gzip compressed data, was "vertex_protocol-1.1.6.tar", max compression
```

## Comparing `vertex_protocol-1.1.5.tar` & `vertex_protocol-1.1.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     3337 2023-07-16 20:07:10.825880 vertex_protocol-1.1.5/README.md
--rw-r--r--   0        0        0     1664 2023-07-16 20:07:10.825880 vertex_protocol-1.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/__init__.py
--rw-r--r--   0        0        0     6634 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/__init__.py
--rw-r--r--   0        0        0      580 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/__init__.py
--rw-r--r--   0        0        0     1394 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/base.py
--rw-r--r--   0        0        0     1108 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/market/__init__.py
--rw-r--r--   0        0        0     3404 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/market/execute.py
--rw-r--r--   0        0        0    10101 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/market/query.py
--rw-r--r--   0        0        0      746 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/perp/__init__.py
--rw-r--r--   0        0        0     1438 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/perp/query.py
--rw-r--r--   0        0        0     1027 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/spot/__init__.py
--rw-r--r--   0        0        0     1191 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/spot/base.py
--rw-r--r--   0        0        0     4782 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/spot/execute.py
--rw-r--r--   0        0        0     2964 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/spot/query.py
--rw-r--r--   0        0        0     1307 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/subaccount/__init__.py
--rw-r--r--   0        0        0     2023 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/subaccount/execute.py
--rw-r--r--   0        0        0     3669 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/apis/subaccount/query.py
--rw-r--r--   0        0        0     2554 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/client/context.py
--rw-r--r--   0        0        0     8786 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/__init__.py
--rw-r--r--   0        0        0    13215 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/Endpoint.json
--rw-r--r--   0        0        0    55374 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/FQuerier.json
--rw-r--r--   0        0        0    17205 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IClearinghouse.json
--rw-r--r--   0        0        0     3385 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IERC20.json
--rw-r--r--   0        0        0     5677 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IEndpoint.json
--rw-r--r--   0        0        0    13112 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IOffchainBook.json
--rw-r--r--   0        0        0    19201 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IPerpEngine.json
--rw-r--r--   0        0        0     6291 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IProductEngine.json
--rw-r--r--   0        0        0    16739 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/ISpotEngine.json
--rw-r--r--   0        0        0     5698 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/abis/MockERC20.json
--rw-r--r--   0        0        0     1013 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
--rw-r--r--   0        0        0      993 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
--rw-r--r--   0        0        0      908 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/deployments/deployment.test.json
--rw-r--r--   0        0        0      426 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/eip712/__init__.py
--rw-r--r--   0        0        0     1189 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/eip712/domain.py
--rw-r--r--   0        0        0     2484 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/eip712/sign.py
--rw-r--r--   0        0        0     4636 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/eip712/types.py
--rw-r--r--   0        0        0     1526 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/loader.py
--rw-r--r--   0        0        0     2914 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/contracts/types.py
--rw-r--r--   0        0        0     1127 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/engine_client/__init__.py
--rw-r--r--   0        0        0    18498 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/engine_client/execute.py
--rw-r--r--   0        0        0    11206 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/engine_client/query.py
--rw-r--r--   0        0        0     5739 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/engine_client/types/__init__.py
--rw-r--r--   0        0        0    18440 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/engine_client/types/execute.py
--rw-r--r--   0        0        0     3429 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/engine_client/types/models.py
--rw-r--r--   0        0        0     9841 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/engine_client/types/query.py
--rw-r--r--   0        0        0      926 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/indexer_client/__init__.py
--rw-r--r--   0        0        0    11793 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/indexer_client/query.py
--rw-r--r--   0        0        0     3077 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/indexer_client/types/__init__.py
--rw-r--r--   0        0        0     5656 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/indexer_client/types/models.py
--rw-r--r--   0        0        0    12832 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/indexer_client/types/query.py
--rw-r--r--   0        0        0      933 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/__init__.py
--rw-r--r--   0        0        0      341 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/backend.py
--rw-r--r--   0        0        0     5301 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/bytes32.py
--rw-r--r--   0        0        0       99 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/enum.py
--rw-r--r--   0        0        0     1136 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/exceptions.py
--rw-r--r--   0        0        0     1094 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/expiration.py
--rw-r--r--   0        0        0     1020 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/math.py
--rw-r--r--   0        0        0     2089 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/model.py
--rw-r--r--   0        0        0      863 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/nonce.py
--rw-r--r--   0        0        0      503 2023-07-16 20:07:10.829880 vertex_protocol-1.1.5/vertex_protocol/utils/subaccount.py
--rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3337 2023-08-02 20:23:25.909049 vertex_protocol-1.1.6/README.md
+-rw-r--r--   0        0        0     1664 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/__init__.py
+-rw-r--r--   0        0        0     6634 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/__init__.py
+-rw-r--r--   0        0        0      580 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/__init__.py
+-rw-r--r--   0        0        0     1394 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/base.py
+-rw-r--r--   0        0        0     1108 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/market/__init__.py
+-rw-r--r--   0        0        0     3516 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/market/execute.py
+-rw-r--r--   0        0        0    10439 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/market/query.py
+-rw-r--r--   0        0        0      746 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/perp/__init__.py
+-rw-r--r--   0        0        0     1438 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/perp/query.py
+-rw-r--r--   0        0        0     1027 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/__init__.py
+-rw-r--r--   0        0        0     1191 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/base.py
+-rw-r--r--   0        0        0     4782 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/execute.py
+-rw-r--r--   0        0        0     2964 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/query.py
+-rw-r--r--   0        0        0     1307 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/__init__.py
+-rw-r--r--   0        0        0     2023 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/execute.py
+-rw-r--r--   0        0        0     3669 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/query.py
+-rw-r--r--   0        0        0     2554 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/client/context.py
+-rw-r--r--   0        0        0     8786 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/__init__.py
+-rw-r--r--   0        0        0    13215 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/Endpoint.json
+-rw-r--r--   0        0        0    55374 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/FQuerier.json
+-rw-r--r--   0        0        0    17205 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IClearinghouse.json
+-rw-r--r--   0        0        0     3385 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IERC20.json
+-rw-r--r--   0        0        0     5677 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IEndpoint.json
+-rw-r--r--   0        0        0    13112 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IOffchainBook.json
+-rw-r--r--   0        0        0    19201 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IPerpEngine.json
+-rw-r--r--   0        0        0     6291 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IProductEngine.json
+-rw-r--r--   0        0        0    16739 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/ISpotEngine.json
+-rw-r--r--   0        0        0     5698 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/abis/MockERC20.json
+-rw-r--r--   0        0        0     1013 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json
+-rw-r--r--   0        0        0      993 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json
+-rw-r--r--   0        0        0      908 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.test.json
+-rw-r--r--   0        0        0      426 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/__init__.py
+-rw-r--r--   0        0        0     1189 2023-08-02 20:23:25.913054 vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/domain.py
+-rw-r--r--   0        0        0     2484 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/sign.py
+-rw-r--r--   0        0        0     4636 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/types.py
+-rw-r--r--   0        0        0     1526 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/contracts/loader.py
+-rw-r--r--   0        0        0     2914 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/contracts/types.py
+-rw-r--r--   0        0        0     1127 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/__init__.py
+-rw-r--r--   0        0        0    18741 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/execute.py
+-rw-r--r--   0        0        0    12030 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/query.py
+-rw-r--r--   0        0        0     5739 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/types/__init__.py
+-rw-r--r--   0        0        0    18756 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/types/execute.py
+-rw-r--r--   0        0        0     3505 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/types/models.py
+-rw-r--r--   0        0        0     9927 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/engine_client/types/query.py
+-rw-r--r--   0        0        0      926 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/__init__.py
+-rw-r--r--   0        0        0    11793 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/query.py
+-rw-r--r--   0        0        0     3077 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/__init__.py
+-rw-r--r--   0        0        0     5656 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/models.py
+-rw-r--r--   0        0        0    12832 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/query.py
+-rw-r--r--   0        0        0      933 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/__init__.py
+-rw-r--r--   0        0        0      341 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/backend.py
+-rw-r--r--   0        0        0     5301 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/bytes32.py
+-rw-r--r--   0        0        0       99 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/enum.py
+-rw-r--r--   0        0        0     1136 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/exceptions.py
+-rw-r--r--   0        0        0     1094 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/expiration.py
+-rw-r--r--   0        0        0     1020 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/math.py
+-rw-r--r--   0        0        0     2089 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/model.py
+-rw-r--r--   0        0        0      863 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/nonce.py
+-rw-r--r--   0        0        0      503 2023-08-02 20:23:25.917059 vertex_protocol-1.1.6/vertex_protocol/utils/subaccount.py
+-rw-r--r--   0        0        0     4119 1970-01-01 00:00:00.000000 vertex_protocol-1.1.6/PKG-INFO
```

### Comparing `vertex_protocol-1.1.5/README.md` & `vertex_protocol-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/pyproject.toml` & `vertex_protocol-1.1.6/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vertex-protocol"
-version = "1.1.5"
+version = "1.1.6"
 description = "Vertex Protocol SDK"
 authors = ["Jeury Mejia <jeury@vertexprotocol.com>"]
 homepage = "https://vertexprotocol.com/"
 maintainers = [
   "Frank Jia <frank@vertexprotocol.com>",
   "Clark Oh-Willeke <clark@vertexprotocol.com>"
 ]
```

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/base.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/market/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/market/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/market/execute.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/market/execute.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from vertex_protocol.engine_client.types.execute import (
     BurnLpParams,
     CancelOrdersParams,
     CancelProductOrdersParams,
     ExecuteResponse,
     MintLpParams,
-    PlaceOrderParams,
+    PlaceOrderParams, CancelOrdersResponse,
 )
 from vertex_protocol.client.apis.base import VertexBaseAPI
 
 
 class MarketExecuteAPI(VertexBaseAPI):
     """
     Provides functionality to interact with the Vertex's market execution APIs.
@@ -71,30 +71,30 @@
         """
         Cancels orders through the engine.
 
         Args:
             params (CancelOrdersParams): Parameters required to cancel orders.
 
         Returns:
-            ExecuteResponse: The response from the engine execution.
+            CancelOrdersResponse: A data class object containing information about the canceled product orders.
 
         Raises:
             Exception: If there is an error during the execution or the response status is not "success".
         """
         return self.context.engine_client.cancel_orders(params)
 
     def cancel_product_orders(
-        self, params: CancelProductOrdersParams
+            self, params: CancelProductOrdersParams
     ) -> ExecuteResponse:
         """
         Cancels all orders for provided products through the engine.
 
         Args:
             params (CancelProductOrdersParams): Parameters required to cancel product orders.
 
         Returns:
-            ExecuteResponse: The response from the engine execution.
+            CancelOrdersResponse: A data class object containing information about the canceled product orders.
 
         Raises:
             Exception: If there is an error during the execution or the response status is not "success".
         """
         return self.context.engine_client.cancel_product_orders(params)
```

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/market/query.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/market/query.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from vertex_protocol.client.apis.base import VertexBaseAPI
 from vertex_protocol.engine_client.types.query import (
     AllProductsData,
     MarketLiquidityData,
     MarketPriceData,
     MaxLpMintableData,
     MaxOrderSizeData,
+    ProductSymbolsData,
     SubaccountOpenOrdersData,
     QueryMaxOrderSizeParams,
 )
 from vertex_protocol.indexer_client.types.query import (
     IndexerCandlesticksData,
     IndexerCandlesticksParams,
     IndexerFundingRateData,
@@ -39,14 +40,23 @@
         Retrieves all market states from the off-chain engine.
 
         Returns:
             AllProductsData: A data class object containing information about all products in the engine.
         """
         return self.context.engine_client.get_all_products()
 
+    def get_all_product_symbols(self) -> ProductSymbolsData:
+        """
+        Retrieves all product symbols from the off-chain engine
+
+        Returns:
+            ProductSymbolsData: A list of all products with corresponding symbol.
+        """
+        return self.context.engine_client.get_product_symbols()
+
     def get_market_liquidity(self, product_id: int, depth: int) -> MarketLiquidityData:
         """
         Retrieves liquidity per price tick from the engine.
 
         The engine will skip price levels that have no liquidity,
         so it is not guaranteed that the bids/asks are evenly spaced
```

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/perp/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/perp/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/perp/query.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/perp/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/spot/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/spot/base.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/base.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/spot/execute.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/spot/query.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/spot/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/subaccount/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/subaccount/execute.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/execute.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/apis/subaccount/query.py` & `vertex_protocol-1.1.6/vertex_protocol/client/apis/subaccount/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/client/context.py` & `vertex_protocol-1.1.6/vertex_protocol/client/context.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/Endpoint.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/Endpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/FQuerier.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/FQuerier.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IClearinghouse.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IClearinghouse.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IERC20.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IEndpoint.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IEndpoint.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IOffchainBook.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IOffchainBook.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IPerpEngine.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IPerpEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/IProductEngine.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/IProductEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/ISpotEngine.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/ISpotEngine.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/abis/MockERC20.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/abis/MockERC20.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.arbitrumGoerli.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.arbitrumOne.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/deployments/deployment.test.json` & `vertex_protocol-1.1.6/vertex_protocol/contracts/deployments/deployment.test.json`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/eip712/domain.py` & `vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/domain.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/eip712/sign.py` & `vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/sign.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/eip712/types.py` & `vertex_protocol-1.1.6/vertex_protocol/contracts/eip712/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/loader.py` & `vertex_protocol-1.1.6/vertex_protocol/contracts/loader.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/contracts/types.py` & `vertex_protocol-1.1.6/vertex_protocol/contracts/types.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/engine_client/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/engine_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/engine_client/execute.py` & `vertex_protocol-1.1.6/vertex_protocol/engine_client/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,22 +24,27 @@
     LinkSignerParams,
     LiquidateSubaccountParams,
     MintLpParams,
     OrderParams,
     PlaceOrderParams,
     WithdrawCollateralParams,
     to_execute_request,
+    CancelOrdersResponse,
 )
 from vertex_protocol.contracts.types import VertexExecuteType
 
 from vertex_protocol.utils.exceptions import (
     BadStatusCodeException,
     ExecuteFailedException,
 )
-from vertex_protocol.utils.model import VertexBaseModel, is_instance_of_union
+from vertex_protocol.utils.model import (
+    VertexBaseModel,
+    is_instance_of_union,
+    ensure_data_type,
+)
 from vertex_protocol.utils.nonce import gen_order_nonce
 from vertex_protocol.utils.subaccount import SubaccountParams
 
 
 class EngineExecuteClient:
     """
     Client class for executing operations against the off-chain engine.
@@ -73,27 +78,29 @@
         if isinstance(params.sender, SubaccountParams):
             params.sender.subaccount_owner = (
                 params.sender.subaccount_owner or self.signer.address
             )
             params.sender = params.serialize_sender(params.sender)
         return params
 
-    def _inject_nonce_if_needed(self, params: Type[BaseParams]) -> Type[BaseParams]:
+    def _inject_nonce_if_needed(
+        self, params: Type[BaseParams], use_order_nonce: bool
+    ) -> Type[BaseParams]:
         """
         Inject the nonce if needed.
 
         Args:
             params (Type[BaseParams]): The parameters.
 
         Returns:
             Type[BaseParams]: The parameters with the nonce injected if needed.
         """
         if params.nonce is not None:
             return params
-        params.nonce = self.tx_nonce()
+        params.nonce = self.order_nonce() if use_order_nonce else self.tx_nonce()
         return params
 
     def tx_nonce(self) -> int:
         """
         Get the transaction nonce. Used to perform executes such as `withdraw_collateral`.
 
         Returns:
@@ -109,27 +116,28 @@
             recv_time_ms (int, optional): Received time in milliseconds.
 
         Returns:
             int: The generated order nonce.
         """
         return gen_order_nonce(recv_time_ms)
 
-    def prepare_execute_params(self, params: Type[BaseParams]) -> Type[BaseParams]:  # type: ignore
+    def prepare_execute_params(self, params: Type[BaseParams], use_order_nonce: bool) -> Type[
+        BaseParams]:  # type: ignore
         """
         Prepares the parameters for execution by ensuring that both owner and nonce are correctly set.
 
         Args:
             params (Type[BaseParams]): The original parameters.
 
         Returns:
             Type[BaseParams]: A copy of the original parameters with owner and nonce injected if needed.
         """
         params = deepcopy(params)
         params = self._inject_owner_if_needed(params)
-        params = self._inject_nonce_if_needed(params)
+        params = self._inject_nonce_if_needed(params, use_order_nonce)
         return params
 
     @singledispatchmethod
     def execute(self, params: Union[ExecuteParams, ExecuteRequest]) -> ExecuteResponse:
         """
         Executes the operation defined by the provided parameters.
 
@@ -384,15 +392,15 @@
             params (PlaceOrderParams): Parameters required for placing an order.
             The parameters include the order details and the product_id.
 
         Returns:
             ExecuteResponse: Response of the execution, including status and potential error message.
         """
         params = PlaceOrderParams.parse_obj(params)
-        params.order = self.prepare_execute_params(params.order)  # type: ignore
+        params.order = self.prepare_execute_params(params.order, True)  # type: ignore
         params.signature = params.signature or self._sign(
             VertexExecuteType.PLACE_ORDER, params.order.dict(), params.product_id
         )
         return self.execute(params)
 
     def cancel_orders(self, params: CancelOrdersParams) -> ExecuteResponse:
         """
@@ -401,15 +409,15 @@
         Args:
             params (CancelOrdersParams): Parameters required for canceling orders.
             The parameters include the order digests to be cancelled.
 
         Returns:
             ExecuteResponse: Response of the execution, including status and potential error message.
         """
-        params = self.prepare_execute_params(CancelOrdersParams.parse_obj(params))  # type: ignore
+        params = self.prepare_execute_params(CancelOrdersParams.parse_obj(params), True)  # type: ignore
         params.signature = params.signature or self._sign(
             VertexExecuteType.CANCEL_ORDERS, params.dict()
         )
         return self.execute(params)
 
     def cancel_product_orders(
         self, params: CancelProductOrdersParams
@@ -421,15 +429,15 @@
             params (CancelProductOrdersParams): Parameters required for bulk canceling orders of specific products.
             The parameters include a list of product ids to bulk cancel orders for.
 
         Returns:
             ExecuteResponse: Response of the execution, including status and potential error message.
         """
         params = self.prepare_execute_params(
-            CancelProductOrdersParams.parse_obj(params)  # type: ignore
+            CancelProductOrdersParams.parse_obj(params), True  # type: ignore
         )
         params.signature = params.signature or self._sign(
             VertexExecuteType.CANCEL_PRODUCT_ORDERS, params.dict()
         )
         return self.execute(params)
 
     def withdraw_collateral(self, params: WithdrawCollateralParams) -> ExecuteResponse:
@@ -439,15 +447,15 @@
         Args:
             params (WithdrawCollateralParams): Parameters required for withdrawing collateral.
             The parameters include the collateral details.
 
         Returns:
             ExecuteResponse: Response of the execution, including status and potential error message.
         """
-        params = self.prepare_execute_params(WithdrawCollateralParams.parse_obj(params))  # type: ignore
+        params = self.prepare_execute_params(WithdrawCollateralParams.parse_obj(params), False)  # type: ignore
         params.signature = params.signature or self._sign(
             VertexExecuteType.WITHDRAW_COLLATERAL, params.dict()
         )
         return self.execute(params)
 
     def liquidate_subaccount(
         self, params: LiquidateSubaccountParams
@@ -459,15 +467,15 @@
             params (LiquidateSubaccountParams): Parameters required for liquidating a subaccount.
             The parameters include the liquidatee details.
 
         Returns:
             ExecuteResponse: Response of the execution, including status and potential error message.
         """
         params = self.prepare_execute_params(
-            LiquidateSubaccountParams.parse_obj(params)  # type: ignore
+            LiquidateSubaccountParams.parse_obj(params), False  # type: ignore
         )
         params.signature = params.signature or self._sign(
             VertexExecuteType.LIQUIDATE_SUBACCOUNT,
             params.dict(),
         )
         return self.execute(params)
 
@@ -478,15 +486,15 @@
         Args:
             params (MintLpParams): Parameters required for minting LP tokens.
             The parameters include the LP details.
 
         Returns:
             ExecuteResponse: Response of the execution, including status and potential error message.
         """
-        params = self.prepare_execute_params(MintLpParams.parse_obj(params))  # type: ignore
+        params = self.prepare_execute_params(MintLpParams.parse_obj(params), False)  # type: ignore
         params.signature = params.signature or self._sign(
             VertexExecuteType.MINT_LP,
             params.dict(),
         )
         return self.execute(params)
 
     def burn_lp(self, params: BurnLpParams) -> ExecuteResponse:
@@ -496,15 +504,15 @@
         Args:
             params (BurnLpParams): Parameters required for burning LP tokens.
             The parameters include the LP details.
 
         Returns:
             ExecuteResponse: Response of the execution, including status and potential error message.
         """
-        params = self.prepare_execute_params(BurnLpParams.parse_obj(params))  # type: ignore
+        params = self.prepare_execute_params(BurnLpParams.parse_obj(params), False)  # type: ignore
         params.signature = params.signature or self._sign(
             VertexExecuteType.BURN_LP,
             params.dict(),
         )
         return self.execute(params)
 
     def link_signer(self, params: LinkSignerParams) -> ExecuteResponse:
@@ -514,13 +522,13 @@
         Args:
             params (LinkSignerParams): Parameters required for linking a signer.
             The parameters include the signer details.
 
         Returns:
             ExecuteResponse: Response of the execution, including status and potential error message.
         """
-        params = self.prepare_execute_params(LinkSignerParams.parse_obj(params))  # type: ignore
+        params = self.prepare_execute_params(LinkSignerParams.parse_obj(params), False)  # type: ignore
         params.signature = params.signature or self._sign(
             VertexExecuteType.LINK_SIGNER,
             params.dict(),
         )
         return self.execute(params)
```

### Comparing `vertex_protocol-1.1.5/vertex_protocol/engine_client/query.py` & `vertex_protocol-1.1.6/vertex_protocol/engine_client/query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Optional
 import requests
 from urllib.parse import urlencode
 
 from vertex_protocol.engine_client import EngineClientOpts
+from vertex_protocol.engine_client.types.models import ResponseStatus
 from vertex_protocol.engine_client.types.query import (
     AllProductsData,
     ContractsData,
     FeeRatesData,
     HealthGroupsData,
     LinkedSignerData,
     MarketLiquidityData,
     MarketPriceData,
     MaxLpMintableData,
     MaxOrderSizeData,
     MaxWithdrawableData,
     NoncesData,
+    ProductSymbolsData,
     SubaccountOpenOrdersData,
     OrderData,
     QueryAllProductsParams,
     QueryContractsParams,
     QueryFeeRatesParams,
     QueryHealthGroupsParams,
     QueryLinkedSignerParams,
@@ -81,14 +83,36 @@
             query_res = QueryResponse(**res.json())
         except Exception:
             raise QueryFailedException(res.text)
         if query_res.status != "success":
             raise QueryFailedException(res.text)
         return query_res
 
+    def get_product_symbols(self) -> ProductSymbolsData:
+        """
+        Retrieves symbols for all available products.
+
+        Returns:
+            ProductSymbolsData: Symbols for all available products.
+        """
+        res = requests.get(f"{self.url}/symbols?")
+        if res.status_code != 200:
+            raise BadStatusCodeException(res.text)
+        try:
+            query_res = QueryResponse(
+                status=ResponseStatus.SUCCESS,
+                data=res.json(),
+                error=None,
+                error_code=None,
+                request_type=None,
+            )
+        except Exception:
+            raise QueryFailedException(res.text)
+        return ensure_data_type(query_res.data, list)
+
     def get_status(self) -> StatusData:
         """
         Query the engine for its status.
 
         Returns:
             StatusData: The status of the engine.
         """
```

### Comparing `vertex_protocol-1.1.5/vertex_protocol/engine_client/types/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/engine_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/engine_client/types/execute.py` & `vertex_protocol-1.1.6/vertex_protocol/engine_client/types/execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from vertex_protocol.utils.bytes32 import (
     bytes32_to_hex,
     hex_to_bytes32,
     subaccount_to_bytes32,
 )
 from vertex_protocol.utils.nonce import gen_order_nonce
 from vertex_protocol.utils.subaccount import Subaccount, SubaccountParams
+from vertex_protocol.engine_client.types.query import OrderData
 
 
 Digest = Union[str, bytes]
 
 
 class BaseParams(VertexBaseModel):
     """
@@ -77,22 +78,21 @@
     Attributes:
         priceX18 (int): The price of the order with a precision of 18 decimal places.
 
         amount (int): The amount of the asset to be bought or sold in the order.
 
         expiration (int): The unix timestamp at which the order will expire.
 
-        nonce (int): A unique number used to prevent replay attacks. By default, a new nonce is generated.
-        see `gen_order_nonce` for more info.
+        nonce (Optional[int]): A unique number used to prevent replay attacks.
     """
 
     priceX18: int
     amount: int
     expiration: int
-    nonce: int = gen_order_nonce()
+    nonce: Optional[int]
 
 
 class PlaceOrderParams(SignatureParams):
     """
     Class for defining the parameters needed to place an order.
 
     Attributes:
@@ -116,24 +116,23 @@
     Parameters to cancel specific orders.
 
     Args:
         productIds (list[int]): List of product IDs for the orders to be canceled.
 
         digests (list[Digest]): List of digests of the orders to be canceled.
 
-        nonce (int): A unique number used to prevent replay attacks. By default, a new nonce is generated.
-        see `gen_order_nonce` for more info.
+        nonce (Optional[int]): A unique number used to prevent replay attacks.
 
     Methods:
         serialize_digests: Validates and converts a list of hex digests to bytes32.
     """
 
     productIds: list[int]
     digests: list[Digest]
-    nonce: int = gen_order_nonce()
+    nonce: Optional[int]
 
     @validator("digests")
     def serialize_digests(cls, v: list[Digest]) -> list[bytes]:
         return [hex_to_bytes32(digest) for digest in v]
 
 
 class CancelProductOrdersParams(BaseParamsSigned):
@@ -141,21 +140,20 @@
     Parameters to cancel all orders for specific products.
 
     Args:
         productIds (list[int]): List of product IDs for the orders to be canceled.
 
         digest (str, optional): Optional EIP-712 digest of the CancelProductOrder request.
 
-        nonce (int): A unique number used to prevent replay attacks. By default, a new nonce is generated.
-        see `gen_order_nonce` for more info.
+        nonce (Optional[int]): A unique number used to prevent replay attacks.
     """
 
     productIds: list[int]
     digest: Optional[str]
-    nonce: int = gen_order_nonce()
+    nonce: Optional[int]
 
 
 class WithdrawCollateralParams(BaseParamsSigned):
     """
     Parameters required to withdraw collateral from a specific product.
 
     Attributes:
@@ -535,35 +533,57 @@
     WithdrawCollateralRequest,
     LiquidateSubaccountRequest,
     MintLpRequest,
     BurnLpRequest,
     LinkSignerRequest,
 ]
 
+class PlaceOrderResponse(VertexBaseModel):
+    """
+    Data model for place order response.
+    """
+
+    digest: str
+class CancelOrdersResponse(VertexBaseModel):
+    """
+    Data model for cancelled orders response.
+    """
+
+    cancelled_orders: list[OrderData]
+
+
+ExecuteResponseData = Union[
+    PlaceOrderResponse,
+    CancelOrdersResponse
+]
+
 
 class ExecuteResponse(VertexBaseModel):
     """
     Represents the response returned from executing a request.
 
     Attributes:
         status (ResponseStatus): The status of the response.
 
         signature (Optional[str]): The signature of the response. Only present if the request was successfully executed.
 
+        data (Optional[ExecuteResponseData]): Data returned from execute, not all executes currently return data.
+
         error_code (Optional[int]): The error code, if any error occurred during the execution of the request.
 
         error (Optional[str]): The error message, if any error occurred during the execution of the request.
 
         request_type (Optional[str]): Type of the request.
 
         req (Optional[dict]): The original request that was executed.
     """
 
     status: ResponseStatus
     signature: Optional[str]
+    data: Optional[ExecuteResponseData]
     error_code: Optional[int]
     error: Optional[str]
     request_type: Optional[str]
     req: Optional[dict]
 
 
 def to_execute_request(params: ExecuteParams) -> ExecuteRequest:
```

### Comparing `vertex_protocol-1.1.5/vertex_protocol/engine_client/types/models.py` & `vertex_protocol-1.1.6/vertex_protocol/engine_client/types/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -163,9 +163,14 @@
 
 
 class MaxOrderSizeDirection(StrEnum):
     LONG = "long"
     SHORT = "short"
 
 
+class ProductSymbol(VertexBaseModel):
+    product_id: int
+    symbol: str
+
+
 # (price, amount)
 Liquidity = Annotated[list, conlist(str, min_items=2, max_items=2)]
```

### Comparing `vertex_protocol-1.1.5/vertex_protocol/engine_client/types/query.py` & `vertex_protocol-1.1.6/vertex_protocol/engine_client/types/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from vertex_protocol.engine_client.types.models import (
     ApplyDeltaTx,
     BurnLpTx,
     EngineStatus,
     Liquidity,
     MaxOrderSizeDirection,
     MintLpTx,
+    ProductSymbol,
     ResponseStatus,
     SpotProduct,
     SubaccountHealth,
     SpotProductBalance,
     PerpProduct,
     PerpProductBalance,
 )
@@ -377,14 +378,17 @@
     """
     Data model for the signer linked to a subaccount.
     """
 
     linked_signer: str
 
 
+ProductSymbolsData = list[ProductSymbol]
+
+
 QueryResponseData = Union[
     StatusData,
     ContractsData,
     NoncesData,
     OrderData,
     SubaccountInfoData,
     SubaccountOpenOrdersData,
@@ -393,14 +397,15 @@
     MarketPriceData,
     MaxOrderSizeData,
     MaxWithdrawableData,
     MaxLpMintableData,
     FeeRatesData,
     HealthGroupsData,
     LinkedSignerData,
+    ProductSymbolsData,
 ]
 
 
 class QueryResponse(VertexBaseModel):
     """
     Represents a response to a query request.
```

### Comparing `vertex_protocol-1.1.5/vertex_protocol/indexer_client/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/indexer_client/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/indexer_client/query.py` & `vertex_protocol-1.1.6/vertex_protocol/indexer_client/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/indexer_client/types/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/indexer_client/types/models.py` & `vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/models.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/indexer_client/types/query.py` & `vertex_protocol-1.1.6/vertex_protocol/indexer_client/types/query.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/utils/__init__.py` & `vertex_protocol-1.1.6/vertex_protocol/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/utils/bytes32.py` & `vertex_protocol-1.1.6/vertex_protocol/utils/bytes32.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/utils/exceptions.py` & `vertex_protocol-1.1.6/vertex_protocol/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/utils/expiration.py` & `vertex_protocol-1.1.6/vertex_protocol/utils/expiration.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/utils/math.py` & `vertex_protocol-1.1.6/vertex_protocol/utils/math.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/utils/model.py` & `vertex_protocol-1.1.6/vertex_protocol/utils/model.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/vertex_protocol/utils/nonce.py` & `vertex_protocol-1.1.6/vertex_protocol/utils/nonce.py`

 * *Files identical despite different names*

### Comparing `vertex_protocol-1.1.5/PKG-INFO` & `vertex_protocol-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vertex-protocol
-Version: 1.1.5
+Version: 1.1.6
 Summary: Vertex Protocol SDK
 Home-page: https://vertexprotocol.com/
 Keywords: vertex protocol,vertex sdk,vertex protocol api
 Author: Jeury Mejia
 Author-email: jeury@vertexprotocol.com
 Maintainer: Frank Jia
 Maintainer-email: frank@vertexprotocol.com
```

