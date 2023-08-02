# Comparing `tmp/cats-python-4.5.9.tar.gz` & `tmp/cats_python-4.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cats-python-4.5.9.tar", max compression
+gzip compressed data, was "cats_python-4.6.1.tar", max compression
```

## Comparing `cats-python-4.5.9.tar` & `cats_python-4.6.1.tar`

### file list

```diff
@@ -1,42 +1,39 @@
--rw-r--r--   0        0        0     1068 2021-11-12 08:23:00.727119 cats-python-4.5.9/LICENSE
--rw-r--r--   0        0        0      132 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/__init__.py
--rw-r--r--   0        0        0     3394 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/errors.py
--rw-r--r--   0        0        0      472 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/identity.py
--rw-r--r--   0        0        0      457 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/identity.pyi
--rw-r--r--   0        0        0     5807 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/plugins.py
--rw-r--r--   0        0        0        0 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/test_utils/__init__.py
--rw-r--r--   0        0        0       26 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/test_utils/client/__init__.py
--rw-r--r--   0        0        0     1854 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/test_utils/client/connection.py
--rw-r--r--   0        0        0        0 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/test_utils/pytest/__init__.py
--rw-r--r--   0        0        0     2641 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/test_utils/pytest/fixtures.py
--rw-r--r--   0        0        0       32 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/test_utils/pytest/plugin.py
--rw-r--r--   0        0        0     2681 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/types.py
--rw-r--r--   0        0        0     6076 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/utils.py
--rw-r--r--   0        0        0      189 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/__init__.py
--rw-r--r--   0        0        0    27224 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/action.py
--rw-r--r--   0        0        0     8685 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/action.pyi
--rw-r--r--   0        0        0     2051 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/auth.py
--rw-r--r--   0        0        0       26 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/client/__init__.py
--rw-r--r--   0        0        0     2845 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/client/__main__.py
--rw-r--r--   0        0        0     7327 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/client/connection.py
--rw-r--r--   0        0        0     9696 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/codecs.py
--rw-r--r--   0        0        0     8124 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/compression.py
--rw-r--r--   0        0        0      797 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/config.py
--rw-r--r--   0        0        0    10101 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/connection.py
--rw-r--r--   0        0        0     2575 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/handshake.py
--rw-r--r--   0        0        0      125 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/__init__.py
--rw-r--r--   0        0        0     2700 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/__main__.py
--rw-r--r--   0        0        0     2685 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/application.py
--rw-r--r--   0        0        0     8639 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/connection.py
--rw-r--r--   0        0        0    10624 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/handlers.py
--rw-r--r--   0        0        0     3247 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/handlers.pyi
--rw-r--r--   0        0        0      934 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/middleware.py
--rw-r--r--   0        0        0     9892 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/proxy.py
--rw-r--r--   0        0        0     5405 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/server/server.py
--rw-r--r--   0        0        0      819 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v2/statement.py
--rw-r--r--   0        0        0     1220 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v3/__init__.py
--rw-r--r--   0        0        0     2018 2021-11-12 08:23:00.727119 cats-python-4.5.9/cats/v3/scheme.py
--rw-r--r--   0        0        0     2334 2021-11-12 08:23:00.731119 cats-python-4.5.9/pyproject.toml
--rw-r--r--   0        0        0     1469 2021-11-12 08:23:00.731119 cats-python-4.5.9/wiki/index.md
--rw-r--r--   0        0        0     2878 2021-11-12 08:24:20.219109 cats-python-4.5.9/setup.py
--rw-r--r--   0        0        0     3722 2021-11-12 08:24:20.219597 cats-python-4.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-08-02 07:16:38.762316 cats_python-4.6.1/LICENSE
+-rw-r--r--   0        0        0      133 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/__init__.py
+-rw-r--r--   0        0        0     3394 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/errors.py
+-rw-r--r--   0        0        0      472 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/identity.py
+-rw-r--r--   0        0        0      457 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/identity.pyi
+-rw-r--r--   0        0        0     4636 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/plugins.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/test_utils/__init__.py
+-rw-r--r--   0        0        0       26 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/test_utils/client/__init__.py
+-rw-r--r--   0        0        0     1854 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/test_utils/client/connection.py
+-rw-r--r--   0        0        0        0 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/test_utils/pytest/__init__.py
+-rw-r--r--   0        0        0     2659 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/test_utils/pytest/fixtures.py
+-rw-r--r--   0        0        0       32 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/test_utils/pytest/plugin.py
+-rw-r--r--   0        0        0     2681 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/types.py
+-rw-r--r--   0        0        0     6156 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/utils.py
+-rw-r--r--   0        0        0      189 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/v2/__init__.py
+-rw-r--r--   0        0        0    26281 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/v2/action.py
+-rw-r--r--   0        0        0     8685 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/v2/action.pyi
+-rw-r--r--   0        0        0     2051 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/v2/auth.py
+-rw-r--r--   0        0        0       26 2023-08-02 07:16:38.762316 cats_python-4.6.1/cats/v2/client/__init__.py
+-rw-r--r--   0        0        0     2829 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/client/__main__.py
+-rw-r--r--   0        0        0     7489 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/client/connection.py
+-rw-r--r--   0        0        0     9656 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/codecs.py
+-rw-r--r--   0        0        0     8124 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/compression.py
+-rw-r--r--   0        0        0      797 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/config.py
+-rw-r--r--   0        0        0     9896 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/connection.py
+-rw-r--r--   0        0        0     2575 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/handshake.py
+-rw-r--r--   0        0        0      125 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/__init__.py
+-rw-r--r--   0        0        0     2739 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/__main__.py
+-rw-r--r--   0        0        0     2685 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/application.py
+-rw-r--r--   0        0        0     8349 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/connection.py
+-rw-r--r--   0        0        0    10624 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/handlers.py
+-rw-r--r--   0        0        0     3247 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/handlers.pyi
+-rw-r--r--   0        0        0      934 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/middleware.py
+-rw-r--r--   0        0        0     9986 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/proxy.py
+-rw-r--r--   0        0        0     6334 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/server/server.py
+-rw-r--r--   0        0        0      819 2023-08-02 07:16:38.766316 cats_python-4.6.1/cats/v2/statement.py
+-rw-r--r--   0        0        0     2218 2023-08-02 07:16:38.766316 cats_python-4.6.1/pyproject.toml
+-rw-r--r--   0        0        0     1425 2023-08-02 07:16:38.766316 cats_python-4.6.1/wiki/index.md
+-rw-r--r--   0        0        0     3510 1970-01-01 00:00:00.000000 cats_python-4.6.1/PKG-INFO
```

### Comparing `cats-python-4.5.9/LICENSE` & `cats_python-4.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/errors.py` & `cats_python-4.6.1/cats/errors.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/test_utils/client/connection.py` & `cats_python-4.6.1/cats/test_utils/client/connection.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/test_utils/pytest/fixtures.py` & `cats_python-4.6.1/cats/test_utils/pytest/fixtures.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 from typing import Type
 
-from pytest import PytestWarning, fixture, mark
+import pytest_asyncio
+from pytest import PytestWarning, fixture
 
 from cats.test_utils.client import Connection
 from cats.v2 import Config, Handshake
 from cats.v2.auth import Auth
 from cats.v2.server import Api, Application, Connection as ServerConnection, Middleware, Server, default_error_handler
 
 __all__ = [
@@ -73,31 +74,29 @@
         middleware=cats_middleware,
         auth=cats_auth,
         config=cats_config,
         connection=cats_server_connection,
     )
 
 
-@fixture(scope='session')
-@mark.asyncio
+@pytest_asyncio.fixture(scope='session')
 async def cats_server(cats_app) -> Server:
     """
     Runs an TCP server for each module and return port
     :return:
     """
 
     server = Server(cats_app)
     server.bind_unused_port()
     server.start(1)
     yield server
     await server.shutdown()
 
 
-@fixture
-@mark.asyncio
+@pytest_asyncio.fixture
 async def cats_conn(cats_config, cats_api_version, cats_server) -> Connection:
     """
     Return TCP connection to test TCP server
     """
     conn = Connection(cats_config, cats_api_version)
     await conn.connect('127.0.0.1', cats_server.port, timeout=5)
     async with conn:
```

### Comparing `cats-python-4.5.9/cats/types.py` & `cats_python-4.6.1/cats/types.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/utils.py` & `cats_python-4.6.1/cats/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     'Delay',
     'require',
     'tmp_file',
     'int2hex',
     'bytes2hex',
     'format_amount',
     'filter_json',
+    'str2bytes',
 ]
 
 logging = getLogger('CATS.utils')
 
 
 def to_uint(number: int, length: int = None) -> bytes:
     if length is None:
@@ -135,15 +136,15 @@
     format_amount(0) == "0B"
     format_amount(1750) == "1.7KB"
     format_amount(1234567890) == "1.1GB"
     format_amount(2000, base=10, suffix='r') == "2Gr"
 
     :param num: numeric amount
     :param base: how much does the step takes (default 1024 as for bytes)
-    :param prefix: type prefix (default '')
+    :param prefix: type prefix (default "")
     :param suffix: type suffix (default B as for bytes)
     :return: Formatted amount string
     :raise TypeError:
     """
     if not num:
         return f'0{suffix}'
 
@@ -190,7 +191,11 @@
         return [
             _filter_json_part(v, max_len, max_size)
             for v in (*json[:max_size], f'{len(json) - max_len} more')[:len(json)]
         ]
     if isinstance(json, str) and len(json) > max_len:
         return json[:max_len] + '...'
     return json
+
+
+def str2bytes(s: str) -> bytes:
+    return s.encode('utf-8')
```

### Comparing `cats-python-4.5.9/cats/v2/action.py` & `cats_python-4.6.1/cats/v2/action.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import asyncio
+import math
 from io import BytesIO
 from pathlib import Path
 from struct import Struct
 from time import time_ns
 from typing import NamedTuple, Type, TypeAlias, TypeVar
 
-import math
 import struct_model
 
 from cats.errors import CatsUsageError, InputCancelled, MalformedDataError, ProtocolError
 from cats.types import Bytes, Headers
-from cats.utils import Delay, as_uint, bytes2hex, filter_json, format_amount, int2hex, tmp_file, to_uint
-from cats.v2.codecs import Codec, T_FILE, T_JSON
+from cats.utils import Delay, as_uint, format_amount, int2hex, tmp_file, to_uint
+from cats.v2.codecs import Codec, T_FILE
 from cats.v2.compression import Compressor
 
 __all__ = [
     'ActionLike',
     'Input',
     'BaseAction',
     'BasicAction',
@@ -218,16 +218,14 @@
         buff = bytearray()
         while left > 0:
             chunk, left = await self._recv_chunk(left)
             buff.extend(chunk)
 
         buff = await Compressor.decompress(buff, self.headers, compression=self.compression)
         self.data = await Codec.decode(buff, self.data_type, self.headers)
-        if self.data_type == T_JSON:
-            self.conn.debug(f'[RECV {self.conn.address}] [{int2hex(self.message_id):<4}] <- {filter_json(self.data)}')
 
     async def _recv_large_data(self):
         left = self.data_len
         src, dst = tmp_file(), tmp_file()
 
         try:
             with src.open('wb') as fh:
@@ -241,15 +239,14 @@
             dst.unlink(missing_ok=True)
             raise
         finally:
             src.unlink(missing_ok=True)
 
     async def _recv_chunk(self, left):
         chunk = await self.conn.read(min(left, MAX_CHUNK_READ), partial=True)
-        self.conn.debug(f'[RECV {self.conn.address}] [{int2hex(self.message_id):<4}] <- {bytes2hex(chunk[:64])}...')
         left -= len(chunk)
         return chunk, left
 
     async def _encode(self):
         if self.encoded is None:
             data, data_type = await Codec.encode(self.data, self.headers, self.offset)
         else:
@@ -280,20 +277,17 @@
             max_chunk_size = min(MAX_IN_MEMORY, conn.download_speed) or MAX_IN_MEMORY
             delay = Delay(conn.download_speed)
             while left > 0:
                 size = min(left, max_chunk_size)
                 chunk = fh.read(size)
                 left -= size
                 await delay(size)
-                conn.debug(f'[SEND {conn.address}] [{int2hex(self.message_id):<4}] -> {bytes2hex(chunk[:64])}...')
                 await conn.write(chunk)
         finally:
             fh.close()
-            if data_type == T_JSON:
-                conn.debug(f'[SEND {conn.address}] [{int2hex(self.message_id):<4}] -> {filter_json(self.data)}')
 
     def __repr__(self):
         return f'{type(self).__name__}(data={str(self.data)[:256]}, headers={self.headers}, ' \
                f'status={self.status}, message_id={self.message_id}, ' \
                f'data_len={self.data_len}, data_type={self.data_type}, ' \
                f'compression={self.compression}, encoded={self.encoded})'
 
@@ -452,16 +446,14 @@
     async def _recv_large_chunk(self, fh, chunk_size):
         left = chunk_size
         part, dst = tmp_file(), tmp_file()
         try:
             with part.open('wb') as tmp:
                 while left > 0:
                     chunk = await self.conn.read(min(left, MAX_CHUNK_READ), partial=True)
-                    self.conn.debug(
-                        f'[RECV {self.conn.address}] [{int2hex(self.message_id):<4}] <- {bytes2hex(chunk[:64])}...')
                     left -= len(chunk)
                     tmp.write(chunk)
             await Compressor.decompress_file(part, dst, self.headers, compression=self.compression)
             data_len = dst.stat().st_size
             with dst.open('rb') as tmp:
                 while i := tmp.read(MAX_IN_MEMORY):
                     fh.write(i)
@@ -471,15 +463,14 @@
             dst.unlink(missing_ok=True)
 
     async def _recv_small_chunk(self, fh, chunk_size):
         left = chunk_size
         part = bytearray()
         while left > 0:
             chunk = await self.conn.read(min(left, MAX_CHUNK_READ), partial=True)
-            self.conn.debug(f'[RECV {self.conn.address}] [{int2hex(self.message_id):<4}] <- {bytes2hex(chunk[:64])}...')
             left -= len(chunk)
             part += chunk
         part = await Compressor.decompress(part, self.headers, compression=self.compression)
         fh.write(part)
         return len(part)
 
     async def _encode_gen(self, conn):
@@ -537,18 +528,18 @@
             chunk_size = len(chunk)
             if chunk_size >= 1 << 32:
                 raise MalformedDataError('Provided data chunk exceeded max chunk size', data=data, headers=self.headers)
 
             await delay(chunk_size + 4)
             await conn.write(to_uint(chunk_size, 4))
             await conn.write(chunk)
-            conn.debug(f'[SEND {conn.address}] [{int2hex(self.message_id):<4}] -> {bytes2hex(chunk[:64])}...')
         await conn.write(b'\x00\x00\x00\x00')
 
-    async def _async_gen(self, gen, chunk_size):
+    @staticmethod
+    async def _async_gen(gen, chunk_size):
         size = max(chunk_size, MAX_IN_MEMORY) or MAX_IN_MEMORY
         if hasattr(gen, '__iter__'):
             for item in gen:
                 for i in range(math.ceil(len(item) / size)):
                     yield item[i * size:]
         else:
             async for item in gen:
```

### Comparing `cats-python-4.5.9/cats/v2/action.pyi` & `cats_python-4.6.1/cats/v2/action.pyi`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/auth.py` & `cats_python-4.6.1/cats/v2/auth.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/client/__main__.py` & `cats_python-4.6.1/cats/v2/client/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,37 @@
 from tornado.iostream import StreamClosedError
 
+from cats import str2bytes
 from cats.errors import HandshakeError, ProtocolError
 from cats.v2.action import PingAction
 
 
-async def main(host: str, port: int,
-               handshake: bytes | None,
-               api: int,
-               input_timeout: float,
-               idle_timeout: float,
-               tls: bool,
-               debug: bool):
+async def main(
+        host: str, port: int,
+        handshake: bytes | None,
+        api: int,
+        input_timeout: float,
+        idle_timeout: float,
+        tls: bool,
+        debug: bool
+):
     import logging
     from cats.v2 import Config, SHA256TimeHandshake
     from cats.v2.client import Connection
 
     logging.basicConfig(level='DEBUG' if debug else 'INFO', force=True)
 
     if handshake is not None:
         handshake = SHA256TimeHandshake(secret_key=handshake, valid_window=1, timeout=5.0)
     config = Config(
         idle_timeout=idle_timeout,
         input_timeout=input_timeout,
         input_limit=5,
         debug=debug,
-        handshake=handshake
+        handshake=handshake,
     )
     conn = Connection(config, api_version=api)
     ssl_options = None
     if tls:
         from ssl import SSLContext, PROTOCOL_TLS_CLIENT, CERT_REQUIRED
         ssl_options = SSLContext(protocol=PROTOCOL_TLS_CLIENT)
         ssl_options.verify_mode = CERT_REQUIRED
@@ -39,34 +42,49 @@
         await PingAction().send(conn)
         exit(int(not conn.is_open))
     except (HandshakeError, ProtocolError):
         exit(0)
     except StreamClosedError:
         exit(1)
     except Exception:
-        exit(500)
-        raise
+        raise exit(500)
 
 
 if __name__ == '__main__':
     import asyncio
     import argparse
 
     parser = argparse.ArgumentParser()
-    parser.add_argument('--host', '-H', dest='host', type=str,
-                        default='127.0.0.1', help='CATS.v2.server host. Default: 127.0.0.1')
-    parser.add_argument('--port', '-P', dest='port', type=int,
-                        default=9191, help='CATS.v2.server port. Default: 9191')
-    parser.add_argument('--handshake', dest='handshake', type=bytes,
-                        default=None, help='Handshake secret key. Default: [disabled]')
-    parser.add_argument('--input-timeout', dest='input_timeout', type=float,
-                        default=120.0, help='Server`s input timeout. Default: 120.0')
-    parser.add_argument('--api', '-A', dest='api', type=int,
-                        default=1, help='API version. Default: 1')
-    parser.add_argument('--idle-timeout', dest='idle_timeout', type=float,
-                        default=120.0, help='Server`s idle timeout. Default: 120.0')
-    parser.add_argument('--tls', '-T', dest='tls', action='store_true',
-                        default=False, help='Enable TLS. Default: False')
-    parser.add_argument('--debug', '-D', dest='debug', action='store_true',
-                        default=False, help='Enable debug. Default: False')
+    parser.add_argument(
+        '--host', '-H', dest='host', type=str,
+        default='127.0.0.1', help='CATS.v2.server host. Default: 127.0.0.1',
+    )
+    parser.add_argument(
+        '--port', '-P', dest='port', type=int,
+        default=9191, help='CATS.v2.server port. Default: 9191',
+    )
+    parser.add_argument(
+        '--handshake', dest='handshake', type=str2bytes,
+        default=None, help='Handshake secret key. Default: [disabled]',
+    )
+    parser.add_argument(
+        '--input-timeout', dest='input_timeout', type=float,
+        default=120.0, help='Server`s input timeout. Default: 120.0',
+    )
+    parser.add_argument(
+        '--api', '-A', dest='api', type=int,
+        default=1, help='API version. Default: 1',
+    )
+    parser.add_argument(
+        '--idle-timeout', dest='idle_timeout', type=float,
+        default=120.0, help='Server`s idle timeout. Default: 120.0',
+    )
+    parser.add_argument(
+        '--tls', '-T', dest='tls', action='store_true',
+        default=False, help='Enable TLS. Default: False',
+    )
+    parser.add_argument(
+        '--debug', '-D', dest='debug', action='store_true',
+        default=False, help='Enable debug. Default: False',
+    )
     args = vars(parser.parse_args())
     asyncio.run(main(**args))
```

### Comparing `cats-python-4.5.9/cats/v2/client/connection.py` & `cats_python-4.6.1/cats/v2/client/connection.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,18 @@
     PROTOCOL_VERSION: int = 2
     logging = getLogger('CATS.Client')
 
     def __init__(self, conf: Config, api_version: int):
         super().__init__(conf)
         self.api_version: int = api_version
         self.time_delta: float = 0.0
-        self.subscriptions: dict[int, dict[int, Callable[[Action], Awaitable[None] | None]]] = defaultdict(dict)
+        self.subscriptions: dict[
+            int, dict[int, Callable[[Action], Awaitable[None] | None]]] = defaultdict(
+            dict
+        )
         self._sub_id: int = 0
         self._listener: asyncio.Task | None = None
         self._sender: asyncio.Task | None = None
         self._pinger: asyncio.Task | None = None
         self._recv_pool: dict[int, asyncio.Future] = {}
         self._stream: IOStream | None = None
         self.address: tuple[str, int] = '0.0.0.0', 0
@@ -69,16 +72,19 @@
 
         await self.recv_loop()
 
     async def init(self):
         await self.write(to_uint(self.PROTOCOL_VERSION, 4))
         result = await self.read(4)
         if result != bytes(4):
-            raise ProtocolError(f'Unsupported protocol version. '
-                                f'Please upgrade your client to: {as_uint(result)}', conn=self)
+            raise ProtocolError(
+                f'Unsupported protocol version. '
+                f'Please upgrade your client to: {as_uint(result)}',
+                conn=self
+            )
 
         client_stmt = ClientStatement(
             api=self.api_version,
             client_time=time_ns() // 1000_000,
             scheme_format='JSON',
             compressors=['gzip', 'zlib'],
             default_compression='zlib',
@@ -120,47 +126,72 @@
                 if inspect.isawaitable(res):
                     await res
 
     async def handle_ping_action(self, action: PingAction):
         self.debug(f'Pong {action.send_time} [-] {action.recv_time}')
         await action.dump_data(0)
 
-    def subscribe(self, handler_id: int, handler: Callable[[Action], Awaitable[None] | None]) -> int:
+    def subscribe(
+        self,
+        handler_id: int,
+        handler: Callable[[Action], Awaitable[None] | None]
+    ) -> int:
         self._sub_id += 1
         self.subscriptions[handler_id][self._sub_id] = handler
         return self._sub_id
 
-    def unsubscribe(self, handler_id: int, handler: Callable[[Action], Awaitable[None] | None] | int) -> None:
+    def unsubscribe(
+        self,
+        handler_id: int,
+        handler: Callable[[Action], Awaitable[None] | None] | int
+    ) -> None:
         if handler_id in self.subscriptions:
             if isinstance(handler, int):
                 self.subscriptions[handler_id].pop(handler, None)
             else:
                 self.subscriptions[handler_id] = {
                     k: v for k, v in self.subscriptions[handler_id]
                     if v is not handler
                 }
 
     async def set_download_speed(self, speed=0):
         await self.write(b'\x05')
         await self.write(to_uint(speed, 4))
 
-    async def send(self, handler_id: int, data=None, message_id=None, compression=None, *,
-                   headers=None, status=None) -> ActionLike | None:
-        action = Action(data=data, headers=headers, status=status,
-                        message_id=self.get_free_message_id() if message_id is None else message_id,
-                        handler_id=handler_id, compression=compression)
+    async def send(
+        self,
+        handler_id: int,
+        data=None,
+        message_id=None,
+        compression=None, *,
+        headers=None, status=None
+    ) -> ActionLike | None:
+        action = Action(
+            data=data, headers=headers, status=status,
+            message_id=self.get_free_message_id() if message_id is None else message_id,
+            handler_id=handler_id, compression=compression
+        )
         await action.send(self)
         return await self.recv(action.message_id)
 
-    async def send_stream(self, handler_id: int, data: BytesAnyGen, data_type: int,
-                          message_id=None, compression=None, *,
-                          headers=None, status=None) -> ActionLike | None:
-        action = StreamAction(data=data, headers=headers, status=status,
-                              message_id=self.get_free_message_id() if message_id is None else message_id,
-                              handler_id=handler_id, data_type=data_type, compression=compression)
+    async def send_stream(
+        self,
+        handler_id: int,
+        data: BytesAnyGen,
+        data_type: int,
+        message_id=None,
+        compression=None, *,
+        headers=None,
+        status=None
+    ) -> ActionLike | None:
+        action = StreamAction(
+            data=data, headers=headers, status=status,
+            message_id=self.get_free_message_id() if message_id is None else message_id,
+            handler_id=handler_id, data_type=data_type, compression=compression
+        )
         await action.send(self)
         return await self.recv(action.message_id)
 
     async def recv(self, message_id: int) -> Action | None:
         future = asyncio.Future()
         self._recv_pool[message_id] = future
         return await future
```

### Comparing `cats-python-4.5.9/cats/v2/codecs.py` & `cats_python-4.6.1/cats/v2/codecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os.path import getsize
 from pathlib import Path
 from typing import IO, TypeAlias
 
 import ujson
 
 from cats.errors import *
-from cats.plugins import BaseModel, BaseSerializer, Form, ModelSchema, scheme_json
+from cats.plugins import BaseModel, BaseSerializer, Form, scheme_json
 from cats.types import Byte, Json, List, T_Headers
 from cats.utils import tmp_file
 
 __all__ = [
     'FileInfo',
     'Files',
     'BaseCodec',
@@ -88,19 +88,19 @@
     type_id = 0x01
     type_name = 'json'
 
     @classmethod
     async def encode(cls, data: Json | Form | list[Form], headers: T_Headers, offset: int = 0) -> bytes:
         try:
             if data:
-                if isinstance(data, (BaseModel, BaseSerializer, ModelSchema)):
+                if isinstance(data, (BaseModel, BaseSerializer)):
                     return scheme_json(type(data), data, many=False, plain=True)
                 elif isinstance(data, List):
                     data = list(data)
-                    if isinstance(data[0], (BaseModel, BaseSerializer, ModelSchema)):
+                    if isinstance(data[0], (BaseModel, BaseSerializer)):
                         return scheme_json(type(data[0]), data, many=True, plain=True)
             return await cls._encode(data, offset=offset)
         except TypeError as err:
             raise InvalidCodecError(f'{cls} does not support {type(data)}', data=data, headers=headers) from err
 
     @classmethod
     async def _encode(cls, data: Json, offset: int = 0) -> bytes:
@@ -273,15 +273,15 @@
         if data_type not in cls.codecs:
             raise CodecError(f'Failed to decode data: Type {data_type} not supported', data=buff, headers=headers)
 
         return await cls.codecs[data_type].decode(buff, headers)
 
     def get_codec_name(self, type_id: int, default: str = 'unknown') -> str:
         """
-        Returns Type Name by it's id (w/ fallback to default)
+        Returns Type Name by its id (w/ fallback to default)
         :param type_id:
         :param default:
         :return:
         """
         try:
             return self.codecs[type_id].type_name
         except KeyError:
```

### Comparing `cats-python-4.5.9/cats/v2/compression.py` & `cats_python-4.6.1/cats/v2/compression.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/config.py` & `cats_python-4.6.1/cats/v2/config.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/connection.py` & `cats_python-4.6.1/cats/v2/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import asyncio
 from contextlib import asynccontextmanager
 from logging import Logger
 from traceback import format_tb
 from typing import TypeVar
 
-import rollbar
 from tornado.iostream import IOStream
 
 from cats.errors import ProtocolError
 from cats.identity import Identity
 from cats.types import BytesAnyGen
 from cats.v2 import C_NONE, Compressor
 from cats.v2.action import BaseAction, Input
@@ -126,18 +125,15 @@
         action_type_id = await self.read(1)
         action_class = BaseAction.get_class_by_type_id(action_type_id)
         if action_class is None:
             raise ProtocolError(f'Received unknown Action Type ID [{action_type_id.hex()}]', conn=self)
 
         try:
             await self.handle(await action_class.init(self))
-        except self.conf.ignore_errors as err:
-            self.close(err)
         except Exception as err:
-            rollbar.report_exc_info(extra_data=self.identity_scope_user)  # FIXME: Use plugins/middleware for this
             self.close(err)
 
     def on_tick_done(self, task):
         try:
             if exc := task.exception():
                 self.close(exc)
         except (asyncio.CancelledError, asyncio.InvalidStateError) as err:
```

### Comparing `cats-python-4.5.9/cats/v2/handshake.py` & `cats_python-4.6.1/cats/v2/handshake.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/server/__main__.py` & `cats_python-4.6.1/cats/v2/server/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from cats.utils import str2bytes
+
+
 def main(host: str, port: int,
          handshake: bytes | None,
          api: int,
          input_timeout: float,
          idle_timeout: float,
          tls: bool,
          debug: bool):
@@ -45,15 +48,15 @@
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument('--host', '-H', dest='host', type=str,
                         default='0.0.0.0', help='CATS.v2.server host. Default: 0.0.0.0')
     parser.add_argument('--port', '-P', dest='port', type=int,
                         default=9191, help='CATS.v2.server port. Default: 9191')
-    parser.add_argument('--handshake', dest='handshake', type=bytes,
+    parser.add_argument('--handshake', dest='handshake', type=str2bytes,
                         default=None, help='Handshake secret key. Default: [disabled]')
     parser.add_argument('--input-timeout', dest='input_timeout', type=float,
                         default=120.0, help='Input timeout. Default: 120.0')
     parser.add_argument('--api', '-A', dest='api', type=int,
                         default=1, help='API version. Default: 1')
     parser.add_argument('--idle-timeout', dest='idle_timeout', type=float,
                         default=120.0, help='Idle timeout. Default: 120.0')
```

### Comparing `cats-python-4.5.9/cats/v2/server/application.py` & `cats_python-4.6.1/cats/v2/server/application.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/server/connection.py` & `cats_python-4.6.1/cats/v2/server/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 import functools
 from logging import getLogger
 from random import randint
 from time import time_ns
 from typing import Iterable
 
-import rollbar
 from tornado.iostream import IOStream
 
 from cats.errors import ProtocolError
 from cats.identity import Identity, IdentityObject
 from cats.types import BytesAnyGen
 from cats.utils import as_uint
 from cats.v2.action import *
@@ -94,29 +93,23 @@
         elif isinstance(action, PingAction):
             self.debug(f'Ping {action.send_time} [-] {action.recv_time}')
             await action.send(self)
             await action.dump_data(0)
         elif isinstance(action, Action):
             async with self.preserve_message_id(action.message_id):
                 handler = self.dispatch(action.handler_id)
-                try:
-                    result = await self.app.run(handler(action))
-                    if result is not None:
-                        if not isinstance(result, Action):
-                            raise ProtocolError('Returned invalid response', conn=self)
-
-                        result.handler_id = action.handler_id
-                        result.message_id = action.message_id
-                        result.offset = action.offset
-                        await result.send(self)
-                except action.conn.conf.ignore_errors:
-                    raise
-                except Exception:
-                    rollbar.report_exc_info(extra_data=self.identity_scope_user)
-                    raise
+                result = await self.app.run(handler(action))
+                if result is not None:
+                    if not isinstance(result, Action):
+                        raise ProtocolError('Returned invalid response', conn=self)
+
+                    result.handler_id = action.handler_id
+                    result.message_id = action.message_id
+                    result.offset = action.offset
+                    await result.send(self)
 
     def dispatch(self, handler_id):
         handlers = self.app.get_handlers_by_id(handler_id)
         if isinstance(handlers, HandlerItem):
             return handlers.handler
 
         elif isinstance(handlers, list):
```

### Comparing `cats-python-4.5.9/cats/v2/server/handlers.py` & `cats_python-4.6.1/cats/v2/server/handlers.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/server/handlers.pyi` & `cats_python-4.6.1/cats/v2/server/handlers.pyi`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/server/middleware.py` & `cats_python-4.6.1/cats/v2/server/middleware.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/cats/v2/server/proxy.py` & `cats_python-4.6.1/cats/v2/server/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,40 +73,42 @@
     # Now, try and parse the proxy line as desired.
     proxy_line = line[:idx]
     fields: list[bytes] = proxy_line.split(b' ')
     if len(fields) != 6:
         raise ProxyProtocolInvalidLine()
 
     # Check if the proxy line is for v1 of the protocol.
-    if fields[0] == b"PROXY":
-        try:
-            if fields[1] == b"TCP4" or fields[1] == b"TCP6":
-                source_addr = fields[2]
-                dest_addr = fields[3]
-                source_port = int(fields[4])
-                dest_port = int(fields[5])
-            else:
-                raise ProxyProtocolInvalidAddress()
-        except:
+    if fields[0] != b"PROXY":
+        raise ProxyProtocolInvalidLine()
+
+    try:
+        if fields[1] == b"TCP4" or fields[1] == b"TCP6":
+            source_addr = fields[2]
+            dest_addr = fields[3]
+            source_port = int(fields[4])
+            dest_port = int(fields[5])
+        else:
             raise ProxyProtocolInvalidAddress()
+    except ValueError:
+        raise ProxyProtocolInvalidAddress()
 
-        return {
-                   'client_ip': source_addr.decode('utf-8'),
-                   'client_port': source_port,
-                   'local_ip': dest_addr.decode('utf-8'),
-                   'local_port': dest_port
-               }, int(idx + 2)
-    raise ProxyProtocolInvalidLine()
+    return {
+        'client_ip': source_addr.decode('utf-8'),
+        'client_port': source_port,
+        'local_ip': dest_addr.decode('utf-8'),
+        'local_port': dest_port
+    }, int(idx + 2)
 
 
+# noinspection PyProtectedMember
 def putback_line_in_stream(line: bytes | bytearray, stream: IOStream):
     """
-    HACKY: This call reinjects the given line back into the stream.
+    HACKY: This call re-injects the given line back into the stream.
 
-    This emulates a "putback" or "unget" operation. This is subject to
+    This emulates a "putback" or "un-get" operation. This is subject to
     break, though, so it should be used with caution, since it uses
     tornado internals.
     """
     # line_len = len(line)
     # stream._read_buffer_pos -= line_len
     # stream._read_buffer_size += line_len
     if not line:
@@ -156,36 +158,37 @@
 
 def handle_with_proxy(fn: tcpserver.TCPServer.handle_stream = None):
     if fn is None:
         return handle_with_proxy
 
     @wraps(fn)
     async def handle_stream(self, stream: IOStream, address: tuple[str, int]):
+        # noinspection PyBroadException
         try:
             addr = await parse_proxy_line_from_buff(stream)
             if addr is not None:
                 address = (addr['client_ip'], addr['client_port'])
                 stream.proxy_addr = addr
             return await fn(self, stream, address)
         except iostream.StreamClosedError:
             raise
-        except:
+        except Exception:
             return await fn(self, stream, address)
 
     return handle_stream
 
 
 class ProxyProtocolTCPServer(tcpserver.TCPServer):
     """
     Wrapper for tornado.tcpserver.TCPServer that parses out the
     HAProxy PROXY protocol and attaches the actual IP to the stream
     as an attribute named 'proxy_addr'.
 
     The proxy protocol spec is defined here:
-    http://www.haproxy.org/download/1.8/doc/proxy-protocol.txt
+    https://www.haproxy.org/download/1.8/doc/proxy-protocol.txt
     """
 
     async def handle_stream(self, stream: IOStream, address: tuple[str, int]):
         try:
             addr = await parse_proxy_line_from_buff(stream)
             if addr is not None:
                 stream.proxy_addr = addr
@@ -247,46 +250,48 @@
 
 
 class ProxyProtocolHTTPServer(httpserver.HTTPServer):
     """
     Wrapper for tornado.httpserver.HTTPServer that parses out the
     HAProxy PROXY protocol and sets the appropriate remote_ip as
     defined here:
-    http://www.haproxy.org/download/1.8/doc/proxy-protocol.txt
+    https://www.haproxy.org/download/1.8/doc/proxy-protocol.txt
     """
 
     async def handle_stream(self, stream: IOStream, address: tuple[str, int]):
         """
         Creates the stream for this connection.
 
         This parses out the proxy protocol from the request and injects the
         relevant fields onto the given stream object at: `stream.proxy_addr`
         """
+        # noinspection PyBroadException
         try:
             addr = await parse_proxy_line_from_buff(stream)
             if addr is not None:
                 stream.proxy_addr = addr
 
             # Use our parsed address here.
             super(ProxyProtocolHTTPServer, self).handle_stream(stream, address)
         except iostream.StreamClosedError:
             pass
-        except:
+        except Exception:
             super(ProxyProtocolHTTPServer, self).handle_stream(stream, address)
 
     def start_request(self, server_conn, request_conn):
         """
         Override so that we can inject the real ip for `self.request.remote_ip`
         in each request.
         """
         delegate = super(ProxyProtocolHTTPServer, self).start_request(server_conn, request_conn)
 
         # If the real client IP was parsed via the proxy protocol, the address would
         # have been attached to the socket in the 'proxy_addr' attribute, so we try
         # to fetch it. If we couldn't, just ignore it and default to the usual
         # behavior. (Should we log it instead?)
+        # noinspection PyBroadException
         try:
             proxy_addr = server_conn.stream.proxy_addr
             addr = proxy_addr['client_ip']
             return ProxyProtocolAdapter(delegate, request_conn, proxy_ip=addr)
         except Exception as e:
             return delegate
```

### Comparing `cats-python-4.5.9/cats/v2/server/server.py` & `cats_python-4.6.1/cats/v2/server/server.py`

 * *Files 16% similar despite different names*

```diff
@@ -10,57 +10,94 @@
 from tornado.testing import bind_unused_port
 
 from cats.errors import CatsError
 from cats.utils import as_uint, to_uint
 from cats.v2.connection import ConnType, Connection
 from cats.v2.server.application import Application
 from cats.v2.server.connection import Connection as ServerConnection
+from cats.v2.server.proxy import handle_with_proxy
 
 __all__ = [
     'Server',
 ]
 
-from cats.v2.server.proxy import handle_with_proxy
-
 logging = getLogger('CATS.Server')
 
 
 class Server(TCPServer):
     __slots__ = ('app', 'port', 'connections')
     protocols: tuple[int, int] = 2, 2
     instances: list['Server'] = []
 
-    def __init__(self, app: Application,
-                 ssl_options: dict[str] | ssl.SSLContext | None = None,
-                 max_buffer_size: int | None = None,
-                 read_chunk_size: int | None = None):
+    def __init__(
+            self, app: Application,
+            ssl_options: dict[str] | ssl.SSLContext | None = None,
+            max_buffer_size: int | None = None,
+            read_chunk_size: int | None = None
+    ):
         self.app: Application = app
         self.port: int | None = None
         self.connections: list[Connection] = []
-        super().__init__(ssl_options=ssl_options, max_buffer_size=max_buffer_size, read_chunk_size=read_chunk_size)
+        super().__init__(
+            ssl_options=ssl_options,
+            max_buffer_size=max_buffer_size,
+            read_chunk_size=read_chunk_size
+        )
 
     @classmethod
-    async def broadcast(cls, channel: str, handler_id: int, data=None, message_id: int = None, compression: int = None,
-                        *, headers=None, status: int = None):
-        return await asyncio.gather(*(
-            conn.send(handler_id, data, message_id, compression, headers=headers, status=status)
-            for server in cls.running_servers()
-            for conn in server.app.channel(channel)
-        ))
+    async def broadcast(
+            cls,
+            channel: str,
+            handler_id: int,
+            data=None,
+            message_id: int = None,
+            compression: int = None,
+            *, headers=None, status: int = None
+    ):
+        return await asyncio.gather(
+            *(
+                conn.send(
+                    handler_id,
+                    data,
+                    message_id,
+                    compression,
+                    headers=headers,
+                    status=status
+                )
+                for server in cls.running_servers()
+                for conn in server.app.channel(channel)
+            )
+        )
 
     @classmethod
-    async def conditional_broadcast(cls, channel: str, _filter: Callable[['Server', Connection], bool],
-                                    handler_id: int, data=None, message_id: int = None,
-                                    compression: int = None, *, headers=None, status: int = None):
-        return await asyncio.gather(*(
-            conn.send(handler_id, data, message_id, compression, headers=headers, status=status)
-            for server in cls.running_servers()
-            for conn in server.app.channel(channel)
-            if _filter(server, conn)
-        ))
+    async def conditional_broadcast(
+            cls,
+            channel: str,
+            _filter: Callable[['Server', Connection], bool],
+            handler_id: int,
+            data=None,
+            message_id: int = None,
+            compression: int = None,
+            *, headers=None, status: int = None
+    ):
+        return await asyncio.gather(
+            *(
+                conn.send(
+                    handler_id,
+                    data,
+                    message_id,
+                    compression,
+                    headers=headers,
+                    status=status
+                )
+                for server in cls.running_servers()
+                for conn in server.app.channel(channel)
+                if _filter(server, conn)
+            )
+        )
 
     @handle_with_proxy
     async def handle_stream(self, stream: IOStream, address: tuple[str, int]) -> None:
         try:
             protocol_version = as_uint(await stream.read_bytes(4))
             if not self.protocols[0] <= protocol_version <= self.protocols[1]:
                 await stream.write(to_uint(self.protocols[1], 4))
@@ -73,15 +110,20 @@
                 await conn.init()
                 await conn.start()
             conn.debug(f'[STOP {address}]')
         except self.app.config.stream_errors:
             pass
 
     @asynccontextmanager
-    async def create_connection(self, stream: IOStream, address: tuple[str, int], protocol: int) -> ConnType:
+    async def create_connection(
+            self,
+            stream: IOStream,
+            address: tuple[str, int],
+            protocol: int,
+    ) -> ConnType:
         conn_class = self.app.ConnectionClass or ServerConnection
         conn = conn_class(stream, address, protocol, self.app.config, self.app)
         try:
             self.connections.append(conn)
             self.app.attach_conn_to_channel(conn, '__all__')
             async with conn:
                 yield conn
@@ -118,22 +160,37 @@
 
     def bind_unused_port(self):
         sock, port = bind_unused_port()
         self.add_socket(sock)
         self.port = port
         logging.info(f'Starting server at 127.0.0.1:{port}')
 
-    def bind(self, port: int, address: str = None, family: socket.AddressFamily = socket.AF_UNSPEC,
-             backlog: int = 128, reuse_port: bool = False) -> None:
-        super().bind(port, address, family, backlog, reuse_port)
+    def bind(
+            self,
+            port: int,
+            address: str | None = None,
+            family: socket.AddressFamily = socket.AF_UNSPEC,
+            backlog: int = 128,
+            flags: int | None = None,
+            reuse_port: bool = False
+    ) -> None:
+        super().bind(port, address, family, backlog, flags, reuse_port)
         self.port = port
         logging.info(f'Starting server at {address}:{port}')
 
-    def listen(self, port: int, address: str = "") -> None:
-        super().listen(port, address)
+    def listen(
+            self,
+            port: int,
+            address: str | None = None,
+            family: socket.AddressFamily = socket.AF_UNSPEC,
+            backlog: int = 128,
+            flags: int | None = None,
+            reuse_port: bool = False,
+    ) -> None:
+        super().listen(port, address, family, backlog, flags, reuse_port)
         self.port = port
         logging.info(f'Starting server at {address}:{port}')
 
     def __new__(cls, *args, **kwargs):
         obj = super().__new__(cls)
         cls.instances.append(obj)
         return obj
```

### Comparing `cats-python-4.5.9/cats/v2/statement.py` & `cats_python-4.6.1/cats/v2/statement.py`

 * *Files identical despite different names*

### Comparing `cats-python-4.5.9/pyproject.toml` & `cats_python-4.6.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cats-python"
-version = "4.5.9"
+version = "4.6.1"
 description = "Cifrazia Action Transport System for Python"
 authors = ["Bogdan Parfenov <adam.brian.bright@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://adambrianbright.github.io/cats-python/"
 repository = "https://github.com/AdamBrianBright/cats-python"
 documentation = "https://adambrianbright.github.io/cats-python/"
@@ -35,41 +35,39 @@
 
 [tool.poetry.urls]
 "ChangeLog" = "https://adambrianbright.github.io/cats-python/changelog"
 "Bug Tracker" = "https://github.com/AdamBrianBright/cats-python/issues"
 "Contact Author" = "https://vk.com/adam_bright"
 
 [tool.poetry.dependencies]
-python = ">=3.10.0rc2, <4.0"
+python = ">=3.10.0, <3.11"
 
-richerr = "^0.1.1"
-struct-model-python = "^0.1.0"
+richerr = "^0.2.3"
+struct-model-python = "^0.1.1"
 
-pytz = "^2021.1"
+pytz = "^2023.3"
 tornado = "^6.1"
-ujson = "^4.1.0"
-PyYAML = "^5.4.1"
+PyYAML = "^6.0"
 toml = "^0.10.2"
-msgpack = "^1.0.2"
+msgpack = "^1.0.3"
 Django = { version = ">=2.0, <3.0", optional = true }
-djangorestframework = { version = ">=3.12.4", optional = true }
-pydantic = { version = ">=1.8.2", optional = true }
-djantic = { version = ">=0.3.3", optional = true }
-rollbar = "^0.16.2"
+djangorestframework = { version = "3.13", optional = true }
+pydantic = { version = ">=2.1.0", optional = true }
+ujson = "^5.1.0"
 
 [tool.poetry.extras]
 django = ["Django", "djangorestframework"]
 pydantic = ["pydantic"]
-djantic = ["djantic", "pydantic", "Django"]
 
-[tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
-pytest-asyncio = "^0.15.1"
-pydantic = "^1.8.2"
-coverage = "^6.0.2"
 
 [tool.poetry.plugins."pytest11"]
 "pytest_cats" = "cats.test_utils.pytest.plugin"
 
+[tool.poetry.group.dev.dependencies]
+pytest = "^7.4.0"
+pytest-asyncio = "^0.21.1"
+pydantic = "^2.1.1"
+coverage = "^7.2.7"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cats-python-4.5.9/wiki/index.md` & `cats_python-4.6.1/wiki/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+!!!WARNING
+This package is deprecated and should not be used. It will continue to exist until fully migrated and will be archived.
+
+THIS PACKAGE MAY BE DELETED. DO NOT USE IT.
+!!!
+
 # Welcome
 
 [![PyPI version](https://badge.fury.io/py/cats-python.svg)](https://badge.fury.io/py/cats-python) [![codecov](https://codecov.io/gh/Cifrazia/cats-python/branch/master/graph/badge.svg?token=MMDPS40REC)](https://codecov.io/gh/Cifrazia/cats-python) [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FCifrazia%2Fcats-python.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FCifrazia%2Fcats-python?ref=badge_shield)
 
 ## Cifrazia Action Transport System
 
 CATS - is a TCP based byte protocol for persistence package exchanging. This so-called protocol is designed specifically
@@ -20,14 +26,11 @@
 + Custom [handshakes](protocol/2.0.md#handshake)
 + ~~Local and global encryption~~
 
 [!ref](get-started.md)
 
 ## Requirements
 
-+ Python `^3.9`
++ Python `3.10`
 + Tornado `^6.1`
-+ Sentry SDK `^1.1.0`
-+ uJSON `^4.0.2`
-+ PyTZ `^2021.1`
-
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FCifrazia%2Fcats-python.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FCifrazia%2Fcats-python?ref=badge_large)
++ uJSON `^5.1`
++ PyTZ `^2023.3`
```

### Comparing `cats-python-4.5.9/PKG-INFO` & `cats_python-4.6.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,61 @@
 Metadata-Version: 2.1
 Name: cats-python
-Version: 4.5.9
+Version: 4.6.1
 Summary: Cifrazia Action Transport System for Python
 Home-page: https://adambrianbright.github.io/cats-python/
 License: MIT
 Keywords: cifrazia,tcp,rpc,cats,tornado
 Author: Bogdan Parfenov
 Author-email: adam.brian.bright@gmail.com
-Requires-Python: >=3.10.0rc2,<4.0
+Requires-Python: >=3.10.0,<3.11
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Framework :: AsyncIO
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Natural Language :: Russian
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Operating System :: OS Independent
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
 Provides-Extra: django
-Provides-Extra: djantic
 Provides-Extra: pydantic
-Requires-Dist: Django (>=2.0,<3.0); extra == "django" or extra == "djantic"
-Requires-Dist: PyYAML (>=5.4.1,<6.0.0)
-Requires-Dist: djangorestframework (>=3.12.4); extra == "django"
-Requires-Dist: djantic (>=0.3.3); extra == "djantic"
-Requires-Dist: msgpack (>=1.0.2,<2.0.0)
-Requires-Dist: pydantic (>=1.8.2); extra == "pydantic" or extra == "djantic"
-Requires-Dist: pytz (>=2021.1,<2022.0)
-Requires-Dist: richerr (>=0.1.1,<0.2.0)
-Requires-Dist: rollbar (>=0.16.2,<0.17.0)
-Requires-Dist: struct-model-python (>=0.1.0,<0.2.0)
+Requires-Dist: Django (>=2.0,<3.0) ; extra == "django"
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: djangorestframework (==3.13) ; extra == "django"
+Requires-Dist: msgpack (>=1.0.3,<2.0.0)
+Requires-Dist: pydantic (>=2.1.0) ; extra == "pydantic"
+Requires-Dist: pytz (>=2023.3,<2024.0)
+Requires-Dist: richerr (>=0.2.3,<0.3.0)
+Requires-Dist: struct-model-python (>=0.1.1,<0.2.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tornado (>=6.1,<7.0)
-Requires-Dist: ujson (>=4.1.0,<5.0.0)
+Requires-Dist: ujson (>=5.1.0,<6.0.0)
 Project-URL: Bug Tracker, https://github.com/AdamBrianBright/cats-python/issues
 Project-URL: ChangeLog, https://adambrianbright.github.io/cats-python/changelog
 Project-URL: Contact Author, https://vk.com/adam_bright
 Project-URL: Documentation, https://adambrianbright.github.io/cats-python/
 Project-URL: Repository, https://github.com/AdamBrianBright/cats-python
 Description-Content-Type: text/markdown
 
+!!!WARNING
+This package is deprecated and should not be used. It will continue to exist until fully migrated and will be archived.
+
+THIS PACKAGE MAY BE DELETED. DO NOT USE IT.
+!!!
+
 # Welcome
 
 [![PyPI version](https://badge.fury.io/py/cats-python.svg)](https://badge.fury.io/py/cats-python) [![codecov](https://codecov.io/gh/Cifrazia/cats-python/branch/master/graph/badge.svg?token=MMDPS40REC)](https://codecov.io/gh/Cifrazia/cats-python) [![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FCifrazia%2Fcats-python.svg?type=shield)](https://app.fossa.com/projects/git%2Bgithub.com%2FCifrazia%2Fcats-python?ref=badge_shield)
 
 ## Cifrazia Action Transport System
 
 CATS - is a TCP based byte protocol for persistence package exchanging. This so-called protocol is designed specifically
@@ -71,14 +74,12 @@
 + Custom [handshakes](protocol/2.0.md#handshake)
 + ~~Local and global encryption~~
 
 [!ref](get-started.md)
 
 ## Requirements
 
-+ Python `^3.9`
++ Python `3.10`
 + Tornado `^6.1`
-+ Sentry SDK `^1.1.0`
-+ uJSON `^4.0.2`
-+ PyTZ `^2021.1`
++ uJSON `^5.1`
++ PyTZ `^2023.3`
 
-[![FOSSA Status](https://app.fossa.com/api/projects/git%2Bgithub.com%2FCifrazia%2Fcats-python.svg?type=large)](https://app.fossa.com/projects/git%2Bgithub.com%2FCifrazia%2Fcats-python?ref=badge_large)
```

