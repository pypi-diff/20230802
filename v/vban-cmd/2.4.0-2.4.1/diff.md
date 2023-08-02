# Comparing `tmp/vban_cmd-2.4.0.tar.gz` & `tmp/vban_cmd-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.4.0.tar", max compression
+gzip compressed data, was "vban_cmd-2.4.1.tar", max compression
```

## Comparing `vban_cmd-2.4.0.tar` & `vban_cmd-2.4.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.4.0/LICENSE
--rw-r--r--   0        0        0      951 2023-08-02 14:44:12.954817 vban_cmd-2.4.0/pyproject.toml
--rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.4.0/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.4.0/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.4.0/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.4.0/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.4.0/vban_cmd/config.py
--rw-r--r--   0        0        0      220 2023-08-02 14:36:24.956502 vban_cmd-2.4.0/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.4.0/vban_cmd/event.py
--rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.4.0/vban_cmd/factory.py
--rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.4.0/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.4.0/vban_cmd/kinds.py
--rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.4.0/vban_cmd/macrobutton.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.4.0/vban_cmd/meta.py
--rw-r--r--   0        0        0     9625 2023-07-25 14:57:29.669770 vban_cmd-2.4.0/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.4.0/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.4.0/vban_cmd/subject.py
--rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.4.0/vban_cmd/util.py
--rw-r--r--   0        0        0     5735 2023-07-26 10:30:31.333522 vban_cmd-2.4.0/vban_cmd/vban.py
--rw-r--r--   0        0        0     7391 2023-07-12 03:47:07.637840 vban_cmd-2.4.0/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6879 2023-07-25 14:56:03.314782 vban_cmd-2.4.0/vban_cmd/worker.py
--rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.4.1/LICENSE
+-rw-r--r--   0        0        0      951 2023-08-02 16:17:42.142733 vban_cmd-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.4.1/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.4.1/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.4.1/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.4.1/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.4.1/vban_cmd/config.py
+-rw-r--r--   0        0        0      220 2023-08-02 14:36:24.956502 vban_cmd-2.4.1/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.4.1/vban_cmd/event.py
+-rw-r--r--   0        0        0     6888 2023-08-02 16:14:19.633476 vban_cmd-2.4.1/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.4.1/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.4.1/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.4.1/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.4.1/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9625 2023-07-25 14:57:29.669770 vban_cmd-2.4.1/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.4.1/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.4.1/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.4.1/vban_cmd/util.py
+-rw-r--r--   0        0        0     5735 2023-07-26 10:30:31.333522 vban_cmd-2.4.1/vban_cmd/vban.py
+-rw-r--r--   0        0        0     7423 2023-08-02 16:15:23.555395 vban_cmd-2.4.1/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6879 2023-07-25 14:56:03.314782 vban_cmd-2.4.1/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.4.1/PKG-INFO
```

### Comparing `vban_cmd-2.4.0/LICENSE` & `vban_cmd-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/pyproject.toml` & `vban_cmd-2.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.4.0"
+version = "2.4.1"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.4.0/README.md` & `vban_cmd-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/bus.py` & `vban_cmd-2.4.1/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/command.py` & `vban_cmd-2.4.1/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/config.py` & `vban_cmd-2.4.1/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/event.py` & `vban_cmd-2.4.1/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/factory.py` & `vban_cmd-2.4.1/vban_cmd/factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import logging
 from abc import abstractmethod
 from enum import IntEnum
 from functools import cached_property
-from typing import Iterable, NoReturn
+from typing import Iterable
 
 from .bus import request_bus_obj as bus
 from .command import Command
 from .config import request_config as configs
 from .error import VBANCMDError
 from .kinds import KindMapClass
 from .kinds import request_kind_map as kindmap
@@ -37,15 +37,15 @@
             f"Finished building buses for {self._factory}",
             f"Finished building commands for {self._factory}",
             f"Finished building macrobuttons for {self._factory}",
             f"Finished building vban in/out streams for {self._factory}",
         )
         self.logger = logger.getChild(self.__class__.__name__)
 
-    def _pinfo(self, name: str) -> NoReturn:
+    def _pinfo(self, name: str) -> None:
         """prints progress status for each step"""
         name = name.split("_")[1]
         self.logger.info(self._info[int(getattr(self.BuilderProgress, name))])
 
     def make_strip(self):
         self._factory.strip = tuple(
             strip(i < self.kind.phys_in, self._factory, i)
```

### Comparing `vban_cmd-2.4.0/vban_cmd/iremote.py` & `vban_cmd-2.4.1/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/kinds.py` & `vban_cmd-2.4.1/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/macrobutton.py` & `vban_cmd-2.4.1/vban_cmd/macrobutton.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/meta.py` & `vban_cmd-2.4.1/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/packet.py` & `vban_cmd-2.4.1/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/strip.py` & `vban_cmd-2.4.1/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/subject.py` & `vban_cmd-2.4.1/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/util.py` & `vban_cmd-2.4.1/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/vban.py` & `vban_cmd-2.4.1/vban_cmd/vban.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/vban_cmd/vbancmd.py` & `vban_cmd-2.4.1/vban_cmd/vbancmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             return conn["connection"]
         raise VBANCMDError("no ip provided and no vban.toml located.")
 
     def __enter__(self):
         self.login()
         return self
 
-    def login(self):
+    def login(self) -> None:
         """Starts the subscriber and updater threads (unless in outbound mode)"""
         if not self.outbound:
             self.running = True
             self.event.info()
 
             self.subscriber = Subscriber(self)
             self.subscriber.start()
@@ -150,15 +150,15 @@
         """True iff a level value has changed."""
         return self._ldirty
 
     @property
     def public_packet(self):
         return self._public_packet
 
-    def clear_dirty(self):
+    def clear_dirty(self) -> None:
         while self.pdirty:
             time.sleep(self.DELAY)
 
     def _get_levels(self, packet) -> Iterable:
         """
         returns both level arrays (strip_levels, bus_levels) BEFORE math conversion
 
@@ -208,15 +208,15 @@
             }
             self.logger.debug(
                 f"profile '{name}' extends '{extended}', profiles merged.."
             )
         self.apply(config)
         self.logger.info(f"Profile '{name}' applied!")
 
-    def logout(self):
+    def logout(self) -> None:
         self.running = False
         time.sleep(0.2)
         [sock.close() for sock in self.socks]
         self.logger.info(f"{type(self).__name__}: Successfully logged out of {self}")
 
-    def __exit__(self, exc_type, exc_value, exc_traceback):
+    def __exit__(self, exc_type, exc_value, exc_traceback) -> None:
         self.logout()
```

### Comparing `vban_cmd-2.4.0/vban_cmd/worker.py` & `vban_cmd-2.4.1/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.4.0/PKG-INFO` & `vban_cmd-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

