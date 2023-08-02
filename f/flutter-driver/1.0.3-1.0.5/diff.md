# Comparing `tmp/flutter-driver-1.0.3.tar.gz` & `tmp/flutter-driver-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flutter-driver-1.0.3.tar", last modified: Wed Jun  7 08:30:58 2023, max compression
+gzip compressed data, was "flutter-driver-1.0.5.tar", last modified: Wed Aug  2 09:00:11 2023, max compression
```

## Comparing `flutter-driver-1.0.3.tar` & `flutter-driver-1.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 08:30:58.514473 flutter-driver-1.0.3/
--rw-rw-rw-   0        0        0     1087 2023-05-04 06:13:55.000000 flutter-driver-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0     5709 2023-06-07 08:30:58.512984 flutter-driver-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4642 2023-06-07 07:44:09.000000 flutter-driver-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 08:30:58.460408 flutter-driver-1.0.3/flutter_driver/
--rw-rw-rw-   0        0        0       79 2023-05-22 00:27:16.000000 flutter-driver-1.0.3/flutter_driver/__init__.py
--rw-rw-rw-   0        0        0     5064 2023-06-07 06:48:20.000000 flutter-driver-1.0.3/flutter_driver/command.py
--rw-rw-rw-   0        0        0     8385 2023-06-07 07:15:31.000000 flutter-driver-1.0.3/flutter_driver/driver.py
--rw-rw-rw-   0        0        0     5935 2023-05-22 00:43:02.000000 flutter-driver-1.0.3/flutter_driver/jsonrpc.py
--rw-rw-rw-   0        0        0     3003 2023-06-07 07:27:49.000000 flutter-driver-1.0.3/flutter_driver/runner.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:30:58.509512 flutter-driver-1.0.3/flutter_driver.egg-info/
--rw-rw-rw-   0        0        0     5709 2023-06-07 08:30:58.000000 flutter-driver-1.0.3/flutter_driver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      348 2023-06-07 08:30:58.000000 flutter-driver-1.0.3/flutter_driver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 08:30:58.000000 flutter-driver-1.0.3/flutter_driver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-06-07 08:30:58.000000 flutter-driver-1.0.3/flutter_driver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-06-07 08:30:58.000000 flutter-driver-1.0.3/flutter_driver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 08:30:58.514969 flutter-driver-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1478 2023-06-07 08:30:52.000000 flutter-driver-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:00:11.545075 flutter-driver-1.0.5/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 06:13:55.000000 flutter-driver-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     5709 2023-08-02 09:00:11.544083 flutter-driver-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4642 2023-06-07 07:44:09.000000 flutter-driver-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 09:00:11.510354 flutter-driver-1.0.5/flutter_driver/
+-rw-rw-rw-   0        0        0      107 2023-07-25 09:51:28.000000 flutter-driver-1.0.5/flutter_driver/__init__.py
+-rw-rw-rw-   0        0        0     5935 2023-07-24 06:27:37.000000 flutter-driver-1.0.5/flutter_driver/command.py
+-rw-rw-rw-   0        0        0     9570 2023-07-27 06:26:30.000000 flutter-driver-1.0.5/flutter_driver/driver.py
+-rw-rw-rw-   0        0        0     5988 2023-06-08 02:39:46.000000 flutter-driver-1.0.5/flutter_driver/jsonrpc.py
+-rw-rw-rw-   0        0        0     4423 2023-07-27 10:07:20.000000 flutter-driver-1.0.5/flutter_driver/runner.py
+drwxrwxrwx   0        0        0        0 2023-08-02 09:00:11.541108 flutter-driver-1.0.5/flutter_driver.egg-info/
+-rw-rw-rw-   0        0        0     5709 2023-08-02 09:00:09.000000 flutter-driver-1.0.5/flutter_driver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      348 2023-08-02 09:00:09.000000 flutter-driver-1.0.5/flutter_driver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 09:00:09.000000 flutter-driver-1.0.5/flutter_driver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-08-02 09:00:09.000000 flutter-driver-1.0.5/flutter_driver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-02 09:00:09.000000 flutter-driver-1.0.5/flutter_driver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 09:00:11.545579 flutter-driver-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1470 2023-08-02 08:59:40.000000 flutter-driver-1.0.5/setup.py
```

### Comparing `flutter-driver-1.0.3/LICENSE.txt` & `flutter-driver-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flutter-driver-1.0.3/PKG-INFO` & `flutter-driver-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flutter-driver
-Version: 1.0.3
+Version: 1.0.5
 Summary: An flutter automation driver for python
 Home-page: https://github.com/183181731/flutter-driver
 Author: ndaeqa-wang
 Author-email: 183181731@qq.com
 License: MIT
 Keywords: flutter windows,python client,ui automation
 Platform: UNKNOWN
```

### Comparing `flutter-driver-1.0.3/README.md` & `flutter-driver-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flutter-driver-1.0.3/flutter_driver/command.py` & `flutter-driver-1.0.5/flutter_driver/command.py`

 * *Files 11% similar despite different names*

```diff
@@ -165,8 +165,35 @@
         params.update(self.finder)
         return {
             'method': 'ext.flutter.driver',
             'params': params,
         }
     
     def parse_response(self, response):
+        return response['response']
+
+class DragCommand(Command):
+    def __init__(self, driver, start_x, start_y, offset_x, offset_y, duration, isolate_id):
+        super().__init__(driver, isolate_id)
+        self.start_x = start_x
+        self.start_y = start_y
+        self.offset_x = offset_x
+        self.offset_y = offset_y
+        self.duration = duration
+
+    def build_command(self):
+        params = {
+            'command': 'drag',            
+            'start_x': self.start_x,
+            'start_y': self.start_y,
+            'offset_x': self.offset_x,
+            'offset_y': self.offset_y,
+            'duration': self.duration,
+            'isolateId': self.isolate_id,
+        }
+        return {
+            'method': 'ext.flutter.driver',
+            'params': params,
+        }
+    
+    def parse_response(self, response):
         return response['response']
```

### Comparing `flutter-driver-1.0.3/flutter_driver/driver.py` & `flutter-driver-1.0.5/flutter_driver/driver.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         return cls._instance        
 
     async def connect(self):
         """
         connect to flutter driver
         """
         if self.client is None:
-            self.client = Server(self.observatory_url, timeout=5)
+            self.client = Server(self.observatory_url, timeout=10)
             await self.client.ws_connect()
             self.command_executor = CommandExecutor()
             await self.get_isolate_id()
 
     async def close(self):
         """close driver ws connect
         """
@@ -58,37 +58,37 @@
             _type_: _description_
         """
         command = FindElementCommand(self, finder, self.isolate_id)
         self.command_executor.add_command(command)
         await self.command_executor.execute_commands()
         return FlutterElement(self, finder)
 
-    async def find_element_by_semantics_label(self, label, isRegExp=False):
-        return await self.find_element(FlutterFinder().by_semantics_label(label, isRegExp))
+    async def find_element_by_semantics_label(self, label, isRegExp=False, index=None):
+        return await self.find_element(FlutterFinder().by_semantics_label(label, isRegExp, index))
 
-    async def find_element_by_text(self, text):
-        return await self.find_element(FlutterFinder().by_text(text))
+    async def find_element_by_text(self, text, index=None):
+        return await self.find_element(FlutterFinder().by_text(text, index))
 
-    async def find_element_by_tooltip(self, tooltip):
-        return await self.find_element(FlutterFinder().by_tooltip_message(tooltip))
+    async def find_element_by_tooltip(self, tooltip, index=None):
+        return await self.find_element(FlutterFinder().by_tooltip_message(tooltip, index))
 
-    async def find_element_by_type(self, widget_type):
-        return await self.find_element(FlutterFinder().by_type(widget_type))
+    async def find_element_by_type(self, widget_type, index=None):
+        return await self.find_element(FlutterFinder().by_type(widget_type, index))
 
-    async def find_element_by_value_key(self, value, type='String'):   # other type is int
-        return await self.find_element(FlutterFinder().by_value_key(value, type))
+    async def find_element_by_value_key(self, value, type='String', index=None):   # other type is int
+        return await self.find_element(FlutterFinder().by_value_key(value, type, index))
 
     async def find_page_back(self):
         return await self.find_element(FlutterFinder().page_back())
     
-    async def find_ancestor(self, of, matching, matchRoot=False, firstMatchOnly=False):
-        return await self.find_element(FlutterFinder().by_ancestor(of, matching, matchRoot, firstMatchOnly))
+    async def find_ancestor(self, of, matching, matchRoot=False, firstMatchOnly=False, index=None):
+        return await self.find_element(FlutterFinder().by_ancestor(of, matching, matchRoot, firstMatchOnly, index))
 
-    async def find_descendant(self, of, matching, matchRoot=False, firstMatchOnly=False):
-        return await self.find_element(FlutterFinder().by_descendant(of, matching, matchRoot, firstMatchOnly))
+    async def find_descendant(self, of, matching, matchRoot=False, firstMatchOnly=False, index=None):
+        return await self.find_element(FlutterFinder().by_descendant(of, matching, matchRoot, firstMatchOnly, index))
 
     async def tap_element(self, finder):
         command = TapElementCommand(self, finder, self.isolate_id)
         self.command_executor.add_command(command)
         await self.command_executor.execute_commands()
 
     async def get_text(self, finder):
@@ -127,33 +127,36 @@
             path (string): save image to .png path
         """
         command = GetScreenShotCommand(self)
         result = await command.execute()
         with open(path, "wb") as f:
             f.write(base64.b64decode(result))
 
+    async def drag(self, start_x, start_y, offset_x, offset_y, duration):
+        command = DragCommand(self, start_x, start_y, offset_x, offset_y, duration, self.isolate_id)
+        self.command_executor.add_command(command)
+        await self.command_executor.execute_commands()
+
 class FlutterElement:
     def __init__(self, driver, finder):
         """_summary_
 
         Args:
             driver (FlutterDriver): driver for Flutter Application
             finder (FlutterFinder): finder for Element
         """
         self.driver = driver
         self.finder = finder
 
     async def click(self):
-        """click element
-        """
+        """click element"""
         await self.driver.tap_element(self.finder)
 
     async def clear(self):
-        """clean text in element
-        """
+        """clean text in element"""
         await self.driver.enter_text('')
 
     async def get_text(self):
         """get element text
 
         Returns:
             string: Text on FlutterElement
@@ -181,63 +184,85 @@
             "height": bottom_right["dy"] - top_left["dy"]
         }
 
 class FlutterFinder:
     def __init__(self):
         pass
 
-    def by_semantics_label(self, label, isRegExp):
-        return {
+    def by_semantics_label(self, label, isRegExp, index=None):
+        finder = {
             "finderType":"BySemanticsLabel",
             "label": label,
-            'isRegExp': isRegExp
+            'isRegExp': isRegExp,
         }
+        if (index!=None):
+            finder.update({ "index": index })
+        return finder
 
-    def by_text(self, text):
-        return {
+    def by_text(self, text, index=None):
+        finder = {
             "finderType":"ByText",
             "text": text
         }
+        if (index!=None):
+            finder.update({ "index": index })
+        return finder
 
-    def by_tooltip_message(self, message):    
-        return {
+    def by_tooltip_message(self, message, index=None):    
+        finder = {
             "finderType":"ByTooltipMessage",
             "text": message
         }
+        if (index!=None):
+            finder.update({ "index": index })
+        return finder
+    
 
-    def by_type(self, type):
-        return {
+    def by_type(self, type, index=None):
+        finder = {
             "finderType":"ByType",
             "type": type
         }
+        if (index!=None):
+            finder.update({ "index": index })
+        return finder
 
-    def by_value_key(self, value, type):
-        return {
+    def by_value_key(self, value, type, index=None):
+        finder = {
             "finderType":"ByValueKey",
             "keyValueString": value,
             "keyValueType": type,
         }
+        if (index!=None):
+            finder.update({ "index": index })
+        return finder
 
-    def by_ancestor(self, of, matching, matchRoot, firstMatchOnly):
-        return {
+    def by_ancestor(self, of, matching, matchRoot, firstMatchOnly, index=None):
+        finder = {
             "finderType":"Ancestor",
             "of": json.dumps(of),
             "matching": json.dumps(matching),
             "matchRoot": matchRoot,
             "firstMatchOnly": firstMatchOnly
         }
+        if (index!=None):
+            finder.update({ "index": index })
+        return finder
 
-    def by_descendant(self, of, matching, matchRoot=False, firstMatchOnly=False):
-        return {
+    def by_descendant(self, of, matching, matchRoot=False, firstMatchOnly=False, index=None):
+        finder = {
             "finderType":"Descendant",
             "of": json.dumps(of),
             "matching": json.dumps(matching),
             "matchRoot": matchRoot,
             "firstMatchOnly": firstMatchOnly
         }
+        if (index!=None):
+            finder.update({ "index": index })
+        return finder
 
     def page_back(self):
         return {
             "finderType":"PageBack"
         }
 
 class CommandExecutor:
```

### Comparing `flutter-driver-1.0.3/flutter_driver/jsonrpc.py` & `flutter-driver-1.0.5/flutter_driver/jsonrpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 from aiohttp import ClientError
 from aiohttp.http_exceptions import HttpProcessingError
 import async_timeout
 import jsonrpc_base
 from jsonrpc_base import TransportError
 
 class Server(jsonrpc_base.Server):
-    """A connection to a HTTP JSON-RPC server, backed by aiohttp"""
+    """A connection to a HTTP JSON-RPC server, backed by aiohttp
 
+    Args:
+        jsonrpc_base (url): ws url
+    """
     def __init__(self, url, session=None, **connect_kwargs):
         super().__init__()
         self._session = session or aiohttp.ClientSession()
         self._loop = asyncio.get_event_loop()
 
         # True if we made our own session
         self._internal_session = session is None
```

### Comparing `flutter-driver-1.0.3/flutter_driver.egg-info/PKG-INFO` & `flutter-driver-1.0.5/flutter_driver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flutter-driver
-Version: 1.0.3
+Version: 1.0.5
 Summary: An flutter automation driver for python
 Home-page: https://github.com/183181731/flutter-driver
 Author: ndaeqa-wang
 Author-email: 183181731@qq.com
 License: MIT
 Keywords: flutter windows,python client,ui automation
 Platform: UNKNOWN
```

### Comparing `flutter-driver-1.0.3/setup.py` & `flutter-driver-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,27 +3,27 @@
 import io
 import os
 
 from setuptools import find_packages, setup
 
 setup(
     name='flutter-driver',
-    version='1.0.3',
+    version='1.0.5',
     description='An flutter automation driver for python',
     long_description=io.open(os.path.join(os.path.dirname('__file__'), 'README.md'), encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     keywords=[
         'flutter windows',
         'python client',
         'ui automation'
     ],
     author='ndaeqa-wang',
     author_email='183181731@qq.com',
     url='https://github.com/183181731/flutter-driver',
-    packages=find_packages(include=['flutter_driver','tests']),
+    packages=find_packages(include=['flutter_driver']),
     license='MIT',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

