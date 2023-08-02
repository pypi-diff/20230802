# Comparing `tmp/DmxOscServer-1.0.1.tar.gz` & `tmp/DmxOscServer-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/pi/Documents/DmxOscServer/dist/.tmp-7t31qi_v/DmxOscServer-1.0.1.tar", last modified: Mon Jul 31 18:19:19 2023, max compression
+gzip compressed data, was "/home/pi/Documents/DmxOscServer/dist/.tmp-k_s_joz3/DmxOscServer-1.0.2.tar", last modified: Wed Aug  2 17:06:11 2023, max compression
```

## Comparing `DmxOscServer-1.0.1.tar` & `DmxOscServer-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/
--rw-r--r--   0 pi        (1000) pi        (1000)     2265 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)     1829 2023-07-31 18:18:06.000000 DmxOscServer-1.0.1/README.md
--rw-r--r--   0 pi        (1000) pi        (1000)       78 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/setup.cfg
--rw-r--r--   0 pi        (1000) pi        (1000)      865 2023-07-31 18:17:17.000000 DmxOscServer-1.0.1/setup.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer/
--rw-r--r--   0 pi        (1000) pi        (1000)     3450 2023-07-31 18:10:14.000000 DmxOscServer-1.0.1/src/DmxOscServer/DmxOscServer.py
--rw-r--r--   0 pi        (1000) pi        (1000)     1609 2023-07-31 17:31:17.000000 DmxOscServer-1.0.1/src/DmxOscServer/Fixture.py
--rw-r--r--   0 pi        (1000) pi        (1000)       68 2023-07-30 18:25:02.000000 DmxOscServer-1.0.1/src/DmxOscServer/__init__.py
-drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/
--rw-r--r--   0 pi        (1000) pi        (1000)     2265 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/PKG-INFO
--rw-r--r--   0 pi        (1000) pi        (1000)      317 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/SOURCES.txt
--rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/dependency_links.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/requires.txt
--rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-07-31 18:19:19.000000 DmxOscServer-1.0.1/src/DmxOscServer.egg-info/top_level.txt
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2266 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)     1830 2023-08-02 17:03:56.000000 DmxOscServer-1.0.2/README.md
+-rw-r--r--   0 pi        (1000) pi        (1000)       78 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/setup.cfg
+-rw-r--r--   0 pi        (1000) pi        (1000)      865 2023-08-02 16:30:11.000000 DmxOscServer-1.0.2/setup.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer/
+-rw-r--r--   0 pi        (1000) pi        (1000)     4162 2023-08-02 16:47:34.000000 DmxOscServer-1.0.2/src/DmxOscServer/DmxOscServer.py
+-rw-r--r--   0 pi        (1000) pi        (1000)     1609 2023-07-31 17:31:17.000000 DmxOscServer-1.0.2/src/DmxOscServer/Fixture.py
+-rw-r--r--   0 pi        (1000) pi        (1000)       68 2023-07-30 18:25:02.000000 DmxOscServer-1.0.2/src/DmxOscServer/__init__.py
+drwxr-xr-x   0 pi        (1000) pi        (1000)        0 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/
+-rw-r--r--   0 pi        (1000) pi        (1000)     2266 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/PKG-INFO
+-rw-r--r--   0 pi        (1000) pi        (1000)      317 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/SOURCES.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)        1 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/dependency_links.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       11 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/requires.txt
+-rw-r--r--   0 pi        (1000) pi        (1000)       13 2023-08-02 17:06:11.000000 DmxOscServer-1.0.2/src/DmxOscServer.egg-info/top_level.txt
```

### Comparing `DmxOscServer-1.0.1/PKG-INFO` & `DmxOscServer-1.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DmxOscServer
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python Lib to create a DMX compatible OSC server with handlers
 Home-page: https://dmxoscserver.readthedocs.io/en/latest/
 Author: Miniontoby
 Project-URL: Bug Reports, https://github.com/Miniontoby/DmxOscServer/issues
 Project-URL: Source, https://github.com/Miniontoby/DmxOscServer
 Keywords: dmx,osc,server
 Requires-Python: >=3.5
@@ -29,16 +29,16 @@
 To create a simple DMX OSC Server that will listen on 0.0.0.0:9000 you can use this code:
 
 ```py
 from DmxOscServer import DmxOscServer
 
 server = DmxOscServer()
 
-# Register a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
-@server.new_fixture(0, 0, 3)
+# Define a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
+@server.define_fixture(0, 0, 3)
 def my_rgb_handler(fixture, address, *args):
     fixture.values[address] = args[0]
     print (fixture.values)
 
 server.run()
 ```
```

### Comparing `DmxOscServer-1.0.1/README.md` & `DmxOscServer-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,16 +17,16 @@
 To create a simple DMX OSC Server that will listen on 0.0.0.0:9000 you can use this code:
 
 ```py
 from DmxOscServer import DmxOscServer
 
 server = DmxOscServer()
 
-# Register a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
-@server.new_fixture(0, 0, 3)
+# Define a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
+@server.define_fixture(0, 0, 3)
 def my_rgb_handler(fixture, address, *args):
     fixture.values[address] = args[0]
     print (fixture.values)
 
 server.run()
 ```
```

### Comparing `DmxOscServer-1.0.1/setup.py` & `DmxOscServer-1.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="DmxOscServer",
-    version="1.0.1",
+    version="1.0.2",
     description="A Python Lib to create a DMX compatible OSC server with handlers",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://dmxoscserver.readthedocs.io/en/latest/",
     author="Miniontoby",
     keywords="dmx, osc, server",
     package_dir={"": "src"},
```

### Comparing `DmxOscServer-1.0.1/src/DmxOscServer/DmxOscServer.py` & `DmxOscServer-1.0.2/src/DmxOscServer/DmxOscServer.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,107 +9,148 @@
 class DmxOscServer():
   """
   Instantiate a DMX OSC Server
   """
   def __init__(self):
     self.fixtures = {
       "all": [],
-      "per-universe": []
+      "per-universe": {}
     }
 
     self.dispatcher = Dispatcher()
     self.dispatcher.map("/*/dmx/*", self.dmx_handler)
 
   def dmx_handler(self, address, *args):
     """
     The OSC Handler for the DMX Messages
 
-    This shouldn't be called by anything other than the Dispatcher
+    This shouldn't be called by anything other than the OSC Dispatcher
     """
     matches = search(r"^\/([0-9]+)\/dmx\/([0-9]+)", address) # /0/dmx/0 -> /<universe>/dmx/<addr>
     universe,address = int(matches[1]),int(matches[2])
     for fixture in self.list_fixtures(universe):
       if address in fixture: return fixture(address, *args)
 
   def add_fixture(self, fixture):
     """
     Adds a new Fixture to the fixture list
 
-    :param fixture: The Fixture to add
-    :type fixture: Fixture
+    :param Fixture fixture: The Fixture to add
+    :raises TypeError: if the fixture is not a Fixture
+
+
+    Example
+    ---------
+
+    .. code-block:: python3
+
+       from DmxOscServer import DmxOscServer, Fixture
+
+       server = DmxOscServer()
+
+       def handler(fixture, address, *args): return
+
+       fix = Fixture(0, 0, 3, handler)
+       server.add_fixture(fix)
     """
-    if not(isinstance(fixture, Fixture)): raise Exception("Not a fixture!")
+    if not(isinstance(fixture, Fixture)): raise TypeError("Not a Fixture!")
     self.fixtures["all"].append(fixture)
-    if not(fixture.universe in self.fixtures["per-universe"]):
-      if fixture.universe > 10: raise Exception("Sorry but WHY do you need 10 universes?")
-      while len(self.fixtures["per-universe"]) <= fixture.universe:
-        self.fixtures["per-universe"].append([])
+    if not(fixture.universe in self.fixtures["per-universe"]): self.fixtures["per-universe"][fixture.universe] = []
     self.fixtures["per-universe"][fixture.universe].append(fixture)
 
   def add_fixtures(self, *fixtures):
     """
     Adds multiple Fixtures to the fixture list
 
-    :param fixtures: The Fixtures to add
-    :type fixtures: Fixture[]
+    :param Fixture \*fixtures: The Fixtures to add
+
+
+    Example
+    ---------
+
+    .. code-block:: python3
+
+       from DmxOscServer import DmxOscServer, Fixture
+
+       server = DmxOscServer()
+
+       def handler(fixture, address, *args): return
+
+       fix1 = Fixture(0, 0, 3, handler)
+       fix2 = Fixture(0, 3, 3, handler)
+
+       server.add_fixtures(fix1, fix2)
     """
     for fixture in fixtures: self.add_fixture(fixture)
 
-  def new_fixture(self, universe, starting_addr, channels):
+  def define_fixture(self, universe, starting_addr, channels):
     """
-    Allows you to create a new fixture using a function decorator
+    Allows you to define a new fixture using a function decorator
 
-    :param universe: The universe for this Fixture
-    :type universe: int
-    :param starting_addr: The starting address for this Fixture
-    :type starting_addr: int
-    :param channels: The amount of channel that this Fixture should have
-    :type channels: int
+    :param int universe: The universe for this Fixture
+    :param int starting_addr: The starting address for this Fixture
+    :param int channels: The amount of channel that this Fixture should have
 
 
     Example
     ---------
 
     .. code-block:: python3
 
-       @server.new_fixture(0, 0, 3)
+       from DmxOscServer import DmxOscServer, Fixture
+
+       server = DmxOscServer()
+
+       @server.define_fixture(0, 0, 3)
        def rgb_handler(fixture, address, *args):
            fixture.values[address] = args[0]
-
     """
     def decorator(func):
       result = Fixture(universe, starting_addr, channels, func)
       self.add_fixture(result)
       return result
 
     return decorator
 
   def list_fixtures(self, universe=False):
     """
     If `universe` is set to False, it will return all the Fixtures
     If `universe` is set to a universe number, it will return all the Fixtures of that universe
 
     :param universe: Specifies the universe. Set to False for all Fixtures
-    :type universe: int|False
+    :type universe: int or False
 
     :returns: List of Fixtures
     :rtype: Fixture[]
+
+
+    Example
+    ---------
+
+    .. code-block:: python3
+
+       from DmxOscServer import DmxOscServer
+
+       server = DmxOscServer()
+
+       # Add fixtures here
+
+       all_fixtures = server.list_fixtures()
+       universe_zero_fixtures = server.list_fixtures(0)
     """
     if universe is False: return self.fixtures["all"]
-    elif len(self.fixtures["per-universe"]) > universe: return self.fixtures["per-universe"][universe]
+    elif universe in self.fixtures["per-universe"]: return self.fixtures["per-universe"][universe]
     else: return []
 
   def run(self, ip="0.0.0.0", port=9000):
     """
     Start the server run
 
     Should be called always AFTER all fixtures are added
 
-    :param ip: The IP address to listen on
-    :type ip: str
-    :param port: The Port to listen on
-    :type port: int
+    :param str ip: The IP address to listen on
+    :param int port: The Port to listen on
     """
     self.osc_server = osc_server.ThreadingOSCUDPServer((ip, port), self.dispatcher)
     print ("Serving on {}".format(self.osc_server.server_address))
     self.osc_server.serve_forever()
```

### Comparing `DmxOscServer-1.0.1/src/DmxOscServer/Fixture.py` & `DmxOscServer-1.0.2/src/DmxOscServer/Fixture.py`

 * *Files identical despite different names*

### Comparing `DmxOscServer-1.0.1/src/DmxOscServer.egg-info/PKG-INFO` & `DmxOscServer-1.0.2/src/DmxOscServer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DmxOscServer
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python Lib to create a DMX compatible OSC server with handlers
 Home-page: https://dmxoscserver.readthedocs.io/en/latest/
 Author: Miniontoby
 Project-URL: Bug Reports, https://github.com/Miniontoby/DmxOscServer/issues
 Project-URL: Source, https://github.com/Miniontoby/DmxOscServer
 Keywords: dmx,osc,server
 Requires-Python: >=3.5
@@ -29,16 +29,16 @@
 To create a simple DMX OSC Server that will listen on 0.0.0.0:9000 you can use this code:
 
 ```py
 from DmxOscServer import DmxOscServer
 
 server = DmxOscServer()
 
-# Register a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
-@server.new_fixture(0, 0, 3)
+# Define a 3 channel Fixture at address 0 at universe 0 which will execute my_rgb_handler when called
+@server.define_fixture(0, 0, 3)
 def my_rgb_handler(fixture, address, *args):
     fixture.values[address] = args[0]
     print (fixture.values)
 
 server.run()
 ```
```

