# Comparing `tmp/serial_packets-0.2.0.tar.gz` & `tmp/serial_packets-0.2.1.tar.gz`

## Comparing `serial_packets-0.2.0.tar` & `serial_packets-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/__init__.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/_packets.py
--rw-r--r--   0        0        0    17761 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/client.py
--rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/packet_decoder.py
--rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/packet_encoder.py
--rw-r--r--   0        0        0     7691 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/packets.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.2.0/src/serial_packets/py.typed
--rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.2.0/.gitignore
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.2.0/LICENSE
--rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.2.0/README.md
--rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.2.1/src/serial_packets/__init__.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 serial_packets-0.2.1/src/serial_packets/_packets.py
+-rw-r--r--   0        0        0    17761 2020-02-02 00:00:00.000000 serial_packets-0.2.1/src/serial_packets/client.py
+-rw-r--r--   0        0        0     7536 2020-02-02 00:00:00.000000 serial_packets-0.2.1/src/serial_packets/packet_decoder.py
+-rw-r--r--   0        0        0     4130 2020-02-02 00:00:00.000000 serial_packets-0.2.1/src/serial_packets/packet_encoder.py
+-rw-r--r--   0        0        0     8151 2020-02-02 00:00:00.000000 serial_packets-0.2.1/src/serial_packets/packets.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 serial_packets-0.2.1/src/serial_packets/py.typed
+-rw-r--r--   0        0        0        5 2020-02-02 00:00:00.000000 serial_packets-0.2.1/.gitignore
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 serial_packets-0.2.1/LICENSE
+-rw-r--r--   0        0        0    16147 2020-02-02 00:00:00.000000 serial_packets-0.2.1/README.md
+-rw-r--r--   0        0        0     1061 2020-02-02 00:00:00.000000 serial_packets-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0    16419 2020-02-02 00:00:00.000000 serial_packets-0.2.1/PKG-INFO
```

### Comparing `serial_packets-0.2.0/src/serial_packets/_packets.py` & `serial_packets-0.2.1/src/serial_packets/_packets.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.2.0/src/serial_packets/client.py` & `serial_packets-0.2.1/src/serial_packets/client.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.2.0/src/serial_packets/packet_decoder.py` & `serial_packets-0.2.1/src/serial_packets/packet_decoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.2.0/src/serial_packets/packet_encoder.py` & `serial_packets-0.2.1/src/serial_packets/packet_encoder.py`

 * *Files identical despite different names*

### Comparing `serial_packets-0.2.0/src/serial_packets/packets.py` & `serial_packets-0.2.1/src/serial_packets/packets.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self.__data: bytearray = bytearray()
         self.__bytes_read: int = 0
         self.__read_error: bool = False
 
     def hex_str(self, max_bytes=None) -> str:
         """Returns a string with a hex dump fo the bytes. Can be long."""
         if (max_bytes is None) or (self.size() <= max_bytes):
-            return  self.__data.hex(sep=' ')
+            return self.__data.hex(sep=' ')
         prefix = self.__data[:max_bytes].hex(sep=" ")
         return f"{prefix} ... ({self.size() - max_bytes} more)"
 
     def data_bytes(self) -> bytearray:
         """Return a copy of the data bytes."""
         return self.__data.copy()
 
@@ -166,15 +166,15 @@
             self.__read_error = True
             return None
         result = int.from_bytes(self.__data[self.__bytes_read:self.__bytes_read + 2],
                                 byteorder='big',
                                 signed=False)
         self.__bytes_read += 2
         return result
-      
+
     def read_int24(self) -> int | None:
         """Decodes the next 3 bytes as a 24 bits signed big endian value.
         Returns the 24 bit number and advances the reading location by 3 bytes,
         or returns None if insufficient number of bytes to read.
         """
         if self.__read_error or self.__bytes_read + 3 > len(self.__data):
             self.__read_error = True
@@ -205,7 +205,20 @@
         assert (n >= 0)
         if self.__read_error or self.__bytes_read + n > len(self.__data):
             self.__read_error = True
             return None
         result = self.__data[self.__bytes_read:self.__bytes_read + n]
         self.__bytes_read += n
         return result
+
+    def read_str(self) -> str | None:
+        """Returns the next string or null if read error."""
+        if self.__read_error or self.__bytes_read + 1 > len(self.__data):
+            self.__read_error = True
+            return None
+        # Read length byte.
+        n = self.read_uint8()
+        # Read characters.
+        str_bytes = self.read_bytes(n)
+        if self.__read_error:
+            return None
+        return str_bytes.decode("utf-8")
```

### Comparing `serial_packets-0.2.0/LICENSE` & `serial_packets-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serial_packets-0.2.0/README.md` & `serial_packets-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `serial_packets-0.2.0/pyproject.toml` & `serial_packets-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "serial_packets"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Zapta", email="zapta@zapta.com" },
 ]
 description = "A Python impelementation of the Serial Packets protocol"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `serial_packets-0.2.0/PKG-INFO` & `serial_packets-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serial_packets
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python impelementation of the Serial Packets protocol
 Project-URL: Homepage, https://github.com/zapta/serial_packets_py
 Project-URL: Bug Tracker, https://github.com/zapta/serial_packets_py/issues
 Author-email: Zapta <zapta@zapta.com>
 License-File: LICENSE
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Operating System :: OS Independent
```

