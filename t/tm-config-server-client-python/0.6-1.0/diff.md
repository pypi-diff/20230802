# Comparing `tmp/tm_config_server_client_python-0.6.tar.gz` & `tmp/tm_config_server_client_python-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tm_config_server_client_python-0.6.tar", last modified: Tue Aug  1 10:07:17 2023, max compression
+gzip compressed data, was "dist/tm_config_server_client_python-1.0.tar", last modified: Wed Aug  2 07:10:37 2023, max compression
```

## Comparing `tm_config_server_client_python-0.6.tar` & `tm_config_server_client_python-1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/
--rw-r--r--   0 jayant     (501) staff       (20)      253 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/PKG-INFO
--rw-rw-r--   0 jayant     (501) staff       (20)       38 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/setup.cfg
--rw-rw-r--   0 jayant     (501) staff       (20)      279 2023-08-01 10:07:13.000000 tm_config_server_client_python-0.6/setup.py
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/tm_config_server_client_python/
--rw-r--r--   0 jayant     (501) staff       (20)     3628 2023-08-01 10:06:51.000000 tm_config_server_client_python-0.6/tm_config_server_client_python/Pythonclient.py
--rw-rw-r--   0 jayant     (501) staff       (20)       39 2023-08-01 09:53:59.000000 tm_config_server_client_python-0.6/tm_config_server_client_python/__init__.py
-drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/tm_config_server_client_python.egg-info/
--rw-r--r--   0 jayant     (501) staff       (20)      253 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/tm_config_server_client_python.egg-info/PKG-INFO
--rw-r--r--   0 jayant     (501) staff       (20)      377 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/tm_config_server_client_python.egg-info/SOURCES.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/tm_config_server_client_python.egg-info/dependency_links.txt
--rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/tm_config_server_client_python.egg-info/not-zip-safe
--rw-r--r--   0 jayant     (501) staff       (20)       31 2023-08-01 10:07:17.000000 tm_config_server_client_python-0.6/tm_config_server_client_python.egg-info/top_level.txt
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/
+-rw-r--r--   0 jayant     (501) staff       (20)      253 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)       38 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/setup.cfg
+-rw-rw-r--   0 jayant     (501) staff       (20)      279 2023-08-02 07:10:28.000000 tm_config_server_client_python-1.0/setup.py
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/tm_config_server_client_python/
+-rw-r--r--   0 jayant     (501) staff       (20)     1106 2023-08-02 07:10:04.000000 tm_config_server_client_python-1.0/tm_config_server_client_python/Playclient.py
+-rw-r--r--   0 jayant     (501) staff       (20)     3546 2023-08-02 06:57:22.000000 tm_config_server_client_python-1.0/tm_config_server_client_python/Pythonclient.py
+-rw-rw-r--   0 jayant     (501) staff       (20)       39 2023-08-02 06:55:00.000000 tm_config_server_client_python-1.0/tm_config_server_client_python/__init__.py
+drwxr-xr-x   0 jayant     (501) staff       (20)        0 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/tm_config_server_client_python.egg-info/
+-rw-r--r--   0 jayant     (501) staff       (20)      253 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/tm_config_server_client_python.egg-info/PKG-INFO
+-rw-r--r--   0 jayant     (501) staff       (20)      412 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/tm_config_server_client_python.egg-info/SOURCES.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/tm_config_server_client_python.egg-info/dependency_links.txt
+-rw-r--r--   0 jayant     (501) staff       (20)        1 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/tm_config_server_client_python.egg-info/not-zip-safe
+-rw-r--r--   0 jayant     (501) staff       (20)       31 2023-08-02 07:10:37.000000 tm_config_server_client_python-1.0/tm_config_server_client_python.egg-info/top_level.txt
```

### Comparing `tm_config_server_client_python-0.6/tm_config_server_client_python/Pythonclient.py` & `tm_config_server_client_python-1.0/tm_config_server_client_python/Pythonclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,14 @@
 import sys
 import requests
 import os
 import re
 class PythonClient:
 
     @staticmethod
-    def hello_world():
-        return "I am testing this code"
-
-    @staticmethod
     def required_properties_func(configs, keyword):
         required_properties = {}
         for config in configs:
             if keyword in config["name"]:
                 required_properties.update({k: v for k, v in config["source"].items() if k not in required_properties})
         return required_properties
```

