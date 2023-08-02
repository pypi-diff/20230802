# Comparing `tmp/pyensign-0.7b0.tar.gz` & `tmp/pyensign-0.8b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyensign-0.7b0.tar", last modified: Wed May 31 20:40:58 2023, max compression
+gzip compressed data, was "dist/pyensign-0.8b0.tar", last modified: Wed Aug  2 13:29:29 2023, max compression
```

## Comparing `pyensign-0.7b0.tar` & `pyensign-0.8b0.tar`

### file list

```diff
@@ -1,54 +1,62 @@
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.854409 pyensign-0.7b0/
--rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-05-16 21:00:20.000000 pyensign-0.7b0/CONTRIBUTING.md
--rw-r--r--   0 patrick    (501) staff       (20)     2360 2023-05-31 19:58:09.000000 pyensign-0.7b0/DESCRIPTION.md
--rw-r--r--   0 patrick    (501) staff       (20)      180 2023-05-16 21:00:20.000000 pyensign-0.7b0/MANIFEST.in
--rw-r--r--   0 patrick    (501) staff       (20)      394 2023-05-16 21:00:20.000000 pyensign-0.7b0/Makefile
--rw-r--r--   0 patrick    (501) staff       (20)     3752 2023-05-31 20:40:58.854558 pyensign-0.7b0/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     4329 2023-05-31 19:58:28.000000 pyensign-0.7b0/README.md
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.846230 pyensign-0.7b0/pyensign/
--rw-r--r--   0 patrick    (501) staff       (20)      507 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.848027 pyensign-0.7b0/pyensign/api/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.850724 pyensign-0.7b0/pyensign/api/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7865 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)    19552 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
--rw-r--r--   0 patrick    (501) staff       (20)      786 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/event.py
--rw-r--r--   0 patrick    (501) staff       (20)     7539 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/api/v1beta1/event_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/groups_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     4416 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/api/v1beta1/topic_pb2.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.851841 pyensign-0.7b0/pyensign/auth/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     3937 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/client.py
--rw-r--r--   0 patrick    (501) staff       (20)      347 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/auth/tokens.py
--rw-r--r--   0 patrick    (501) staff       (20)    11976 2023-05-31 18:56:39.000000 pyensign-0.7b0/pyensign/connection.py
--rw-r--r--   0 patrick    (501) staff       (20)    10517 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/ensign.py
--rw-r--r--   0 patrick    (501) staff       (20)     1905 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/events.py
--rw-r--r--   0 patrick    (501) staff       (20)     3601 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/exceptions.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852166 pyensign-0.7b0/pyensign/mimetype/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852581 pyensign-0.7b0/pyensign/mimetype/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
--rw-r--r--   0 patrick    (501) staff       (20)     5383 2023-05-31 15:33:48.000000 pyensign-0.7b0/pyensign/mimetypes.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.852880 pyensign-0.7b0/pyensign/region/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/__init__.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.853269 pyensign-0.7b0/pyensign/region/v1beta1/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/v1beta1/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)     7945 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/region/v1beta1/region_pb2.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.854128 pyensign-0.7b0/pyensign/utils/
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-31 18:56:39.000000 pyensign-0.7b0/pyensign/utils/__init__.py
--rw-r--r--   0 patrick    (501) staff       (20)      983 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyensign/utils/cache.py
--rw-r--r--   0 patrick    (501) staff       (20)     1089 2023-05-31 15:33:49.000000 pyensign-0.7b0/pyensign/utils/tasks.py
--rw-r--r--   0 patrick    (501) staff       (20)      964 2023-05-31 19:17:18.000000 pyensign-0.7b0/pyensign/version.py
-drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-05-31 20:40:58.847769 pyensign-0.7b0/pyensign.egg-info/
--rw-r--r--   0 patrick    (501) staff       (20)     3752 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/PKG-INFO
--rw-r--r--   0 patrick    (501) staff       (20)     1076 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/SOURCES.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/dependency_links.txt
--rw-r--r--   0 patrick    (501) staff       (20)        1 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/not-zip-safe
--rw-r--r--   0 patrick    (501) staff       (20)       89 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/requires.txt
--rw-r--r--   0 patrick    (501) staff       (20)        9 2023-05-31 20:40:58.000000 pyensign-0.7b0/pyensign.egg-info/top_level.txt
--rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.7b0/pyproject.toml
--rw-r--r--   0 patrick    (501) staff       (20)       88 2023-05-31 18:56:39.000000 pyensign-0.7b0/requirements.txt
--rw-r--r--   0 patrick    (501) staff       (20)       38 2023-05-31 20:40:58.854916 pyensign-0.7b0/setup.cfg
--rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-05-16 21:00:20.000000 pyensign-0.7b0/setup.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.696667 pyensign-0.8b0/
+-rw-r--r--   0 patrick    (501) staff       (20)    10536 2023-05-16 21:00:20.000000 pyensign-0.8b0/CONTRIBUTING.md
+-rw-r--r--   0 patrick    (501) staff       (20)     2265 2023-07-14 17:39:51.000000 pyensign-0.8b0/DESCRIPTION.md
+-rw-r--r--   0 patrick    (501) staff       (20)      180 2023-05-16 21:00:20.000000 pyensign-0.8b0/MANIFEST.in
+-rw-r--r--   0 patrick    (501) staff       (20)      394 2023-05-16 21:00:20.000000 pyensign-0.8b0/Makefile
+-rw-r--r--   0 patrick    (501) staff       (20)     3657 2023-08-02 13:29:29.696819 pyensign-0.8b0/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     5605 2023-07-27 19:02:28.000000 pyensign-0.8b0/README.md
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.689160 pyensign-0.8b0/pyensign/
+-rw-r--r--   0 patrick    (501) staff       (20)      507 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.690847 pyensign-0.8b0/pyensign/api/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/api/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.692545 pyensign-0.8b0/pyensign/api/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/api/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7865 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/api/v1beta1/ensign_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)    19552 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/api/v1beta1/ensign_pb2_grpc.py
+-rw-r--r--   0 patrick    (501) staff       (20)      809 2023-06-20 18:33:01.000000 pyensign-0.8b0/pyensign/api/v1beta1/event.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7539 2023-05-31 15:33:48.000000 pyensign-0.8b0/pyensign/api/v1beta1/event_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2367 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/api/v1beta1/groups_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4416 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/api/v1beta1/topic_pb2.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.693949 pyensign-0.8b0/pyensign/auth/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/auth/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5262 2023-08-02 13:23:09.000000 pyensign-0.8b0/pyensign/auth/client.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2053 2023-07-31 21:26:18.000000 pyensign-0.8b0/pyensign/auth/interceptor.py
+-rw-r--r--   0 patrick    (501) staff       (20)      347 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/auth/tokens.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10644 2023-07-31 21:26:18.000000 pyensign-0.8b0/pyensign/connection.py
+-rw-r--r--   0 patrick    (501) staff       (20)    15390 2023-07-27 19:02:28.000000 pyensign-0.8b0/pyensign/ensign.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6362 2023-07-27 19:04:33.000000 pyensign-0.8b0/pyensign/events.py
+-rw-r--r--   0 patrick    (501) staff       (20)     6047 2023-07-31 17:23:40.000000 pyensign-0.8b0/pyensign/exceptions.py
+-rw-r--r--   0 patrick    (501) staff       (20)     4112 2023-07-20 22:03:03.000000 pyensign-0.8b0/pyensign/iterator.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.694210 pyensign-0.8b0/pyensign/mimetype/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/mimetype/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.694595 pyensign-0.8b0/pyensign/mimetype/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/mimetype/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2376 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/mimetype/v1beta1/mimetype_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)     5383 2023-05-31 15:33:48.000000 pyensign-0.8b0/pyensign/mimetypes.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1031 2023-07-27 21:08:34.000000 pyensign-0.8b0/pyensign/nack.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2418 2023-07-27 19:02:28.000000 pyensign-0.8b0/pyensign/publisher.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.694853 pyensign-0.8b0/pyensign/region/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/region/__init__.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.695262 pyensign-0.8b0/pyensign/region/v1beta1/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/region/v1beta1/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     7945 2023-05-16 21:00:20.000000 pyensign-0.8b0/pyensign/region/v1beta1/region_pb2.py
+-rw-r--r--   0 patrick    (501) staff       (20)    10993 2023-07-20 22:30:43.000000 pyensign-0.8b0/pyensign/stream.py
+-rw-r--r--   0 patrick    (501) staff       (20)     2092 2023-07-27 19:02:28.000000 pyensign-0.8b0/pyensign/subscriber.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.696450 pyensign-0.8b0/pyensign/utils/
+-rw-r--r--   0 patrick    (501) staff       (20)        0 2023-05-31 18:56:39.000000 pyensign-0.8b0/pyensign/utils/__init__.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1454 2023-06-28 21:07:54.000000 pyensign-0.8b0/pyensign/utils/cache.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1542 2023-07-20 22:16:22.000000 pyensign-0.8b0/pyensign/utils/queue.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1089 2023-07-20 22:16:39.000000 pyensign-0.8b0/pyensign/utils/tasks.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1297 2023-06-28 21:07:54.000000 pyensign-0.8b0/pyensign/utils/topics.py
+-rw-r--r--   0 patrick    (501) staff       (20)     1108 2023-08-02 13:27:17.000000 pyensign-0.8b0/pyensign/version.py
+drwxr-xr-x   0 patrick    (501) staff       (20)        0 2023-08-02 13:29:29.690604 pyensign-0.8b0/pyensign.egg-info/
+-rw-r--r--   0 patrick    (501) staff       (20)     3657 2023-08-02 13:29:29.000000 pyensign-0.8b0/pyensign.egg-info/PKG-INFO
+-rw-r--r--   0 patrick    (501) staff       (20)     1256 2023-08-02 13:29:29.000000 pyensign-0.8b0/pyensign.egg-info/SOURCES.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-08-02 13:29:29.000000 pyensign-0.8b0/pyensign.egg-info/dependency_links.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        1 2023-08-02 13:29:29.000000 pyensign-0.8b0/pyensign.egg-info/not-zip-safe
+-rw-r--r--   0 patrick    (501) staff       (20)       64 2023-08-02 13:29:29.000000 pyensign-0.8b0/pyensign.egg-info/requires.txt
+-rw-r--r--   0 patrick    (501) staff       (20)        9 2023-08-02 13:29:29.000000 pyensign-0.8b0/pyensign.egg-info/top_level.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       47 2023-06-20 18:33:01.000000 pyensign-0.8b0/pyproject.toml
+-rw-r--r--   0 patrick    (501) staff       (20)       63 2023-06-20 18:33:01.000000 pyensign-0.8b0/requirements.txt
+-rw-r--r--   0 patrick    (501) staff       (20)       38 2023-08-02 13:29:29.697169 pyensign-0.8b0/setup.cfg
+-rw-r--r--   0 patrick    (501) staff       (20)     4023 2023-05-16 21:00:20.000000 pyensign-0.8b0/setup.py
```

### Comparing `pyensign-0.7b0/CONTRIBUTING.md` & `pyensign-0.8b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/DESCRIPTION.md` & `pyensign-0.8b0/DESCRIPTION.md`

 * *Files 14% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 
 ```python
 await client.publish("weather", event)
 await client.publish("weather", event1, event2)
 await client.publish("weather", [event1, event2])
 ```
 
-Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
+Subscribe to one or more topics by providing the topic name(s) or ID(s).
 
 ```python
-topic_id = await client.topic_id("weather")
-async for event in client.subscribe(topic_id):
-    print("Received event: {}".format(event))
+async for event in client.subscribe("weather"):
+    print("Received event with data: {}".format(event.data))
+    event.ack()
 ```
 
 ## Advanced Usage
 
 The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
 
 ```python
 async def handle_ack(self, ack):
     ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
     print(f"Event committed at {ts}")
 
 async def handle_nack(self, nack):
     print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
 
-await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
+await client.publish("weather", event, on_ack=handle_ack, on_nack=handle_nack)
 ```
```

### Comparing `pyensign-0.7b0/PKG-INFO` & `pyensign-0.8b0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.7b0
+Version: 0.8b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7b0
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.8b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
@@ -41,35 +41,35 @@
         
         ```python
         await client.publish("weather", event)
         await client.publish("weather", event1, event2)
         await client.publish("weather", [event1, event2])
         ```
         
-        Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
+        Subscribe to one or more topics by providing the topic name(s) or ID(s).
         
         ```python
-        topic_id = await client.topic_id("weather")
-        async for event in client.subscribe(topic_id):
-            print("Received event: {}".format(event))
+        async for event in client.subscribe("weather"):
+            print("Received event with data: {}".format(event.data))
+            event.ack()
         ```
         
         ## Advanced Usage
         
         The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
         
         ```python
         async def handle_ack(self, ack):
             ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
             print(f"Event committed at {ts}")
         
         async def handle_nack(self, nack):
             print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
         
-        await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
+        await client.publish("weather", event, on_ack=handle_ack, on_nack=handle_nack)
         ```
 Keywords: python,setup,pypi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

### Comparing `pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2.py` & `pyensign-0.8b0/pyensign/api/v1beta1/ensign_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/api/v1beta1/ensign_pb2_grpc.py` & `pyensign-0.8b0/pyensign/api/v1beta1/ensign_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/api/v1beta1/event.py` & `pyensign-0.8b0/pyensign/api/v1beta1/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if not isinstance(event, event_pb2.Event):
         raise TypeError("event must be a protobuf event")
 
     if not isinstance(topic_id, ULID):
         raise TypeError("topic_id must be a ULID")
 
     return event_pb2.EventWrapper(
-        event=event.SerializeToString(), topic_id=topic_id.bytes
+        local_id=ULID().bytes, event=event.SerializeToString(), topic_id=topic_id.bytes
     )
 
 
 def unwrap(event_wrapper):
     """
     Unwrap an event from an EventWrapper.
     """
```

### Comparing `pyensign-0.7b0/pyensign/api/v1beta1/event_pb2.py` & `pyensign-0.8b0/pyensign/api/v1beta1/event_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/api/v1beta1/groups_pb2.py` & `pyensign-0.8b0/pyensign/api/v1beta1/groups_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/api/v1beta1/topic_pb2.py` & `pyensign-0.8b0/pyensign/api/v1beta1/topic_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/connection.py` & `pyensign-0.8b0/pyensign/connection.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,26 @@
 import grpc
 import asyncio
+from ulid import ULID
 from grpc import aio
+from datetime import timedelta
 
 from pyensign.api.v1beta1 import topic_pb2
 from pyensign.api.v1beta1 import ensign_pb2
 from pyensign.utils.tasks import WorkerPool
-from pyensign.api.v1beta1 import ensign_pb2_grpc
 from pyensign.exceptions import catch_rpc_error
-from pyensign.api.v1beta1.event import wrap, unwrap
-from pyensign.exceptions import EnsignError, EnsignTypeError
+from pyensign.api.v1beta1 import ensign_pb2_grpc
+from pyensign.auth.interceptor import (
+    MetadataUnaryInterceptor,
+    MetadataStreamInterceptor,
+)
+from pyensign.stream import Publisher, Subscriber
+from pyensign.exceptions import (
+    EnsignClientClosingError,
+)
 
 
 class Connection:
     """
     Connection defines a gRPC connection to an Ensign server.
     """
 
@@ -30,294 +38,275 @@
         auth : grpc.AuthMetadataPlugin or None
             Plugin that provides an access token for per-request authentication.
         """
 
         addrParts = addrport.split(":", 2)
         if len(addrParts) != 2 or not addrParts[0] or not addrParts[1]:
             raise ValueError("Invalid address:port format")
+        self.addrport = addrport
+
+        self.insecure = insecure
+        self.auth = auth
+
+    def create_channel(self):
+        """
+        Create a new gRPC channel from the connection parameters. The caller is
+        responsible for closing the channel.
+        """
+
+        interceptors = []
+        if self.auth is not None:
+            creds_fn = self.auth.credentials
+            interceptors.append(MetadataUnaryInterceptor(creds_fn))
+            interceptors.append(MetadataStreamInterceptor(creds_fn))
 
-        if insecure:
-            if auth is not None:
-                raise ValueError("Cannot use auth with insecure=True")
-            self.channel = aio.insecure_channel(addrport)
+        if self.insecure:
+            channel = aio.insecure_channel(self.addrport, interceptors=interceptors)
         else:
-            credentials = grpc.ssl_channel_credentials()
-            if auth is not None:
-                call_credentials = grpc.metadata_call_credentials(
-                    auth, name="auth gateway"
-                )
-                credentials = grpc.composite_channel_credentials(
-                    credentials, call_credentials
-                )
-            self.channel = aio.secure_channel(addrport, credentials)
+            channel = aio.secure_channel(
+                self.addrport,
+                credentials=grpc.ssl_channel_credentials(),
+                interceptors=interceptors,
+            )
+
+        return channel
 
 
 class Client:
     """
-    Client defines a high level client that makes requests to an Ensign server.
+    Client defines the actual gRPC client that makes requests to an Ensign server.
     """
 
-    def __init__(self, connection):
+    def __init__(
+        self,
+        connection,
+        client_id="",
+        topic_cache=None,
+        reconnect_tick=timedelta(milliseconds=750),
+        reconnect_timeout=timedelta(minutes=5),
+    ):
         """
-        Create a new client from an established connection.
+        Create a new client for making requests to Ensign. The connection is not
+        established until the connect() method is called.
 
         Parameters
         ----------
         connection : Connection
             The connection to the Ensign server
         """
 
-        self.channel = connection.channel
-        self.stub = ensign_pb2_grpc.EnsignStub(self.channel)
-        self.publish_streams = {}
-        self.subscribe_streams = {}
-        self.pool = WorkerPool(max_workers=10, max_queue_size=100)
+        self.connection = connection
+        self.channel = None
+        self.publishers = {}
+        self.subscribers = {}
+        self.pool = None
+        self.topics = topic_cache
+        self.reconnect_tick = reconnect_tick
+        self.reconnect_timeout = reconnect_timeout
+        self.shutdown = None
+
+        # Create client ID if not provided, which exists for the lifetime of the client
+        # and persists across reconnects
+        if client_id == "":
+            self.client_id = str(ULID())
+        else:
+            self.client_id = client_id
+
+    def _ensure_ready(self):
+        """
+        Create the gRPC channel and stub if not already connected. This is done at call
+        time rather than when the client is created to ensure that user code runs in
+        the same event loop as the gRPC library. This function also creates the worker
+        pool and shutdown event signal if not already created.
+        TODO: We could avoid this by requiring the Ensign client to be created in the
+        event loop, e.g. async with Client(...) as client: ..., but the current syntax
+        is a bit easier.
+        """
+
+        if not self.channel:
+            self.channel = self.connection.create_channel()
+            self.stub = ensign_pb2_grpc.EnsignStub(self.channel)
+
+        if not self.pool:
+            self.pool = WorkerPool(max_workers=10, max_queue_size=100)
+
+        if not self.shutdown:
+            self.shutdown = asyncio.Event()
 
     @catch_rpc_error
-    async def publish(
-        self, topic_id, events, ack_callback=None, nack_callback=None, client_id=""
-    ):
-        # Create a hash of the topic ID
-        topic_hash = str(topic_id)
+    async def publish(self, topic, events, on_ack=None, on_nack=None):
+        # Ensure we have a gRPC channel
+        self._ensure_ready()
+
+        if self.shutdown.is_set():
+            raise EnsignClientClosingError("client is closing")
 
-        # Check if there is already an open stream for this topic
-        if topic_hash in self.publish_streams:
-            stream = self.publish_streams[topic_hash]
+        # Attempt to hash the topic, which fails if there is no topic ID
+        try:
+            topic_hash = hash(topic)
+        except ValueError:
+            topic_hash = None
+
+        # Check if there is already an open publish stream for this topic
+        if topic_hash and topic_hash in self.publishers:
+            publisher = self.publishers[topic_hash]
         else:
-            # Create the stream for this topic
-            stream = Stream()
-            self.publish_streams[topic_hash] = stream
-
-            async def next_request():
-                # First message must be an OpenStream request
-                # TODO: Should we send topics here?
-                yield ensign_pb2.PublisherRequest(
-                    open_stream=ensign_pb2.OpenStream(client_id=client_id)
-                )
-
-                # The rest of the messages should be wrapped events
-                while True:
-                    req = await stream.read_request()
-                    if req is None:
-                        break
-                    yield req
-
-            async def publish_stream():
-                async for rep in self.stub.Publish(next_request()):
-                    rep_type = rep.WhichOneof("embed")
-                    if not stream.ready.is_set() and rep_type != "ready":
-                        raise EnsignTypeError(
-                            "expected ready response, got {}".format(rep_type)
-                        )
-                    if rep_type == "ready":
-                        # TODO: Parse topic map from stream_ready response
-                        stream.ready.set()
-                    elif rep_type == "ack":
-                        if ack_callback:
-                            await ack_callback(rep.ack)
-                    elif rep_type == "nack":
-                        if nack_callback:
-                            await nack_callback(rep.nack)
-                    elif rep_type == "close_stream":
-                        await stream.close()
-                        break
-                    else:
-                        raise EnsignTypeError(f"unexpected response type: {rep_type}")
+            # Create the publish stream for this topic
+            publisher = Publisher(
+                self,
+                topic,
+                on_ack=on_ack,
+                on_nack=on_nack,
+                reconnect_tick=self.reconnect_tick,
+                reconnect_timeout=self.reconnect_timeout,
+            )
+
+            # Connect to the publish stream
+            # TODO: Distinguish between authentication errors, topic errors, and connection errors
+            await publisher.connect()
+
+            # After connect we should have the topic ID from the server, so compute the
+            # hash and save the open publisher stream
+            topic_hash = hash(topic)
+            self.publishers[topic_hash] = publisher
 
-            # Create a concurrent task to handle the stream
+            # Run the publisher as a concurrent task which handles reconnects
             await self.pool.schedule(
-                publish_stream(),
-                done_callback=lambda: self.publish_streams.pop(topic_hash),
+                publisher.run(),
+                done_callback=lambda: self.publishers.pop(topic_hash, None),
             )
 
-        async def queue_events():
-            for event in events:
-                req = ensign_pb2.PublisherRequest(event=wrap(event, topic_id))
-                await stream.write_request(req)
-
         # Create a concurrent task to queue the events from the user
-        await self.pool.schedule(queue_events())
+        await self.pool.schedule(publisher.queue_events(events))
 
     @catch_rpc_error
-    async def subscribe(self, topic_ids, client_id="", query="", consumer_group=None):
-        # Create a hash of the topic IDs
-        topic_hash = frozenset([id for id in topic_ids])
+    async def subscribe(self, topics, query="", consumer_group=None):
+        # Ensure we have a gRPC channel
+        self._ensure_ready()
+
+        if self.shutdown.is_set():
+            raise EnsignClientClosingError("client is closing")
+
+        # Create a hash of the topics
+        topic_hash = frozenset([t for t in topics])
 
         # Check if there is already an open stream for these topics
-        if topic_hash in self.subscribe_streams:
-            stream = self.subscribe_streams[topic_hash]
+        if topic_hash in self.subscribers:
+            subscriber = self.subscribers[topic_hash]
         else:
-            # Create the stream for these topics
-            stream = Stream()
-            self.subscribe_streams[topic_hash] = stream
-
-            async def next_request():
-                # First message must be a Subscription request with the topic
-                sub = ensign_pb2.Subscription(
-                    client_id=client_id,
-                    topics=topic_ids,
-                    query=query,
-                    group=consumer_group,
-                )
-                yield ensign_pb2.SubscribeRequest(subscription=sub)
-
-                # Return acks and nacks to the server
-                while True:
-                    yield await stream.read_request()
-
-            async def subscribe_stream():
-                async for rep in self.stub.Subscribe(next_request()):
-                    rep_type = rep.WhichOneof("embed")
-                    if not stream.ready.is_set() and rep_type != "ready":
-                        stream.write_response(
-                            EnsignTypeError(
-                                "expected ready response, got {}".format(rep_type)
-                            )
-                        )
-                        break
-                    if rep_type == "ready":
-                        stream.ready.set()
-                    elif rep_type == "event":
-                        await stream.write_response(rep.event)
-                    elif rep_type == "close_stream":
-                        await stream.close()
-                        break
-                    else:
-                        stream.write_response(
-                            EnsignTypeError(f"unexpected response type: {rep_type}")
-                        )
-                        break
+            # Create the subscribe stream for these topics
+            subscriber = Subscriber(
+                self,
+                topics,
+                query=query,
+                consumer_group=consumer_group,
+                reconnect_tick=self.reconnect_tick,
+                reconnect_timeout=self.reconnect_timeout,
+            )
+            self.subscribers[topic_hash] = subscriber
+
+            # Connect to the subscribe stream
+            # TODO: Distinguish between authentication errors, topic errors, and connection errors
+            await subscriber.connect()
 
-            # Create a concurrent task to handle the stream
+            # Run the subscriber as a concurrent task which handles reconnects
             await self.pool.schedule(
-                subscribe_stream(),
-                done_callback=lambda: self.subscribe_streams.pop(topic_hash),
+                subscriber.run(),
+                done_callback=lambda: self.subscribers.pop(topic_hash, None),
             )
 
-        # Yield events from the stream
-        while True:
-            rep = await stream.read_response()
-            if rep is None:
-                break
-            elif isinstance(rep, EnsignError):
-                raise rep
-            else:
-                # Ack back to the stream
-                # TODO: Allow the user to ack or nack the event
-                await stream.write_request(ensign_pb2.SubscribeRequest(ack=ensign_pb2.Ack(id=rep.id)))
-
-                yield unwrap(rep)
+        # Consume the events and yield them to the caller
+        async for event in subscriber.consume():
+            yield event
 
     @catch_rpc_error
     async def list_topics(self, page_size=100, next_page_token=""):
+        self._ensure_ready()
         params = ensign_pb2.PageInfo(
             page_size=page_size, next_page_token=next_page_token
         )
         rep = await self.stub.ListTopics(params)
         return rep.topics, rep.next_page_token
 
     @catch_rpc_error
     async def create_topic(self, topic):
+        self._ensure_ready()
         return await self.stub.CreateTopic(topic)
 
     @catch_rpc_error
     async def retrieve_topic(self, id):
+        self._ensure_ready()
         topic = topic_pb2.Topic(id=id)
         return await self.stub.RetrieveTopic(topic)
 
     @catch_rpc_error
     async def archive_topic(self, id):
+        self._ensure_ready()
         params = topic_pb2.TopicMod(
             id=id, operation=topic_pb2.TopicMod.Operation.ARCHIVE
         )
         rep = await self.stub.DeleteTopic(params)
         return rep.id, rep.state
 
     @catch_rpc_error
     async def destroy_topic(self, id):
+        self._ensure_ready()
         params = topic_pb2.TopicMod(
             id=id, operation=topic_pb2.TopicMod.Operation.DESTROY
         )
         rep = await self.stub.DeleteTopic(params)
         return rep.id, rep.state
 
     @catch_rpc_error
     async def topic_names(self, page_size=100, next_page_token=""):
+        self._ensure_ready()
         params = ensign_pb2.PageInfo(
             page_size=page_size, next_page_token=next_page_token
         )
         rep = await self.stub.TopicNames(params)
         return rep.topic_names, rep.next_page_token
 
     @catch_rpc_error
     async def topic_exists(self, topic_id=None, project_id=None, topic_name=""):
+        self._ensure_ready()
         params = topic_pb2.TopicName(
             topic_id=topic_id, project_id=project_id, name=topic_name
         )
         rep = await self.stub.TopicExists(params)
         return rep.query, rep.exists
 
     @catch_rpc_error
     async def info(self, topics=[]):
+        self._ensure_ready()
         return await self.stub.Info(ensign_pb2.InfoRequest(topics=topics))
 
     @catch_rpc_error
     async def status(self, attempts=0, last_checked_at=None):
+        self._ensure_ready()
         params = ensign_pb2.HealthCheck(
             attempts=attempts, last_checked_at=last_checked_at
         )
         rep = await self.stub.Status(params)
         return rep.status, rep.version, rep.uptime, rep.not_before, rep.not_after
 
     async def close(self):
         """
         Close the connection to the server and all ongoing streams.
         """
-        await self.pool.release()
         await self.channel.close()
+        await self._close_streams()
+        self.channel = None
 
+    async def _close_streams(self):
+        # Prevent new streams from being created
+        self.shutdown.set()
+
+        # Close all ongoing publishers and subscribers
+        while self.publishers:
+            _, publisher = self.publishers.popitem()
+            await publisher.close()
+
+        while self.subscribers:
+            _, subscriber = self.subscribers.popitem()
+            await subscriber.close()
 
-class Stream:
-    """
-    Stream implements an in-memory bidirectional buffer for non-blocking communication
-    between coroutines. The stream has a ready state that can be used to signal when the
-    stream is ready to receive requests.
-    """
-
-    def __init__(self, max_queue_size=100):
-        self._request_queue = asyncio.Queue(maxsize=max_queue_size)
-        self._response_queue = asyncio.Queue(maxsize=max_queue_size)
-        self.ready = asyncio.Event()
-
-    async def write_request(self, message):
-        """
-        Write a request to the stream, blocks if the queue is full.
-        """
-        await self._request_queue.put(message)
-
-    async def read_request(self):
-        """
-        Read a request from the stream, blocks if the queue is empty.
-        """
-        return await self._request_queue.get()
-
-    async def write_response(self, message):
-        """
-        Write a response to the stream, blocks if the queue is full.
-        """
-        await self._response_queue.put(message)
-
-    async def read_response(self):
-        """
-        Read a response from the stream, blocks if the queue is empty.
-        """
-        return await self._response_queue.get()
-
-    async def close(self):
-        """
-        Close the stream by sending a message to both the request and response streams.
-        The main purpose of this is to unblock pending consumers. Otherwise, consumers
-        will block indefinitely on read_request() or read_response(). This means that
-        consumers should be prepared to handle None responses from reads.
-        """
-        await self._request_queue.put(None)
-        await self._response_queue.put(None)
+        await self.pool.release()
```

### Comparing `pyensign-0.7b0/pyensign/mimetype/v1beta1/mimetype_pb2.py` & `pyensign-0.8b0/pyensign/mimetype/v1beta1/mimetype_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/mimetypes.py` & `pyensign-0.8b0/pyensign/mimetypes.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/region/v1beta1/region_pb2.py` & `pyensign-0.8b0/pyensign/region/v1beta1/region_pb2.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/utils/cache.py` & `pyensign-0.8b0/pyensign/utils/cache.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,16 +4,27 @@
 class Cache:
     """
     Cache is a simple cache that maps keys to values to avoid repeated RPC calls to
     Ensign. This is not thread-safe.
     TODO: Implement max size and evictions.
     """
 
-    def __init__(self):
+    def __init__(self, read_only=False):
+        """
+        Create a new cache.
+
+        Parameters
+        ----------
+        read_only : bool (default: False)
+            If True, the cache will not be writeable. This creates a disabled cache
+            where get() will always raise a CacheMissError, exists() will always return
+            False, and add() is a no-op.
+        """
         self._index = {}
+        self._read_only = read_only
 
     def get(self, key):
         """
         Get a value by name, an exception is raised if the key does not exist in the
         cache.
         """
         try:
@@ -21,20 +32,22 @@
         except KeyError as e:
             raise CacheMissError(key) from e
 
     def add(self, key, value):
         """
         Add a value by key to the cache, overwriting the existing key.
         """
-        self._index[key] = value
+        if not self._read_only:
+            self._index[key] = value
 
     def exists(self, key):
         """
         Returns True if the key exists in the cache.
         """
         return key in self._index
 
     def clear(self):
         """
         Reset the cache, deleting all keys.
         """
-        self._index.clear()
+        if not self._read_only:
+            self._index.clear()
```

### Comparing `pyensign-0.7b0/pyensign/utils/tasks.py` & `pyensign-0.8b0/pyensign/utils/tasks.py`

 * *Files identical despite different names*

### Comparing `pyensign-0.7b0/pyensign/version.py` & `pyensign-0.8b0/pyensign/version.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,39 @@
 ##########################################################################
 ## Module Info
 ##########################################################################
 
 __version_info__ = {
     "major": 0,
-    "minor": 7,
+    "minor": 8,
     "micro": 0,
     "releaselevel": "beta",
     "serial": 0,
 }
 
 ##########################################################################
 ## Helper Functions
 ##########################################################################
 
 
 def get_version(short=False):
     """
-    Prints the version.
+    Returns the version string for pyensign.
     """
     assert __version_info__["releaselevel"] in ("alpha", "beta", "final")
     vers = [
         "%(major)i.%(minor)i" % __version_info__,
     ]
     if __version_info__["micro"]:
         vers.append(".%(micro)i" % __version_info__)
     if __version_info__["releaselevel"] != "final" and not short:
         vers.append(
             "%s%i" % (__version_info__["releaselevel"][0], __version_info__["serial"])
         )
     return "".join(vers)
+
+
+def user_agent():
+    """
+    Returns the user agent string for pyensign.
+    """
+    return "pyensign/" + get_version()
```

### Comparing `pyensign-0.7b0/pyensign.egg-info/PKG-INFO` & `pyensign-0.8b0/pyensign.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pyensign
-Version: 0.7b0
+Version: 0.8b0
 Summary: Ensign driver, SDK, and helpers for Python
 Home-page: https://github.com/rotationalio/pyensign
 Author: Patrick Deziel
 Author-email: deziel.patrick@gmail.com
 Maintainer: Patrick Deziel
 Maintainer-email: deziel.patrick@gmail.com
 License: BSD
-Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.7b0
+Download-URL: https://github.com/rotationalio/pyensign/tarball/v0.8b0
 Description: # PyEnsign
         
         PyEnsign is the official Python SDK for [Ensign](https://rotational.io/ensign), a distributed event store and stream-processing platform. This library allows you to interact with the Ensign API directly from Python in order to create [publishers](https://ensign.rotational.dev/eventing/glossary/#publisher) and [subscribers](https://ensign.rotational.dev/eventing/glossary/#subscriber).
         
         ## Installation
         
         ```
@@ -41,35 +41,35 @@
         
         ```python
         await client.publish("weather", event)
         await client.publish("weather", event1, event2)
         await client.publish("weather", [event1, event2])
         ```
         
-        Subscribe to one or more topic IDs. Topic IDs are assigned by Ensign so a common pattern is to first retrieve the topic ID from the topic name.
+        Subscribe to one or more topics by providing the topic name(s) or ID(s).
         
         ```python
-        topic_id = await client.topic_id("weather")
-        async for event in client.subscribe(topic_id):
-            print("Received event: {}".format(event))
+        async for event in client.subscribe("weather"):
+            print("Received event with data: {}".format(event.data))
+            event.ack()
         ```
         
         ## Advanced Usage
         
         The `publish` coroutine accepts asynchronous callbacks so the client can distinguish between committed and uncommitted events. Callbacks are invoked when acks and nacks are received from the server and the first argument passed to the callback is the `Ack` or `Nack` itself. An `Ack` contains a committed timestamp. A `Nack` is returned if the event couldn't be committed and contains the ID of the event along with an error describing what went wrong.
         
         ```python
         async def handle_ack(self, ack):
             ts = datetime.fromtimestamp(ack.committed.seconds + ack.committed.nanos / 1e9)
             print(f"Event committed at {ts}")
         
         async def handle_nack(self, nack):
             print(f"Could not commit event {nack.id} with error {nack.code}: {nack.error}")
         
-        await client.publish("weather", event, ack_callback=handle_ack, nack_callback=handle_nack)
+        await client.publish("weather", event, on_ack=handle_ack, on_nack=handle_nack)
         ```
 Keywords: python,setup,pypi
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
```

### Comparing `pyensign-0.7b0/pyensign.egg-info/SOURCES.txt` & `pyensign-0.8b0/pyensign.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,20 @@
 setup.cfg
 setup.py
 pyensign/__init__.py
 pyensign/connection.py
 pyensign/ensign.py
 pyensign/events.py
 pyensign/exceptions.py
+pyensign/iterator.py
 pyensign/mimetypes.py
+pyensign/nack.py
+pyensign/publisher.py
+pyensign/stream.py
+pyensign/subscriber.py
 pyensign/version.py
 pyensign.egg-info/PKG-INFO
 pyensign.egg-info/SOURCES.txt
 pyensign.egg-info/dependency_links.txt
 pyensign.egg-info/not-zip-safe
 pyensign.egg-info/requires.txt
 pyensign.egg-info/top_level.txt
@@ -26,17 +31,20 @@
 pyensign/api/v1beta1/ensign_pb2_grpc.py
 pyensign/api/v1beta1/event.py
 pyensign/api/v1beta1/event_pb2.py
 pyensign/api/v1beta1/groups_pb2.py
 pyensign/api/v1beta1/topic_pb2.py
 pyensign/auth/__init__.py
 pyensign/auth/client.py
+pyensign/auth/interceptor.py
 pyensign/auth/tokens.py
 pyensign/mimetype/__init__.py
 pyensign/mimetype/v1beta1/__init__.py
 pyensign/mimetype/v1beta1/mimetype_pb2.py
 pyensign/region/__init__.py
 pyensign/region/v1beta1/__init__.py
 pyensign/region/v1beta1/region_pb2.py
 pyensign/utils/__init__.py
 pyensign/utils/cache.py
-pyensign/utils/tasks.py
+pyensign/utils/queue.py
+pyensign/utils/tasks.py
+pyensign/utils/topics.py
```

### Comparing `pyensign-0.7b0/setup.py` & `pyensign-0.8b0/setup.py`

 * *Files identical despite different names*

