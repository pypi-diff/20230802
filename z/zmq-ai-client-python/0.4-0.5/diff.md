# Comparing `tmp/zmq_ai_client_python-0.4.tar.gz` & `tmp/zmq_ai_client_python-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zmq_ai_client_python-0.4.tar", last modified: Wed Aug  2 14:38:34 2023, max compression
+gzip compressed data, was "zmq_ai_client_python-0.5.tar", last modified: Wed Aug  2 14:42:14 2023, max compression
```

## Comparing `zmq_ai_client_python-0.4.tar` & `zmq_ai_client_python-0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:38:34.132409 zmq_ai_client_python-0.4/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      252 2023-08-02 14:38:34.132409 zmq_ai_client_python-0.4/PKG-INFO
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      429 2023-08-02 08:28:16.000000 zmq_ai_client_python-0.4/README.md
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       38 2023-08-02 14:38:34.132409 zmq_ai_client_python-0.4/setup.cfg
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      507 2023-08-02 14:38:10.000000 zmq_ai_client_python-0.4/setup.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:38:34.128409 zmq_ai_client_python-0.4/zmq_ai_client_python/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      184 2023-08-02 10:27:31.000000 zmq_ai_client_python-0.4/zmq_ai_client_python/__init__.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)     1081 2023-08-02 07:19:04.000000 zmq_ai_client_python-0.4/zmq_ai_client_python/client.py
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      548 2023-08-02 07:19:19.000000 zmq_ai_client_python-0.4/zmq_ai_client_python/client_test.py
-drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:38:34.132409 zmq_ai_client_python-0.4/zmq_ai_client_python.egg-info/
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      252 2023-08-02 14:38:34.000000 zmq_ai_client_python-0.4/zmq_ai_client_python.egg-info/PKG-INFO
--rw-rw-r--   0 qimia     (1000) qimia     (1000)      337 2023-08-02 14:38:34.000000 zmq_ai_client_python-0.4/zmq_ai_client_python.egg-info/SOURCES.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)        1 2023-08-02 14:38:34.000000 zmq_ai_client_python-0.4/zmq_ai_client_python.egg-info/dependency_links.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       14 2023-08-02 14:38:34.000000 zmq_ai_client_python-0.4/zmq_ai_client_python.egg-info/requires.txt
--rw-rw-r--   0 qimia     (1000) qimia     (1000)       21 2023-08-02 14:38:34.000000 zmq_ai_client_python-0.4/zmq_ai_client_python.egg-info/top_level.txt
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:42:14.834254 zmq_ai_client_python-0.5/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      252 2023-08-02 14:42:14.834254 zmq_ai_client_python-0.5/PKG-INFO
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      429 2023-08-02 08:28:16.000000 zmq_ai_client_python-0.5/README.md
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       38 2023-08-02 14:42:14.834254 zmq_ai_client_python-0.5/setup.cfg
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      535 2023-08-02 14:42:03.000000 zmq_ai_client_python-0.5/setup.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:42:14.834254 zmq_ai_client_python-0.5/zmq_ai_client_python/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      184 2023-08-02 10:27:31.000000 zmq_ai_client_python-0.5/zmq_ai_client_python/__init__.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)     1081 2023-08-02 07:19:04.000000 zmq_ai_client_python-0.5/zmq_ai_client_python/client.py
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      548 2023-08-02 07:19:19.000000 zmq_ai_client_python-0.5/zmq_ai_client_python/client_test.py
+drwxrwxr-x   0 qimia     (1000) qimia     (1000)        0 2023-08-02 14:42:14.834254 zmq_ai_client_python-0.5/zmq_ai_client_python.egg-info/
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      252 2023-08-02 14:42:14.000000 zmq_ai_client_python-0.5/zmq_ai_client_python.egg-info/PKG-INFO
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)      337 2023-08-02 14:42:14.000000 zmq_ai_client_python-0.5/zmq_ai_client_python.egg-info/SOURCES.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)        1 2023-08-02 14:42:14.000000 zmq_ai_client_python-0.5/zmq_ai_client_python.egg-info/dependency_links.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       14 2023-08-02 14:42:14.000000 zmq_ai_client_python-0.5/zmq_ai_client_python.egg-info/requires.txt
+-rw-rw-r--   0 qimia     (1000) qimia     (1000)       21 2023-08-02 14:42:14.000000 zmq_ai_client_python-0.5/zmq_ai_client_python.egg-info/top_level.txt
```

### Comparing `zmq_ai_client_python-0.4/zmq_ai_client_python/client.py` & `zmq_ai_client_python-0.5/zmq_ai_client_python/client.py`

 * *Files identical despite different names*

### Comparing `zmq_ai_client_python-0.4/zmq_ai_client_python/client_test.py` & `zmq_ai_client_python-0.5/zmq_ai_client_python/client_test.py`

 * *Files identical despite different names*

