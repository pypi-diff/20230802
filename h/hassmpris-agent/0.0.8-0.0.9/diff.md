# Comparing `tmp/hassmpris_agent-0.0.8.tar.gz` & `tmp/hassmpris_agent-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hassmpris_agent-0.0.8.tar", last modified: Fri Jun 24 15:12:13 2022, max compression
+gzip compressed data, was "hassmpris_agent-0.0.9.tar", last modified: Mon Jun 27 22:46:21 2022, max compression
```

## Comparing `hassmpris_agent-0.0.8.tar` & `hassmpris_agent-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:13.857127 hassmpris_agent-0.0.8/
--rw-rw-r--   0 user      (1000) user      (1000)      248 2022-06-23 01:35:58.000000 hassmpris_agent-0.0.8/Jenkinsfile
--rw-rw-r--   0 user      (1000) user      (1000)      130 2022-06-23 00:20:52.000000 hassmpris_agent-0.0.8/MANIFEST.in
--rw-rw-r--   0 user      (1000) user      (1000)     1319 2022-06-24 15:12:13.857127 hassmpris_agent-0.0.8/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      893 2022-06-23 02:13:51.000000 hassmpris_agent-0.0.8/README.md
--rw-rw-r--   0 user      (1000) user      (1000)       21 2022-06-23 00:33:59.000000 hassmpris_agent-0.0.8/build.parameters
--rw-rw-r--   0 user      (1000) user      (1000)     1674 2022-06-24 14:48:24.000000 hassmpris_agent-0.0.8/hassmpris-agent.spec
--rw-rw-r--   0 user      (1000) user      (1000)      615 2022-06-23 01:45:06.000000 hassmpris_agent-0.0.8/mypy.ini
--rw-rw-r--   0 user      (1000) user      (1000)       85 2022-06-22 16:48:33.000000 hassmpris_agent-0.0.8/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)      934 2022-06-24 15:12:13.858126 hassmpris_agent-0.0.8/setup.cfg
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:13.844127 hassmpris_agent-0.0.8/src/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:13.854127 hassmpris_agent-0.0.8/src/hassmpris_agent/
--rw-r--r--   0 user      (1000) user      (1000)      130 2022-06-24 14:48:21.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     1548 2022-06-23 01:39:25.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/auth.py
--rw-r--r--   0 user      (1000) user      (1000)      948 2022-06-22 17:03:24.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/config.py
--rw-r--r--   0 user      (1000) user      (1000)     1486 2022-06-22 16:30:27.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/control.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:13.855127 hassmpris_agent-0.0.8/src/hassmpris_agent/mpris/
--rw-r--r--   0 user      (1000) user      (1000)        0 2022-06-21 13:30:00.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/mpris/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     8968 2022-06-21 14:41:20.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/mpris/dbus.py
--rw-r--r--   0 user      (1000) user      (1000)     9029 2022-06-24 00:16:25.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/mpris/grpc.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2022-06-23 00:50:58.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/py.typed
--rw-r--r--   0 user      (1000) user      (1000)     3972 2022-06-24 14:29:45.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/server.py
--rw-r--r--   0 user      (1000) user      (1000)     9921 2022-06-23 16:30:37.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/settings.py
--rw-r--r--   0 user      (1000) user      (1000)     7983 2022-06-24 08:23:12.000000 hassmpris_agent-0.0.8/src/hassmpris_agent/verify.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:13.855127 hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)     1319 2022-06-24 15:12:12.000000 hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      759 2022-06-24 15:12:13.000000 hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2022-06-24 15:12:12.000000 hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)      115 2022-06-24 15:12:13.000000 hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/entry_points.txt
--rw-rw-r--   0 user      (1000) user      (1000)      107 2022-06-24 15:12:13.000000 hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       16 2022-06-24 15:12:13.000000 hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/top_level.txt
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-24 15:12:13.857127 hassmpris_agent-0.0.8/tests/
--rw-r--r--   0 user      (1000) user      (1000)      745 2022-06-21 00:25:36.000000 hassmpris_agent-0.0.8/tests/conftest.py
--rw-r--r--   0 user      (1000) user      (1000)       35 2022-06-23 00:59:31.000000 hassmpris_agent-0.0.8/tests/test_dummy.py
--rw-rw-r--   0 user      (1000) user      (1000)      254 2022-06-24 14:46:33.000000 hassmpris_agent-0.0.8/tox.ini
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:46:21.911042 hassmpris_agent-0.0.9/
+-rw-rw-r--   0 user      (1000) user      (1000)      248 2022-06-23 01:35:58.000000 hassmpris_agent-0.0.9/Jenkinsfile
+-rw-rw-r--   0 user      (1000) user      (1000)      130 2022-06-23 00:20:52.000000 hassmpris_agent-0.0.9/MANIFEST.in
+-rw-rw-r--   0 user      (1000) user      (1000)     1319 2022-06-27 22:46:21.911042 hassmpris_agent-0.0.9/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      893 2022-06-23 02:13:51.000000 hassmpris_agent-0.0.9/README.md
+-rw-rw-r--   0 user      (1000) user      (1000)       21 2022-06-23 00:33:59.000000 hassmpris_agent-0.0.9/build.parameters
+-rw-rw-r--   0 user      (1000) user      (1000)     1674 2022-06-27 22:45:52.000000 hassmpris_agent-0.0.9/hassmpris-agent.spec
+-rw-rw-r--   0 user      (1000) user      (1000)      615 2022-06-23 01:45:06.000000 hassmpris_agent-0.0.9/mypy.ini
+-rw-rw-r--   0 user      (1000) user      (1000)       85 2022-06-22 16:48:33.000000 hassmpris_agent-0.0.9/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)      935 2022-06-27 22:46:21.912042 hassmpris_agent-0.0.9/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:46:21.900042 hassmpris_agent-0.0.9/src/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:46:21.908042 hassmpris_agent-0.0.9/src/hassmpris_agent/
+-rw-rw-r--   0 user      (1000) user      (1000)      130 2022-06-27 22:45:52.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     1548 2022-06-23 01:39:25.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/auth.py
+-rw-r--r--   0 user      (1000) user      (1000)      948 2022-06-22 17:03:24.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/config.py
+-rw-r--r--   0 user      (1000) user      (1000)     1486 2022-06-22 16:30:27.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/control.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:46:21.910042 hassmpris_agent-0.0.9/src/hassmpris_agent/mpris/
+-rw-r--r--   0 user      (1000) user      (1000)        0 2022-06-21 13:30:00.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/mpris/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     8968 2022-06-21 14:41:20.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/mpris/dbus.py
+-rw-rw-r--   0 user      (1000) user      (1000)     9874 2022-06-27 22:45:52.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/mpris/grpc.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2022-06-23 00:50:58.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/py.typed
+-rw-r--r--   0 user      (1000) user      (1000)     3972 2022-06-24 14:29:45.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/server.py
+-rw-r--r--   0 user      (1000) user      (1000)     9921 2022-06-23 16:30:37.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/settings.py
+-rw-r--r--   0 user      (1000) user      (1000)     7983 2022-06-24 08:23:12.000000 hassmpris_agent-0.0.9/src/hassmpris_agent/verify.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:46:21.910042 hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)     1319 2022-06-27 22:46:21.000000 hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      759 2022-06-27 22:46:21.000000 hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2022-06-27 22:46:21.000000 hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      115 2022-06-27 22:46:21.000000 hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 user      (1000) user      (1000)      108 2022-06-27 22:46:21.000000 hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       16 2022-06-27 22:46:21.000000 hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2022-06-27 22:46:21.911042 hassmpris_agent-0.0.9/tests/
+-rw-r--r--   0 user      (1000) user      (1000)      745 2022-06-21 00:25:36.000000 hassmpris_agent-0.0.9/tests/conftest.py
+-rw-r--r--   0 user      (1000) user      (1000)       35 2022-06-23 00:59:31.000000 hassmpris_agent-0.0.9/tests/test_dummy.py
+-rw-rw-r--   0 user      (1000) user      (1000)      255 2022-06-27 22:45:52.000000 hassmpris_agent-0.0.9/tox.ini
```

### Comparing `hassmpris_agent-0.0.8/PKG-INFO` & `hassmpris_agent-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassmpris_agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: Linux desktop agent to allow MPRIS multimedia control from Home Assistant
 Home-page: https://github.com/Rudd-O/hassmpris
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Description-Content-Type: text/markdown
```

### Comparing `hassmpris_agent-0.0.8/README.md` & `hassmpris_agent-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/hassmpris-agent.spec` & `hassmpris_agent-0.0.9/hassmpris-agent.spec`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 %define dunder_name hassmpris_agent
 %define _name hassmpris-agent
 
 %define mybuildnumber %{?build_number}%{?!build_number:1}
 
 Name:           python-%{_name}
-Version:        0.0.8
+Version:        0.0.9
 Release:        %{mybuildnumber}%{?dist}
 Summary:        Linux desktop agent to allow MPRIS multimedia control from Home Assistant
 
 License:        LGPLv2.1
 URL:            https://github.com/Rudd-O/%{dunder_name}
 Source:         %{url}/archive/v%{version}/%{dunder_name}-%{version}.tar.gz
```

### Comparing `hassmpris_agent-0.0.8/mypy.ini` & `hassmpris_agent-0.0.9/mypy.ini`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/setup.cfg` & `hassmpris_agent-0.0.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	cryptography
 	dasbus
 	PyGObject
 	pyxdg
 	blindecdh>=0.1.8
 	shortauthstrings>=0.1.8
 	cakes>=0.1.6
-	hassmpris>=0.1.8
+	hassmpris>=0.1.10
 package_dir = 
 	= src
 packages = find:
 
 [options.entry_points]
 console_scripts = 
 	hassmpris-agent = hassmpris_agent.server:main
```

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent/auth.py` & `hassmpris_agent-0.0.9/src/hassmpris_agent/auth.py`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent/config.py` & `hassmpris_agent-0.0.9/src/hassmpris_agent/config.py`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent/control.py` & `hassmpris_agent-0.0.9/src/hassmpris_agent/control.py`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent/mpris/dbus.py` & `hassmpris_agent-0.0.9/src/hassmpris_agent/mpris/dbus.py`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent/mpris/grpc.py` & `hassmpris_agent-0.0.9/src/hassmpris_agent/mpris/grpc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+import logging
 from typing import (
     Deque,
     Any,
     List,
     Optional,
     TypeVar,
     Callable,
     cast,
     Generator,
 )
 from google.protobuf.empty_pb2 import Empty
 from functools import wraps
 import collections
 import threading
-from queue import Queue
+from queue import Queue, Empty as QueueEmpty
 
 from concurrent import futures
 
 from hassmpris.certs import PEM
 
 import json
 import grpc
@@ -25,14 +26,17 @@
 from cryptography.x509 import Certificate
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey
 
 from hassmpris.proto import mpris_pb2_grpc, mpris_pb2
 from hassmpris_agent.mpris.dbus import DBusMPRISInterface
 
 
+_LOGGER = logging.getLogger(__name__)
+
+
 def playback_status_to_PlayerStatus(playback_status: str) -> int:
     map = {
         "playing": mpris_pb2.PlayerStatus.PLAYING,
         "paused": mpris_pb2.PlayerStatus.PAUSED,
         "stopped": mpris_pb2.PlayerStatus.STOPPED,
     }
     s: int = map[playback_status.lower()]
@@ -121,56 +125,64 @@
     def _handle_player_appeared(
         self,
         unused_mpris: Any,
         player_id: str,
     ) -> None:
         print("player %s appeared" % player_id)
         m = mpris_pb2.MPRISUpdateReply(
-            player_id=player_id,
-            status=mpris_pb2.PlayerStatus.APPEARED,
+            player=mpris_pb2.MPRISPlayerUpdate(
+                player_id=player_id,
+                status=mpris_pb2.PlayerStatus.APPEARED,
+            )
         )
         self._push_to_queues(m)
 
     def _handle_player_gone(
         self,
         unused_mpris: Any,
         player_id: str,
     ) -> None:
         print("player %s gone" % player_id)
         m = mpris_pb2.MPRISUpdateReply(
-            player_id=player_id,
-            status=mpris_pb2.PlayerStatus.GONE,
+            player=mpris_pb2.MPRISPlayerUpdate(
+                player_id=player_id,
+                status=mpris_pb2.PlayerStatus.GONE,
+            )
         )
         self._push_to_queues(m)
 
     def _handle_player_playback_status_changed(
         self,
         unused_mpris: Any,
         player_id: str,
         playback_status: str,
     ) -> None:
         s = playback_status_to_PlayerStatus(playback_status)
         print("player %s status changed: %s" % (player_id, s))
         m = mpris_pb2.MPRISUpdateReply(
-            player_id=player_id,
-            status=s,
+            player=mpris_pb2.MPRISPlayerUpdate(
+                player_id=player_id,
+                status=s,
+            )
         )
         self._push_to_queues(m)
 
     def _handle_player_metadata_changed(
         self,
         unused_mpris: Any,
         player_id: str,
         metadata: Any,
     ) -> None:
         s = metadata_to_json_metadata(metadata)
         print("player %s metadata changed: %s" % (player_id, s))
         m = mpris_pb2.MPRISUpdateReply(
-            player_id=player_id,
-            json_metadata=s,
+            player=mpris_pb2.MPRISPlayerUpdate(
+                player_id=player_id,
+                json_metadata=s,
+            )
         )
         self._push_to_queues(m)
 
     def _push_to_queues(self, m: Optional[mpris_pb2.MPRISUpdateReply]) -> None:
         with self.queues_lock:
             queues = list(self.queues)
         for q in queues:
@@ -180,38 +192,52 @@
     def Updates(
         self,
         request: mpris_pb2.MPRISUpdateRequest,
         context: grpc.ServicerContext,
     ) -> Generator[mpris_pb2.MPRISUpdateReply, None, None]:
         q: Queue[Optional[mpris_pb2.MPRISUpdateReply]] = Queue()
         for player in self.mpris.get_players().values():
-            m = mpris_pb2.MPRISUpdateReply(
+            kws = dict(
                 player_id=player.player_id,
-                status=mpris_pb2.PlayerStatus.APPEARED,
-            )
-            m = mpris_pb2.MPRISUpdateReply(
-                player_id=player.player_id,
-                status=playback_status_to_PlayerStatus(player.playback_status),
+                status=playback_status_to_PlayerStatus(
+                    player.playback_status,
+                ),
             )
             if player.metadata:
+                kws["json_metadata"] = metadata_to_json_metadata(
+                    player.metadata,
+                )
+
                 m = mpris_pb2.MPRISUpdateReply(
-                    player_id=player.player_id,
-                    json_metadata=metadata_to_json_metadata(player.metadata),
+                    player=mpris_pb2.MPRISPlayerUpdate(
+                        **kws,
+                    ),
                 )
             q.put(m)
         with self.queues_lock:
             self.queues.append(q)
-        while True:
-            m = q.get()
-            if m is None:
-                break
-            else:
-                yield m
-        with self.queues_lock:
-            self.queues.remove(q)
+            _LOGGER.info("Clients connected now: %d", len(self.queues))
+        try:
+            while True:
+                try:
+                    m = q.get(timeout=10)
+                except QueueEmpty:
+                    m = mpris_pb2.MPRISUpdateReply(
+                        heartbeat=mpris_pb2.MPRISUpdateHeartbeat(),
+                    )
+                if m is None:
+                    break
+                else:
+                    yield m
+        except Exception:
+            _LOGGER.exception("Problem relaying status update to client")
+        finally:
+            with self.queues_lock:
+                self.queues.remove(q)
+                _LOGGER.info("Clients connected now: %d", len(self.queues))
 
     def stop(self) -> None:
         self.__del__()
 
     @player_id_validated
     @with_mpris
     def ChangePlayerStatus(
```

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent/server.py` & `hassmpris_agent-0.0.9/src/hassmpris_agent/server.py`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent/settings.py` & `hassmpris_agent-0.0.9/src/hassmpris_agent/settings.py`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent/verify.py` & `hassmpris_agent-0.0.9/src/hassmpris_agent/verify.py`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/PKG-INFO` & `hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hassmpris-agent
-Version: 0.0.8
+Version: 0.0.9
 Summary: Linux desktop agent to allow MPRIS multimedia control from Home Assistant
 Home-page: https://github.com/Rudd-O/hassmpris
 Author: Manuel Amador (Rudd-O)
 Author-email: rudd-o@rudd-o.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 (LGPLv2)
 Description-Content-Type: text/markdown
```

### Comparing `hassmpris_agent-0.0.8/src/hassmpris_agent.egg-info/SOURCES.txt` & `hassmpris_agent-0.0.9/src/hassmpris_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hassmpris_agent-0.0.8/tests/conftest.py` & `hassmpris_agent-0.0.9/tests/conftest.py`

 * *Files identical despite different names*

