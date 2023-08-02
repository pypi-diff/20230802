# Comparing `tmp/async_rmq_v-0.3.1.tar.gz` & `tmp/async_rmq_v-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_rmq_v-0.3.1.tar", last modified: Wed Aug  2 00:35:05 2023, max compression
+gzip compressed data, was "async_rmq_v-0.3.2.tar", last modified: Wed Aug  2 00:48:37 2023, max compression
```

## Comparing `async_rmq_v-0.3.1.tar` & `async_rmq_v-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 00:35:05.480197 async_rmq_v-0.3.1/
--rw-rw-rw-   0        0        0      227 2023-08-02 00:35:05.481197 async_rmq_v-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 00:35:05.441198 async_rmq_v-0.3.1/async_rmq/
--rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.1/async_rmq/_init_.py
--rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.1/async_rmq/abstract_rmq_consumer.py
--rw-rw-rw-   0        0        0     2199 2023-08-02 00:16:28.000000 async_rmq_v-0.3.1/async_rmq/abstract_rmq_rpc_server.py
--rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.1/async_rmq/abtract_rmq_rpc_client.py
--rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.1/async_rmq/consumer_threading.py
--rw-rw-rw-   0        0        0    10297 2023-08-02 00:28:43.000000 async_rmq_v-0.3.1/async_rmq/rmq_functions.py
-drwxrwxrwx   0        0        0        0 2023-08-02 00:35:05.477201 async_rmq_v-0.3.1/async_rmq_v.egg-info/
--rw-rw-rw-   0        0        0      227 2023-08-02 00:35:05.000000 async_rmq_v-0.3.1/async_rmq_v.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      389 2023-08-02 00:35:05.000000 async_rmq_v-0.3.1/async_rmq_v.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 00:35:05.000000 async_rmq_v-0.3.1/async_rmq_v.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 00:34:17.000000 async_rmq_v-0.3.1/async_rmq_v.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       10 2023-08-02 00:35:05.000000 async_rmq_v-0.3.1/async_rmq_v.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 00:35:05.498206 async_rmq_v-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0      254 2023-08-02 00:34:13.000000 async_rmq_v-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 00:48:37.728464 async_rmq_v-0.3.2/
+-rw-rw-rw-   0        0        0      227 2023-08-02 00:48:37.729462 async_rmq_v-0.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1039 2023-07-12 20:12:09.000000 async_rmq_v-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 00:48:37.698466 async_rmq_v-0.3.2/async_rmq/
+-rw-rw-rw-   0        0        0        0 2023-07-12 20:12:09.000000 async_rmq_v-0.3.2/async_rmq/_init_.py
+-rw-rw-rw-   0        0        0     2439 2023-08-01 23:25:28.000000 async_rmq_v-0.3.2/async_rmq/abstract_rmq_consumer.py
+-rw-rw-rw-   0        0        0     2199 2023-08-02 00:16:28.000000 async_rmq_v-0.3.2/async_rmq/abstract_rmq_rpc_server.py
+-rw-rw-rw-   0        0        0     2638 2023-08-01 23:26:38.000000 async_rmq_v-0.3.2/async_rmq/abtract_rmq_rpc_client.py
+-rw-rw-rw-   0        0        0     1956 2023-08-01 23:26:38.000000 async_rmq_v-0.3.2/async_rmq/consumer_threading.py
+-rw-rw-rw-   0        0        0    10297 2023-08-02 00:28:43.000000 async_rmq_v-0.3.2/async_rmq/rmq_functions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 00:48:37.725468 async_rmq_v-0.3.2/async_rmq_v.egg-info/
+-rw-rw-rw-   0        0        0      227 2023-08-02 00:48:37.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      389 2023-08-02 00:48:37.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 00:48:37.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 00:45:46.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       10 2023-08-02 00:48:37.000000 async_rmq_v-0.3.2/async_rmq_v.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 00:48:37.735463 async_rmq_v-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      254 2023-08-02 00:48:25.000000 async_rmq_v-0.3.2/setup.py
```

### Comparing `async_rmq_v-0.3.1/README.md` & `async_rmq_v-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.1/async_rmq/abstract_rmq_consumer.py` & `async_rmq_v-0.3.2/async_rmq/abstract_rmq_consumer.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.1/async_rmq/abstract_rmq_rpc_server.py` & `async_rmq_v-0.3.2/async_rmq/abstract_rmq_rpc_server.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.1/async_rmq/abtract_rmq_rpc_client.py` & `async_rmq_v-0.3.2/async_rmq/abtract_rmq_rpc_client.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.1/async_rmq/consumer_threading.py` & `async_rmq_v-0.3.2/async_rmq/consumer_threading.py`

 * *Files identical despite different names*

### Comparing `async_rmq_v-0.3.1/async_rmq/rmq_functions.py` & `async_rmq_v-0.3.2/async_rmq/rmq_functions.py`

 * *Files identical despite different names*

