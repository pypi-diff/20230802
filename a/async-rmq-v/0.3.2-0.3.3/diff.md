# Comparing `tmp/async_rmq_v-0.3.2.tar.gz` & `tmp/async_rmq_v-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_rmq_v-0.3.2.tar", last modified: Wed Aug  2 00:48:37 2023, max compression
+gzip compressed data, was "async_rmq_v-0.3.3.tar", last modified: Wed Aug  2 10:39:19 2023, max compression
```

## Comparing `async_rmq_v-0.3.2.tar` & `async_rmq_v-0.3.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 00:48:37.728464 async_rmq_v-0.3.2/
--rw-rw-rw-   0        0        0      227 2023-08-02 00:48:37.729462 async_rmq_v-0.3.2/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 00:48:37.698466 async_rmq_v-0.3.2/async_rmq/
--rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.2/async_rmq/_init_.py
--rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.2/async_rmq/abstract_rmq_consumer.py
--rw-rw-rw-   0        0        0     2199 2023-08-02 00:16:28.000000 async_rmq_v-0.3.2/async_rmq/abstract_rmq_rpc_server.py
--rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.2/async_rmq/abtract_rmq_rpc_client.py
--rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.2/async_rmq/consumer_threading.py
--rw-rw-rw-   0        0        0    10297 2023-08-02 00:28:43.000000 async_rmq_v-0.3.2/async_rmq/rmq_functions.py
-drwxrwxrwx   0        0        0        0 2023-08-02 00:48:37.725468 async_rmq_v-0.3.2/async_rmq_v.egg-info/
--rw-rw-rw-   0        0        0      227 2023-08-02 00:48:37.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-08-02 00:48:37.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 00:48:37.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-08-02 00:48:37.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 00:48:37.735463 async_rmq_v-0.3.2/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-08-02 00:48:25.000000 async_rmq_v-0.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:39:19.688300 async_rmq_v-0.3.3/
+-rw-rw-rw-   0        0        0      227 2023-08-02 10:39:19.690051 async_rmq_v-0.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 10:39:19.618391 async_rmq_v-0.3.3/async_rmq/
+-rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.3/async_rmq/_init_.py
+-rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.3/async_rmq/abstract_rmq_consumer.py
+-rw-rw-rw-   0        0        0     2199 2023-08-02 00:16:28.000000 async_rmq_v-0.3.3/async_rmq/abstract_rmq_rpc_server.py
+-rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.3/async_rmq/abtract_rmq_rpc_client.py
+-rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.3/async_rmq/consumer_threading.py
+-rw-rw-rw-   0        0        0    10587 2023-08-02 10:37:56.000000 async_rmq_v-0.3.3/async_rmq/rmq_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:39:19.683972 async_rmq_v-0.3.3/async_rmq_v.egg-info/
+-rw-rw-rw-   0        0        0      227 2023-08-02 10:39:19.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-08-02 10:39:19.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:39:19.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-08-02 10:39:19.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 10:39:19.715665 async_rmq_v-0.3.3/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-08-02 10:38:31.000000 async_rmq_v-0.3.3/setup.py
```

### Comparing `async_rmq_v-0.3.2/README.md` & `async_rmq_v-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.2/async_rmq/abstract_rmq_consumer.py` & `async_rmq_v-0.3.3/async_rmq/abstract_rmq_consumer.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.2/async_rmq/abstract_rmq_rpc_server.py` & `async_rmq_v-0.3.3/async_rmq/abstract_rmq_rpc_server.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.2/async_rmq/abtract_rmq_rpc_client.py` & `async_rmq_v-0.3.3/async_rmq/abtract_rmq_rpc_client.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.2/async_rmq/consumer_threading.py` & `async_rmq_v-0.3.3/async_rmq/consumer_threading.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.2/async_rmq/rmq_functions.py` & `async_rmq_v-0.3.3/async_rmq/rmq_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,15 +110,21 @@
                                               queue_params,
                                               exchange_params,
                                               dl_enabled,
                                               dl_exchange_name)
         consumer = consumer_class(
             queue=queue
         )
-        await consumer.consume()
+
+        try:
+            await consumer.consume()
+        except Exception as err:
+            logger.info("GOT EXCEPTION WHILE consuming. reconnecting " + ("T" if rabbitmq_connection.reconnecting else "F"))
+            logger.info("GOT EXCEPTION WHILE consuming. err type " + type(err).__name__)
+            logger.info("GOT EXCEPTION WHILE consuming. err " + err.__format__(""))
 
     logger.info("Shutdown complete")
     await rabbitmq_connection.close()
 
 # Running a consumer
 async def run_rpc_server(rpc_server_class: RPCRabbitMQServer,
                          resp_exchange_name: str,
@@ -136,17 +142,16 @@
                          dl_enabled: Optional[bool] = False,
                          dl_queue_name: Optional[str] = None,
                          dl_queue_params: Optional[dict] = {},
                          dl_exchange_name: Optional[str] = None,
                          dl_exchange_type: Optional[str] = None,
                          dl_exchange_params: Optional[dict] = {},
                          dl_bindings: Optional[list] = []) -> None:
-    # loop = asyncio.get_event_loop()
-    # rabbitmq_connection = await get_rmq_connection(host, port, login, password, vhost, loop)
-    rabbitmq_connection = await get_rmq_connection(host, port, login, password, vhost)
+    loop = asyncio.get_event_loop()
+    rabbitmq_connection = await get_rmq_connection(host, port, login, password, vhost, loop)
 
     async with rabbitmq_connection.channel() as channel:
         await channel.set_qos(prefetch_count=1)
 
         if dl_enabled:
             dead_letter_queue, dead_letter_exchange = await _prepare_dead_letter_queue(channel,
                                                                                        dl_queue_name,
@@ -195,15 +200,15 @@
                 routing_key=routing_key
             )
 
         except ChannelNotFoundEntity:
             logger.warning("The message could not be sent because the exchange with the name '%s' was not found"
                            % exchange_name)
 
-async def get_rmq_connection(host: str, port: int, login: str, password: str, vhost: str, loop: Optional = None):
+async def get_rmq_connection(host: str, port: int, login: str, password: str, vhost: str, loop: Optional[asyncio.AbstractEventLoop] = None):
     connection = await aio_pika.connect_robust(
         host=host,
         port=port,
         login=login,
         password=password,
         virtualhost=vhost,
         loop=loop
```

