# Comparing `tmp/airtouch5py-0.2.7.tar.gz` & `tmp/airtouch5py-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airtouch5py-0.2.7.tar", max compression
+gzip compressed data, was "airtouch5py-0.2.8.tar", max compression
```

## Comparing `airtouch5py-0.2.7.tar` & `airtouch5py-0.2.8.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/LICENSE
--rw-r--r--   0        0        0       47 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/README.md
--rw-r--r--   0        0        0     4986 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/airtouch5_client.py
--rw-r--r--   0        0        0     9683 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/airtouch5_simple_client.py
--rw-r--r--   0        0        0     2208 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/data_packet_factory.py
--rw-r--r--   0        0        0    20400 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packet_decoder.py
--rw-r--r--   0        0        0    15561 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packet_encoder.py
--rw-r--r--   0        0        0      410 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packet_fields.py
--rw-r--r--   0        0        0     2199 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packet_reader.py
--rw-r--r--   0        0        0     3053 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packets/ac_ability.py
--rw-r--r--   0        0        0     2368 2023-07-31 21:40:15.796410 airtouch5py-0.2.7/airtouch5py/packets/ac_control.py
--rw-r--r--   0        0        0      395 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/ac_error_information.py
--rw-r--r--   0        0        0     2390 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/ac_status.py
--rw-r--r--   0        0        0      295 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/console_version.py
--rw-r--r--   0        0        0      254 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/datapacket.py
--rw-r--r--   0        0        0     1478 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/zone_control.py
--rw-r--r--   0        0        0      556 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/zone_name.py
--rw-r--r--   0        0        0     1694 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/airtouch5py/packets/zone_status.py
--rw-r--r--   0        0        0      382 2023-07-31 21:40:15.800410 airtouch5py-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/LICENSE
+-rw-r--r--   0        0        0       47 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/README.md
+-rw-r--r--   0        0        0     4986 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/airtouch5_client.py
+-rw-r--r--   0        0        0     9683 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/airtouch5_simple_client.py
+-rw-r--r--   0        0        0     2208 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/data_packet_factory.py
+-rw-r--r--   0        0        0    20432 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packet_decoder.py
+-rw-r--r--   0        0        0    15561 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packet_encoder.py
+-rw-r--r--   0        0        0      410 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packet_fields.py
+-rw-r--r--   0        0        0     2199 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packet_reader.py
+-rw-r--r--   0        0        0     3053 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packets/ac_ability.py
+-rw-r--r--   0        0        0     2368 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packets/ac_control.py
+-rw-r--r--   0        0        0      395 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packets/ac_error_information.py
+-rw-r--r--   0        0        0     2390 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packets/ac_status.py
+-rw-r--r--   0        0        0      295 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packets/console_version.py
+-rw-r--r--   0        0        0      254 2023-08-02 02:20:36.576600 airtouch5py-0.2.8/airtouch5py/packets/datapacket.py
+-rw-r--r--   0        0        0     1478 2023-08-02 02:20:36.580600 airtouch5py-0.2.8/airtouch5py/packets/zone_control.py
+-rw-r--r--   0        0        0      556 2023-08-02 02:20:36.580600 airtouch5py-0.2.8/airtouch5py/packets/zone_name.py
+-rw-r--r--   0        0        0     1694 2023-08-02 02:20:36.580600 airtouch5py-0.2.8/airtouch5py/packets/zone_status.py
+-rw-r--r--   0        0        0      382 2023-08-02 02:20:36.580600 airtouch5py-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      469 1970-01-01 00:00:00.000000 airtouch5py-0.2.8/PKG-INFO
```

### Comparing `airtouch5py-0.2.7/LICENSE` & `airtouch5py-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/airtouch5_client.py` & `airtouch5py-0.2.8/airtouch5py/airtouch5_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/airtouch5_simple_client.py` & `airtouch5py-0.2.8/airtouch5py/airtouch5_simple_client.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/data_packet_factory.py` & `airtouch5py-0.2.8/airtouch5py/data_packet_factory.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/packet_decoder.py` & `airtouch5py-0.2.8/airtouch5py/packet_decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -392,15 +392,15 @@
 
         while len(bytes) > 2:
             # Byte 3 AC number
             ac_number = struct.unpack(">B", bytes[0:1])[0]
             # Byte 4 Following data length
             length = struct.unpack(">B", bytes[1:2])[0]
             # Byte 5-20 AC Name (Null terminated if nulls fit)
-            name = bytes[2:18].decode("ascii").split("\x00")[0]
+            name = bytes[2:18].decode(errors="ignore").split("\x00")[0]
             # Byte 21 start zone number
             start_zone_number = struct.unpack(">B", bytes[18:19])[0]
             # Byte 22 zone count
             zone_count = struct.unpack(">B", bytes[19:20])[0]
 
             bits.clear()
             bits.frombytes(bytes[20:22])
@@ -476,15 +476,15 @@
         ac_number = struct.unpack(">B", bytes[0:1])[0]
         if len(bytes) == 1:
             return AcErrorInformationRequestData(ac_number)
 
         # Byte 4 error info length
         error_length = struct.unpack(">B", bytes[1:2])[0]
         # Byte 5-error_length error info
-        error_info = bytes[2 : 2 + error_length].decode("ascii")
+        error_info = bytes[2 : 2 + error_length].decode(errors="ignore")
         return AcErrorInformationData(ac_number, error_info)
 
     def decode_zone_name(self, bytes: bytes) -> Data:
         if len(bytes) == 0:
             return ZoneNameRequestData(None)
         if len(bytes) == 1:
             return ZoneNameRequestData(struct.unpack(">B", bytes[0:1])[0])
@@ -493,15 +493,15 @@
 
         while len(bytes) > 2:
             # Byte 3 Zone number
             zone_number = struct.unpack(">B", bytes[0:1])[0]
             # Byte 4 Name  length
             length = struct.unpack(">B", bytes[1:2])[0]
             # Byte 5..n Zone Name
-            name = bytes[2 : 2 + length].decode("ascii")
+            name = bytes[2 : 2 + length].decode(errors="ignore")
 
             names.append(ZoneName(zone_number, name))
             # We've now used the first 2 + length bytes, so remove them from the buffer
             bytes = bytes[2 + length :]
 
         return ZoneNameData(names)
 
@@ -510,10 +510,10 @@
             return ConsoleVersionRequestData()
 
         # Byte 3 Update sign (0 - latest, Other - new version)
         has_update = struct.unpack(">B", bytes[0:1])[0] != 0
         # Byte 4 version string length
         length = struct.unpack(">B", bytes[1:2])[0]
         # Byte 5..n Version string
-        version = bytes[2 : 2 + length].decode("ascii")
+        version = bytes[2 : 2 + length].decode(errors="ignore")
 
         return ConsoleVersionData(has_update, version)
```

### Comparing `airtouch5py-0.2.7/airtouch5py/packet_encoder.py` & `airtouch5py-0.2.8/airtouch5py/packet_encoder.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/packet_reader.py` & `airtouch5py-0.2.8/airtouch5py/packet_reader.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/packets/ac_ability.py` & `airtouch5py-0.2.8/airtouch5py/packets/ac_ability.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/packets/ac_control.py` & `airtouch5py-0.2.8/airtouch5py/packets/ac_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/packets/ac_status.py` & `airtouch5py-0.2.8/airtouch5py/packets/ac_status.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/packets/zone_control.py` & `airtouch5py-0.2.8/airtouch5py/packets/zone_control.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/packets/zone_name.py` & `airtouch5py-0.2.8/airtouch5py/packets/zone_name.py`

 * *Files identical despite different names*

### Comparing `airtouch5py-0.2.7/airtouch5py/packets/zone_status.py` & `airtouch5py-0.2.8/airtouch5py/packets/zone_status.py`

 * *Files identical despite different names*

