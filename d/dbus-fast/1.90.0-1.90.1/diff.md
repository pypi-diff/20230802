# Comparing `tmp/dbus_fast-1.90.0.tar.gz` & `tmp/dbus_fast-1.90.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbus_fast-1.90.0.tar", max compression
+gzip compressed data, was "dbus_fast-1.90.1.tar", max compression
```

## Comparing `dbus_fast-1.90.0.tar` & `dbus_fast-1.90.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     1083 2023-08-02 19:15:21.904996 dbus_fast-1.90.0/LICENSE
--rw-r--r--   0        0        0     9404 2023-08-02 19:15:21.904996 dbus_fast-1.90.0/README.md
--rw-r--r--   0        0        0     1252 2023-08-02 19:15:21.904996 dbus_fast-1.90.0/build_ext.py
--rw-r--r--   0        0        0     2552 2023-08-02 19:15:22.737009 dbus_fast-1.90.0/pyproject.toml
--rw-r--r--   0        0        0     1982 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/__init__.py
--rw-r--r--   0        0        0      401 2023-08-02 19:15:22.705009 dbus_fast-1.90.0/src/dbus_fast/__version__.py
--rw-r--r--   0        0        0        0 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/__init__.py
--rw-r--r--   0        0        0      211 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/_cython_compat.py
--rw-r--r--   0        0        0     3521 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/address.py
--rw-r--r--   0        0        0      275 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/constants.py
--rw-r--r--   0        0        0     2463 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/marshaller.pxd
--rw-r--r--   0        0        0     7785 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/marshaller.py
--rw-r--r--   0        0        0     5777 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/unmarshaller.pxd
--rw-r--r--   0        0        0    28577 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/unmarshaller.py
--rw-r--r--   0        0        0     5660 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/_private/util.py
--rw-r--r--   0        0        0       90 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/aio/__init__.py
--rw-r--r--   0        0        0    17702 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/aio/message_bus.py
--rw-r--r--   0        0        0      100 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/aio/message_reader.pxd
--rw-r--r--   0        0        0     1480 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/aio/message_reader.py
--rw-r--r--   0        0        0     7045 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/aio/proxy_object.py
--rw-r--r--   0        0        0     4285 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/auth.py
--rw-r--r--   0        0        0     5490 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/constants.py
--rw-r--r--   0        0        0     1982 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/errors.py
--rw-r--r--   0        0        0       90 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/glib/__init__.py
--rw-r--r--   0        0        0    16304 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/glib/message_bus.py
--rw-r--r--   0        0        0    10724 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/glib/proxy_object.py
--rw-r--r--   0        0        0    22462 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/introspection.py
--rw-r--r--   0        0        0       53 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/main.py
--rw-r--r--   0        0        0     1215 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/message.pxd
--rw-r--r--   0        0        0    11766 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/message.py
--rw-r--r--   0        0        0     1333 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/message_bus.pxd
--rw-r--r--   0        0        0    46915 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/message_bus.py
--rw-r--r--   0        0        0    14103 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/proxy_object.py
--rw-r--r--   0        0        0        0 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/py.typed
--rw-r--r--   0        0        0      524 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/service.pxd
--rw-r--r--   0        0        0    22231 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/service.py
--rw-r--r--   0        0        0      352 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/signature.pxd
--rw-r--r--   0        0        0    16502 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/signature.py
--rw-r--r--   0        0        0      181 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/unpack.pxd
--rw-r--r--   0        0        0      622 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/unpack.py
--rw-r--r--   0        0        0     5239 2023-08-02 19:15:21.908996 dbus_fast-1.90.0/src/dbus_fast/validators.py
--rw-r--r--   0        0        0    10450 1970-01-01 00:00:00.000000 dbus_fast-1.90.0/setup.py
--rw-r--r--   0        0        0    10607 1970-01-01 00:00:00.000000 dbus_fast-1.90.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-08-02 19:36:25.204682 dbus_fast-1.90.1/LICENSE
+-rw-r--r--   0        0        0     9404 2023-08-02 19:36:25.204682 dbus_fast-1.90.1/README.md
+-rw-r--r--   0        0        0     1252 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/build_ext.py
+-rw-r--r--   0        0        0     2552 2023-08-02 19:36:26.236685 dbus_fast-1.90.1/pyproject.toml
+-rw-r--r--   0        0        0     1982 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/src/dbus_fast/__init__.py
+-rw-r--r--   0        0        0      401 2023-08-02 19:36:26.192685 dbus_fast-1.90.1/src/dbus_fast/__version__.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/src/dbus_fast/_private/__init__.py
+-rw-r--r--   0        0        0      211 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/src/dbus_fast/_private/_cython_compat.py
+-rw-r--r--   0        0        0     3521 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/src/dbus_fast/_private/address.py
+-rw-r--r--   0        0        0      275 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/src/dbus_fast/_private/constants.py
+-rw-r--r--   0        0        0     2463 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/src/dbus_fast/_private/marshaller.pxd
+-rw-r--r--   0        0        0     7785 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/src/dbus_fast/_private/marshaller.py
+-rw-r--r--   0        0        0     5777 2023-08-02 19:36:25.208682 dbus_fast-1.90.1/src/dbus_fast/_private/unmarshaller.pxd
+-rw-r--r--   0        0        0    28577 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/_private/unmarshaller.py
+-rw-r--r--   0        0        0     5660 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/_private/util.py
+-rw-r--r--   0        0        0       90 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/aio/__init__.py
+-rw-r--r--   0        0        0    17732 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/aio/message_bus.py
+-rw-r--r--   0        0        0      100 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/aio/message_reader.pxd
+-rw-r--r--   0        0        0     1494 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/aio/message_reader.py
+-rw-r--r--   0        0        0     7045 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/aio/proxy_object.py
+-rw-r--r--   0        0        0     4295 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/auth.py
+-rw-r--r--   0        0        0     5490 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/constants.py
+-rw-r--r--   0        0        0     1982 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/errors.py
+-rw-r--r--   0        0        0       90 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/glib/__init__.py
+-rw-r--r--   0        0        0    16397 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/glib/message_bus.py
+-rw-r--r--   0        0        0    10724 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/glib/proxy_object.py
+-rw-r--r--   0        0        0    22597 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/introspection.py
+-rw-r--r--   0        0        0       53 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/main.py
+-rw-r--r--   0        0        0     1215 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/message.pxd
+-rw-r--r--   0        0        0    11766 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/message.py
+-rw-r--r--   0        0        0     1333 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/message_bus.pxd
+-rw-r--r--   0        0        0    46915 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/message_bus.py
+-rw-r--r--   0        0        0    14103 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/proxy_object.py
+-rw-r--r--   0        0        0        0 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/py.typed
+-rw-r--r--   0        0        0      524 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/service.pxd
+-rw-r--r--   0        0        0    22261 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/service.py
+-rw-r--r--   0        0        0      352 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/signature.pxd
+-rw-r--r--   0        0        0    16502 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/signature.py
+-rw-r--r--   0        0        0      181 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/unpack.pxd
+-rw-r--r--   0        0        0      622 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/unpack.py
+-rw-r--r--   0        0        0     5239 2023-08-02 19:36:25.212682 dbus_fast-1.90.1/src/dbus_fast/validators.py
+-rw-r--r--   0        0        0    10450 1970-01-01 00:00:00.000000 dbus_fast-1.90.1/setup.py
+-rw-r--r--   0        0        0    10607 1970-01-01 00:00:00.000000 dbus_fast-1.90.1/PKG-INFO
```

### Comparing `dbus_fast-1.90.0/LICENSE` & `dbus_fast-1.90.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/README.md` & `dbus_fast-1.90.1/README.md`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/build_ext.py` & `dbus_fast-1.90.1/build_ext.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/pyproject.toml` & `dbus_fast-1.90.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbus-fast"
-version = "1.90.0"
+version = "1.90.1"
 description = "A faster version of dbus-next"
 authors = ["Bluetooth Devices Authors <bluetooth@koston.org>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/bluetooth-devices/dbus-fast"
 documentation = "https://dbus-fast.readthedocs.io"
 classifiers = [
```

### Comparing `dbus_fast-1.90.0/src/dbus_fast/__init__.py` & `dbus_fast-1.90.1/src/dbus_fast/__init__.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/_private/address.py` & `dbus_fast-1.90.1/src/dbus_fast/_private/address.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/_private/marshaller.pxd` & `dbus_fast-1.90.1/src/dbus_fast/_private/marshaller.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/_private/marshaller.py` & `dbus_fast-1.90.1/src/dbus_fast/_private/marshaller.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/_private/unmarshaller.pxd` & `dbus_fast-1.90.1/src/dbus_fast/_private/unmarshaller.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/_private/unmarshaller.py` & `dbus_fast-1.90.1/src/dbus_fast/_private/unmarshaller.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/_private/util.py` & `dbus_fast-1.90.1/src/dbus_fast/_private/util.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/aio/message_bus.py` & `dbus_fast-1.90.1/src/dbus_fast/aio/message_bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             )
         )
 
     def _write_without_remove_writer(self) -> None:
         """Call the write callback without removing the writer."""
         self.write_callback(remove_writer=False)
 
-    def schedule_write(self, msg: Message = None, future=None) -> None:
+    def schedule_write(self, msg: Optional[Message] = None, future=None) -> None:
         queue_is_empty = not self.messages
         if msg is not None:
             self.buffer_message(msg, future)
         if self.bus.unique_name:
             # Optimization: try to send now if the queue
             # is empty. With bleak this usually means we
             # can send right away 99% of the time which
@@ -154,17 +154,17 @@
     :vartype connected: bool
     """
 
     __slots__ = ("_loop", "_auth", "_writer", "_disconnect_future")
 
     def __init__(
         self,
-        bus_address: str = None,
+        bus_address: Optional[str] = None,
         bus_type: BusType = BusType.SESSION,
-        auth: Authenticator = None,
+        auth: Optional[Authenticator] = None,
         negotiate_unix_fd: bool = False,
     ) -> None:
         super().__init__(bus_address, bus_type, ProxyObject, negotiate_unix_fd)
         self._loop = asyncio.get_running_loop()
 
         self._writer = _MessageWriter(self)
```

### Comparing `dbus_fast-1.90.0/src/dbus_fast/aio/message_reader.py` & `dbus_fast-1.90.1/src/dbus_fast/aio/message_reader.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def build_message_reader(
     sock: Optional[socket.socket],
     process: Callable[[Message], None],
     finalize: Callable[[Optional[Exception]], None],
     negotiate_unix_fd: bool,
-) -> None:
+) -> Callable[[], None]:
     """Build a callable that reads messages from the unmarshaller and passes them to the process function."""
     unmarshaller = Unmarshaller(None, sock, negotiate_unix_fd)
 
     def _message_reader() -> None:
         """Reads messages from the unmarshaller and passes them to the process function."""
         try:
             while True:
```

### Comparing `dbus_fast-1.90.0/src/dbus_fast/aio/proxy_object.py` & `dbus_fast-1.90.1/src/dbus_fast/aio/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/auth.py` & `dbus_fast-1.90.1/src/dbus_fast/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 
     :param uid: The uid to use when connecting to the message bus. Use UID_NOT_SPECIFIED to use the uid known to the kernel.
     :vartype uid: int
 
     :sealso: https://dbus.freedesktop.org/doc/dbus-specification.html#auth-protocol
     """
 
-    def __init__(self, uid: int = None) -> None:
+    def __init__(self, uid: Optional[int] = None) -> None:
         self.negotiate_unix_fd: bool = False
         self.negotiating_fds: bool = False
         self.uid: Optional[int] = uid
 
     def _authentication_start(self, negotiate_unix_fd: bool = False) -> str:
         self.negotiate_unix_fd = negotiate_unix_fd
         uid = self.uid
```

### Comparing `dbus_fast-1.90.0/src/dbus_fast/constants.py` & `dbus_fast-1.90.1/src/dbus_fast/constants.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/errors.py` & `dbus_fast-1.90.1/src/dbus_fast/errors.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/glib/message_bus.py` & `dbus_fast-1.90.1/src/dbus_fast/glib/message_bus.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,17 +155,17 @@
     :ivar unique_name: The unique name of the message bus connection. It will
         be :class:`None` until the message bus connects.
     :vartype unique_name: str
     """
 
     def __init__(
         self,
-        bus_address: str = None,
+        bus_address: Optional[str] = None,
         bus_type: BusType = BusType.SESSION,
-        auth: Authenticator = None,
+        auth: Optional[Authenticator] = None,
     ):
         if _import_error:
             raise _import_error
 
         super().__init__(bus_address, bus_type, ProxyObject)
         self._main_context = GLib.main_context_default()
         # buffer messages until connect
@@ -181,15 +181,18 @@
             self._process_message(msg)
         except Exception as e:
             logging.error(
                 f"got unexpected error processing a message: {e}.\n{traceback.format_exc()}"
             )
 
     def connect(
-        self, connect_notify: Callable[["MessageBus", Optional[Exception]], None] = None
+        self,
+        connect_notify: Optional[
+            Callable[["MessageBus", Optional[Exception]], None]
+        ] = None,
     ):
         """Connect this message bus to the DBus daemon.
 
         This method or the synchronous version must be called before the
         message bus can be used.
 
         :param connect_notify: A callback that will be called with this message
@@ -268,15 +271,17 @@
             raise connection_error
 
         return self
 
     def call(
         self,
         msg: Message,
-        reply_notify: Callable[[Optional[Message], Optional[Exception]], None] = None,
+        reply_notify: Optional[
+            Callable[[Optional[Message], Optional[Exception]], None]
+        ] = None,
     ):
         """Send a method call and asynchronously wait for a reply from the DBus
         daemon.
 
         :param msg: The method call message to send.
         :type msg: :class:`Message <dbus_fast.Message>`
         :param reply_notify: A callback that will be called with the reply to
```

### Comparing `dbus_fast-1.90.0/src/dbus_fast/glib/proxy_object.py` & `dbus_fast-1.90.1/src/dbus_fast/glib/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/introspection.py` & `dbus_fast-1.90.1/src/dbus_fast/introspection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import xml.etree.ElementTree as ET
-from typing import List, Union
+from typing import List, Optional, Union
 
 from .constants import ArgDirection, PropertyAccess
 from .errors import InvalidIntrospectionError
 from .signature import SignatureType, get_signature_tree
 from .validators import assert_interface_name_valid, assert_member_name_valid
 
 # https://dbus.freedesktop.org/doc/dbus-specification.html#introspection-format
@@ -27,16 +27,16 @@
         - :class:`InvalidSignatureError <dbus_fast.InvalidSignatureError>` - If the signature is not valid.
         - :class:`InvalidIntrospectionError <dbus_fast.InvalidIntrospectionError>` - If the signature is not a single complete type.
     """
 
     def __init__(
         self,
         signature: Union[SignatureType, str],
-        direction: List[ArgDirection] = None,
-        name: str = None,
+        direction: Optional[List[ArgDirection]] = None,
+        name: Optional[str] = None,
     ):
         if name is not None:
             assert_member_name_valid(name)
 
         type_ = None
         if type(signature) is SignatureType:
             type_ = signature
@@ -101,15 +101,15 @@
     :ivar signature: The collected signature of the output arguments.
     :vartype signature: str
 
     :raises:
         - :class:`InvalidMemberNameError <dbus_fast.InvalidMemberNameError>` - If the name of the signal is not a valid member name.
     """
 
-    def __init__(self, name: str, args: List[Arg] = None):
+    def __init__(self, name: Optional[str], args: Optional[List[Arg]] = None):
         if name is not None:
             assert_member_name_valid(name)
 
         self.name = name
         self.args = args or []
         self.signature = "".join(arg.signature for arg in self.args)
 
@@ -308,17 +308,17 @@
     :raises:
         - :class:`InvalidInterfaceNameError <dbus_fast.InvalidInterfaceNameError>` - If the name is not a valid interface name.
     """
 
     def __init__(
         self,
         name: str,
-        methods: List[Method] = None,
-        signals: List[Signal] = None,
-        properties: List[Property] = None,
+        methods: Optional[List[Method]] = None,
+        signals: Optional[List[Signal]] = None,
+        properties: Optional[List[Property]] = None,
     ):
         assert_interface_name_valid(name)
 
         self.name = name
         self.methods = methods if methods is not None else []
         self.signals = signals if signals is not None else []
         self.properties = properties if properties is not None else []
@@ -391,15 +391,18 @@
     :vartype is_root: bool
 
     :raises:
         - :class:`InvalidIntrospectionError <dbus_fast.InvalidIntrospectionError>` - If the name is not a valid node name.
     """
 
     def __init__(
-        self, name: str = None, interfaces: List[Interface] = None, is_root: bool = True
+        self,
+        name: Optional[str] = None,
+        interfaces: Optional[List[Interface]] = None,
+        is_root: bool = True,
     ):
         if not is_root and not name:
             raise InvalidIntrospectionError('child nodes must have a "name" attribute')
 
         self.interfaces = interfaces if interfaces is not None else []
         self.nodes = []
         self.name = name
@@ -483,15 +486,15 @@
                     elem.tail = i
 
         xml = self.to_xml()
         indent(xml)
         return header + ET.tostring(xml, encoding="unicode").rstrip()
 
     @staticmethod
-    def default(name: str = None) -> "Node":
+    def default(name: Optional[str] = None) -> "Node":
         """Create a :class:`Node` with the default interfaces supported by this library.
 
         The default interfaces include:
 
         * ``org.freedesktop.DBus.Introspectable``
         * ``org.freedesktop.DBus.Peer``
         * ``org.freedesktop.DBus.Properties``
```

### Comparing `dbus_fast-1.90.0/src/dbus_fast/message.pxd` & `dbus_fast-1.90.1/src/dbus_fast/message.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/message.py` & `dbus_fast-1.90.1/src/dbus_fast/message.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/message_bus.pxd` & `dbus_fast-1.90.1/src/dbus_fast/message_bus.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/message_bus.py` & `dbus_fast-1.90.1/src/dbus_fast/message_bus.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/proxy_object.py` & `dbus_fast-1.90.1/src/dbus_fast/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/service.pxd` & `dbus_fast-1.90.1/src/dbus_fast/service.pxd`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/service.py` & `dbus_fast-1.90.1/src/dbus_fast/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.introspection = intr.Method(name, in_args, out_args)
         self.in_signature = in_signature
         self.out_signature = out_signature
         self.in_signature_tree = get_signature_tree(in_signature)
         self.out_signature_tree = get_signature_tree(out_signature)
 
 
-def method(name: str = None, disabled: bool = False):
+def method(name: Optional[str] = None, disabled: bool = False):
     """A decorator to mark a class method of a :class:`ServiceInterface` to be a DBus service method.
 
     The parameters and return value must each be annotated with a signature
     string of a single complete DBus type.
 
     This class method will be called when a client calls the method on the DBus
     interface. The parameters given to the function come from the calling
@@ -145,15 +145,15 @@
         self.signature = signature
         self.signature_tree = signature_tree
         self.name = name
         self.disabled = disabled
         self.introspection = intr.Signal(self.name, args)
 
 
-def signal(name: str = None, disabled: bool = False):
+def signal(name: Optional[str] = None, disabled: bool = False):
     """A decorator to mark a class method of a :class:`ServiceInterface` to be a DBus signal.
 
     The signal is broadcast on the bus when the decorated class method is
     called by the user.
 
     If the signal has an out argument, the class method must have a return type
     annotation with a signature string of a single complete DBus type and the
@@ -267,15 +267,15 @@
         result.prop_setter = fn
         result.set_options(self.options)
         return result
 
 
 def dbus_property(
     access: PropertyAccess = PropertyAccess.READWRITE,
-    name: str = None,
+    name: Optional[str] = None,
     disabled: bool = False,
 ):
     """A decorator to mark a class method of a :class:`ServiceInterface` to be a DBus property.
 
     The class method must be a Python getter method with a return annotation
     that is a signature string of a single complete DBus type. When a client
     gets the property through the ``org.freedesktop.DBus.Properties``
@@ -346,17 +346,17 @@
     def __init__(self, name: str):
         # TODO cannot be overridden by a dbus member
         self.name = name
         self.__methods: List[_Method] = []
         self.__properties: List[_Property] = []
         self.__signals: List[_Signal] = []
         self.__buses = set()
-        self.__handlers: dict[
+        self.__handlers: Dict[
             BaseMessageBus,
-            dict[_Method, Callable[[Message, Callable[[Message], None]], None]],
+            Dict[_Method, Callable[[Message, Callable[[Message], None]], None]],
         ] = {}
 
         for name, member in inspect.getmembers(type(self)):
             member_dict = getattr(member, "__dict__", {})
             if type(member) is _Property:
                 # XXX The getter and the setter may show up as different
                 # members if they have different names. But if they have the
```

### Comparing `dbus_fast-1.90.0/src/dbus_fast/signature.py` & `dbus_fast-1.90.1/src/dbus_fast/signature.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/unpack.py` & `dbus_fast-1.90.1/src/dbus_fast/unpack.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/src/dbus_fast/validators.py` & `dbus_fast-1.90.1/src/dbus_fast/validators.py`

 * *Files identical despite different names*

### Comparing `dbus_fast-1.90.0/setup.py` & `dbus_fast-1.90.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ['dbus_fast', 'dbus_fast._private', 'dbus_fast.aio', 'dbus_fast.glib']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'dbus-fast',
-    'version': '1.90.0',
+    'version': '1.90.1',
     'description': 'A faster version of dbus-next',
     'long_description': '# dbus-fast\n\n<p align="center">\n  <a href="https://github.com/bluetooth-devices/dbus-fast/actions?query=workflow%3ACI">\n    <img src="https://img.shields.io/github/workflow/status/bluetooth-devices/dbus-fast/CI/main?label=CI&logo=github&style=flat-square" alt="CI Status" >\n  </a>\n  <a href="https://dbus-fast.readthedocs.io">\n    <img src="https://img.shields.io/readthedocs/dbus-fast.svg?logo=read-the-docs&logoColor=fff&style=flat-square" alt="Documentation Status">\n  </a>\n  <a href="https://codecov.io/gh/bluetooth-devices/dbus-fast">\n    <img src="https://img.shields.io/codecov/c/github/bluetooth-devices/dbus-fast.svg?logo=codecov&logoColor=fff&style=flat-square" alt="Test coverage percentage">\n  </a>\n</p>\n<p align="center">\n  <a href="https://python-poetry.org/">\n    <img src="https://img.shields.io/badge/packaging-poetry-299bd7?style=flat-square&logo=data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAA4AAAASCAYAAABrXO8xAAAACXBIWXMAAAsTAAALEwEAmpwYAAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAJJSURBVHgBfZLPa1NBEMe/s7tNXoxW1KJQKaUHkXhQvHgW6UHQQ09CBS/6V3hKc/AP8CqCrUcpmop3Cx48eDB4yEECjVQrlZb80CRN8t6OM/teagVxYZi38+Yz853dJbzoMV3MM8cJUcLMSUKIE8AzQ2PieZzFxEJOHMOgMQQ+dUgSAckNXhapU/NMhDSWLs1B24A8sO1xrN4NECkcAC9ASkiIJc6k5TRiUDPhnyMMdhKc+Zx19l6SgyeW76BEONY9exVQMzKExGKwwPsCzza7KGSSWRWEQhyEaDXp6ZHEr416ygbiKYOd7TEWvvcQIeusHYMJGhTwF9y7sGnSwaWyFAiyoxzqW0PM/RjghPxF2pWReAowTEXnDh0xgcLs8l2YQmOrj3N7ByiqEoH0cARs4u78WgAVkoEDIDoOi3AkcLOHU60RIg5wC4ZuTC7FaHKQm8Hq1fQuSOBvX/sodmNJSB5geaF5CPIkUeecdMxieoRO5jz9bheL6/tXjrwCyX/UYBUcjCaWHljx1xiX6z9xEjkYAzbGVnB8pvLmyXm9ep+W8CmsSHQQY77Zx1zboxAV0w7ybMhQmfqdmmw3nEp1I0Z+FGO6M8LZdoyZnuzzBdjISicKRnpxzI9fPb+0oYXsNdyi+d3h9bm9MWYHFtPeIZfLwzmFDKy1ai3p+PDls1Llz4yyFpferxjnyjJDSEy9CaCx5m2cJPerq6Xm34eTrZt3PqxYO1XOwDYZrFlH1fWnpU38Y9HRze3lj0vOujZcXKuuXm3jP+s3KbZVra7y2EAAAAAASUVORK5CYII=" alt="Poetry">\n  </a>\n  <a href="https://github.com/ambv/black">\n    <img src="https://img.shields.io/badge/code%20style-black-000000.svg?style=flat-square" alt="black">\n  </a>\n  <a href="https://github.com/pre-commit/pre-commit">\n    <img src="https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white&style=flat-square" alt="pre-commit">\n  </a>\n</p>\n<p align="center">\n  <a href="https://pypi.org/project/dbus-fast/">\n    <img src="https://img.shields.io/pypi/v/dbus-fast.svg?logo=python&logoColor=fff&style=flat-square" alt="PyPI Version">\n  </a>\n  <img src="https://img.shields.io/pypi/pyversions/dbus-fast.svg?style=flat-square&logo=python&amp;logoColor=fff" alt="Supported Python versions">\n  <img src="https://img.shields.io/pypi/l/dbus-fast.svg?style=flat-square" alt="License">\n</p>\n\nA faster version of dbus-next originally from the [great DBus next library](https://github.com/altdesktop/python-dbus-next) ❤️\n\n## Installation\n\nInstall this via pip (or your favourite package manager):\n\n`pip install dbus-fast`\n\n[Documentation](https://dbus-fast.readthedocs.io/en/latest/)\n\ndbus-fast is a Python library for DBus that aims to be a performant fully featured high level library primarily geared towards integration of applications into Linux desktop and mobile environments.\n\nDesktop application developers can use this library for integrating their applications into desktop environments by implementing common DBus standard interfaces or creating custom plugin interfaces.\n\nDesktop users can use this library to create their own scripts and utilities to interact with those interfaces for customization of their desktop environment.\n\ndbus-fast plans to improve over other DBus libraries for Python in the following ways:\n\n- Zero dependencies and pure Python 3\n- An optional cython extension is available to speed up (un)marshalling\n- Focus on performance\n- Support for multiple IO backends including asyncio and the GLib main loop.\n- Nonblocking IO suitable for GUI development.\n- Target the latest language features of Python for beautiful services and clients.\n- Complete implementation of the DBus type system without ever guessing types.\n- Integration tests for all features of the library.\n- Completely documented public API.\n\n## Installing\n\nThis library is available on PyPi as [dbus-fast](https://pypi.org/project/dbus-fast/).\n\n```\npip3 install dbus-fast\n```\n\n## The Client Interface\n\nTo use a service on the bus, the library constructs a proxy object you can use to call methods, get and set properties, and listen to signals.\n\nFor more information, see the [overview for the high-level client](https://dbus-fast.readthedocs.io/en/latest/high-level-client/index.html).\n\nThis example connects to a media player and controls it with the [MPRIS](https://specifications.freedesktop.org/mpris-spec/latest/) DBus interface.\n\n```python\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\n\n\nasync def main():\n    bus = await MessageBus().connect()\n    # the introspection xml would normally be included in your project, but\n    # this is convenient for development\n    introspection = await bus.introspect(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\')\n\n    obj = bus.get_proxy_object(\'org.mpris.MediaPlayer2.vlc\', \'/org/mpris/MediaPlayer2\', introspection)\n    player = obj.get_interface(\'org.mpris.MediaPlayer2.Player\')\n    properties = obj.get_interface(\'org.freedesktop.DBus.Properties\')\n\n    # call methods on the interface (this causes the media player to play)\n    await player.call_play()\n\n    volume = await player.get_volume()\n    print(f\'current volume: {volume}, setting to 0.5\')\n\n    await player.set_volume(0.5)\n\n    # listen to signals\n    def on_properties_changed(interface_name, changed_properties, invalidated_properties):\n        for changed, variant in changed_properties.items():\n            print(f\'property changed: {changed} - {variant.value}\')\n\n    properties.on_properties_changed(on_properties_changed)\n\n    await asyncio.Event().wait()\n\nasyncio.run(main())\n```\n\n## The Service Interface\n\nTo define a service on the bus, use the `ServiceInterface` class and decorate class methods to specify DBus methods, properties, and signals with their type signatures.\n\nFor more information, see the [overview for the high-level service](https://python-dbus-fast.readthedocs.io/en/latest/high-level-service/index.html).\n\n```python\nfrom dbus_fast.service import ServiceInterface, method, dbus_property, signal, Variant\nfrom dbus_fast.aio MessageBus\n\nimport asyncio\n\nclass ExampleInterface(ServiceInterface):\n    def __init__(self, name):\n        super().__init__(name)\n        self._string_prop = \'kevin\'\n\n    @method()\n    def Echo(self, what: \'s\') -> \'s\':\n        return what\n\n    @method()\n    def GetVariantDict() -> \'a{sv}\':\n        return {\n            \'foo\': Variant(\'s\', \'bar\'),\n            \'bat\': Variant(\'x\', -55),\n            \'a_list\': Variant(\'as\', [\'hello\', \'world\'])\n        }\n\n    @dbus_property()\n    def string_prop(self) -> \'s\':\n        return self._string_prop\n\n    @string_prop.setter\n    def string_prop_setter(self, val: \'s\'):\n        self._string_prop = val\n\n    @signal()\n    def signal_simple(self) -> \'s\':\n        return \'hello\'\n\nasync def main():\n    bus = await MessageBus().connect()\n    interface = ExampleInterface(\'test.interface\')\n    bus.export(\'/test/path\', interface)\n    # now that we are ready to handle requests, we can request name from D-Bus\n    await bus.request_name(\'test.name\')\n    # wait indefinitely\n    await asyncio.Event().wait()\n\nasyncio.run(main())\n```\n\n## The Low-Level Interface\n\nThe low-level interface works with DBus messages directly.\n\nFor more information, see the [overview for the low-level interface](https://python-dbus-fast.readthedocs.io/en/latest/low-level-interface/index.html).\n\n```python\nfrom dbus_fast.message import Message, MessageType\nfrom dbus_fast.aio import MessageBus\n\nimport asyncio\nimport json\n\n\nasync def main():\n    bus = await MessageBus().connect()\n\n    reply = await bus.call(\n        Message(destination=\'org.freedesktop.DBus\',\n                path=\'/org/freedesktop/DBus\',\n                interface=\'org.freedesktop.DBus\',\n                member=\'ListNames\'))\n\n    if reply.message_type == MessageType.ERROR:\n        raise Exception(reply.body[0])\n\n    print(json.dumps(reply.body[0], indent=2))\n\n\nasyncio.run(main())\n```\n\n## Projects that use python-dbus-fast\n\n- [Bluetooth Adapters](https://github.com/bluetooth-devices/bluetooth-adapters)\n\n## Contributing\n\nContributions are welcome. Development happens on [Github](https://github.com/Bluetooth-Devices/dbus-fast).\n\nBefore you commit, run `pre-commit run --all-files` to run the linter, code formatter, and the test suite.\n\n## Copyright\n\nYou can use this code under an MIT license (see LICENSE).\n\n- © 2019, Tony Crisci\n- © 2022, Bluetooth Devices authors\n\n## Contributors ✨\n\nThanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):\n\n<!-- prettier-ignore-start -->\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- markdownlint-disable -->\n<!-- markdownlint-enable -->\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n<!-- prettier-ignore-end -->\n\nThis project follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification. Contributions of any kind welcome!\n\n## Credits\n\nThis package was created with\n[Cookiecutter](https://github.com/audreyr/cookiecutter) and the\n[browniebroke/cookiecutter-pypackage](https://github.com/browniebroke/cookiecutter-pypackage)\nproject template.\n',
     'author': 'Bluetooth Devices Authors',
     'author_email': 'bluetooth@koston.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/bluetooth-devices/dbus-fast',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup package_dir = \ {'':
 'src'} packages = \ ['dbus_fast', 'dbus_fast._private', 'dbus_fast.aio',
 'dbus_fast.glib'] package_data = \ {'': ['*']} setup_kwargs = { 'name': 'dbus-
-fast', 'version': '1.90.0', 'description': 'A faster version of dbus-next',
+fast', 'version': '1.90.1', 'description': 'A faster version of dbus-next',
 'long_description': '# dbus-fast\n\n
      \n \n_[CI_Status]\n\n \n_[Documentation_Status]\n\n \n_[Test_coverage
                                 percentage]\n\n
 \n
              \n \n_[Poetry]\n\n \n_[black]\n\n \n_[pre-commit]\n\n
 \n
       \n \n_[PyPI_Version]\n\n [Supported Python versions]\n [License]\n
```

### Comparing `dbus_fast-1.90.0/PKG-INFO` & `dbus_fast-1.90.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbus-fast
-Version: 1.90.0
+Version: 1.90.1
 Summary: A faster version of dbus-next
 Home-page: https://github.com/bluetooth-devices/dbus-fast
 License: MIT
 Author: Bluetooth Devices Authors
 Author-email: bluetooth@koston.org
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

