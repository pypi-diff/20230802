# Comparing `tmp/microservicebus-py-0.9.8.tar.gz` & `tmp/microservicebus-py-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microservicebus-py-0.9.8.tar", last modified: Wed Aug  2 09:45:40 2023, max compression
+gzip compressed data, was "microservicebus-py-0.9.9.tar", last modified: Wed Aug  2 18:20:10 2023, max compression
```

## Comparing `microservicebus-py-0.9.8.tar` & `microservicebus-py-0.9.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 09:45:40.200931 microservicebus-py-0.9.8/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-08-02 09:45:40.196930 microservicebus-py-0.9.8/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.8/README.md
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 09:45:39.712525 microservicebus-py-0.9.8/microservicebus_py.egg-info/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/PKG-INFO
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/SOURCES.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/dependency_links.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/entry_points.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-08-02 09:45:39.000000 microservicebus-py-0.9.8/microservicebus_py.egg-info/top_level.txt
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-08-02 09:45:40.202929 microservicebus-py-0.9.8/setup.cfg
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.8/setup.py
-drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 09:45:40.163307 microservicebus-py-0.9.8/src/
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.8/src/axians.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     5689 2023-05-31 17:27:32.000000 microservicebus-py-0.9.8/src/base_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1609 2023-06-08 22:01:37.000000 microservicebus-py-0.9.8/src/logger_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)    33829 2023-08-02 09:29:44.000000 microservicebus-py-0.9.8/src/msb_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6541 2023-07-07 07:09:27.000000 microservicebus-py-0.9.8/src/orchestrator_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.8/src/queue_message.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.8/src/rauc_handler.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.8/src/start.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.8/src/terminal_service.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.8/src/test.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.8/src/utils.py
--rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.8/src/vpn_helper.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 18:20:10.457509 microservicebus-py-0.9.9/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-08-02 18:20:10.444195 microservicebus-py-0.9.9/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3680 2022-12-12 08:25:32.000000 microservicebus-py-0.9.9/README.md
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 18:20:09.408379 microservicebus-py-0.9.9/microservicebus_py.egg-info/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4745 2023-08-02 18:20:08.000000 microservicebus-py-0.9.9/microservicebus_py.egg-info/PKG-INFO
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      455 2023-08-02 18:20:08.000000 microservicebus-py-0.9.9/microservicebus_py.egg-info/SOURCES.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        1 2023-08-02 18:20:08.000000 microservicebus-py-0.9.9/microservicebus_py.egg-info/dependency_links.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       55 2023-08-02 18:20:08.000000 microservicebus-py-0.9.9/microservicebus_py.egg-info/entry_points.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)        4 2023-08-02 18:20:08.000000 microservicebus-py-0.9.9/microservicebus_py.egg-info/top_level.txt
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)       38 2023-08-02 18:20:10.461518 microservicebus-py-0.9.9/setup.cfg
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     1707 2023-06-02 09:59:05.000000 microservicebus-py-0.9.9/setup.py
+drwxrwxrwx   0 mikael    (1000) mikael    (1000)        0 2023-08-02 18:20:10.351764 microservicebus-py-0.9.9/src/
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      807 2022-12-19 11:22:24.000000 microservicebus-py-0.9.9/src/axians.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6287 2023-08-02 17:42:27.000000 microservicebus-py-0.9.9/src/base_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4854 2023-08-02 17:47:38.000000 microservicebus-py-0.9.9/src/logger_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)    34195 2023-08-02 11:09:22.000000 microservicebus-py-0.9.9/src/msb_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     6541 2023-07-07 07:09:27.000000 microservicebus-py-0.9.9/src/orchestrator_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      340 2022-03-14 19:13:32.000000 microservicebus-py-0.9.9/src/queue_message.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     4414 2022-12-02 13:59:45.000000 microservicebus-py-0.9.9/src/rauc_handler.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      846 2023-06-02 09:05:37.000000 microservicebus-py-0.9.9/src/start.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3311 2023-01-09 21:54:56.000000 microservicebus-py-0.9.9/src/terminal_service.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)      672 2022-03-23 09:36:17.000000 microservicebus-py-0.9.9/src/test.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3971 2023-06-02 09:05:37.000000 microservicebus-py-0.9.9/src/utils.py
+-rwxrwxrwx   0 mikael    (1000) mikael    (1000)     3136 2022-12-12 08:35:01.000000 microservicebus-py-0.9.9/src/vpn_helper.py
```

### Comparing `microservicebus-py-0.9.8/PKG-INFO` & `microservicebus-py-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.8/README.md` & `microservicebus-py-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/microservicebus_py.egg-info/PKG-INFO` & `microservicebus-py-0.9.9/microservicebus_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microservicebus-py
-Version: 0.9.8
+Version: 0.9.9
 Summary: Python agent for microServiceBus.com. Please visit https://microservicebus.com for more information.
 Home-page: https://github.com/axians/microservicebus-py
 Author: AXIANS IoT Operations
 Author-email: microservicebus@axians.com
 License: MIT
 Description: # microservicebus-py
```

### Comparing `microservicebus-py-0.9.8/setup.py` & `microservicebus-py-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/src/axians.py` & `microservicebus-py-0.9.9/src/axians.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/src/base_service.py` & `microservicebus-py-0.9.9/src/base_service.py`

 * *Files 8% similar despite different names*

```diff
@@ -68,19 +68,32 @@
         await asyncio.sleep(0)
 
     async def Debug(self, message):
         msg = QueueMessage(self.id, "logger", "_debug", message)
         task = asyncio.create_task(self.queue.put(msg))
         await asyncio.sleep(0)
 
-    async def ThrowError(self, message):
+    async def ThrowError(self, message, fault_code = None, fault_description = None):
+        if isinstance(message,dict):
+            if(fault_code != None):
+                message["fault_code"] = fault_code
+            if(fault_description != None):
+                message["fault_description"] = fault_description
+                
         msg = QueueMessage(self.id, "logger", "_error", message)
         task = asyncio.create_task(self.queue.put(msg))
         await asyncio.sleep(0)
 
+    async def Track(self, message, description = None):
+        if(description != None):
+            message["description"] = description
+        msg = QueueMessage(self.id, "logger", "_track", message)
+        task = asyncio.create_task(self.queue.put(msg))
+        await asyncio.sleep(0)
+
     async def SubmitMessage(self, message):
         msg = QueueMessage(self.id, "com", "_sendEvent", message)
         asyncio.create_task(self.queue.put(msg))
         await asyncio.sleep(0)
 
     async def StartService(self, service):
         msg = QueueMessage(self.id, "orchestrator", "_start_service", service)
```

### Comparing `microservicebus-py-0.9.8/src/msb_handler.py` & `microservicebus-py-0.9.9/src/msb_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,19 +160,19 @@
             "OrganizationID": settings["organizationId"],
             "npmVersion": packageInfo["version"] ,
             "sas": settings["sas"],
             "ipAddresses": ipAddresses,
             "recoveredSignIn": "False",
             "macAddresses": [':'.join(re.findall('..', '%012x' % uuid.getnode()))]
         }
-
+        await self.Debug("Signing in")
         # Use for debugging
         #self.connection.send("signIn", [hostData])
         self.connection.send("signInAsync", [hostData])
-        await self.Debug("Signing in")
+        #await self.Debug("Signing in")
 
     def sign_in_sync(self, settings, first_sign_in):
         asyncio.run(self.sign_in(settings, first_sign_in))
 
     async def create_node(self):
         mac = ':'.join(re.findall('..', '%012x' % uuid.getnode()))
         await self.Debug(mac)
@@ -350,18 +350,21 @@
         self.connection.on(
             "dockerComposeDown", lambda response: self.not_implemented("dockerComposeDown"))
         # self.connection.on(
         #     "downloadFile", lambda response: self.not_implemented("downloadFile"))
         self.connection.on(
             "uploadFile", lambda response: self.not_implemented("uploadFile"))
         # endregion
+        try:
+            self.connection.start()
+        except Exception as ex:
+            await self.ThrowError(f"Unable to start SignalR!")
+            self._missedheartbeat = 100
 
-        self.connection.start()
         time.sleep(2)
-        print(self.settings)
 
         if "policies" not in self.settings:
             self.settings["policies"] = { "disconnectPolicy": { "heartbeatTimeout": 180, "missedHearbeatLimit": 3}}
 
         heartbeatTimeout = self.settings["policies"]["disconnectPolicy"]["heartbeatTimeout"]
         self.set_interval(self.send_heartbeat, heartbeatTimeout)
         await self.Debug(f"Start hearbeat at {heartbeatTimeout} seconds interval")
@@ -492,15 +495,20 @@
                 self.restart()
         
         #asyncio.run(self.Debug(f"Send heatbeat"))        
         self._missedheartbeat += 1
         self.connection.send("heartBeat", ["echo"])
     
     def receive_heartbeat(self, message):
-        self._missedheartbeat = 0
+        if self.signed_in == False:
+            asyncio.run(self.Debug(f"Received heatbeat but node has not successfully logged in yet"))
+            self._missedheartbeat += 1
+        else:
+            self._missedheartbeat = 0
+
         try:
             connection_id = parse.parse_qs(parse.urlparse(self.connection.transport.url).query)['id'][0]
             asyncio.run(self.Debug(f"Received heatbeat => connection_id: {connection_id}"))
         except Exception as ex:
             asyncio.run(self.Debug(f"Received heatbeat => error: {ex}"))
 
     def handle_error(self, message):
```

### Comparing `microservicebus-py-0.9.8/src/orchestrator_service.py` & `microservicebus-py-0.9.9/src/orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/src/rauc_handler.py` & `microservicebus-py-0.9.9/src/rauc_handler.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/src/start.py` & `microservicebus-py-0.9.9/src/start.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/src/terminal_service.py` & `microservicebus-py-0.9.9/src/terminal_service.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/src/test.py` & `microservicebus-py-0.9.9/src/test.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/src/utils.py` & `microservicebus-py-0.9.9/src/utils.py`

 * *Files identical despite different names*

### Comparing `microservicebus-py-0.9.8/src/vpn_helper.py` & `microservicebus-py-0.9.9/src/vpn_helper.py`

 * *Files identical despite different names*

