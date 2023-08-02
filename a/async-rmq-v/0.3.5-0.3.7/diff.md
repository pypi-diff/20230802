# Comparing `tmp/async_rmq_v-0.3.5.tar.gz` & `tmp/async_rmq_v-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_rmq_v-0.3.5.tar", last modified: Wed Aug  2 13:49:10 2023, max compression
+gzip compressed data, was "async_rmq_v-0.3.7.tar", last modified: Wed Aug  2 14:03:10 2023, max compression
```

## Comparing `async_rmq_v-0.3.5.tar` & `async_rmq_v-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 13:49:10.757158 async_rmq_v-0.3.5/
--rw-rw-rw-   0        0        0      227 2023-08-02 13:49:10.757494 async_rmq_v-0.3.5/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 13:49:10.726999 async_rmq_v-0.3.5/async_rmq/
--rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.5/async_rmq/_init_.py
--rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.5/async_rmq/abstract_rmq_consumer.py
--rw-rw-rw-   0        0        0     2446 2023-08-02 13:46:12.000000 async_rmq_v-0.3.5/async_rmq/abstract_rmq_rpc_server.py
--rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.5/async_rmq/abtract_rmq_rpc_client.py
--rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.5/async_rmq/consumer_threading.py
--rw-rw-rw-   0        0        0    10893 2023-08-02 13:48:54.000000 async_rmq_v-0.3.5/async_rmq/rmq_functions.py
-drwxrwxrwx   0        0        0        0 2023-08-02 13:49:10.752995 async_rmq_v-0.3.5/async_rmq_v.egg-info/
--rw-rw-rw-   0        0        0      227 2023-08-02 13:49:10.000000 async_rmq_v-0.3.5/async_rmq_v.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-08-02 13:49:10.000000 async_rmq_v-0.3.5/async_rmq_v.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 13:49:10.000000 async_rmq_v-0.3.5/async_rmq_v.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.5/async_rmq_v.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-08-02 13:49:10.000000 async_rmq_v-0.3.5/async_rmq_v.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 13:49:10.760995 async_rmq_v-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-08-02 13:49:04.000000 async_rmq_v-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:03:10.826233 async_rmq_v-0.3.7/
+-rw-rw-rw-   0        0        0      227 2023-08-02 14:03:10.826870 async_rmq_v-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 14:03:10.790068 async_rmq_v-0.3.7/async_rmq/
+-rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.7/async_rmq/_init_.py
+-rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.7/async_rmq/abstract_rmq_consumer.py
+-rw-rw-rw-   0        0        0     2605 2023-08-02 14:02:40.000000 async_rmq_v-0.3.7/async_rmq/abstract_rmq_rpc_server.py
+-rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.7/async_rmq/abtract_rmq_rpc_client.py
+-rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.7/async_rmq/consumer_threading.py
+-rw-rw-rw-   0        0        0    10893 2023-08-02 13:48:54.000000 async_rmq_v-0.3.7/async_rmq/rmq_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:03:10.822872 async_rmq_v-0.3.7/async_rmq_v.egg-info/
+-rw-rw-rw-   0        0        0      227 2023-08-02 14:03:10.000000 async_rmq_v-0.3.7/async_rmq_v.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-08-02 14:03:10.000000 async_rmq_v-0.3.7/async_rmq_v.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 14:03:10.000000 async_rmq_v-0.3.7/async_rmq_v.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.7/async_rmq_v.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-08-02 14:03:10.000000 async_rmq_v-0.3.7/async_rmq_v.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 14:03:10.830875 async_rmq_v-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-08-02 14:03:06.000000 async_rmq_v-0.3.7/setup.py
```

### Comparing `async_rmq_v-0.3.5/README.md` & `async_rmq_v-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.5/async_rmq/abstract_rmq_consumer.py` & `async_rmq_v-0.3.7/async_rmq/abstract_rmq_consumer.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.5/async_rmq/abstract_rmq_rpc_server.py` & `async_rmq_v-0.3.7/async_rmq/abstract_rmq_rpc_server.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,24 +31,25 @@
 
             async for message in queue_iterator:
 
                 try:
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
                         response = await self.process_message(message)
+                        logger.info("CHECK channel before response publish, channel closed: %s" % ("T" if self.resp_exchange.channel.is_closed else "F"))
                         try:
                             await self.resp_exchange.publish(
                                 Message(
                                     body=response,
                                     correlation_id=message.correlation_id,
                                 ),
                                 routing_key=message.reply_to,
                             )
                         except Exception as err:
-                            logger.warning('Couldnt sent response message for some reason %s, %s' % (type(err).__name__, err.__format__))
+                            logger.warning('Couldnt sent response message for some reason %s, %s' % (type(err).__name__, err.__format__("")))
 
                 except asyncio.exceptions.TimeoutError:
                     await self.on_finish()
 
                     if self.consuming_flag:
                         await asyncio.sleep(self.iterator_timeout_sleep)
```

### Comparing `async_rmq_v-0.3.5/async_rmq/abtract_rmq_rpc_client.py` & `async_rmq_v-0.3.7/async_rmq/abtract_rmq_rpc_client.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.5/async_rmq/consumer_threading.py` & `async_rmq_v-0.3.7/async_rmq/consumer_threading.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.5/async_rmq/rmq_functions.py` & `async_rmq_v-0.3.7/async_rmq/rmq_functions.py`

 * *Files identical despite different names*

