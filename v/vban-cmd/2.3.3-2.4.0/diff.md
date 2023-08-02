# Comparing `tmp/vban_cmd-2.3.3.tar.gz` & `tmp/vban_cmd-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vban_cmd-2.3.3.tar", max compression
+gzip compressed data, was "vban_cmd-2.4.0.tar", max compression
```

## Comparing `vban_cmd-2.3.3.tar` & `vban_cmd-2.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.3.3/LICENSE
--rw-r--r--   0        0        0      951 2023-07-25 15:22:56.363154 vban_cmd-2.3.3/pyproject.toml
--rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.3.3/README.md
--rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.3.3/vban_cmd/__init__.py
--rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.3.3/vban_cmd/bus.py
--rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.3.3/vban_cmd/command.py
--rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.3.3/vban_cmd/config.py
--rw-r--r--   0        0        0      197 2023-06-25 10:36:23.500662 vban_cmd-2.3.3/vban_cmd/error.py
--rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.3.3/vban_cmd/event.py
--rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.3.3/vban_cmd/factory.py
--rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.3.3/vban_cmd/iremote.py
--rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.3.3/vban_cmd/kinds.py
--rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.3.3/vban_cmd/macrobutton.py
--rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.3.3/vban_cmd/meta.py
--rw-r--r--   0        0        0     9625 2023-07-25 14:57:29.669770 vban_cmd-2.3.3/vban_cmd/packet.py
--rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.3.3/vban_cmd/strip.py
--rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.3.3/vban_cmd/subject.py
--rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.3.3/vban_cmd/util.py
--rw-r--r--   0        0        0     5996 2023-07-12 09:23:28.333915 vban_cmd-2.3.3/vban_cmd/vban.py
--rw-r--r--   0        0        0     7391 2023-07-12 03:47:07.637840 vban_cmd-2.3.3/vban_cmd/vbancmd.py
--rw-r--r--   0        0        0     6879 2023-07-25 14:56:03.314782 vban_cmd-2.3.3/vban_cmd/worker.py
--rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-03-24 12:30:28.474287 vban_cmd-2.4.0/LICENSE
+-rw-r--r--   0        0        0      951 2023-08-02 14:44:12.954817 vban_cmd-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    12875 2023-07-15 07:15:00.451610 vban_cmd-2.4.0/README.md
+-rw-r--r--   0        0        0       70 2022-07-12 16:30:51.963399 vban_cmd-2.4.0/vban_cmd/__init__.py
+-rw-r--r--   0        0        0     5276 2023-06-25 10:36:16.654167 vban_cmd-2.4.0/vban_cmd/bus.py
+-rw-r--r--   0        0        0     1127 2023-06-25 10:36:19.263212 vban_cmd-2.4.0/vban_cmd/command.py
+-rw-r--r--   0        0        0     5855 2023-07-11 17:23:11.340063 vban_cmd-2.4.0/vban_cmd/config.py
+-rw-r--r--   0        0        0      220 2023-08-02 14:36:24.956502 vban_cmd-2.4.0/vban_cmd/error.py
+-rw-r--r--   0        0        0     1621 2023-06-22 09:26:30.424951 vban_cmd-2.4.0/vban_cmd/event.py
+-rw-r--r--   0        0        0     6902 2023-07-08 06:42:16.984039 vban_cmd-2.4.0/vban_cmd/factory.py
+-rw-r--r--   0        0        0     4130 2023-07-25 14:58:38.295129 vban_cmd-2.4.0/vban_cmd/iremote.py
+-rw-r--r--   0        0        0     2418 2023-07-25 14:54:48.277200 vban_cmd-2.4.0/vban_cmd/kinds.py
+-rw-r--r--   0        0        0     1158 2023-07-25 15:00:05.263943 vban_cmd-2.4.0/vban_cmd/macrobutton.py
+-rw-r--r--   0        0        0     2992 2023-06-25 10:36:33.230612 vban_cmd-2.4.0/vban_cmd/meta.py
+-rw-r--r--   0        0        0     9625 2023-07-25 14:57:29.669770 vban_cmd-2.4.0/vban_cmd/packet.py
+-rw-r--r--   0        0        0    10137 2023-06-25 12:32:36.307607 vban_cmd-2.4.0/vban_cmd/strip.py
+-rw-r--r--   0        0        0     2277 2023-06-25 10:36:40.287522 vban_cmd-2.4.0/vban_cmd/subject.py
+-rw-r--r--   0        0        0     2525 2023-07-12 03:46:12.026345 vban_cmd-2.4.0/vban_cmd/util.py
+-rw-r--r--   0        0        0     5735 2023-07-26 10:30:31.333522 vban_cmd-2.4.0/vban_cmd/vban.py
+-rw-r--r--   0        0        0     7391 2023-07-12 03:47:07.637840 vban_cmd-2.4.0/vban_cmd/vbancmd.py
+-rw-r--r--   0        0        0     6879 2023-07-25 14:56:03.314782 vban_cmd-2.4.0/vban_cmd/worker.py
+-rw-r--r--   0        0        0    12994 1970-01-01 00:00:00.000000 vban_cmd-2.4.0/PKG-INFO
```

### Comparing `vban_cmd-2.3.3/LICENSE` & `vban_cmd-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/pyproject.toml` & `vban_cmd-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vban-cmd"
-version = "2.3.3"
+version = "2.4.0"
 description = "Python interface for the VBAN RT Packet Service (Sendtext)"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/vban-cmd-python"
 
 [tool.poetry.dependencies]
```

### Comparing `vban_cmd-2.3.3/README.md` & `vban_cmd-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/bus.py` & `vban_cmd-2.4.0/vban_cmd/bus.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/command.py` & `vban_cmd-2.4.0/vban_cmd/command.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/config.py` & `vban_cmd-2.4.0/vban_cmd/config.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/event.py` & `vban_cmd-2.4.0/vban_cmd/event.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/factory.py` & `vban_cmd-2.4.0/vban_cmd/factory.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/iremote.py` & `vban_cmd-2.4.0/vban_cmd/iremote.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/kinds.py` & `vban_cmd-2.4.0/vban_cmd/kinds.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/macrobutton.py` & `vban_cmd-2.4.0/vban_cmd/macrobutton.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/meta.py` & `vban_cmd-2.4.0/vban_cmd/meta.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/packet.py` & `vban_cmd-2.4.0/vban_cmd/packet.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/strip.py` & `vban_cmd-2.4.0/vban_cmd/strip.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/subject.py` & `vban_cmd-2.4.0/vban_cmd/subject.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/util.py` & `vban_cmd-2.4.0/vban_cmd/util.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/vban.py` & `vban_cmd-2.4.0/vban_cmd/vban.py`

 * *Files 7% similar despite different names*

```diff
@@ -131,26 +131,23 @@
 
     @property
     def bit(self) -> int:
         return
 
 
 class VbanAudioInstream(VbanInstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Audio Instream"""
 
 
 class VbanMidiInstream(VbanInstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Midi Instream"""
 
 
 class VbanTextInstream(VbanInstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Text Instream"""
 
 
 class VbanOutstream(VbanStream):
     """
     class representing a vban outstream
 
     Subclasses VbanStream
@@ -161,21 +158,19 @@
 
     @property
     def direction(self) -> str:
         return "out"
 
 
 class VbanAudioOutstream(VbanOutstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Audio Outstream"""
 
 
 class VbanMidiOutstream(VbanOutstream):
-    def __str__(self):
-        return f"{type(self).__name__}{self._remote.kind}{self.index}"
+    """Represents a VBAN Midi Outstream"""
 
 
 def _make_stream_pair(remote, kind):
     num_instream, num_outstream, num_midi, num_text = kind.vban
 
     def _generate_streams(i, dir):
         """generator function for creating instream/outstream tuples"""
```

### Comparing `vban_cmd-2.3.3/vban_cmd/vbancmd.py` & `vban_cmd-2.4.0/vban_cmd/vbancmd.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/vban_cmd/worker.py` & `vban_cmd-2.4.0/vban_cmd/worker.py`

 * *Files identical despite different names*

### Comparing `vban_cmd-2.3.3/PKG-INFO` & `vban_cmd-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vban-cmd
-Version: 2.3.3
+Version: 2.4.0
 Summary: Python interface for the VBAN RT Packet Service (Sendtext)
 Home-page: https://github.com/onyx-and-iris/vban-cmd-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

