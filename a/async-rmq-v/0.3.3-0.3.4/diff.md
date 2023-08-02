# Comparing `tmp/async_rmq_v-0.3.3.tar.gz` & `tmp/async_rmq_v-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_rmq_v-0.3.3.tar", last modified: Wed Aug  2 10:39:19 2023, max compression
+gzip compressed data, was "async_rmq_v-0.3.4.tar", last modified: Wed Aug  2 13:25:45 2023, max compression
```

## Comparing `async_rmq_v-0.3.3.tar` & `async_rmq_v-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 10:39:19.688300 async_rmq_v-0.3.3/
--rw-rw-rw-   0        0        0      227 2023-08-02 10:39:19.690051 async_rmq_v-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 10:39:19.618391 async_rmq_v-0.3.3/async_rmq/
--rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.3/async_rmq/_init_.py
--rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.3/async_rmq/abstract_rmq_consumer.py
--rw-rw-rw-   0        0        0     2199 2023-08-02 00:16:28.000000 async_rmq_v-0.3.3/async_rmq/abstract_rmq_rpc_server.py
--rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.3/async_rmq/abtract_rmq_rpc_client.py
--rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.3/async_rmq/consumer_threading.py
--rw-rw-rw-   0        0        0    10587 2023-08-02 10:37:56.000000 async_rmq_v-0.3.3/async_rmq/rmq_functions.py
-drwxrwxrwx   0        0        0        0 2023-08-02 10:39:19.683972 async_rmq_v-0.3.3/async_rmq_v.egg-info/
--rw-rw-rw-   0        0        0      227 2023-08-02 10:39:19.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-08-02 10:39:19.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 10:39:19.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-08-02 10:39:19.000000 async_rmq_v-0.3.3/async_rmq_v.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 10:39:19.715665 async_rmq_v-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-08-02 10:38:31.000000 async_rmq_v-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:25:45.044138 async_rmq_v-0.3.4/
+-rw-rw-rw-   0        0        0      227 2023-08-02 13:25:45.045417 async_rmq_v-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 13:25:45.010138 async_rmq_v-0.3.4/async_rmq/
+-rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.4/async_rmq/_init_.py
+-rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.4/async_rmq/abstract_rmq_consumer.py
+-rw-rw-rw-   0        0        0     2199 2023-08-02 00:16:28.000000 async_rmq_v-0.3.4/async_rmq/abstract_rmq_rpc_server.py
+-rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.4/async_rmq/abtract_rmq_rpc_client.py
+-rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.4/async_rmq/consumer_threading.py
+-rw-rw-rw-   0        0        0    10545 2023-08-02 13:25:00.000000 async_rmq_v-0.3.4/async_rmq/rmq_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:25:45.041181 async_rmq_v-0.3.4/async_rmq_v.egg-info/
+-rw-rw-rw-   0        0        0      227 2023-08-02 13:25:44.000000 async_rmq_v-0.3.4/async_rmq_v.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-08-02 13:25:44.000000 async_rmq_v-0.3.4/async_rmq_v.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:25:44.000000 async_rmq_v-0.3.4/async_rmq_v.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.4/async_rmq_v.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-08-02 13:25:44.000000 async_rmq_v-0.3.4/async_rmq_v.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 13:25:45.054744 async_rmq_v-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-08-02 13:25:32.000000 async_rmq_v-0.3.4/setup.py
```

### Comparing `async_rmq_v-0.3.3/README.md` & `async_rmq_v-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.3/async_rmq/abstract_rmq_consumer.py` & `async_rmq_v-0.3.4/async_rmq/abstract_rmq_consumer.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.3/async_rmq/abstract_rmq_rpc_server.py` & `async_rmq_v-0.3.4/async_rmq/abstract_rmq_rpc_server.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.3/async_rmq/abtract_rmq_rpc_client.py` & `async_rmq_v-0.3.4/async_rmq/abtract_rmq_rpc_client.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.3/async_rmq/consumer_threading.py` & `async_rmq_v-0.3.4/async_rmq/consumer_threading.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.3/async_rmq/rmq_functions.py` & `async_rmq_v-0.3.4/async_rmq/rmq_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -114,17 +114,18 @@
         consumer = consumer_class(
             queue=queue
         )
 
         try:
             await consumer.consume()
         except Exception as err:
-            logger.info("GOT EXCEPTION WHILE consuming. reconnecting " + ("T" if rabbitmq_connection.reconnecting else "F"))
             logger.info("GOT EXCEPTION WHILE consuming. err type " + type(err).__name__)
             logger.info("GOT EXCEPTION WHILE consuming. err " + err.__format__(""))
+            consumer.stop_consuming()
+            raise err
 
     logger.info("Shutdown complete")
     await rabbitmq_connection.close()
 
 # Running a consumer
 async def run_rpc_server(rpc_server_class: RPCRabbitMQServer,
                          resp_exchange_name: str,
@@ -207,15 +208,16 @@
 async def get_rmq_connection(host: str, port: int, login: str, password: str, vhost: str, loop: Optional[asyncio.AbstractEventLoop] = None):
     connection = await aio_pika.connect_robust(
         host=host,
         port=port,
         login=login,
         password=password,
         virtualhost=vhost,
-        loop=loop
+        loop=loop,
+        timeout=200
     )
     return connection
 
 
 def get_exchange_type(s):
     if s == ExchangeType.DIRECT.value:
         return ExchangeType.DIRECT
```

