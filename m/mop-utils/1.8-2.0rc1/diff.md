# Comparing `tmp/mop_utils-1.8.tar.gz` & `tmp/mop_utils-2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mop_utils-1.8.tar", last modified: Mon Apr 17 06:46:56 2023, max compression
+gzip compressed data, was "mop_utils-2.0rc1.tar", last modified: Wed Aug  2 03:16:53 2023, max compression
```

## Comparing `mop_utils-1.8.tar` & `mop_utils-2.0rc1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 06:46:56.875088 mop_utils-1.8/
--rw-rw-rw-   0        0        0      108 2023-04-17 06:46:56.874088 mop_utils-1.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 06:46:56.822549 mop_utils-1.8/mop_utils/
--rw-rw-rw-   0        0        0       89 2023-02-13 07:03:05.000000 mop_utils-1.8/mop_utils/__init__.py
--rw-rw-rw-   0        0        0     4529 2023-04-13 06:22:23.000000 mop_utils-1.8/mop_utils/base_model_wrapper.py
--rw-rw-rw-   0        0        0       39 2023-02-16 07:10:11.000000 mop_utils-1.8/mop_utils/constant.py
--rw-rw-rw-   0        0        0     6264 2023-03-31 08:33:06.000000 mop_utils-1.8/mop_utils/inference_wrapper.py
-drwxrwxrwx   0        0        0        0 2023-04-17 06:46:56.873089 mop_utils-1.8/mop_utils.egg-info/
--rw-rw-rw-   0        0        0      108 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 06:46:56.000000 mop_utils-1.8/mop_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 06:46:56.876088 mop_utils-1.8/setup.cfg
--rw-rw-rw-   0        0        0      345 2023-04-17 06:44:13.000000 mop_utils-1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:16:53.032363 mop_utils-2.0rc1/
+-rw-rw-rw-   0        0        0      111 2023-08-02 03:16:53.032363 mop_utils-2.0rc1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 03:16:53.016770 mop_utils-2.0rc1/mop_utils/
+-rw-rw-rw-   0        0        0       89 2023-07-20 02:05:32.000000 mop_utils-2.0rc1/mop_utils/__init__.py
+-rw-rw-rw-   0        0        0     7960 2023-08-02 00:56:41.000000 mop_utils-2.0rc1/mop_utils/base_model_wrapper.py
+-rw-rw-rw-   0        0        0       39 2023-07-20 05:50:46.000000 mop_utils-2.0rc1/mop_utils/constant.py
+-rw-rw-rw-   0        0        0     6270 2023-08-02 00:56:29.000000 mop_utils-2.0rc1/mop_utils/inference_wrapper.py
+-rw-rw-rw-   0        0        0     5884 2023-07-28 08:43:44.000000 mop_utils-2.0rc1/mop_utils/util.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:16:53.032363 mop_utils-2.0rc1/mop_utils.egg-info/
+-rw-rw-rw-   0        0        0      111 2023-08-02 03:16:52.000000 mop_utils-2.0rc1/mop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-08-02 03:16:52.000000 mop_utils-2.0rc1/mop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 03:16:52.000000 mop_utils-2.0rc1/mop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-02 03:16:52.000000 mop_utils-2.0rc1/mop_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 03:16:52.000000 mop_utils-2.0rc1/mop_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 03:16:53.032363 mop_utils-2.0rc1/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-08-02 03:15:10.000000 mop_utils-2.0rc1/setup.py
```

### Comparing `mop_utils-1.8/mop_utils/inference_wrapper.py` & `mop_utils-2.0rc1/mop_utils/inference_wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,17 +161,17 @@
     # print(res)
     # text_dict = [{"text": "354"}]
     # res = mop_run(text_dict, True)
     # print(res)
 
     dynamic_batch = {
         'enable': True,
-        'maxBatchSize': 12,
-        'idleBatchSize': 3,
-        'maxBatchInterval': 0.2
+        'max_batch_size': 12,
+        'idle_batch_size': 3,
+        'max_batch_interval': 0.2
     }
 
     mop_init(model_root, dynamic_batch)
 
     text_dict = {"text": "354"}
     res = mop_run(text_dict, True)
     print(res)
```

