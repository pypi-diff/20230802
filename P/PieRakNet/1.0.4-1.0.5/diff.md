# Comparing `tmp/PieRakNet-1.0.4.tar.gz` & `tmp/PieRakNet-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PieRakNet-1.0.4.tar", last modified: Thu Jul 13 07:17:06 2023, max compression
+gzip compressed data, was "PieRakNet-1.0.5.tar", last modified: Wed Aug  2 07:38:57 2023, max compression
```

## Comparing `PieRakNet-1.0.4.tar` & `PieRakNet-1.0.5.tar`

### file list

```diff
@@ -1,43 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 07:17:06.270688 PieRakNet-1.0.4/
--rw-rw-rw-   0        0        0    35823 2023-06-29 08:26:14.000000 PieRakNet-1.0.4/LICENSE
--rw-rw-rw-   0        0        0      985 2023-07-13 07:17:06.267691 PieRakNet-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-13 07:17:02.760366 PieRakNet-1.0.4/PieRakNet.egg-info/
--rw-rw-rw-   0        0        0      985 2023-07-13 07:17:01.000000 PieRakNet-1.0.4/PieRakNet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1194 2023-07-13 07:17:01.000000 PieRakNet-1.0.4/PieRakNet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 07:17:01.000000 PieRakNet-1.0.4/PieRakNet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-07-13 07:17:01.000000 PieRakNet-1.0.4/PieRakNet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       75 2023-07-04 10:38:51.000000 PieRakNet-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-13 07:17:05.194071 PieRakNet-1.0.4/pieraknet/
--rw-rw-rw-   0        0        0      119 2023-07-07 07:59:21.000000 PieRakNet-1.0.4/pieraknet/__init__.py
--rw-rw-rw-   0        0        0     4988 2023-07-06 07:52:28.000000 PieRakNet-1.0.4/pieraknet/buffer.py
--rw-rw-rw-   0        0        0    10384 2023-07-06 11:36:48.000000 PieRakNet-1.0.4/pieraknet/connection.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:17:05.480377 PieRakNet-1.0.4/pieraknet/handlers/
--rw-rw-rw-   0        0        0        0 2023-07-13 07:13:46.000000 PieRakNet-1.0.4/pieraknet/handlers/__init__.py
--rw-rw-rw-   0        0        0      702 2023-07-06 10:31:49.000000 PieRakNet-1.0.4/pieraknet/handlers/connection_request.py
--rw-rw-rw-   0        0        0     1636 2023-07-04 11:31:23.000000 PieRakNet-1.0.4/pieraknet/handlers/offline_ping.py
--rw-rw-rw-   0        0        0      473 2023-07-06 10:31:49.000000 PieRakNet-1.0.4/pieraknet/handlers/online_ping.py
--rw-rw-rw-   0        0        0     2658 2023-07-04 12:22:51.000000 PieRakNet-1.0.4/pieraknet/handlers/open_connection_request_1.py
--rw-rw-rw-   0        0        0     1955 2023-07-06 10:40:18.000000 PieRakNet-1.0.4/pieraknet/handlers/open_connection_request_2.py
-drwxrwxrwx   0        0        0        0 2023-07-13 07:17:06.263703 PieRakNet-1.0.4/pieraknet/packets/
--rw-rw-rw-   0        0        0        0 2023-07-13 07:13:46.000000 PieRakNet-1.0.4/pieraknet/packets/__init__.py
--rw-rw-rw-   0        0        0     2558 2023-07-04 10:50:56.000000 PieRakNet-1.0.4/pieraknet/packets/acknowledgement.py
--rw-rw-rw-   0        0        0      462 2023-07-06 09:33:49.000000 PieRakNet-1.0.4/pieraknet/packets/connection_request.py
--rw-rw-rw-   0        0        0      627 2023-07-06 09:49:21.000000 PieRakNet-1.0.4/pieraknet/packets/connection_request_accepted.py
--rw-rw-rw-   0        0        0      130 2023-07-04 09:50:06.000000 PieRakNet-1.0.4/pieraknet/packets/disconnect.py
--rw-rw-rw-   0        0        0     3245 2023-07-06 07:52:28.000000 PieRakNet-1.0.4/pieraknet/packets/frame_set.py
--rw-rw-rw-   0        0        0      865 2023-07-06 10:03:10.000000 PieRakNet-1.0.4/pieraknet/packets/game_packet.py
--rw-rw-rw-   0        0        0      403 2023-07-04 10:03:15.000000 PieRakNet-1.0.4/pieraknet/packets/incompatible_protocol.py
--rw-rw-rw-   0        0        0      525 2023-07-06 09:26:49.000000 PieRakNet-1.0.4/pieraknet/packets/new_incoming_connection.py
--rw-rw-rw-   0        0        0      391 2023-07-03 09:27:19.000000 PieRakNet-1.0.4/pieraknet/packets/offline_ping.py
--rw-rw-rw-   0        0        0      719 2023-07-13 07:15:53.000000 PieRakNet-1.0.4/pieraknet/packets/offline_pong.py
--rw-rw-rw-   0        0        0      331 2023-07-06 08:55:38.000000 PieRakNet-1.0.4/pieraknet/packets/online_ping.py
--rw-rw-rw-   0        0        0      463 2023-07-06 08:55:38.000000 PieRakNet-1.0.4/pieraknet/packets/online_pong.py
--rw-rw-rw-   0        0        0      487 2023-07-04 10:03:16.000000 PieRakNet-1.0.4/pieraknet/packets/open_connection_reply_1.py
--rw-rw-rw-   0        0        0      612 2023-07-04 10:03:16.000000 PieRakNet-1.0.4/pieraknet/packets/open_connection_reply_2.py
--rw-rw-rw-   0        0        0      419 2023-07-06 10:04:05.000000 PieRakNet-1.0.4/pieraknet/packets/open_connection_request_1.py
--rw-rw-rw-   0        0        0      514 2023-07-04 09:44:42.000000 PieRakNet-1.0.4/pieraknet/packets/open_connection_request_2.py
--rw-rw-rw-   0        0        0      548 2023-07-03 09:29:51.000000 PieRakNet-1.0.4/pieraknet/packets/packet.py
--rw-rw-rw-   0        0        0      608 2023-07-06 10:03:10.000000 PieRakNet-1.0.4/pieraknet/protocol_info.py
--rw-rw-rw-   0        0        0     3695 2023-07-07 08:44:14.000000 PieRakNet-1.0.4/pieraknet/server.py
--rw-rw-rw-   0        0        0       42 2023-07-13 07:17:06.270688 PieRakNet-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-07-13 07:12:27.000000 PieRakNet-1.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:38:57.509613 PieRakNet-1.0.5/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-08-02 07:38:57.509613 PieRakNet-1.0.5/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:38:57.505613 PieRakNet-1.0.5/PieRakNet.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-08-02 07:38:57.000000 PieRakNet-1.0.5/PieRakNet.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-08-02 07:38:57.000000 PieRakNet-1.0.5/PieRakNet.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 07:38:57.000000 PieRakNet-1.0.5/PieRakNet.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-08-02 07:38:57.000000 PieRakNet-1.0.5/PieRakNet.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:38:57.505613 PieRakNet-1.0.5/pieraknet/
+-rw-r--r--   0 root         (0) root         (0)      116 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4963 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/buffer.py
+-rw-r--r--   0 root         (0) root         (0)    10161 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/connection.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:38:57.505613 PieRakNet-1.0.5/pieraknet/handlers/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/handlers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      716 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/handlers/connection_request.py
+-rw-r--r--   0 root         (0) root         (0)     1606 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/handlers/offline_ping.py
+-rw-r--r--   0 root         (0) root         (0)      459 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/handlers/online_ping.py
+-rw-r--r--   0 root         (0) root         (0)     2613 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/handlers/open_connection_request_1.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/handlers/open_connection_request_2.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 07:38:57.509613 PieRakNet-1.0.5/pieraknet/packets/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/acknowledgement.py
+-rw-r--r--   0 root         (0) root         (0)      445 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/connection_request.py
+-rw-r--r--   0 root         (0) root         (0)      607 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/connection_request_accepted.py
+-rw-r--r--   0 root         (0) root         (0)      124 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/disconnect.py
+-rw-r--r--   0 root         (0) root         (0)     3157 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/frame_set.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/game_packet.py
+-rw-r--r--   0 root         (0) root         (0)      388 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/incompatible_protocol.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/new_incoming_connection.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/offline_ping.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/offline_pong.py
+-rw-r--r--   0 root         (0) root         (0)      317 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/online_ping.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/online_pong.py
+-rw-r--r--   0 root         (0) root         (0)      470 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/open_connection_reply_1.py
+-rw-r--r--   0 root         (0) root         (0)      593 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/open_connection_reply_2.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/open_connection_request_1.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/open_connection_request_2.py
+-rw-r--r--   0 root         (0) root         (0)      526 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/packets/packet.py
+-rw-r--r--   0 root         (0) root         (0)      587 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/protocol_info.py
+-rw-r--r--   0 root         (0) root         (0)     3612 2023-08-02 07:32:45.000000 PieRakNet-1.0.5/pieraknet/server.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 07:38:57.509613 PieRakNet-1.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1163 2023-08-02 07:37:32.000000 PieRakNet-1.0.5/setup.py
```

### Comparing `PieRakNet-1.0.4/PKG-INFO` & `PieRakNet-1.0.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1
-Name: PieRakNet
-Version: 1.0.4
-Summary: RakNet implementation, written in Python. Created for PieMC.
-Home-page: https://github.com/PieMC-Dev/PieRakNet
-Author: lapismyt
-Author-email: nikitagavrilin005@gmail.com
-Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
-Project-URL: Developer, https://github.com/PieMC-Dev
-Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Networking
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PieRakNet
-RakNet implementation, written in Python. Created for PieMC.
+Metadata-Version: 2.1
+Name: PieRakNet
+Version: 1.0.5
+Summary: RakNet implementation, written in Python. Created for PieMC.
+Home-page: https://github.com/PieMC-Dev/PieRakNet
+Author: lapismyt
+Author-email: nikitagavrilin005@gmail.com
+License: UNKNOWN
+Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
+Project-URL: Developer, https://github.com/PieMC-Dev
+Description: # PieRakNet
+        RakNet implementation, written in Python. Created for PieMC.
+        
+Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Networking
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
```

### Comparing `PieRakNet-1.0.4/PieRakNet.egg-info/PKG-INFO` & `PieRakNet-1.0.5/PieRakNet.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1
-Name: PieRakNet
-Version: 1.0.4
-Summary: RakNet implementation, written in Python. Created for PieMC.
-Home-page: https://github.com/PieMC-Dev/PieRakNet
-Author: lapismyt
-Author-email: nikitagavrilin005@gmail.com
-Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
-Project-URL: Developer, https://github.com/PieMC-Dev
-Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
-Classifier: Development Status :: 3 - Alpha
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Games/Entertainment
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: System :: Networking
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# PieRakNet
-RakNet implementation, written in Python. Created for PieMC.
+Metadata-Version: 2.1
+Name: PieRakNet
+Version: 1.0.5
+Summary: RakNet implementation, written in Python. Created for PieMC.
+Home-page: https://github.com/PieMC-Dev/PieRakNet
+Author: lapismyt
+Author-email: nikitagavrilin005@gmail.com
+License: UNKNOWN
+Project-URL: Example, https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md
+Project-URL: Developer, https://github.com/PieMC-Dev
+Description: # PieRakNet
+        RakNet implementation, written in Python. Created for PieMC.
+        
+Keywords: python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet
+Platform: UNKNOWN
+Classifier: Development Status :: 3 - Alpha
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet
+Classifier: Topic :: Games/Entertainment
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Networking
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
```

### Comparing `PieRakNet-1.0.4/PieRakNet.egg-info/SOURCES.txt` & `PieRakNet-1.0.5/PieRakNet.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 PieRakNet.egg-info/PKG-INFO
 PieRakNet.egg-info/SOURCES.txt
 PieRakNet.egg-info/dependency_links.txt
 PieRakNet.egg-info/top_level.txt
 pieraknet/__init__.py
```

### Comparing `PieRakNet-1.0.4/pieraknet/buffer.py` & `PieRakNet-1.0.5/pieraknet/buffer.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,169 +1,176 @@
-#
-#
-# //--------\\    [----------]   ||--------]   ||\      /||    ||----------]
-# ||        ||         ||        ||            ||\\    //||    ||
-# ||        //         ||        ||======|     || \\  // ||    ||
-# ||-------//          ||        ||            ||  \\//  ||    ||
-# ||                   ||        ||            ||   —–   ||    ||
-# ||              [----------]   ||--------]   ||        ||    ||----------]
-# This program is free software: you can redistribute it and/or modify
-# it under the terms of the GNU Lesser General Public License as published by
-# the Free Software Foundation, either version 3 of the License, or
-# (at your option) any later version.
-#
-# @author PieMC Team
-# @link http://www.PieMC-Dev.github.io/
-#
-#
-#
-
-import struct
-from io import BytesIO
-
-
-class UnsupportedIPVersion(Exception):
-    pass
-
-
-class EOSError(Exception):
-    pass
-
-
-class BuffError(Exception):
-    pass
-
-
-class Buffer(BytesIO):
-    def feos(self):
-        if len(bytes(self.getvalue()).decode()[self.tell()]) == 0:
-            return True
-        else:
-            return False
-
-    def read_packet_id(self):  # Read Packet ID
-        return self.read_byte()
-
-    def write_packet_id(self, data):
-        self.write_byte(str(data))
-
-    def read_byte(self):
-        return struct.unpack('b', self.read(1))[0]
-
-    def write_byte(self, data):
-        if not isinstance(data, bytes):
-            data = str(data).encode()
-        self.write(struct.pack('b', int(data)))
-
-    def read_ubyte(self):
-        return struct.unpack('B', self.read(1))[0]
-
-    def write_ubyte(self, data):
-        if not isinstance(data, bytes):
-            data = data.encode('utf-8')
-        self.write(struct.pack('B', data))
-
-    def read_short(self):
-        return struct.unpack('>h', self.read(2))[0]
-
-    def write_short(self, data):
-        self.write(struct.pack('>h', data))
-
-    def read_unsigned_short(self):
-        return struct.unpack('>H', self.read(2))[0]
-
-    def write_unsigned_short(self, data):
-        self.write(struct.pack('>H', data))
-
-    def read_magic(self):
-        return self.read(16)
-
-    def write_magic(self, data=b'00ffff00fefefefefdfdfdfd12345678'):
-        if not isinstance(data, bytes):
-            data = data.encode('utf-8')
-        self.write(data)
-
-    def read_long(self):
-        return struct.unpack('>q', self.read(8))[0]
-
-    def write_long(self, data):
-        self.write(struct.pack('>q', data))
-
-    def read_ulong(self):
-        return struct.unpack('>Q', self.read(8))[0]
-
-    def write_ulong(self, data):
-        self.write(struct.pack('>Q', data))
-
-    def read_int(self):
-        return struct.unpack(">i", self.read(4))[0]
-
-    def write_int(self, data):
-        self.write(struct.pack('>i', data))
-
-    def read_uint(self):
-        return struct.unpack(">I", self.read(4))[0]
-
-    def write_uint(self, data):
-        self.write(struct.pack('>I', data))
-
-    def read_bool(self):
-        return struct.unpack('?', self.read(1))[0]
-
-    def write_bool(self, data):
-        self.write(struct.pack('?', data))
-
-    def read_uint24le(self):
-        return struct.unpack("<I", self.read(3) + b'\x00')[0]
-
-    def write_uint24le(self, data):
-        self.write(struct.pack("<I", data)[:3])
-
-    def read_string(self):
-        length = self.read_short()
-        string = self.read(length).decode('utf-8')
-        return string
-
-    def write_string(self, data):
-        self.write_short(len(data))
-        if not isinstance(data, bytes):
-            data = data.encode('utf-8')
-        self.write(data)
-
-    def read_address(self):
-        ipv = self.read_byte()
-        if ipv == 4:
-            hostname_parts = []
-            for part in range(4):
-                hostname_parts.append(str(~self.read_byte() & 0xff))
-            hostname = ".".join(hostname_parts)
-            port = self.read_unsigned_short()
-            return hostname, port
-        else:
-            raise UnsupportedIPVersion('IP version is not 4')
-
-    def write_address(self, address: tuple):
-        self.write_byte(4)
-        hostname_parts: list = address[0].split('.')
-        for part in hostname_parts:
-            self.write_byte(~int(part) & 0xff)
-        self.write_short(address[1])
-
-    def read_var_int(self):
-        value: int = 0
-        for i in range(0, 35, 7):
-            number = self.read_ubyte()
-            value |= ((number & 0x7f) << i)
-            if (number & 0x80) == 0:
-                return value
-        raise BuffError("VarInt is too big")
-
-    def write_var_int(self, value: int) -> None:
-        value &= 0xffffffff
-        for i in range(0, 5):
-            to_write: int = value & 0x7f
-            value >>= 7
-            if value != 0:
-                self.write_ubyte(to_write | 0x80)
-            else:
-                self.write_ubyte(to_write)
-                break
+#
+#
+# //--------\\    [----------]   ||--------]   ||\      /||    ||----------]
+# ||        ||         ||        ||            ||\\    //||    ||
+# ||        //         ||        ||======|     || \\  // ||    ||
+# ||-------//          ||        ||            ||  \\//  ||    ||
+# ||                   ||        ||            ||   —–   ||    ||
+# ||              [----------]   ||--------]   ||        ||    ||----------]
+# This program is free software: you can redistribute it and/or modify
+# it under the terms of the GNU Lesser General Public License as published by
+# the Free Software Foundation, either version 3 of the License, or
+# (at your option) any later version.
+#
+# @author PieMC Team
+# @link http://www.PieMC-Dev.github.io/
+#
+#
+#
+
+import struct
+from io import BytesIO
+
+
+class UnsupportedIPVersion(Exception):
+    pass
+
+
+class EOSError(Exception):
+    pass
+
+
+class BuffError(Exception):
+    pass
+
+
+class Buffer(BytesIO):
+    def feos(self):
+        if len(self.getvalue()[self.tell():]) == 0:
+            return True
+        else:
+            return False
+
+    def read_packet_id(self):  # Read Packet ID
+        return self.read_byte()
+
+    def write_packet_id(self, data):
+        self.write_byte(str(data))
+
+    def read_byte(self):
+        return struct.unpack('B', self.read(1))[0]
+
+    def write_byte(self, data):
+        if not isinstance(data, bytes):
+            data = str(data).encode()
+        self.write(struct.pack('B', int(data)))
+
+    def read_ubyte(self):
+        return struct.unpack('<B', self.read(1))[0]
+
+    def write_ubyte(self, data):
+        if not isinstance(data, bytes):
+            data = data.encode('utf-8')
+        self.write(struct.pack('<B', data))
+
+    def read_short(self):
+        shrt = self.read(2)
+        print(shrt)
+        return struct.unpack('>h', shrt)[0]
+
+    def write_short(self, data):
+        self.write(struct.pack('>h', data))
+
+    def read_unsigned_short(self):
+        ushrt = self.read(2)
+        print(ushrt)
+        return struct.unpack('>H', ushrt)[0]
+
+    def write_unsigned_short(self, data):
+        self.write(struct.pack('>H', data))
+
+    def read_magic(self):
+        return self.read(16)
+
+    def write_magic(self, data=b'00ffff00fefefefefdfdfdfd12345678'):
+        if not isinstance(data, bytes):
+            data = data.encode('utf-8')
+        self.write(data)
+
+    def read_long(self):
+        return struct.unpack('>q', self.read(8))[0]
+
+    def write_long(self, data):
+        self.write(struct.pack('>q', data))
+
+    def read_ulong(self):
+        return struct.unpack('>Q', self.read(8))[0]
+
+    def write_ulong(self, data):
+        self.write(struct.pack('>Q', data))
+
+    def read_int(self):
+        dat = self.read(4)
+        print(dat)
+        return struct.unpack(">i", dat)[0]
+
+    def write_int(self, data):
+        self.write(struct.pack('>i', data))
+
+    def read_uint(self):
+        return struct.unpack(">I", self.read(4))[0]
+
+    def write_uint(self, data):
+        self.write(struct.pack('>I', data))
+
+    def read_bool(self):
+        return struct.unpack('?', self.read(1))[0]
+
+    def write_bool(self, data):
+        self.write(struct.pack('?', data))
+
+    def read_uint24le(self):
+        uint24le = self.read(3) + b'\x00'
+        return struct.unpack("<I", uint24le)[0]
+
+    def write_uint24le(self, data):
+        self.write(struct.pack("<I", data)[:3])
+
+    def read_string(self):
+        length = self.read_short()
+        string = self.read(length).decode('utf-8')
+        return string
+
+    def write_string(self, data):
+        self.write_short(len(data))
+        if not isinstance(data, bytes):
+            data = data.encode('utf-8')
+        self.write(data)
+
+    def read_address(self):
+        ipv = self.read_byte()
+        if ipv == 4:
+            hostname_parts = []
+            for part in range(4):
+                hostname_parts.append(str(~self.read_byte() & 0xff))
+            hostname = ".".join(hostname_parts)
+            port = self.read_unsigned_short()
+            return hostname, port
+        else:
+            raise UnsupportedIPVersion('IP version is not 4')
+
+    def write_address(self, address: tuple):
+        self.write_byte(4)
+        hostname_parts: list = address[0].split('.')
+        for part in hostname_parts:
+            self.write_byte(~int(part) & 0xff)
+        self.write_unsigned_short(address[1])
+
+    def read_var_int(self):
+        value: int = 0
+        for i in range(0, 35, 7):
+            number = self.read_ubyte()
+            value |= ((number & 0x7f) << i)
+            if (number & 0x80) == 0:
+                return value
+        raise BuffError("VarInt is too big")
+
+    def write_var_int(self, value: int) -> None:
+        value &= 0xffffffff
+        for i in range(0, 5):
+            to_write: int = value & 0x7f
+            value >>= 7
+            if value != 0:
+                self.write_ubyte(to_write | 0x80)
+            else:
+                self.write_ubyte(to_write)
+                break
```

### Comparing `PieRakNet-1.0.4/pieraknet/connection.py` & `PieRakNet-1.0.5/pieraknet/connection.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-import time
-from pieraknet.packets.frame_set import FrameSet, Frame
-from pieraknet.protocol_info import ProtocolInfo
-from pieraknet.packets.acknowledgement import Ack, Nack
-from pieraknet.handlers.connection_request import ConnectionRequestHandler
-from pieraknet.handlers.online_ping import OnlinePingHandler
-from pieraknet.packets.online_ping import OnlinePing
-from pieraknet.packets.new_incoming_connection import NewIncomingConnection
-from pieraknet.packets.disconnect import Disconnect
-
-
-class Connection:
-    def __init__(self, address, server, mtu_size, guid):
-        self.address = address
-        self.mtu_size = mtu_size
-        self.server = server
-        self.guid = guid
-        self.connected = False
-        self.recovery_queue = {}
-        self.ack_queue = []
-        self.nack_queue = []
-        self.fragmented_packets = {}
-        self.compound_id = 0
-        self.client_sequence_numbers = []
-        # self.server_sequence_numbers = []
-        self.client_sequence_number = 0
-        self.server_sequence_number = 0
-        self.queue = FrameSet()
-        self.server_reliable_frame_index = 0
-        self.client_reliable_frame_index = 0
-        self.channel_index = [0] * 32
-        self.last_receive_time = time.time()
-
-    def update(self):
-        if (time.time() - self.last_receive_time) >= self.server.timeout:
-            self.disconnect()
-        self.send_ack_queue()
-        self.send_nack_queue()
-        self.send_queue()
-
-    def send_data(self, data: bytes):
-        self.server.send(data, self.address)
-
-    def handle(self, data):
-        self.last_receive_time = time.time()
-        if data[0] == ProtocolInfo.ACK:
-            self.handle_ack(data)
-        elif data[0] == ProtocolInfo.NACK:
-            self.handle_nack(data)
-        elif ProtocolInfo.FRAME_SET_0 <= data[0] <= ProtocolInfo.FRAME_SET_F:
-            self.handle_frame_set(data)
-
-    def handle_ack(self, data: bytes):
-        packet = Ack(data)
-        packet.decode()
-        for sequence_number in packet.sequence_numbers:
-            if sequence_number in self.recovery_queue:
-                del self.recovery_queue[sequence_number]
-
-    def handle_nack(self, data: bytes):
-        packet = Nack(data)
-        packet.decode()
-        for sequence_number in packet.sequence_numbers:
-            if sequence_number in self.recovery_queue:
-                lost_packet = self.recovery_queue[sequence_number]
-                lost_packet.sequence_number = self.server_sequence_number
-                self.server_sequence_number += 1
-                lost_packet.encode()
-                self.send_data(lost_packet.data)
-                del self.recovery_queue[sequence_number]
-
-    def handle_frame_set(self, data: bytes):
-        packet = FrameSet(data)
-        packet.decode()
-        if packet.sequence_number not in self.client_sequence_numbers:
-            if packet.sequence_number in self.nack_queue:
-                self.nack_queue.remove(packet.sequence_number)
-            self.client_sequence_numbers.append(packet.sequence_number)
-            self.ack_queue.append(packet.sequence_number)
-            hole_size = packet.sequence_number - self.client_sequence_number
-            if hole_size > 0:
-                for sequence_number in range(self.client_sequence_number + 1, hole_size):
-                    if sequence_number not in self.client_sequence_numbers:
-                        self.nack_queue.append(sequence_number)
-            self.client_sequence_number: int = packet.sequence_number
-            for frame in packet.frames:
-                if not (2 <= frame.reliability <= 7 and frame.reliability != 5):
-                    self.handle_frame(frame)
-                else:
-                    hole_size = frame.reliable_frame_index - self.client_reliable_frame_index
-                    if hole_size == 0:
-                        self.handle_frame(frame)
-                        self.client_reliable_frame_index += 1
-
-    def handle_fragmented_frame(self, packet):
-        if packet.compound_id not in self.fragmented_packets:
-            self.fragmented_packets[packet.compound_id] = {packet.index: packet}
-        else:
-            self.fragmented_packets[packet.compound_id][packet.index] = packet
-        if len(self.fragmented_packets[packet.compound_id]) == packet.compound_size:
-            new_frame = Frame()
-            new_frame.body = b''
-            for i in range(0, packet.compound_size):
-                new_frame.body += self.fragmented_packets[packet.compound_id][i].body
-            del self.fragmented_packets[packet.compound_id]
-            self.handle_frame(new_frame)
-
-    def handle_frame(self, packet):
-        if packet.fragmented:
-            self.handle_fragmented_frame(packet)
-        else:
-            if not self.connected:
-                if packet.body[0] == ProtocolInfo.CONNECTION_REQUEST:
-                    new_frame = Frame()
-                    new_frame.reliability = 0
-                    new_frame.body = ConnectionRequestHandler.handle(packet.body, self.server, self)
-                    self.add_to_queue(new_frame)
-                elif packet.body[0] == ProtocolInfo.NEW_INCOMING_CONNECTION:
-                    packet = NewIncomingConnection(packet.body)
-                    packet.decode()
-                    if packet.server_address[1] == self.server.port:
-                        self.connected = True
-                        if hasattr(self.server, "interface"):
-                            if hasattr(self.server.interface, "on_new_incoming_connection"):
-                                self.server.interface.on_new_incoming_connection(self)
-            elif packet.body[0] == ProtocolInfo.ONLINE_PING:
-                new_frame = Frame()
-                new_frame.reliability = 0
-                new_frame.body = OnlinePingHandler.handle(OnlinePing(packet.body), self, self.server)
-                self.add_to_queue(new_frame, False)
-            elif packet.body[0] == ProtocolInfo.DISCONNECT:
-                self.disconnect()
-            elif packet.body[0] == ProtocolInfo.GAME_PACKET:
-                if hasattr(self.server, "interface"):
-                    if hasattr(self.server.interface, "on_game_packet"):
-                        self.server.interface.on_game_packet(packet, self)
-            else:
-                if hasattr(self.server, "interface"):
-                    if hasattr(self.server.interface, "on_unknown_packet"):
-                        self.server.interface.on_unknown_packet(packet, self)
-
-    def send_queue(self):
-        if len(self.queue.frames) > 0:
-            self.queue.sequence_number = self.server_sequence_number
-            self.server_sequence_number += 1
-            self.recovery_queue[self.queue.sequence_number] = self.queue
-            self.queue.encode()
-            self.send_data(self.queue.getvalue())
-            self.queue = FrameSet()
-
-    def add_to_queue(self, packet: Frame, is_immediate=True):
-        if 2 <= packet.reliability <= 7 and packet.reliability != 5:
-            packet.reliable_frame_index = self.server_reliable_frame_index
-            self.server_reliable_frame_index += 1
-            if packet.reliability == 3:
-                packet.ordered_frame_index = self.channel_index[packet.order_channel]
-                self.channel_index[packet.order_channel] += 1
-        if packet.get_size() > self.mtu_size:
-            fragmented_body = []
-            for i in range(0, len(packet.body), self.mtu_size):
-                fragmented_body.append(packet.body[i:i + self.mtu_size])
-            for index, body in enumerate(fragmented_body):
-                new_packet = Frame()
-                new_packet.fragmented = True
-                new_packet.reliability = packet.reliability
-                new_packet.compound_id = self.compound_id
-                new_packet.compound_size = len(fragmented_body)
-                new_packet.index = index
-                new_packet.body = body
-                if index != 0:
-                    new_packet.reliable_frame_index = self.server_reliable_frame_index
-                    self.server_reliable_frame_index += 1
-                if new_packet.reliability == 3:
-                    new_packet.ordered_frame_index = packet.ordered_frame_index
-                    new_packet.order_channel = packet.order_channel
-                if is_immediate:
-                    self.queue.frames.append(new_packet)
-                    self.send_queue()
-                else:
-                    frame_size: int = new_packet.get_size()
-                    queue_size: int = self.queue.get_size()
-                    if frame_size + queue_size >= self.mtu_size:
-                        self.send_queue()
-                    self.queue.frames.append(new_packet)
-            self.compound_id += 1
-        else:
-            if is_immediate:
-                self.queue.frames.append(packet)
-                self.send_queue()
-            else:
-                frame_size: int = packet.get_size()
-                queue_size: int = self.queue.get_size()
-                if frame_size + queue_size >= self.mtu_size:
-                    self.send_queue()
-                self.queue.frames.append(packet)
-
-    def send_ack_queue(self):
-        if len(self.ack_queue) > 0:
-            packet = Ack()
-            packet.sequence_numbers = self.ack_queue
-            self.ack_queue = []
-            packet.encode()
-            self.send_data(packet.getvalue())
-
-    def send_nack_queue(self):
-        if len(self.nack_queue) > 0:
-            packet = Nack()
-            packet.sequence_numbers = self.nack_queue
-            self.nack_queue = []
-            packet.encode()
-            self.send_data(packet.getvalue())
-
-    def disconnect(self):
-        new_frame = Frame()
-        new_frame.reliability = 0
-        disconnect_packet = Disconnect()
-        disconnect_packet.encode()
-        new_frame.body = disconnect_packet.getvalue()
-        self.add_to_queue(new_frame)
-        self.server.remove_connection(self.address)
-        if hasattr(self.server, "interface"):
-            if hasattr(self.server.interface, "on_disconnect"):
-                self.server.interface.on_disconnect(self)
+import time
+from pieraknet.packets.frame_set import FrameSet, Frame
+from pieraknet.protocol_info import ProtocolInfo
+from pieraknet.packets.acknowledgement import Ack, Nack
+from pieraknet.handlers.connection_request import ConnectionRequestHandler
+from pieraknet.handlers.online_ping import OnlinePingHandler
+from pieraknet.packets.online_ping import OnlinePing
+from pieraknet.packets.new_incoming_connection import NewIncomingConnection
+from pieraknet.packets.disconnect import Disconnect
+
+
+class Connection:
+    def __init__(self, address, server, mtu_size, guid):
+        self.address = address
+        self.mtu_size = mtu_size
+        self.server = server
+        self.guid = guid
+        self.connected = False
+        self.recovery_queue = {}
+        self.ack_queue = []
+        self.nack_queue = []
+        self.fragmented_packets = {}
+        self.compound_id = 0
+        self.client_sequence_numbers = []
+        # self.server_sequence_numbers = []
+        self.client_sequence_number = 0
+        self.server_sequence_number = 0
+        self.queue = FrameSet()
+        self.server_reliable_frame_index = 0
+        self.client_reliable_frame_index = 0
+        self.channel_index = [0] * 32
+        self.last_receive_time = time.time()
+
+    def update(self):
+        if (time.time() - self.last_receive_time) >= self.server.timeout:
+            self.disconnect()
+        self.send_ack_queue()
+        self.send_nack_queue()
+        self.send_queue()
+
+    def send_data(self, data: bytes):
+        self.server.send(data, self.address)
+
+    def handle(self, data):
+        self.last_receive_time = time.time()
+        if data[0] == ProtocolInfo.ACK:
+            self.handle_ack(data)
+        elif data[0] == ProtocolInfo.NACK:
+            self.handle_nack(data)
+        elif ProtocolInfo.FRAME_SET_0 <= data[0] <= ProtocolInfo.FRAME_SET_F:
+            self.handle_frame_set(data)
+
+    def handle_ack(self, data: bytes):
+        packet = Ack(data)
+        packet.decode()
+        for sequence_number in packet.sequence_numbers:
+            if sequence_number in self.recovery_queue:
+                del self.recovery_queue[sequence_number]
+
+    def handle_nack(self, data: bytes):
+        packet = Nack(data)
+        packet.decode()
+        for sequence_number in packet.sequence_numbers:
+            if sequence_number in self.recovery_queue:
+                lost_packet = self.recovery_queue[sequence_number]
+                lost_packet.sequence_number = self.server_sequence_number
+                self.server_sequence_number += 1
+                lost_packet.encode()
+                self.send_data(lost_packet.data)
+                del self.recovery_queue[sequence_number]
+
+    def handle_frame_set(self, data: bytes):
+        packet = FrameSet(data)
+        packet.decode()
+        if packet.sequence_number not in self.client_sequence_numbers:
+            if packet.sequence_number in self.nack_queue:
+                self.nack_queue.remove(packet.sequence_number)
+            self.client_sequence_numbers.append(packet.sequence_number)
+            self.ack_queue.append(packet.sequence_number)
+            hole_size = packet.sequence_number - self.client_sequence_number
+            if hole_size > 0:
+                for sequence_number in range(self.client_sequence_number + 1, hole_size):
+                    if sequence_number not in self.client_sequence_numbers:
+                        self.nack_queue.append(sequence_number)
+            self.client_sequence_number: int = packet.sequence_number
+            for frame in packet.frames:
+                if not (2 <= frame.reliability <= 7 and frame.reliability != 5):
+                    self.handle_frame(frame)
+                else:
+                    hole_size = frame.reliable_frame_index - self.client_reliable_frame_index
+                    if hole_size == 0:
+                        self.handle_frame(frame)
+                        self.client_reliable_frame_index += 1
+
+    def handle_fragmented_frame(self, packet):
+        if packet.compound_id not in self.fragmented_packets:
+            self.fragmented_packets[packet.compound_id] = {packet.index: packet}
+        else:
+            self.fragmented_packets[packet.compound_id][packet.index] = packet
+        if len(self.fragmented_packets[packet.compound_id]) == packet.compound_size:
+            new_frame = Frame()
+            new_frame.body = b''
+            for i in range(0, packet.compound_size):
+                new_frame.body += self.fragmented_packets[packet.compound_id][i].body
+            del self.fragmented_packets[packet.compound_id]
+            self.handle_frame(new_frame)
+
+    def handle_frame(self, packet):
+        if packet.fragmented:
+            self.handle_fragmented_frame(packet)
+        else:
+            if not self.connected:
+                if packet.body[0] == ProtocolInfo.CONNECTION_REQUEST:
+                    new_frame = Frame()
+                    new_frame.reliability = 0
+                    new_frame.body = ConnectionRequestHandler.handle(packet.body, self.server, self)
+                    self.add_to_queue(new_frame)
+                elif packet.body[0] == ProtocolInfo.NEW_INCOMING_CONNECTION:
+                    packet = NewIncomingConnection(packet.body)
+                    packet.decode()
+                    if packet.server_address[1] == self.server.port:
+                        self.connected = True
+                        if hasattr(self.server, "interface"):
+                            if hasattr(self.server.interface, "on_new_incoming_connection"):
+                                self.server.interface.on_new_incoming_connection(self)
+            elif packet.body[0] == ProtocolInfo.ONLINE_PING:
+                new_frame = Frame()
+                new_frame.reliability = 0
+                new_frame.body = OnlinePingHandler.handle(OnlinePing(packet.body), self, self.server)
+                self.add_to_queue(new_frame, False)
+            elif packet.body[0] == ProtocolInfo.DISCONNECT:
+                self.disconnect()
+            elif packet.body[0] == ProtocolInfo.GAME_PACKET:
+                if hasattr(self.server, "interface"):
+                    if hasattr(self.server.interface, "on_game_packet"):
+                        self.server.interface.on_game_packet(packet, self)
+            else:
+                if hasattr(self.server, "interface"):
+                    if hasattr(self.server.interface, "on_unknown_packet"):
+                        self.server.interface.on_unknown_packet(packet, self)
+
+    def send_queue(self):
+        if len(self.queue.frames) > 0:
+            self.queue.sequence_number = self.server_sequence_number
+            self.server_sequence_number += 1
+            self.recovery_queue[self.queue.sequence_number] = self.queue
+            self.queue.encode()
+            self.send_data(self.queue.getvalue())
+            self.queue = FrameSet()
+
+    def add_to_queue(self, packet: Frame, is_immediate=True):
+        if 2 <= packet.reliability <= 7 and packet.reliability != 5:
+            packet.reliable_frame_index = self.server_reliable_frame_index
+            self.server_reliable_frame_index += 1
+            if packet.reliability == 3:
+                packet.ordered_frame_index = self.channel_index[packet.order_channel]
+                self.channel_index[packet.order_channel] += 1
+        if packet.get_size() > self.mtu_size:
+            fragmented_body = []
+            for i in range(0, len(packet.body), self.mtu_size):
+                fragmented_body.append(packet.body[i:i + self.mtu_size])
+            for index, body in enumerate(fragmented_body):
+                new_packet = Frame()
+                new_packet.fragmented = True
+                new_packet.reliability = packet.reliability
+                new_packet.compound_id = self.compound_id
+                new_packet.compound_size = len(fragmented_body)
+                new_packet.index = index
+                new_packet.body = body
+                if index != 0:
+                    new_packet.reliable_frame_index = self.server_reliable_frame_index
+                    self.server_reliable_frame_index += 1
+                if new_packet.reliability == 3:
+                    new_packet.ordered_frame_index = packet.ordered_frame_index
+                    new_packet.order_channel = packet.order_channel
+                if is_immediate:
+                    self.queue.frames.append(new_packet)
+                    self.send_queue()
+                else:
+                    frame_size: int = new_packet.get_size()
+                    queue_size: int = self.queue.get_size()
+                    if frame_size + queue_size >= self.mtu_size:
+                        self.send_queue()
+                    self.queue.frames.append(new_packet)
+            self.compound_id += 1
+        else:
+            if is_immediate:
+                self.queue.frames.append(packet)
+                self.send_queue()
+            else:
+                frame_size: int = packet.get_size()
+                queue_size: int = self.queue.get_size()
+                if frame_size + queue_size >= self.mtu_size:
+                    self.send_queue()
+                self.queue.frames.append(packet)
+
+    def send_ack_queue(self):
+        if len(self.ack_queue) > 0:
+            packet = Ack()
+            packet.sequence_numbers = self.ack_queue
+            self.ack_queue = []
+            packet.encode()
+            self.send_data(packet.getvalue())
+
+    def send_nack_queue(self):
+        if len(self.nack_queue) > 0:
+            packet = Nack()
+            packet.sequence_numbers = self.nack_queue
+            self.nack_queue = []
+            packet.encode()
+            self.send_data(packet.getvalue())
+
+    def disconnect(self):
+        new_frame = Frame()
+        new_frame.reliability = 0
+        disconnect_packet = Disconnect()
+        disconnect_packet.encode()
+        new_frame.body = disconnect_packet.getvalue()
+        self.add_to_queue(new_frame)
+        self.server.remove_connection(self.address)
+        if hasattr(self.server, "interface"):
+            if hasattr(self.server.interface, "on_disconnect"):
+                self.server.interface.on_disconnect(self)
```

### Comparing `PieRakNet-1.0.4/pieraknet/handlers/connection_request.py` & `PieRakNet-1.0.5/pieraknet/handlers/connection_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,18 @@
-import time
-from pieraknet.packets.connection_request import ConnectionRequest
-from pieraknet.packets.connection_request_accepted import ConnectionRequestAccepted
-
-
-class ConnectionRequestHandler:
-    @staticmethod
-    def handle(packet: ConnectionRequest, server, connection):
-        packet.decode()
-        new_packet = ConnectionRequestAccepted()
-        new_packet.client_address = connection.address
-        new_packet.system_index = 0
-        new_packet.internal_ids = [('255.255.255.255', 19132)] * 10
-        new_packet.request_time = packet.client_timestamp
-        new_packet.accepted_time = int(time.time())
-        new_packet.encode()
-        return new_packet.getvalue()
+import time
+from pieraknet.packets.connection_request import ConnectionRequest
+from pieraknet.packets.connection_request_accepted import ConnectionRequestAccepted
+
+
+class ConnectionRequestHandler:
+    @staticmethod
+    def handle(packet: bytes, server, connection):
+        packet = ConnectionRequest(packet)
+        packet.decode()
+        new_packet = ConnectionRequestAccepted()
+        new_packet.client_address = connection.address
+        new_packet.system_index = 0
+        new_packet.internal_ids = [('255.255.255.255', 19132)] * 10
+        new_packet.request_time = packet.client_timestamp
+        new_packet.accepted_time = int(time.time())
+        new_packet.encode()
+        return new_packet.getvalue()
```

### Comparing `PieRakNet-1.0.4/pieraknet/handlers/offline_ping.py` & `PieRakNet-1.0.5/pieraknet/handlers/offline_ping.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-from pieraknet.packets.offline_ping import OfflinePing
-from pieraknet.packets.offline_pong import OfflinePong
-
-
-class OfflinePingHandler:
-    @staticmethod
-    def handle(packet: OfflinePing, server, address: tuple):
-        packet.decode()
-        server.logger.debug("New Packet:")
-        server.logger.debug(f"- Packet ID: {str(packet.getvalue()[0])}")
-        server.logger.debug(f"- Packet Body: {str(packet.getvalue()[1:])}")
-        server.logger.debug(f"- Packet Name: Offline Ping")
-        server.logger.debug(f"- Client Timestamp: {str(packet.client_timestamp)}")
-        server.logger.debug(f"- MAGIC: {str(packet.magic)}")
-        server.logger.debug(f"- Client GUID: {str(packet.client_guid)}")
-        new_packet = OfflinePong()
-        new_packet.client_timestamp = packet.client_timestamp
-        new_packet.server_guid = server.guid
-        new_packet.magic = packet.magic  # TODO: server.magic
-        new_packet.server_name = server.name
-        new_packet.encode()
-        server.send(new_packet.getvalue(), address)
-        server.logger.debug("Sent Packet:")
-        server.logger.debug(f"- Packet ID: {str(new_packet.getvalue()[0])}")
-        server.logger.debug(f"- Packet Body: {str(new_packet.getvalue()[1:])}")
-        server.logger.debug(f"- Packet Name: Offline Pong")
-        server.logger.debug(f"- Client Timestamp: {str(new_packet.client_timestamp)}")
-        server.logger.debug(f"- Server GUID: {str(new_packet.server_guid)}")
-        server.logger.debug(f"- MAGIC: {str(new_packet.magic)}")
-        server.logger.debug(f"- Server Name: {str(new_packet.server_name)}")
+from pieraknet.packets.offline_ping import OfflinePing
+from pieraknet.packets.offline_pong import OfflinePong
+
+
+class OfflinePingHandler:
+    @staticmethod
+    def handle(packet: OfflinePing, server, address: tuple):
+        packet.decode()
+        server.logger.debug("New Packet:")
+        server.logger.debug(f"- Packet ID: {str(packet.getvalue()[0])}")
+        server.logger.debug(f"- Packet Body: {str(packet.getvalue()[1:])}")
+        server.logger.debug(f"- Packet Name: Offline Ping")
+        server.logger.debug(f"- Client Timestamp: {str(packet.client_timestamp)}")
+        server.logger.debug(f"- MAGIC: {str(packet.magic)}")
+        server.logger.debug(f"- Client GUID: {str(packet.client_guid)}")
+        new_packet = OfflinePong()
+        new_packet.client_timestamp = packet.client_timestamp
+        new_packet.server_guid = server.guid
+        new_packet.magic = packet.magic  # TODO: server.magic
+        new_packet.server_name = server.name
+        new_packet.encode()
+        server.send(new_packet.getvalue(), address)
+        server.logger.debug("Sent Packet:")
+        server.logger.debug(f"- Packet ID: {str(new_packet.getvalue()[0])}")
+        server.logger.debug(f"- Packet Body: {str(new_packet.getvalue()[1:])}")
+        server.logger.debug(f"- Packet Name: Offline Pong")
+        server.logger.debug(f"- Client Timestamp: {str(new_packet.client_timestamp)}")
+        server.logger.debug(f"- Server GUID: {str(new_packet.server_guid)}")
+        server.logger.debug(f"- MAGIC: {str(new_packet.magic)}")
+        server.logger.debug(f"- Server Name: {str(new_packet.server_name)}")
```

### Comparing `PieRakNet-1.0.4/pieraknet/handlers/open_connection_request_1.py` & `PieRakNet-1.0.5/pieraknet/handlers/open_connection_request_1.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,45 +1,45 @@
-from pieraknet.packets.open_connection_request_1 import OpenConnectionRequest1
-from pieraknet.packets.open_connection_reply_1 import OpenConnectionReply1
-from pieraknet.packets.incompatible_protocol import IncompatibleProtocol
-
-
-class OpenConnectionRequest1Handler:
-    @staticmethod
-    def handle(packet: OpenConnectionRequest1, server, address: tuple):
-        packet.decode()
-        server.logger.debug("New Packet:")
-        server.logger.debug(f"- Packet ID: {str(packet.getvalue()[0])}")
-        server.logger.debug(f"- Packet Body: {str(packet.getvalue()[1:])}")
-        server.logger.debug(f"- Packet Name: Open Connection Request 1")
-        server.logger.debug(f"- MAGIC: {str(packet.magic)}")
-        server.logger.debug(f"- Protocol Version: {str(packet.protocol_version)}")
-        server.logger.debug(f"- MTU size: {str(packet.mtu_size)}")
-        if packet.protocol_version == server.protocol_version:
-            new_packet = OpenConnectionReply1()
-            new_packet.magic = packet.magic
-            new_packet.server_guid = server.guid
-            new_packet.use_security = False
-            new_packet.mtu_size = packet.mtu_size
-        else:
-            new_packet = IncompatibleProtocol()
-            new_packet.protocol_version = server.protocol_version
-            new_packet.magic = packet.magic  # TODO: server.magic
-            new_packet.server_guid = server.guid
-        new_packet.encode()
-        server.send(new_packet.getvalue(), address)
-        server.logger.debug("Sent Packet:")
-        server.logger.debug(f"- Packet ID: {str(new_packet.getvalue()[0])}")
-        server.logger.debug(f"- Packet Body: {str(new_packet.getvalue()[1:])}")
-        if new_packet.packet_type == 'open_connection_reply_1':
-            server.logger.debug(f"- Packet Name: Open Connection Reply 1")
-            server.logger.debug(f"- MAGIC: {str(new_packet.magic)}")
-            server.logger.debug(f"- Server GUID: {str(new_packet.server_guid)}")
-            server.logger.debug(f"- Use Security: {str(new_packet.use_security)}")
-            server.logger.debug(f"- MTU Size: {str(new_packet.mtu_size)}")
-        elif new_packet.packet_type == 'incompatible_protocol':
-            server.logger.debug(f"- Packet Name: Incompatible Protocol")
-            server.logger.debug(f"- Protocol Version: {str(new_packet.magic)}")
-            server.logger.debug(f"- MAGIC: {str(new_packet.magic)}")
-            server.logger.debug(f"- Server: {str(new_packet.magic)}")
-        else:
-            server.logger.critical(f"WTF?! Error: OCR1H - Invalid Sent Packet Type ({str(new_packet.packet_type)}).")
+from pieraknet.packets.open_connection_request_1 import OpenConnectionRequest1
+from pieraknet.packets.open_connection_reply_1 import OpenConnectionReply1
+from pieraknet.packets.incompatible_protocol import IncompatibleProtocol
+
+
+class OpenConnectionRequest1Handler:
+    @staticmethod
+    def handle(packet: OpenConnectionRequest1, server, address: tuple):
+        packet.decode()
+        server.logger.debug("New Packet:")
+        server.logger.debug(f"- Packet ID: {str(packet.getvalue()[0])}")
+        server.logger.debug(f"- Packet Body: {str(packet.getvalue()[1:])}")
+        server.logger.debug(f"- Packet Name: Open Connection Request 1")
+        server.logger.debug(f"- MAGIC: {str(packet.magic)}")
+        server.logger.debug(f"- Protocol Version: {str(packet.protocol_version)}")
+        server.logger.debug(f"- MTU size: {str(packet.mtu_size)}")
+        if packet.protocol_version == server.protocol_version:
+            new_packet = OpenConnectionReply1()
+            new_packet.magic = packet.magic
+            new_packet.server_guid = server.guid
+            new_packet.use_security = False
+            new_packet.mtu_size = packet.mtu_size
+        else:
+            new_packet = IncompatibleProtocol()
+            new_packet.protocol_version = server.protocol_version
+            new_packet.magic = packet.magic  # TODO: server.magic
+            new_packet.server_guid = server.guid
+        new_packet.encode()
+        server.send(new_packet.getvalue(), address)
+        server.logger.debug("Sent Packet:")
+        server.logger.debug(f"- Packet ID: {str(new_packet.getvalue()[0])}")
+        server.logger.debug(f"- Packet Body: {str(new_packet.getvalue()[1:])}")
+        if new_packet.packet_type == 'open_connection_reply_1':
+            server.logger.debug(f"- Packet Name: Open Connection Reply 1")
+            server.logger.debug(f"- MAGIC: {str(new_packet.magic)}")
+            server.logger.debug(f"- Server GUID: {str(new_packet.server_guid)}")
+            server.logger.debug(f"- Use Security: {str(new_packet.use_security)}")
+            server.logger.debug(f"- MTU Size: {str(new_packet.mtu_size)}")
+        elif new_packet.packet_type == 'incompatible_protocol':
+            server.logger.debug(f"- Packet Name: Incompatible Protocol")
+            server.logger.debug(f"- Protocol Version: {str(new_packet.magic)}")
+            server.logger.debug(f"- MAGIC: {str(new_packet.magic)}")
+            server.logger.debug(f"- Server: {str(new_packet.magic)}")
+        else:
+            server.logger.critical(f"WTF?! Error: OCR1H - Invalid Sent Packet Type ({str(new_packet.packet_type)}).")
```

### Comparing `PieRakNet-1.0.4/pieraknet/handlers/open_connection_request_2.py` & `PieRakNet-1.0.5/pieraknet/handlers/open_connection_request_2.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from pieraknet.packets.open_connection_request_2 import OpenConnectionRequest2
-from pieraknet.packets.open_connection_reply_2 import OpenConnectionReply2
-from pieraknet.connection import Connection
-
-
-class OpenConnectionRequest2Handler:
-    @staticmethod
-    def handle(packet: OpenConnectionRequest2, server, address: tuple):
-        packet.decode()
-        server.logger.debug("New Packet:")
-        server.logger.debug(f"- Packet ID: {str(packet.getvalue()[0])}")
-        server.logger.debug(f"- Packet Body: {str(packet.getvalue()[1:])}")
-        server.logger.debug(f"- Packet Name: Open Connection Request 2")
-        server.logger.debug(f"- MAGIC: {str(packet.magic)}")
-        server.logger.debug(f"- Server Address: {str(packet.server_address)}")
-        server.logger.debug(f"- MTU Size: {str(packet.mtu_size)}")
-        server.logger.debug(f"- Client GUID: {str(packet.client_guid)}")
-
-        new_packet = OpenConnectionReply2()
-        new_packet.magic = packet.magic  # TODO: server.magic
-        new_packet.server_guid = server.guid
-        new_packet.client_address = address
-        new_packet.mtu_size = packet.mtu_size
-        new_packet.encode()
-
-        server.send(new_packet.getvalue(), address)
-
-        server.logger.debug("Sent Packet:")
-        server.logger.debug(f"- Packet ID: {str(new_packet.getvalue()[0])}")
-        server.logger.debug(f"- Packet Body: {str(new_packet.getvalue()[1:])}")
-        server.logger.debug(f"- Packet Name: Open Connection Reply 2")
-        server.logger.debug(f"- MAGIC: {str(new_packet.magic)}")
-        server.logger.debug(f"- Server GUID: {str(new_packet.server_guid)}")
-        server.logger.debug(f"- Client Address: {str(new_packet.client_address)}")
-        server.logger.debug(f"- MTU Size: {str(new_packet.mtu_size)}")
-
-        connection = Connection(address, server, packet.mtu_size, packet.client_guid)
-        server.add_connection(connection)
+from pieraknet.packets.open_connection_request_2 import OpenConnectionRequest2
+from pieraknet.packets.open_connection_reply_2 import OpenConnectionReply2
+from pieraknet.connection import Connection
+
+
+class OpenConnectionRequest2Handler:
+    @staticmethod
+    def handle(packet: OpenConnectionRequest2, server, address: tuple):
+        packet.decode()
+        server.logger.debug("New Packet:")
+        server.logger.debug(f"- Packet ID: {str(packet.getvalue()[0])}")
+        server.logger.debug(f"- Packet Body: {str(packet.getvalue()[1:])}")
+        server.logger.debug(f"- Packet Name: Open Connection Request 2")
+        server.logger.debug(f"- MAGIC: {str(packet.magic)}")
+        server.logger.debug(f"- Server Address: {str(packet.server_address)}")
+        server.logger.debug(f"- MTU Size: {str(packet.mtu_size)}")
+        server.logger.debug(f"- Client GUID: {str(packet.client_guid)}")
+
+        new_packet = OpenConnectionReply2()
+        new_packet.magic = packet.magic  # TODO: server.magic
+        new_packet.server_guid = server.guid
+        new_packet.client_address = address
+        new_packet.mtu_size = packet.mtu_size
+        new_packet.encode()
+
+        server.send(new_packet.getvalue(), address)
+
+        server.logger.debug("Sent Packet:")
+        server.logger.debug(f"- Packet ID: {str(new_packet.getvalue()[0])}")
+        server.logger.debug(f"- Packet Body: {str(new_packet.getvalue()[1:])}")
+        server.logger.debug(f"- Packet Name: Open Connection Reply 2")
+        server.logger.debug(f"- MAGIC: {str(new_packet.magic)}")
+        server.logger.debug(f"- Server GUID: {str(new_packet.server_guid)}")
+        server.logger.debug(f"- Client Address: {str(new_packet.client_address)}")
+        server.logger.debug(f"- MTU Size: {str(new_packet.mtu_size)}")
+
+        connection = Connection(address, server, packet.mtu_size, packet.client_guid)
+        server.add_connection(connection)
```

### Comparing `PieRakNet-1.0.4/pieraknet/packets/acknowledgement.py` & `PieRakNet-1.0.5/pieraknet/packets/acknowledgement.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-from pieraknet.packets.packet import Packet
-from pieraknet.buffer import Buffer
-from pieraknet.protocol_info import ProtocolInfo
-
-
-class Acknowledgement(Packet):
-    def __init__(self, data: bytes = b''):
-        super().__init__(data)
-        self.sequence_numbers: list[int] = []
-
-    def decode_payload(self) -> None:
-        self.sequence_numbers.clear()
-        count: int = self.read_short()
-        for i in range(0, count):
-            single: bool = self.read_bool()
-            if not single:
-                index: int = self.read_uint24le()
-                end_index: int = self.read_uint24le()
-                while index <= end_index:
-                    self.sequence_numbers.append(index)
-                    index += 1
-            else:
-                self.sequence_numbers.append(self.read_uint24le())
-
-    def encode_payload(self) -> None:
-        self.sequence_numbers.sort()
-        temp_buffer: Buffer = Buffer()
-        count: int = 0
-        if len(self.sequence_numbers) > 0:
-            start_index: int = self.sequence_numbers[0]
-            end_index: int = self.sequence_numbers[0]
-            for pointer in range(1, len(self.sequence_numbers)):
-                current_index: int = self.sequence_numbers[pointer]
-                diff: int = current_index - end_index
-                if diff == 1:
-                    end_index: int = current_index
-                elif diff > 1:
-                    if start_index == end_index:
-                        temp_buffer.write_bool(True)
-                        temp_buffer.write_uint24le(start_index)
-                        start_index = end_index = current_index
-                    else:
-                        temp_buffer.write_bool(False)
-                        temp_buffer.write_uint24le(start_index)
-                        temp_buffer.write_uint24le(end_index)
-                        start_index = end_index = current_index
-                    count += 1
-            if start_index == end_index:
-                temp_buffer.write_bool(True)
-                temp_buffer.write_uint24le(start_index)
-            else:
-                temp_buffer.write_bool(False)
-                temp_buffer.write_uint24le(start_index)
-                temp_buffer.write_uint24le(end_index)
-            count += 1
-            self.write_short(count)
-            self.write(temp_buffer.getvalue())
-
-
-class Nack(Acknowledgement):
-    packet_id = ProtocolInfo.NACK
-
-
-class Ack(Acknowledgement):
-    packet_id = ProtocolInfo.NACK
+from pieraknet.packets.packet import Packet
+from pieraknet.buffer import Buffer
+from pieraknet.protocol_info import ProtocolInfo
+
+
+class Acknowledgement(Packet):
+    def __init__(self, data: bytes = b''):
+        super().__init__(data)
+        self.sequence_numbers: list[int] = []
+
+    def decode_payload(self) -> None:
+        self.sequence_numbers.clear()
+        count: int = self.read_short()
+        for i in range(0, count):
+            single: bool = self.read_bool()
+            if not single:
+                index: int = self.read_uint24le()
+                end_index: int = self.read_uint24le()
+                while index <= end_index:
+                    self.sequence_numbers.append(index)
+                    index += 1
+            else:
+                self.sequence_numbers.append(self.read_uint24le())
+
+    def encode_payload(self) -> None:
+        self.sequence_numbers.sort()
+        temp_buffer: Buffer = Buffer()
+        count: int = 0
+        if len(self.sequence_numbers) > 0:
+            start_index: int = self.sequence_numbers[0]
+            end_index: int = self.sequence_numbers[0]
+            for pointer in range(1, len(self.sequence_numbers)):
+                current_index: int = self.sequence_numbers[pointer]
+                diff: int = current_index - end_index
+                if diff == 1:
+                    end_index: int = current_index
+                elif diff > 1:
+                    if start_index == end_index:
+                        temp_buffer.write_bool(True)
+                        temp_buffer.write_uint24le(start_index)
+                        start_index = end_index = current_index
+                    else:
+                        temp_buffer.write_bool(False)
+                        temp_buffer.write_uint24le(start_index)
+                        temp_buffer.write_uint24le(end_index)
+                        start_index = end_index = current_index
+                    count += 1
+            if start_index == end_index:
+                temp_buffer.write_bool(True)
+                temp_buffer.write_uint24le(start_index)
+            else:
+                temp_buffer.write_bool(False)
+                temp_buffer.write_uint24le(start_index)
+                temp_buffer.write_uint24le(end_index)
+            count += 1
+            self.write_short(count)
+            self.write(temp_buffer.getvalue())
+
+
+class Nack(Acknowledgement):
+    packet_id = ProtocolInfo.NACK
+
+
+class Ack(Acknowledgement):
+    packet_id = ProtocolInfo.NACK
```

### Comparing `PieRakNet-1.0.4/pieraknet/packets/connection_request_accepted.py` & `PieRakNet-1.0.5/pieraknet/packets/connection_request_accepted.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from pieraknet.packets.packet import Packet
-
-
-class ConnectionRequestAccepted(Packet):
-    packet_id = 0x10
-    packet_type = 'connection_request_accepted'
-
-    client_address: tuple = None
-    system_index: int = None
-    internal_ids: list[tuple] = None
-    request_time: int = None
-    accepted_time: int = None
-
-    def encode_payload(self):
-        self.write_address(self.client_address)
-        self.write_short(self.system_index)
-        for address in self.internal_ids:
-            self.write_address(address)
-        self.write_long(self.request_time)
-        self.write_long(self.accepted_time)
+from pieraknet.packets.packet import Packet
+
+
+class ConnectionRequestAccepted(Packet):
+    packet_id = 0x10
+    packet_type = 'connection_request_accepted'
+
+    client_address: tuple = None
+    system_index: int = None
+    internal_ids: list[tuple] = None
+    request_time: int = None
+    accepted_time: int = None
+
+    def encode_payload(self):
+        self.write_address(self.client_address)
+        self.write_short(self.system_index)
+        for address in self.internal_ids:
+            self.write_address(address)
+        self.write_long(self.request_time)
+        self.write_long(self.accepted_time)
```

### Comparing `PieRakNet-1.0.4/pieraknet/packets/frame_set.py` & `PieRakNet-1.0.5/pieraknet/packets/frame_set.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,88 +1,88 @@
-from pieraknet.packets.packet import Packet
-from pieraknet.buffer import Buffer
-from io import SEEK_CUR
-
-
-class Frame(Buffer):
-    reliability: int = None
-    fragmented: bool = None
-    reliable_frame_index: int = None
-    sequenced_frame_index: int = None
-    ordered_frame_index: int = None
-    order_channel: int = None
-    compound_size: int = None
-    compound_id: int = None
-    index: int = None
-    body: bytes = None
-
-    def decode(self):
-        flags: int = self.read_byte()
-        self.reliability = (flags & 0xf4) >> 5
-        self.fragmented = (flags & 0x10) > 0
-        body_length: int = self.read_unsigned_short() >> 3
-        if 2 <= self.reliability <= 7 and self.reliability != 5:
-            self.reliable_frame_index = self.read_uint24le()
-        if self.reliability == 1 or self.reliability == 4:
-            self.sequenced_frame_index = self.read_uint24le()
-        if self.reliability == 3 or self.reliability == 7:
-            self.ordered_frame_index = self.read_uint24le()
-            self.order_channel = self.read_byte()
-        if self.fragmented:
-            self.compound_size = self.read_int()
-            self.compound_id = self.read_short()
-            self.index = self.read_int()
-        self.body = self.read(body_length)
-
-    def encode(self):
-        self.write_byte((self.reliability << 5) | (0x10 if self.fragmented else 0))
-        self.write_unsigned_short(len(self.body) << 3)
-        if 2 <= self.reliability <= 7 and self.reliability != 5:
-            self.write_uint24le(self.reliable_frame_index)
-        if self.reliability == 1 or self.reliability == 4:
-            self.write_uint24le(self.sequenced_frame_index)
-        if self.reliability == 3 or self.reliability == 7:
-            self.write_uint24le(self.ordered_frame_index)
-            self.write_byte(self.order_channel)
-        if self.fragmented:
-            self.write_int(self.compound_size)
-            self.write_short(self.compound_id)
-            self.write_int(self.index)
-        self.write_uint24le(self.body)
-
-    def get_size(self):
-        length: int = 3
-        if 2 <= self.reliability <= 7 and self.reliability != 5:
-            length += 3
-        if self.reliability == 1 or self.reliability == 4:
-            length += 3
-        if self.reliability == 3 or self.reliability == 7:
-            length += 4
-        if self.fragmented:
-            length += 10
-        return length
-
-
-class FrameSet(Packet):
-    packet_id = 0x80
-    sequence_number: int = None
-    frames: list[Frame] = []
-
-    def decode_payload(self):
-        self.sequence_number = self.read_uint24le()
-        while not self.feos():
-            frame: Frame = Frame(bytes(self.getbuffer())[self.tell():])
-            frame.decode()
-            self.frames.append(frame)
-            self.seek(frame.get_size(), SEEK_CUR)
-
-    def encode_payload(self):
-        self.write_uint24le(self.sequence_number)
-        for frame in self.frames:
-            frame.encode()
-            self.write(bytes(frame.getvalue()))
-
-    def get_size(self):
-        length: int = 4
-        for frame in self.frames:
-            length += frame.get_size()
-        return length
+from pieraknet.packets.packet import Packet
+from pieraknet.buffer import Buffer
+from io import SEEK_CUR
+
+
+class Frame(Buffer):
+    reliability: int = None
+    fragmented: bool = None
+    reliable_frame_index: int = None
+    sequenced_frame_index: int = None
+    ordered_frame_index: int = None
+    order_channel: int = None
+    compound_size: int = None
+    compound_id: int = None
+    index: int = None
+    body: bytes = None
+
+    def decode(self):
+        flags: int = self.read_byte()
+        self.reliability = (flags & 0xf4) >> 5
+        self.fragmented = (flags & 0x10) > 0
+        body_length: int = self.read_unsigned_short() >> 3
+        if 2 <= self.reliability <= 7 and self.reliability != 5:
+            self.reliable_frame_index = self.read_uint24le()
+        if self.reliability == 1 or self.reliability == 4:
+            self.sequenced_frame_index = self.read_uint24le()
+        if self.reliability == 3 or self.reliability == 7:
+            self.ordered_frame_index = self.read_uint24le()
+            self.order_channel = self.read_byte()
+        if self.fragmented:
+            self.compound_size = self.read_int()
+            self.compound_id = self.read_short()
+            self.index = self.read_int()
+        self.body = self.read(body_length)
+
+    def encode(self):
+        self.write_byte((self.reliability << 5) | (0x10 if self.fragmented else 0))
+        self.write_unsigned_short(len(self.body) << 3)
+        if 2 <= self.reliability <= 7 and self.reliability != 5:
+            self.write_uint24le(self.reliable_frame_index)
+        if self.reliability == 1 or self.reliability == 4:
+            self.write_uint24le(self.sequenced_frame_index)
+        if self.reliability == 3 or self.reliability == 7:
+            self.write_uint24le(self.ordered_frame_index)
+            self.write_byte(self.order_channel)
+        if self.fragmented:
+            self.write_int(self.compound_size)
+            self.write_short(self.compound_id)
+            self.write_int(self.index)
+        self.write_uint24le(self.body)
+
+    def get_size(self):
+        length: int = 3
+        if 2 <= self.reliability <= 7 and self.reliability != 5:
+            length += 3
+        if self.reliability == 1 or self.reliability == 4:
+            length += 3
+        if self.reliability == 3 or self.reliability == 7:
+            length += 4
+        if self.fragmented:
+            length += 10
+        return length
+
+
+class FrameSet(Packet):
+    packet_id = 0x80
+    sequence_number: int = None
+    frames: list[Frame] = []
+
+    def decode_payload(self):
+        self.sequence_number = self.read_uint24le()
+        while not self.feos():
+            frame: Frame = Frame(bytes(self.getbuffer())[self.tell():])
+            frame.decode()
+            self.frames.append(frame)
+            self.seek(frame.get_size(), SEEK_CUR)
+
+    def encode_payload(self):
+        self.write_uint24le(self.sequence_number)
+        for frame in self.frames:
+            frame.encode()
+            self.write(bytes(frame.getvalue()))
+
+    def get_size(self):
+        length: int = 4
+        for frame in self.frames:
+            length += frame.get_size()
+        return length
```

### Comparing `PieRakNet-1.0.4/pieraknet/packets/open_connection_reply_2.py` & `PieRakNet-1.0.5/pieraknet/packets/open_connection_reply_2.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from pieraknet.packets.packet import Packet
-
-
-class OpenConnectionReply2(Packet):
-    packet_id = 0x08
-    packet_type = 'open_connection_reply_2'
-
-    magic: bytes = None
-    server_guid: int = None
-    client_address: tuple = None  # ('255.255.255.255', 19132)
-    mtu_size: int = None
-    encryption_enabled: bool = None
-
-    def encode_payload(self):
-        self.write_magic(self.magic)  # TODO: server.magic
-        self.write_long(self.server_guid)
-        self.write_address(self.client_address)
-        self.write_short(self.mtu_size)
-        self.write_bool(self.encryption_enabled)
+from pieraknet.packets.packet import Packet
+
+
+class OpenConnectionReply2(Packet):
+    packet_id = 0x08
+    packet_type = 'open_connection_reply_2'
+
+    magic: bytes = None
+    server_guid: int = None
+    client_address: tuple = None  # ('255.255.255.255', 19132)
+    mtu_size: int = None
+    encryption_enabled: bool = None
+
+    def encode_payload(self):
+        self.write_magic(self.magic)  # TODO: server.magic
+        self.write_long(self.server_guid)
+        self.write_address(self.client_address)
+        self.write_short(self.mtu_size)
+        self.write_bool(self.encryption_enabled)
```

### Comparing `PieRakNet-1.0.4/pieraknet/packets/packet.py` & `PieRakNet-1.0.5/pieraknet/packets/packet.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-from pieraknet.buffer import Buffer
-
-
-class Packet(Buffer):
-    packet_id: int = None
-    packet_type: int = None
-
-    def encode_header(self, data):
-        self.write_packet_id(data)
-
-    def decode_header(self):
-        return self.read_packet_id()
-
-    def encode(self):
-        self.encode_header(self.packet_id)
-        if hasattr(self, 'encode_payload'):
-            self.encode_payload()
-
-    def decode(self):
-        self.decode_header()
-        if hasattr(self, 'decode_payload'):
-            self.decode_payload()
+from pieraknet.buffer import Buffer
+
+
+class Packet(Buffer):
+    packet_id: int = None
+    packet_type: int = None
+
+    def encode_header(self, data):
+        self.write_packet_id(data)
+
+    def decode_header(self):
+        return self.read_packet_id()
+
+    def encode(self):
+        self.encode_header(self.packet_id)
+        if hasattr(self, 'encode_payload'):
+            self.encode_payload()
+
+    def decode(self):
+        self.decode_header()
+        if hasattr(self, 'decode_payload'):
+            self.decode_payload()
```

### Comparing `PieRakNet-1.0.4/pieraknet/protocol_info.py` & `PieRakNet-1.0.5/pieraknet/protocol_info.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-class ProtocolInfo:
-    ONLINE_PING = 0x00
-    OFFLINE_PING = 0x01
-    OFFLINE_PING_OPEN_CONNECTIONS = 0x02
-    ONLINE_PONG = 0x03
-    OFFLINE_PONG = 0x1c
-    OPEN_CONNECTION_REQUEST_1 = 0x05
-    OPEN_CONNECTION_REPLY_1 = 0x06
-    OPEN_CONNECTION_REQUEST_2 = 0x07
-    OPEN_CONNECTION_REPLY_2 = 0x08
-    CONNECTION_REQUEST = 0x09
-    CONNECTION_REQUEST_ACCEPTED = 0x10
-    NEW_INCOMING_CONNECTION = 0x13
-    DISCONNECT = 0x15
-    INCOMPATIBLE_PROTOCOL_VERSION = 0x19
-    FRAME_SET = 0x80
-    FRAME_SET_0 = 0x80
-    FRAME_SET_F = 0x8d
-    NACK = 0xa0
-    ACK = 0xc0
-    GAME_PACKET = 0xfe
+class ProtocolInfo:
+    ONLINE_PING = 0x00
+    OFFLINE_PING = 0x01
+    OFFLINE_PING_OPEN_CONNECTIONS = 0x02
+    ONLINE_PONG = 0x03
+    OFFLINE_PONG = 0x1c
+    OPEN_CONNECTION_REQUEST_1 = 0x05
+    OPEN_CONNECTION_REPLY_1 = 0x06
+    OPEN_CONNECTION_REQUEST_2 = 0x07
+    OPEN_CONNECTION_REPLY_2 = 0x08
+    CONNECTION_REQUEST = 0x09
+    CONNECTION_REQUEST_ACCEPTED = 0x10
+    NEW_INCOMING_CONNECTION = 0x13
+    DISCONNECT = 0x15
+    INCOMPATIBLE_PROTOCOL_VERSION = 0x19
+    FRAME_SET = 0x80
+    FRAME_SET_0 = 0x80
+    FRAME_SET_F = 0x8d
+    NACK = 0xa0
+    ACK = 0xc0
+    GAME_PACKET = 0xfe
```

### Comparing `PieRakNet-1.0.4/pieraknet/server.py` & `PieRakNet-1.0.5/pieraknet/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,93 @@
-import socket
-import random
-import sys
-import time
-import logging
-from pieraknet.protocol_info import ProtocolInfo
-from pieraknet.packets.offline_ping import OfflinePing
-from pieraknet.handlers.offline_ping import OfflinePingHandler
-from pieraknet.packets.open_connection_request_1 import OpenConnectionRequest1
-from pieraknet.handlers.open_connection_request_1 import OpenConnectionRequest1Handler
-from pieraknet.packets.open_connection_request_2 import OpenConnectionRequest2
-from pieraknet.handlers.open_connection_request_2 import OpenConnectionRequest2Handler
-
-
-class ConnectionNotFound(Exception):
-    pass
-
-
-class Server:
-    def __init__(self, hostname='0.0.0.0', port=19132, logger=logging.getLogger(__name__)):
-        self.logger = logger
-        self.start_time = round(time.time(), 2)
-        self.hostname = hostname
-        self.port = port
-        self.ipv = 4
-        self.name = ''
-        self.protocol_version = 11
-        self.guid = random.randint(0, sys.maxsize - 1)
-        self.connections = []
-        self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.SOL_UDP)
-        self.start_time = time.time()
-        self.maxsize = 4096
-        self.magic = b'\x00\xff\xff\x00\xfe\xfe\xfe\xfe\xfd\xfd\xfd\xfd\x12\x34\x56\x78'
-        self.running = False
-        self.timeout = 15
-        self.logger.info('Server initialized.')
-
-    def get_time_ms(self):
-        return round(time.time() - self.start_time, 4)
-
-    def send(self, data, address: tuple):
-        if not (data is bytes):
-            data = str(data)
-            data = data.encode()
-        self.socket.sendto(data, address)
-
-    def get_connection(self, address):
-        for connection in self.connections:
-            if connection.address == address:
-                return connection
-        raise ConnectionNotFound()
-
-    def add_connection(self, connection):
-        self.connections.append(connection)
-
-    def start(self):
-        self.running = True
-        self.socket.bind((self.hostname, self.port))
-        self.logger.info(f"Server started ({str(self.get_time_ms())}s).")
-        while self.running:
-            time.sleep(1 / 20)
-            try:
-                data, client = self.socket.recvfrom(self.maxsize)
-            except OSError:
-                pass
-            else:
-                if data[0] in [ProtocolInfo.OFFLINE_PING, ProtocolInfo.OFFLINE_PING_OPEN_CONNECTIONS]:
-                    packet: OfflinePing = OfflinePing(data)
-                    OfflinePingHandler.handle(packet, self, client)
-                elif data[0] == ProtocolInfo.OPEN_CONNECTION_REQUEST_1:
-                    packet: OpenConnectionRequest1 = OpenConnectionRequest1(data)
-                    OpenConnectionRequest1Handler.handle(packet, self, client)
-                elif data[0] == ProtocolInfo.OPEN_CONNECTION_REQUEST_2:
-                    packet: OpenConnectionRequest2 = OpenConnectionRequest2(data)
-                    OpenConnectionRequest2Handler.handle(packet, self, client)
-                elif ProtocolInfo.FRAME_SET_0 <= data[0] <= ProtocolInfo.FRAME_SET_F:
-                    connection = self.get_connection(client)
-                    connection.handle(data)
-
-    def stop(self):
-        self.running = False
-        self.socket.close()
-        self.logger.info('Server stopped.')
-
-
-if __name__ == '__main__':
-    server = Server()
-    server.name = 'MCPE;PieMC Server;589;1.20.0;2;20;13253860892328930865;Powered by PieMC;Survival;1;19132;19133;'
-    try:
-        server.start()
-    except KeyboardInterrupt:
-        server.logger.info('Stopping...')
-        server.stop()
+import socket
+import random
+import sys
+import time
+import logging
+from pieraknet.protocol_info import ProtocolInfo
+from pieraknet.packets.offline_ping import OfflinePing
+from pieraknet.handlers.offline_ping import OfflinePingHandler
+from pieraknet.packets.open_connection_request_1 import OpenConnectionRequest1
+from pieraknet.handlers.open_connection_request_1 import OpenConnectionRequest1Handler
+from pieraknet.packets.open_connection_request_2 import OpenConnectionRequest2
+from pieraknet.handlers.open_connection_request_2 import OpenConnectionRequest2Handler
+
+
+class ConnectionNotFound(Exception):
+    pass
+
+
+class Server:
+    def __init__(self, hostname='0.0.0.0', port=19132, logger=logging.getLogger(__name__)):
+        self.logger = logger
+        self.start_time = round(time.time(), 2)
+        self.hostname = hostname
+        self.port = port
+        self.ipv = 4
+        self.name = ''
+        self.protocol_version = 11
+        self.guid = random.randint(0, sys.maxsize - 1)
+        self.connections = []
+        self.socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.SOL_UDP)
+        self.start_time = time.time()
+        self.maxsize = 4096
+        self.magic = b'\x00\xff\xff\x00\xfe\xfe\xfe\xfe\xfd\xfd\xfd\xfd\x12\x34\x56\x78'
+        self.running = False
+        self.timeout = 15
+        self.logger.info('Server initialized.')
+
+    def get_time_ms(self):
+        return round(time.time() - self.start_time, 4)
+
+    def send(self, data, address: tuple):
+        if not (isinstance(data, bytes)):
+            data = str(data)
+            data = data.encode()
+        self.socket.sendto(data, address)
+
+    def get_connection(self, address):
+        for connection in self.connections:
+            if connection.address == address:
+                return connection
+        raise ConnectionNotFound()
+
+    def add_connection(self, connection):
+        self.connections.append(connection)
+
+    def start(self):
+        self.running = True
+        self.socket.bind((self.hostname, self.port))
+        self.logger.info(f"Server started ({str(self.get_time_ms())}s).")
+        while self.running:
+            time.sleep(1 / 20)
+            try:
+                data, client = self.socket.recvfrom(self.maxsize)
+            except OSError:
+                pass
+            else:
+                if data[0] in [ProtocolInfo.OFFLINE_PING, ProtocolInfo.OFFLINE_PING_OPEN_CONNECTIONS]:
+                    packet: OfflinePing = OfflinePing(data)
+                    OfflinePingHandler.handle(packet, self, client)
+                elif data[0] == ProtocolInfo.OPEN_CONNECTION_REQUEST_1:
+                    packet: OpenConnectionRequest1 = OpenConnectionRequest1(data)
+                    OpenConnectionRequest1Handler.handle(packet, self, client)
+                elif data[0] == ProtocolInfo.OPEN_CONNECTION_REQUEST_2:
+                    packet: OpenConnectionRequest2 = OpenConnectionRequest2(data)
+                    OpenConnectionRequest2Handler.handle(packet, self, client)
+                elif ProtocolInfo.FRAME_SET_0 <= data[0] <= ProtocolInfo.FRAME_SET_F:
+                    connection = self.get_connection(client)
+                    connection.handle(data)
+
+    def stop(self):
+        self.running = False
+        self.socket.close()
+        self.logger.info('Server stopped.')
+
+
+if __name__ == '__main__':
+    server = Server()
+    server.name = 'MCPE;PieMC Server;589;1.20.0;2;20;13253860892328930865;Powered by PieMC;Survival;1;19132;19133;'
+    try:
+        server.start()
+    except KeyboardInterrupt:
+        server.logger.info('Stopping...')
+        server.stop()
```

### Comparing `PieRakNet-1.0.4/setup.py` & `PieRakNet-1.0.5/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-from setuptools import setup, find_packages
-
-
-def readme():
-    with open('README.md', 'r') as f:
-        return f.read()
-
-
-setup(
-    name='PieRakNet',
-    version='1.0.4',
-    author='lapismyt',
-    author_email='nikitagavrilin005@gmail.com',
-    description='RakNet implementation, written in Python. Created for PieMC.',
-    long_description=readme(),
-    long_description_content_type='text/markdown',
-    url='https://github.com/PieMC-Dev/PieRakNet',
-    packages=find_packages(),
-    # install_requires=[],
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
-        'Programming Language :: Python :: 3.11',
-        'Topic :: Internet',
-        'Topic :: Games/Entertainment',
-        'Topic :: Software Development :: Libraries :: Python Modules',
-        'Topic :: System :: Networking'
-    ],
-    keywords='python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet',
-    project_urls={
-        'Example': 'https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md',
-        'Developer': 'https://github.com/PieMC-Dev'
-    },
-    python_requires='>=3.10'
-)
+from setuptools import setup, find_packages
+
+
+def readme():
+    with open('README.md', 'r') as f:
+        return f.read()
+
+
+setup(
+    name='PieRakNet',
+    version='1.0.5',
+    author='lapismyt',
+    author_email='nikitagavrilin005@gmail.com',
+    description='RakNet implementation, written in Python. Created for PieMC.',
+    long_description=readme(),
+    long_description_content_type='text/markdown',
+    url='https://github.com/PieMC-Dev/PieRakNet',
+    packages=find_packages(),
+    # install_requires=[],
+    classifiers=[
+        'Development Status :: 3 - Alpha',
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+        'Programming Language :: Python :: 3.11',
+        'Topic :: Internet',
+        'Topic :: Games/Entertainment',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: System :: Networking'
+    ],
+    keywords='python python3 raknet rak-net mcpe bedrock rak_net piemc pieraknet',
+    project_urls={
+        'Example': 'https://github.com/PieMC-Dev/PieRakNet/tree/main/EXAMPLE.md',
+        'Developer': 'https://github.com/PieMC-Dev'
+    },
+    python_requires='>=3.10'
+)
```

