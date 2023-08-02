# Comparing `tmp/fyers_sdk-2.1.2.tar.gz` & `tmp/fyers_sdk-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fyers_sdk-2.1.2.tar", last modified: Tue Aug  1 07:48:06 2023, max compression
+gzip compressed data, was "fyers_sdk-2.1.3.tar", last modified: Wed Aug  2 03:49:46 2023, max compression
```

## Comparing `fyers_sdk-2.1.2.tar` & `fyers_sdk-2.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:48:06.793663 fyers_sdk-2.1.2/
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.2/LICENSE.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:48:06.793663 fyers_sdk-2.1.2/PKG-INFO
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.2/README.md
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:48:06.773664 fyers_sdk-2.1.2/fyers_sdk/
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:48:06.793663 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/__init__.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    59911 2023-08-01 07:45:38.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/data_ws.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/defines.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     7541 2023-08-01 07:28:21.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/map.json
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    15427 2023-07-31 06:13:16.000000 fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/order_ws.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.2/fyers_sdk/__init__.py
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27819 2023-07-31 09:12:31.000000 fyers_sdk-2.1.2/fyers_sdk/fyersModel.py
--rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.2/fyers_sdk/fyers_logger.py
-drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-01 07:48:06.789663 fyers_sdk-2.1.2/fyers_sdk.egg-info/
--rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/PKG-INFO
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/SOURCES.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/dependency_links.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/requires.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-01 07:48:06.000000 fyers_sdk-2.1.2/fyers_sdk.egg-info/top_level.txt
--rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-01 07:48:06.793663 fyers_sdk-2.1.2/setup.cfg
--rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-01 07:47:37.000000 fyers_sdk-2.1.2/setup.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-02 03:49:46.533696 fyers_sdk-2.1.3/
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-07-31 10:25:54.000000 fyers_sdk-2.1.3/LICENSE.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-02 03:49:46.533696 fyers_sdk-2.1.3/PKG-INFO
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    10394 2023-07-28 07:31:02.000000 fyers_sdk-2.1.3/README.md
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-02 03:49:46.497690 fyers_sdk-2.1.3/fyers_sdk/
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-02 03:49:46.533696 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        0 2023-07-27 04:29:21.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/__init__.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    60166 2023-08-02 03:49:31.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/data_ws.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     1140 2023-08-01 06:21:10.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/defines.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     9833 2023-08-01 11:59:36.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/map.json
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    13641 2023-08-01 12:03:31.000000 fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/order_ws.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)       18 2023-07-31 06:13:23.000000 fyers_sdk-2.1.3/fyers_sdk/__init__.py
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)    27959 2023-08-01 12:53:43.000000 fyers_sdk-2.1.3/fyers_sdk/fyersModel.py
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)     3795 2023-07-27 04:39:16.000000 fyers_sdk-2.1.3/fyers_sdk/fyers_logger.py
+drwxrwxr-x   0 vinay     (1000) vinay     (1000)        0 2023-08-02 03:49:46.521694 fyers_sdk-2.1.3/fyers_sdk.egg-info/
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)    10791 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      446 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)        1 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)      115 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/requires.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       10 2023-08-02 03:49:46.000000 fyers_sdk-2.1.3/fyers_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 vinay     (1000) vinay     (1000)       38 2023-08-02 03:49:46.533696 fyers_sdk-2.1.3/setup.cfg
+-rwxrwxr-x   0 vinay     (1000) vinay     (1000)     1063 2023-08-02 03:47:35.000000 fyers_sdk-2.1.3/setup.py
```

### Comparing `fyers_sdk-2.1.2/LICENSE.txt` & `fyers_sdk-2.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.2/PKG-INFO` & `fyers_sdk-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers_sdk
-Version: 2.1.2
+Version: 2.1.3
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.2/README.md` & `fyers_sdk-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/data_ws.py` & `fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/data_ws.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,22 +32,22 @@
         self.log_path = log_path
         self.quotes_url = "https://api-t1.fyers.in/data/quotes"
         if log_path:
             self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
-                logger_handler=logging.FileHandler(log_path + "/fyersSocket.log"),
+                logger_handler=logging.FileHandler(log_path + "/fyersDataSocket.log"),
             )
         else:
             self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
-                logger_handler=logging.FileHandler("fyersSocket.log"),
+                logger_handler=logging.FileHandler("fyersDataSocket.log"),
             )
 
     def symbol_to_hsmtoken(self, symbols: list):
         """
         Converts symbols to HSM tokens.
 
         Args:
@@ -152,25 +152,25 @@
             write_to_file (bool, optional): Specifies if the class should run in the background.
                 Defaults to False.
             log_path (str, optional): The path to the log file. Defaults to None.
             litemode (bool, optional): Specifies if the class should run in litemode.
                 Defaults to False.
             reconnect (bool, optional): Specifies if the class should attempt to reconnect on failure.
                 Defaults to False.
-            OnMessage (callable, optional): Callback function to be executed when a message is received.
+            on_message (callable, optional): Callback function to be executed when a message is received.
                 Defaults to None.
-            OnError (callable, optional): Callback function to be executed when an error occurs.
+            on_error (callable, optional): Callback function to be executed when an error occurs.
                 Defaults to None.
-            OnOpen (callable, optional): Callback function to be executed when a connection is established.
+            on_connect (callable, optional): Callback function to be executed when a connection is established.
                 Defaults to None.
-            OnClose (callable, optional): Callback function to be executed when a connection is closed.
+            on_close (callable, optional): Callback function to be executed when a connection is closed.
                 Defaults to None.
         """
 
-        self.__url = "wss://socket.fydev.tech/hsm/v1-5/dev"
+        self.__url = "wss://socket.fyers.in/hsm/v1-5/prod"
         self.__access_token = access_token
         self.__hsm_token = ""
         self.log_path = log_path
         self.lite = litemode
         self.source = "PythonSDK-1.0.0"
         self.channel_num = 1
         self.channels = []
@@ -206,28 +206,27 @@
         self.reconnect_attempts = 0
         self.max_reconnect_attempts = 5
         self.reconnect_delay = 5
         self.index_sym = {}
         self.scrips_sym = {}
         self.symbol_token = {}
         self.ack_bool = False
-        self.__init_connection()
         if log_path:
             self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
-                logger_handler=logging.FileHandler(log_path + "fyersSocket.log"),
+                logger_handler=logging.FileHandler(log_path + "fyersDataSocket.log"),
             )
         else:
             self.data_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=3,
-                logger_handler=logging.FileHandler("fyersSocket.log"),
+                logger_handler=logging.FileHandler("fyersDataSocket.log"),
             )
         file_path = resource_filename('fyers_sdk.FyersWebsocket', 'map.json')
 
         with open(file_path, "r") as file:
             # Imported json file
             mapper = json.load(file)
 
@@ -1390,21 +1389,33 @@
             else:
                 print(f"Response: {message}")
 
     def on_open(self) -> None:
         """
         Performs initialization and waits before executing further actions.
         """
-        if self.__ws_object is not None:
+        if self.__ws_object is None:
             self.__init_connection()
             time.sleep(2)
 
         if self.OnOpen:
             self.OnOpen()
 
+
+    def connect(self) -> None:
+        """
+        Performs initialization and waits before executing further actions.
+        """
+        if self.__ws_object is None:
+            self.__init_connection()
+            time.sleep(2)
+        self.on_open()
+            
+
+
     def on_close(self, message: dict) -> None:
         """
         Handles the close event.
 
         Args:
             message (dict): The close message .
         """
```

### Comparing `fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/defines.py` & `fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/defines.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.2/fyers_sdk/FyersWebsocket/order_ws.py` & `fyers_sdk-2.1.3/fyers_sdk/FyersWebsocket/order_ws.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Callable, Dict, Optional
+from pkg_resources import resource_filename
 import websocket
 from threading import Thread
 import logging
 import threading
 import time
 import json
 from fyers_sdk.FyersWebsocket import defines
@@ -19,45 +20,53 @@
         return cls._instance
 
     def __init__(
         self,
         access_token: str,
         write_to_file: Optional[bool] = False,
         log_path: Optional[str] = None,
-        OnMessage: Optional[Callable] = None,
-        OnError: Optional[Callable] = None,
-        OnOpen: Optional[Callable] = None,
-        OnClose: Optional[Callable] = None,
+        on_message: Optional[Callable] = None,
+        on_error: Optional[Callable] = None,
+        on_connect: Optional[Callable] = None,
+        on_close: Optional[Callable] = None,
     ) -> None:
         """
         Initializes the class instance.
 
         Args:
             access_token (str): The access token to authenticate with.
             write_to_file (bool): Flag indicating whether to save data to file.
             log_path (str, optional): The path to the log file. Defaults to None.
-            OnMessage (callable, optional): Callback function for message events. Defaults to None.
-            OnError (callable, optional): Callback function for error events. Defaults to None.
-            OnOpen (callable, optional): Callback function for open events. Defaults to None.
-            OnClose (callable, optional): Callback function for close events. Defaults to None.
+            on_message (callable, optional): Callback function for message events. Defaults to None.
+            on_error (callable, optional): Callback function for error events. Defaults to None.
+            on_connect (callable, optional): Callback function for open events. Defaults to None.
+            on_close (callable, optional): Callback function for close events. Defaults to None.
         """
         self.__access_token = access_token
         self.__url = "wss://socket.fydev.tech/trade/v3"
         self.log_path = log_path
         self.__ws_object = None
         self.__ws_run = False
         self.ping_thread = None
         self.write_to_file = write_to_file
         self.background_flag = False
-        self.OnMessage = OnMessage
-        self.OnError = OnError
-        self.OnOpen = OnOpen
-        self.OnClose = OnClose
+        self.OnMessage = on_message
+        self.OnError = on_error
+        self.OnOpen = on_connect
+        self.OnClose = on_close
         self.__ws_object = None
         self.__url = "wss://socket.fyers.in/trade/v3"
+        file_path = resource_filename('fyers_sdk.FyersWebsocket', 'map.json')
+        with open(file_path, "r") as file:
+            # Imported json file
+            mapper = json.load(file)
+        self.position_mapper = mapper["position_mapper"]
+        self.order_mapper = mapper["order_mapper"]
+        self.trade_mapper = mapper["trade_mapper"]
+
 
         if log_path:
             self.order_logger = FyersLogger(
                 "FyersDataSocket",
                 "DEBUG",
                 stack_level=2,
                 logger_handler=logging.FileHandler(log_path + "/fyersOrderSocket.log"),
@@ -88,43 +97,18 @@
             msg (str): The message containing position data.
 
         Returns:
             Dict[str, Any] : The parsed position data in a specific format.
 
         """
         try:
-            position_data_keys = [
-                "buy_avg",
-                "buy_qty",
-                "buy_val",
-                "cf_buy_qty",
-                "cf_sell_qty",
-                "day_buy_qty",
-                "day_sell_qty",
-                "fy_token",
-                "id",
-                "net_avg",
-                "net_qty",
-                "pl_realized",
-                "product_type",
-                "segment",
-                "sell_avg",
-                "sell_qty",
-                "sell_val",
-                "symbol",
-                "tran_side",
-            ]
-            position_data = {key: msg["positions"][key] for key in position_data_keys}
-            position_data.update(
-                {
-                    "qty_multi": msg["positions"]["qty_multiplier"],
-                    "rbi_ref_rate": msg["positions"]["rbirefrate"],
-                    "sym_desc": msg["positions"]["symbol_desc"],
-                }
-            )
+            position_data = {}
+            for key , value in self.position_mapper:
+                if key in msg["positions"]:
+                    position_data[value] = msg["positions"][key]
 
             return {"ws_type": 1, "s": msg["s"], "d": position_data}
 
         except Exception as e:
             self.order_logger.error(e)
 
     def __parse_trade_data(self, msg: Dict[str, Any]) -> Dict[str, Any]:
@@ -135,31 +119,21 @@
             msg (str): The message containing trade data.
 
         Returns:
             Dict[str, Any] : The parsed trade data in a specific format.
 
         """
         try:
-            trade_data_keys = [
-                "id_fill",
-                "id",
-                "qty_traded",
-                "price_traded",
-                "traded_val",
-                "product_type",
-                "client_id",
-                "id_exchange",
-                "ord_type",
-                "tran_side",
-                "symbol",
-                "time_epoch",
-                "fy_token",
-            ]
-            trade_data = dict((key, msg["trades"][key]) for key in trade_data_keys)
-            trade_data["tradeNumber"] = msg["trades"]["id"]
+        
+            trade_data = {}
+            for key , value in self.trade_mapper.items():
+                if key in msg["orders"]:
+                    trade_data[value] = msg["orders"][key]
+
+
 
             return {"ws_type": 1, "s": msg["s"], "d": trade_data}
 
         except Exception as e:
             self.order_logger.error(e)
 
     def __parse_order_data(self, msg: Dict[str, Any]) -> Dict[str, Any]:
@@ -169,45 +143,18 @@
         Args:
             msg (Dict[str, Any]): The dictionary containing order update data.
 
         Returns:
             Dict[str, Any]: The parsed order update data in a specific format.
         """
         try:
-            key_map = {
-                "update_time_epoch_oms": "orderDateTime",
-                "id": "exchOrdId",
-                "product_type": "productType",
-                "instrument": "instrument",
-                "side": "side",
-                "ord_status": "status",
-                "qty": "qty",
-                "qty_filled": "filledQty",
-                "qty_remaining": "remainingQuantity",
-                "ord_type": "type",
-                "validity": "orderValidity",
-                "offline_flag": "offlineOrder",
-                "status_msg": "message",
-                "symbol": "symbol",
-                "fy_token": "fyToken",
-                "segment": "segment",
-                "dqQtyRem": "dqQtyRem",
-                "price_limit": "limitPrice",
-                "price_stop": "stopPrice",
-                "qty_disc": "discloseQty",
-                "price_traded": "tradedPrice",
-            }
-            order = msg["orders"]
-            order_data = {key_map[key]: order.get(key, 0) for key in key_map}
-
-            order_data["orderNumStatus"] = (
-                order["id"] + ":" + str(order["org_ord_status"])
-            )
-            order_data["id"] = order["id"]
-            # order_data["slNo"] = int(time.time())
+            order_data = {}
+            for key , value in self.order_mapper.items():
+                if key in msg["orders"]:
+                    order_data[value] = msg["orders"][key]
 
             return {"ws_type": 1, "s": msg["s"], "d": order_data}
 
         except Exception as e:
             self.order_logger.error(e)
 
     def __on_message(self, message: Dict[str, Any]):
```

### Comparing `fyers_sdk-2.1.2/fyers_sdk/fyersModel.py` & `fyers_sdk-2.1.3/fyers_sdk/fyersModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -460,18 +460,22 @@
             data: The data containing the order ID.
 
         Returns:
             The response JSON as a dictionary.
         """
         if self.is_async:
             response = asyncio.run(
-                self.service.get_async_call(Config.orderbook, self.header, params=data)
+                self.service.get_async_call(Config.orderbook, self.header)
             )
         else:
-            response = self.service.get_call(Config.orderbook, self.header, data=data)
+            response = self.service.get_call(Config.orderbook, self.header)
+        id_list = data['id'].split(",")
+        print(id_list)
+        response["orderBook"]= [order for order in response["orderBook"] if order["id"] in id_list]
+
         return response
 
     def orderbook(self) -> dict:
         """
         Retrieves the order information.
 
         Returns:
```

### Comparing `fyers_sdk-2.1.2/fyers_sdk/fyers_logger.py` & `fyers_sdk-2.1.3/fyers_sdk/fyers_logger.py`

 * *Files identical despite different names*

### Comparing `fyers_sdk-2.1.2/fyers_sdk.egg-info/PKG-INFO` & `fyers_sdk-2.1.3/fyers_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyers-sdk
-Version: 2.1.2
+Version: 2.1.3
 Summary: Fyers trading APIs.
 Home-page: https://github.com/FyersDev/fyers-api-py
 Author: Fyers-Tech
 Author-email: support@fyers.in
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fyers_sdk-2.1.2/setup.py` & `fyers_sdk-2.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
      name='fyers_sdk',  
-     version='2.1.2',
+     version='2.1.3',
      author="Fyers-Tech",
      author_email="support@fyers.in",
      description="Fyers trading APIs.",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/FyersDev/fyers-api-py",
      packages=setuptools.find_packages(),
```

