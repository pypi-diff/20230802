# Comparing `tmp/async_rmq_v-0.3.8.tar.gz` & `tmp/async_rmq_v-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_rmq_v-0.3.8.tar", last modified: Wed Aug  2 14:05:56 2023, max compression
+gzip compressed data, was "async_rmq_v-0.3.9.tar", last modified: Wed Aug  2 14:44:33 2023, max compression
```

## Comparing `async_rmq_v-0.3.8.tar` & `async_rmq_v-0.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 14:05:56.165874 async_rmq_v-0.3.8/
--rw-rw-rw-   0        0        0      227 2023-08-02 14:05:56.166904 async_rmq_v-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 14:05:56.134656 async_rmq_v-0.3.8/async_rmq/
--rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.8/async_rmq/_init_.py
--rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.8/async_rmq/abstract_rmq_consumer.py
--rw-rw-rw-   0        0        0     2586 2023-08-02 14:05:43.000000 async_rmq_v-0.3.8/async_rmq/abstract_rmq_rpc_server.py
--rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.8/async_rmq/abtract_rmq_rpc_client.py
--rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.8/async_rmq/consumer_threading.py
--rw-rw-rw-   0        0        0    10893 2023-08-02 13:48:54.000000 async_rmq_v-0.3.8/async_rmq/rmq_functions.py
-drwxrwxrwx   0        0        0        0 2023-08-02 14:05:56.162873 async_rmq_v-0.3.8/async_rmq_v.egg-info/
--rw-rw-rw-   0        0        0      227 2023-08-02 14:05:55.000000 async_rmq_v-0.3.8/async_rmq_v.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-08-02 14:05:56.000000 async_rmq_v-0.3.8/async_rmq_v.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 14:05:55.000000 async_rmq_v-0.3.8/async_rmq_v.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.8/async_rmq_v.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-08-02 14:05:55.000000 async_rmq_v-0.3.8/async_rmq_v.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 14:05:56.176872 async_rmq_v-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-08-02 14:05:49.000000 async_rmq_v-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:44:32.994672 async_rmq_v-0.3.9/
+-rw-rw-rw-   0        0        0      227 2023-08-02 14:44:32.995673 async_rmq_v-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 14:44:32.957205 async_rmq_v-0.3.9/async_rmq/
+-rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.9/async_rmq/_init_.py
+-rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.9/async_rmq/abstract_rmq_consumer.py
+-rw-rw-rw-   0        0        0     2630 2023-08-02 14:42:44.000000 async_rmq_v-0.3.9/async_rmq/abstract_rmq_rpc_server.py
+-rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.9/async_rmq/abtract_rmq_rpc_client.py
+-rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.9/async_rmq/consumer_threading.py
+-rw-rw-rw-   0        0        0    10893 2023-08-02 14:43:12.000000 async_rmq_v-0.3.9/async_rmq/rmq_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:44:32.991671 async_rmq_v-0.3.9/async_rmq_v.egg-info/
+-rw-rw-rw-   0        0        0      227 2023-08-02 14:44:32.000000 async_rmq_v-0.3.9/async_rmq_v.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-08-02 14:44:32.000000 async_rmq_v-0.3.9/async_rmq_v.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 14:44:32.000000 async_rmq_v-0.3.9/async_rmq_v.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.9/async_rmq_v.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-08-02 14:44:32.000000 async_rmq_v-0.3.9/async_rmq_v.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 14:44:32.998753 async_rmq_v-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-08-02 14:44:23.000000 async_rmq_v-0.3.9/setup.py
```

### Comparing `async_rmq_v-0.3.8/README.md` & `async_rmq_v-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.8/async_rmq/abstract_rmq_consumer.py` & `async_rmq_v-0.3.9/async_rmq/abstract_rmq_consumer.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.8/async_rmq/abstract_rmq_rpc_server.py` & `async_rmq_v-0.3.9/async_rmq/abstract_rmq_rpc_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,16 +31,18 @@
 
             async for message in queue_iterator:
 
                 try:
                     async with message.process(requeue=False):
                         assert message.reply_to is not None
                         response = await self.process_message(message)
+
+                        # message.channel.is_closed
                         
-                        if not self.resp_exchange.channel.is_closed:
+                        if not message.channel.is_closed:
                             try:
                                 await self.resp_exchange.publish(
                                     Message(
                                         body=response,
                                         correlation_id=message.correlation_id,
                                     ),
                                     routing_key=message.reply_to,
```

### Comparing `async_rmq_v-0.3.8/async_rmq/abtract_rmq_rpc_client.py` & `async_rmq_v-0.3.9/async_rmq/abtract_rmq_rpc_client.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.8/async_rmq/consumer_threading.py` & `async_rmq_v-0.3.9/async_rmq/consumer_threading.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.8/async_rmq/rmq_functions.py` & `async_rmq_v-0.3.9/async_rmq/rmq_functions.py`

 * *Files identical despite different names*

