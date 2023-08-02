# Comparing `tmp/microservicebus-py-0.9.7.tar.gz` & `tmp/microservicebus-py-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservicebus-py-0.9.7.tar", last modified: Wed Jun 21 15:55:54 2023, max compression
+gzip compressed data, was "microservicebus-py-0.9.8.tar", last modified: Wed Aug  2 09:45:40 2023, max compression
```

## Comparing `microservicebus-py-0.9.7.tar` & `microservicebus-py-0.9.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-21 15:55:54.766540 microservicebus-py-0.9.7/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-21 15:55:54.755114 microservicebus-py-0.9.7/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.7/README.md
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-21 15:55:53.724276 microservicebus-py-0.9.7/microservicebus_py.egg-info/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-06-21 15:55:52.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-06-21 15:55:53.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-06-21 15:55:52.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-06-21 15:55:52.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/entry_points.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-06-21 15:55:52.000000 microservicebus-py-0.9.7/microservicebus_py.egg-info/top_level.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-06-21 15:55:54.771607 microservicebus-py-0.9.7/setup.cfg
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.7/setup.py
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-06-21 15:55:54.645519 microservicebus-py-0.9.7/src/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.7/src/axians.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.7/src/base_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1609 2023-06-08 22:01:37.000000 microservicebus-py-0.9.7/src/logger_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)    31975 2023-06-21 15:52:13.000000 microservicebus-py-0.9.7/src/msb_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6541 2023-06-09 06:40:37.000000 microservicebus-py-0.9.7/src/orchestrator_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.7/src/queue_message.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.7/src/rauc_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.7/src/start.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.7/src/terminal_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.7/src/test.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.7/src/utils.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.7/src/vpn_helper.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 09:45:40.200931 microservicebus-py-0.9.8/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-08-02 09:45:40.196930 microservicebus-py-0.9.8/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.8/README.md
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 09:45:39.712525 microservicebus-py-0.9.8/microservicebus_py.egg-info/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/top_level.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-08-02 09:45:40.202929 microservicebus-py-0.9.8/setup.cfg
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.8/setup.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 09:45:40.163307 microservicebus-py-0.9.8/src/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.8/src/axians.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.8/src/base_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1609 2023-06-08 22:01:37.000000 microservicebus-py-0.9.8/src/logger_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)    33829 2023-08-02 09:29:44.000000 microservicebus-py-0.9.8/src/msb_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6541 2023-07-07 07:09:27.000000 microservicebus-py-0.9.8/src/orchestrator_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.8/src/queue_message.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.8/src/rauc_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.8/src/start.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.8/src/terminal_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.8/src/test.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.8/src/utils.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.8/src/vpn_helper.py
```

### Comparing `microservicebus-py-0.9.7/PKG-INFO` & `microservicebus-py-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.7/README.md` & `microservicebus-py-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/microservicebus_py.egg-info/PKG-INFO` & `microservicebus-py-0.9.8/microservicebus_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.7/setup.py` & `microservicebus-py-0.9.8/setup.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/axians.py` & `microservicebus-py-0.9.8/src/axians.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/base_service.py` & `microservicebus-py-0.9.8/src/base_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/logger_service.py` & `microservicebus-py-0.9.8/src/logger_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/msb_handler.py` & `microservicebus-py-0.9.8/src/msb_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from base_service import BaseService
 from pathlib import Path
+from logging.handlers import RotatingFileHandler
 from signalrcore.hub_connection_builder import HubConnectionBuilder
 from packaging import version
+from urllib import parse
 import asyncio
 import importlib
 import pathlib
 import uuid
 import re
 import sys
 import traceback
@@ -20,14 +22,21 @@
 import urllib.request
 import threading
 import platform
 import utils
 import ssl
 ssl._create_default_https_context = ssl._create_unverified_context
 
+logging.basicConfig (
+    handlers=[RotatingFileHandler('/var/log/microservicebus-py.log', maxBytes=100000, backupCount=7)],
+    format='%(asctime)s: %(message)s',
+    encoding='utf-8',
+    level=logging.WARNING
+)
+
 class microServiceBusHandler(BaseService):
     # region Constructor
     def __init__(self, id, queue):
         self.ready = False
         self._connected = False
         self._reconnect = False
         self.signed_in = False
@@ -246,16 +255,16 @@
             }).build()
 
         self.connection.keepAliveIntervalInMilliseconds = 1000 * 60 * 3
         self.connection.serverTimeoutInMilliseconds = 1000 * 60 * 6
         # Default listeners
         self.connection.on_open(lambda: self.connected())
         self.connection.on_close(lambda: self.disconnected())
-        self.connection.on_error(lambda data: self.debug_sync(f"An exception was thrown closed{data.error}"))
-        self.connection.on_reconnect(lambda: self.debug_sync(f"Reconnected to {self.base_uri}"))
+        self.connection.on_error(lambda data: self.debug_sync(f"An exception was thrown: {data.error}"))
+        self.connection.on_reconnect(lambda args: self.reconnected())
 
         # mSB.com listeners
         self.connection.on("nodeCreated", lambda sign_in_info: self.sign_in_sync(sign_in_info[0], True))
         self.connection.on("signInMessage", lambda sign_in_response: self.successful_sign_in(sign_in_response[0]))
         self.connection.on("updatedToken", lambda args: self.update_token(args[0]))
         self.connection.on("ping", lambda conn_id: self.ping_response(conn_id[0]))
         self.connection.on("errorMessage", lambda arg: self.handle_error(arg))
@@ -273,14 +282,15 @@
         self.connection.on("getVpnSettingsResponse", lambda vpn_response: self.get_vpn_settings_response(
             vpn_response[0], vpn_response[1], vpn_response[2]))
         self.connection.on("refreshVpnSettings", lambda response: self.refresh_vpn_settings_sync(response))
         self.connection.on("sendMessage", lambda args: self.debug_sync(args[0]))
         self.connection.on("startTerminal", lambda args: self.start_terminal(args[0], args[1]))
         self.connection.on("stopTerminal", lambda args: self.stop_terminal())
         self.connection.on("terminalCommand", lambda args: self.terminal_command(args[0]))
+        self.connection.on("downloadFile", lambda args: self.download_file(args[0]))
 
         # region Not implemented event handlers
         self.connection.on(
             "getEndpoints", lambda response: self.not_implemented("getEndpoints"))
         self.connection.on(
             "updateItinerary", lambda response: self.not_implemented("updateItinerary"))
         self.connection.on(
@@ -335,26 +345,26 @@
             "dockerComposeList", lambda response: self.not_implemented("dockerComposeList"))
         self.connection.on("dockerComposeInstall", lambda response: self.not_implemented(
             "dockerComposeInstall"))
         self.connection.on(
             "dockerComposeUp", lambda response: self.not_implemented("dockerComposeUp"))
         self.connection.on(
             "dockerComposeDown", lambda response: self.not_implemented("dockerComposeDown"))
-        self.connection.on(
-            "downloadFile", lambda response: self.not_implemented("downloadFile"))
+        # self.connection.on(
+        #     "downloadFile", lambda response: self.not_implemented("downloadFile"))
         self.connection.on(
             "uploadFile", lambda response: self.not_implemented("uploadFile"))
         # endregion
 
         self.connection.start()
         time.sleep(2)
         print(self.settings)
 
         if "policies" not in self.settings:
-            self.settings["policies"] = { "disconnectPolicy": { "heartbeatTimeout": 30, "missedHearbeatLimit": 3}}
+            self.settings["policies"] = { "disconnectPolicy": { "heartbeatTimeout": 180, "missedHearbeatLimit": 3}}
 
         heartbeatTimeout = self.settings["policies"]["disconnectPolicy"]["heartbeatTimeout"]
         self.set_interval(self.send_heartbeat, heartbeatTimeout)
         await self.Debug(f"Start hearbeat at {heartbeatTimeout} seconds interval")
     # endregion
     # region SignalR callback functions
     def successful_sign_in(self, sign_in_response):
@@ -466,38 +476,54 @@
             self.connection.send("reconnected", [self.settings["id"]])
 
     def disconnected(self):
         self.debug_sync("Connection closed")
         self._connected = False
         self._reconnect = True
 
+    def reconnected(self):
+        self.debug_sync(f"Reconnected to {self.base_uri}")
+
     def send_heartbeat(self):
         if self._missedheartbeat > 1:
             asyncio.run(self.Debug(f"MISSING HEARTBEAT"))
             missedHearbeatLimit = self.settings["policies"]["disconnectPolicy"]["missedHearbeatLimit"]
             if self._missedheartbeat >= missedHearbeatLimit or self.signed_in == False:
                 asyncio.run(self.Debug(f"\033[93m{self._missedheartbeat} missing heartbeats exceeding limit ({missedHearbeatLimit}). Restarting process\033[0m"))
                 self.restart()
         
         #asyncio.run(self.Debug(f"Send heatbeat"))        
         self._missedheartbeat += 1
         self.connection.send("heartBeat", ["echo"])
     
     def receive_heartbeat(self, message):
         self._missedheartbeat = 0
-        #asyncio.run(self.Debug(f"Received heatbeat"))
+        try:
+            connection_id = parse.parse_qs(parse.urlparse(self.connection.transport.url).query)['id'][0]
+            asyncio.run(self.Debug(f"Received heatbeat => connection_id: {connection_id}"))
+        except Exception as ex:
+            asyncio.run(self.Debug(f"Received heatbeat => error: {ex}"))
 
     def handle_error(self, message):
         asyncio.run(self.ThrowError(f"HUB ERROR: {message[0]}"))
-        if len(message) > 1 and message[1] == 9: #Secret is not valid
+        logging.error(f"[msb] \033[91mERROR:\033[0m {message[0]}")
+        self.printf(f"HUB ERROR: {message[0]}")
+        
+        time.sleep(1)
+
+        if len(message) > 1 and message[1] == 9: #Secret is not valid        
             settings = {
                 "hubUri": self.base_uri
             }
             self.save_settings(settings)
             os.execv(sys.executable, ['python'] + sys.argv)
+        elif len(message) > 1 and message[1] == 101: # Connection is lost, reconnect
+            asyncio.run(asyncio.sleep(10))
+            self.restart()
+
 
     def report_state(self, id):
         node_name = self.settings["nodeName"]
         self.printf(f'Fetching environment state from {node_name}')
         self.connection.send(
             'notify', [id, f'Fetching environment state from {node_name}', 'INFO'])
 
@@ -666,14 +692,15 @@
             self.set_interval(func, sec)
             func()
         t = threading.Timer(sec, func_wrapper)
         t.start()
         return t
 
     def refresh_vpn_settings_sync(self, args):
+        asyncio.run(self.Debug(f"Fetching VPN settings"))
         self.connection.send("getVpnSettings", [""])
     
     def get_vpn_settings_response(self, vpnConfig, interfaceName, endpoint):
         message = {'vpnConfig': vpnConfig,
                    'interfaceName': interfaceName,
                    'endpoint': endpoint,
                    'vpnConfigPath': f"{self.msb_dir}/{interfaceName}.conf"}
@@ -689,14 +716,29 @@
     
     def stop_terminal(self):
        asyncio.run(self.SubmitAction("terminal", "_disconnect", {}))
     
     def terminal_command(self, args):
         asyncio.run(self.SubmitAction("terminal", "_forward_command", args[0]))
 
+    def download_file(self, request):
+        try:
+            file_name = request["fileName"]
+            directory = request["directory"]
+            uri = request["uri"]
+            connId = request["connId"]
+            node_name = self.settings["nodeName"]
+            asyncio.run(self.Debug(f"downloading file ({file_name}) to {directory}"))
+            urllib.request.urlretrieve(uri, f"/{directory}/{file_name}")
+            asyncio.run(self.Debug(f"download complete"))
+            message = f"{file_name} has successfully been saved in ${directory} on ${node_name}."
+            self.connection.send("notify", [connId, message, "INFO"])
+
+        except Exception as ex:
+            asyncio.run(self.ThrowError(f"Error in msb.start: {e}"))
     # endregion
     # region Service callbacks
     async def request_connectionstring(self, message):
         action = message.message[0]["action"]     
         await self.SubmitAction(message.source, action, self.settings["receiveConnectionString"])
     async def terminal_output(self, message):
         connectionId = message.message[0]["connectionId"]
```

### Comparing `microservicebus-py-0.9.7/src/orchestrator_service.py` & `microservicebus-py-0.9.8/src/orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/rauc_handler.py` & `microservicebus-py-0.9.8/src/rauc_handler.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/start.py` & `microservicebus-py-0.9.8/src/start.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/terminal_service.py` & `microservicebus-py-0.9.8/src/terminal_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/test.py` & `microservicebus-py-0.9.8/src/test.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/utils.py` & `microservicebus-py-0.9.8/src/utils.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.7/src/vpn_helper.py` & `microservicebus-py-0.9.8/src/vpn_helper.py`

 * *Files identical despite different names*

