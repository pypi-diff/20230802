# Comparing `tmp/globus-compute-sdk-2.2.4a0.tar.gz` & `tmp/globus-compute-sdk-2.3.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-sdk-2.2.4a0.tar", last modified: Fri Jul 14 15:13:58 2023, max compression
+gzip compressed data, was "globus-compute-sdk-2.3.0a0.tar", last modified: Wed Aug  2 19:08:50 2023, max compression
```

## Comparing `globus-compute-sdk-2.2.4a0.tar` & `globus-compute-sdk-2.3.0a0.tar`

### file list

```diff
@@ -1,51 +1,55 @@
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.180184 globus-compute-sdk-2.2.4a0/
--rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/LICENSE
--rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.4a0/MANIFEST.in
--rw-r--r--   0 lei        (501) staff       (20)     1821 2023-07-14 15:13:58.180253 globus-compute-sdk-2.2.4a0/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)      816 2023-04-20 03:21:56.000000 globus-compute-sdk-2.2.4a0/PyPI.md
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.172769 globus-compute-sdk-2.2.4a0/globus_compute_sdk/
--rw-r--r--   0 lei        (501) staff       (20)      433 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/__init__.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.173872 globus-compute-sdk-2.2.4a0/globus_compute_sdk/errors/
--rw-r--r--   0 lei        (501) staff       (20)      320 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/errors/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1921 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/errors/error_types.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.175740 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1505 2023-07-14 14:46:29.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/_environments.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.176316 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/asynchronous/
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/asynchronous/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)      648 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
--rw-r--r--   0 lei        (501) staff       (20)      724 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
--rw-r--r--   0 lei        (501) staff       (20)    11458 2023-04-24 21:22:25.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
--rw-r--r--   0 lei        (501) staff       (20)     2262 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/batch.py
--rw-r--r--   0 lei        (501) staff       (20)    27050 2023-07-06 21:18:52.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/client.py
--rw-r--r--   0 lei        (501) staff       (20)     2400 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/container_spec.py
--rw-r--r--   0 lei        (501) staff       (20)    46344 2023-06-05 19:33:47.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/executor.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.178319 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/
--rw-r--r--   0 lei        (501) staff       (20)      237 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1787 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/client_login.py
--rw-r--r--   0 lei        (501) staff       (20)      855 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/decorators.py
--rw-r--r--   0 lei        (501) staff       (20)      373 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
--rw-r--r--   0 lei        (501) staff       (20)      954 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/login_flow.py
--rw-r--r--   0 lei        (501) staff       (20)     7287 2023-06-12 17:16:14.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/manager.py
--rw-r--r--   0 lei        (501) staff       (20)      710 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/protocol.py
--rw-r--r--   0 lei        (501) staff       (20)     3012 2023-05-05 16:40:44.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
--rw-r--r--   0 lei        (501) staff       (20)     2190 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/whoami.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.178634 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/utils/
--rw-r--r--   0 lei        (501) staff       (20)      212 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/utils/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1207 2023-04-10 19:02:41.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/utils/printing.py
--rw-r--r--   0 lei        (501) staff       (20)     8561 2023-07-06 21:18:52.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/web_client.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.179991 globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/
--rw-r--r--   0 lei        (501) staff       (20)      603 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/__init__.py
--rw-r--r--   0 lei        (501) staff       (20)     1412 2023-06-26 15:08:59.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/base.py
--rw-r--r--   0 lei        (501) staff       (20)     7869 2023-06-13 18:28:48.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/concretes.py
--rw-r--r--   0 lei        (501) staff       (20)     4848 2023-06-26 15:08:59.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/facade.py
--rw-r--r--   0 lei        (501) staff       (20)        0 2023-05-08 21:56:13.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/utils.py
--rw-r--r--   0 lei        (501) staff       (20)      834 2023-07-14 15:12:39.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk/version.py
-drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-07-14 15:13:58.173416 globus-compute-sdk-2.2.4a0/globus_compute_sdk.egg-info/
--rw-r--r--   0 lei        (501) staff       (20)     1821 2023-07-14 15:13:58.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk.egg-info/PKG-INFO
--rw-r--r--   0 lei        (501) staff       (20)     1577 2023-07-14 15:13:58.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 lei        (501) staff       (20)        1 2023-07-14 15:13:58.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 lei        (501) staff       (20)      395 2023-07-14 15:13:58.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk.egg-info/requires.txt
--rw-r--r--   0 lei        (501) staff       (20)       19 2023-07-14 15:13:58.000000 globus-compute-sdk-2.2.4a0/globus_compute_sdk.egg-info/top_level.txt
--rw-r--r--   0 lei        (501) staff       (20)      282 2023-07-14 15:13:58.180520 globus-compute-sdk-2.2.4a0/setup.cfg
--rw-r--r--   0 lei        (501) staff       (20)     3159 2023-07-14 14:46:26.000000 globus-compute-sdk-2.2.4a0/setup.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.966284 globus-compute-sdk-2.3.0a0/
+-rw-rw-r--   0 reid      (1000) reid      (1000)    11330 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/LICENSE
+-rw-rw-r--   0 reid      (1000) reid      (1000)       16 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/MANIFEST.in
+-rw-rw-rw-   0 reid      (1000) reid      (1000)     1821 2023-08-02 19:08:50.966284 globus-compute-sdk-2.3.0a0/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)      816 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/PyPI.md
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.958284 globus-compute-sdk-2.3.0a0/globus_compute_sdk/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      433 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/__init__.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.962284 globus-compute-sdk-2.3.0a0/globus_compute_sdk/errors/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      320 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/errors/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1921 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/errors/error_types.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.962284 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      987 2023-07-28 22:41:17.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/_environments.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.962284 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/asynchronous/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/asynchronous/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      648 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      724 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3063 2023-08-02 17:10:59.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/batch.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    23723 2023-08-02 17:10:59.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/client.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2400 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/container_spec.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)    54739 2023-08-02 17:10:59.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/executor.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.966284 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      237 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1787 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/client_login.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      855 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/decorators.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      373 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/globus_auth.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      954 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7287 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/manager.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      710 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/protocol.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3012 2023-07-28 22:41:17.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2190 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/whoami.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.966284 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/utils/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      212 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/utils/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1207 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/utils/printing.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      470 2023-07-28 22:41:17.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/utils/uuid_like.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     8831 2023-08-01 03:35:29.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/web_client.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.966284 globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/
+-rw-rw-r--   0 reid      (1000) reid      (1000)      603 2023-07-28 22:41:17.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1412 2023-07-28 22:41:17.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/base.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     7869 2023-07-28 22:41:17.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/concretes.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     4848 2023-07-28 22:41:17.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/facade.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/utils.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)      834 2023-08-02 18:43:27.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk/version.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.958284 globus-compute-sdk-2.3.0a0/globus_compute_sdk.egg-info/
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1821 2023-08-02 19:08:50.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk.egg-info/PKG-INFO
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1615 2023-08-02 19:08:50.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk.egg-info/SOURCES.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)        1 2023-08-02 19:08:50.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk.egg-info/dependency_links.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      395 2023-08-02 19:08:50.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk.egg-info/requires.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)       19 2023-08-02 19:08:50.000000 globus-compute-sdk-2.3.0a0/globus_compute_sdk.egg-info/top_level.txt
+-rw-rw-r--   0 reid      (1000) reid      (1000)      282 2023-08-02 19:08:50.966284 globus-compute-sdk-2.3.0a0/setup.cfg
+-rw-rw-r--   0 reid      (1000) reid      (1000)     3159 2023-07-28 22:41:17.000000 globus-compute-sdk-2.3.0a0/setup.py
+drwxrwxrwx   0 reid      (1000) reid      (1000)        0 2023-08-02 19:08:50.966284 globus-compute-sdk-2.3.0a0/tests/
+-rw-rw-r--   0 reid      (1000) reid      (1000)        0 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/tests/__init__.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     1962 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/tests/conftest.py
+-rw-rw-r--   0 reid      (1000) reid      (1000)     2276 2023-07-28 22:37:35.000000 globus-compute-sdk-2.3.0a0/tests/utils.py
```

### Comparing `globus-compute-sdk-2.2.4a0/LICENSE` & `globus-compute-sdk-2.3.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/PKG-INFO` & `globus-compute-sdk-2.3.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.2.4a0
+Version: 2.3.0a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.2.4a0/PyPI.md` & `globus-compute-sdk-2.3.0a0/PyPI.md`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/errors/error_types.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/errors/error_types.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/_environments.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/_environments.py`

 * *Files 19% similar despite different names*

```diff
@@ -23,25 +23,10 @@
     }
     for test_env in ["sandbox", "test", "integration", "staging"]:
         urls[test_env] = f"https://compute.api.{test_env}.globuscs.info"
 
     return urls.get(env, urls["production"])
 
 
-def get_web_socket_url(envname: str | None) -> str:
-    env = envname or _get_envname()
-    urls = {
-        "production": "wss://compute.api.globus.org/ws/v2/",
-        "dev": "wss://api.dev.funcx.org/ws/v2/",
-        "local": "ws://localhost:6000/v2",
-    }
-    return urls.get(env, urls["production"])
-
-
-def urls_might_mismatch(service_url: str, socket_url: str) -> bool:
-    parsed_service, parsed_socket = urlparse(service_url), urlparse(socket_url)
-    return parsed_service.hostname != parsed_socket.hostname
-
-
 def remove_url_path(url: str):
     parsed_url = urlparse(url)
     return f"{parsed_url.scheme}://{parsed_url.netloc}"
```

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/asynchronous/compute_future.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/asynchronous/compute_future.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/asynchronous/compute_task.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/asynchronous/compute_task.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/client.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 from __future__ import annotations
 
-import asyncio
 import json
 import logging
 import os
 import typing as t
 import uuid
 import warnings
 
 from globus_compute_sdk.errors import (
     SerializationError,
     TaskExecutionFailed,
     TaskPending,
 )
-from globus_compute_sdk.sdk._environments import (
-    get_web_service_url,
-    get_web_socket_url,
-    urls_might_mismatch,
-)
-from globus_compute_sdk.sdk.asynchronous.compute_task import ComputeTask
-from globus_compute_sdk.sdk.asynchronous.ws_polling_task import WebSocketPollingTask
+from globus_compute_sdk.sdk._environments import get_web_service_url
+from globus_compute_sdk.sdk.utils.uuid_like import UUID_LIKE_T
 from globus_compute_sdk.sdk.web_client import FunctionRegistrationData
 from globus_compute_sdk.serialize import ComputeSerializer, SerializationStrategy
 from globus_compute_sdk.version import __version__, compare_versions
 
 from .batch import Batch
 from .login_manager import LoginManager, LoginManagerProtocol, requires_login
 
 logger = logging.getLogger(__name__)
 
-_FUNCX_HOME = os.path.join("~", ".globus_compute")
-
 
 class Client:
     """Main class for interacting with the Globus Compute service
 
     Holds helper operations for performing common tasks with the Globus Compute service.
     """
 
@@ -45,26 +37,19 @@
         "FUNCX_SCOPE",
         "https://auth.globus.org/scopes/facd7ccc-c5f4-42aa-916b-a0e270e2c2a9/all",
     )
 
     def __init__(
         self,
         http_timeout=None,
-        funcx_home=_FUNCX_HOME,
-        asynchronous: bool | None = None,
-        loop=None,
+        funcx_home=None,
         environment: str | None = None,
-        funcx_service_address: str | None = None,
-        results_ws_uri: str | None = None,
-        warn_about_url_mismatch: bool | None = None,
         task_group_id: t.Union[None, uuid.UUID, str] = None,
+        funcx_service_address: str | None = None,
         do_version_check: bool = True,
-        openid_authorizer: t.Any = None,
-        search_authorizer: t.Any = None,
-        fx_authorizer: t.Any = None,
         *,
         code_serialization_strategy: SerializationStrategy | None = None,
         data_serialization_strategy: SerializationStrategy | None = None,
         login_manager: LoginManagerProtocol | None = None,
         **kwargs,
     ):
         """
@@ -72,98 +57,75 @@
 
         Parameters
         ----------
         http_timeout: int
             Timeout for any call to service in seconds.
             Default is no timeout
 
-        environment: str
-            For internal use only. The name of the environment to use. Sets
-            funcx_service_address and results_ws_uri unless they are already passed in.
+            DEPRECATED - see self.web_client
 
-        funcx_service_address: str
-            For internal use only. The address of the web service.
+        funcx_home: any
+            DEPRECATED - was never used
 
-        results_ws_uri: str
-            For internal use only. The address of the websocket service.
+        environment: str
+            For internal use only. The name of the environment to use. Sets
+            funcx_service_address appropriately, unless already set.
 
-            DEPRECATED - use Executor instead.
+        task_group_id: str|uuid.UUID
+            Set the TaskGroup ID (a UUID) for this Client instance.
+            Typically, one uses this to submit new tasks to an existing
+            session or to reestablish Executor futures.
+            Default: None (will be auto generated)
 
-        warn_about_url_mismatch: bool
-            For internal use only. If true, a warning is logged if funcx_service_address
-            and results_ws_uri appear to point to different environments.
+            DEPRECATED - use create_batch or the executor instead
 
-            DEPRECATED - use Executor instead.
+        funcx_service_address: str
+            For internal use only. The address of the web service.
 
         do_version_check: bool
             Set to ``False`` to skip the version compatibility check on client
             initialization
             Default: True
 
-        asynchronous: bool
-            Should the API use asynchronous interactions with the web service?
-            Currently only impacts the run method.
-
-            DEPRECATED - this was an early attempt at asynchronous result gathering.
-                Use the Executor instead.
-
-            Default: False
-
-        loop: AbstractEventLoop
-            If asynchronous mode is requested, then you can provide an optional
-            event loop instance. If None, then we will access asyncio.get_event_loop()
-
-            DEPRECATED - part of an early attempt at asynchronous result gathering.
-                Use the Executor instead.
-
-            Default: None
-
-        task_group_id: str|uuid.UUID
-            Set the TaskGroup ID (a UUID) for this Client instance.
-            Typically, one uses this to submit new tasks to an existing
-            session or to reestablish Executor futures.
-            Default: None (will be auto generated)
-
         code_serialization_strategy: SerializationStrategy
             Strategy to use when serializing function code. If None,
             globus_compute_sdk.serialize.DEFAULT_STRATEGY_CODE will be used.
 
         data_serialization_strategy: SerializationStrategy
             Strategy to use when serializing function arguments. If None,
             globus_compute_sdk.serialize.DEFAULT_STRATEGY_DATA will be used.
 
-        Keyword arguments are the same as for BaseClient.
-
+        login_manager: LoginManagerProtocol
+            Allows login logic to be overridden for specific use cases. If None, a
+            LoginManager will be used.
         """
-        # resolve URLs if not set
-        if funcx_service_address is None:
-            funcx_service_address = get_web_service_url(environment)
-
-        self._task_status_table: t.Dict[str, t.Dict] = {}
-        self.funcx_home = os.path.expanduser(funcx_home)
-        self.session_task_group_id = (
-            task_group_id and str(task_group_id) or str(uuid.uuid4())
-        )
-
         for arg, name in [
-            (openid_authorizer, "openid_authorizer"),
-            (fx_authorizer, "fx_authorizer"),
-            (search_authorizer, "search_authorizer"),
-            (asynchronous, "asynchronous"),
-            (loop, "loop"),
-            (results_ws_uri, "results_ws_uri"),
-            (warn_about_url_mismatch, "warn_about_url_mismatch"),
+            (http_timeout, "http_timeout"),
+            (funcx_home, "funcx_home"),
+            (task_group_id, "task_group_id"),
         ]:
             if arg is not None:
                 msg = (
                     f"The '{name}' argument is deprecated. "
                     "It will be removed in a future release."
                 )
                 warnings.warn(msg)
 
+        for arg_name in kwargs:
+            msg = (
+                f"The '{arg_name}' argument is unrecognized. "
+                "(It might have been removed in a previous release.)"
+            )
+            warnings.warn(msg)
+
+        if funcx_service_address is None:
+            funcx_service_address = get_web_service_url(environment)
+
+        self._task_status_table: dict[str, dict] = {}
+
         # if a login manager was passed, no login flow is triggered
         if login_manager is not None:
             self.login_manager: LoginManagerProtocol = login_manager
         # but if login handling is implicit (as when no login manager is passed)
         # then ensure that the user is logged in
         else:
             self.login_manager = LoginManager(environment=environment)
@@ -178,43 +140,14 @@
         )
 
         self.funcx_service_address = funcx_service_address
 
         if do_version_check:
             self.version_check()
 
-        self.results_ws_uri = None
-        self.asynchronous = asynchronous or False
-        if asynchronous:
-            self.loop = loop if loop else asyncio.get_event_loop()
-
-            if results_ws_uri is None:
-                results_ws_uri = get_web_socket_url(environment)
-            self.results_ws_uri = results_ws_uri
-
-            if warn_about_url_mismatch and urls_might_mismatch(
-                funcx_service_address, results_ws_uri
-            ):  # noqa
-                logger.warning(
-                    f"funcx_service_address={funcx_service_address} and "
-                    f"results_ws_uri={results_ws_uri} "
-                    "look like they might point to different environments.  "
-                    "Double check that they are the correct URLs."
-                )
-
-            # Start up an asynchronous polling loop in the background
-            self.ws_polling_task = WebSocketPollingTask(
-                self,
-                self.loop,
-                init_task_group_id=self.session_task_group_id,
-                results_ws_uri=self.results_ws_uri,
-            )
-        else:
-            self.loop = None
-
     def version_check(self, endpoint_version: str | None = None) -> None:
         """Check this client version meets the service's minimum supported version.
 
         Raises a VersionMismatch error on failure.
         """
         data = self.web_client.get_version()
 
@@ -357,126 +290,103 @@
                     )
             else:
                 results[task_id] = self._task_status_table[task_id]
 
         return results
 
     @requires_login
-    def run(self, *args, endpoint_id=None, function_id=None, **kwargs) -> str:
+    def run(
+        self, *args, endpoint_id: UUID_LIKE_T, function_id: UUID_LIKE_T, **kwargs
+    ) -> str:
         """Initiate an invocation
 
         Parameters
         ----------
         *args : Any
             Args as specified by the function signature
         endpoint_id : uuid str
             Endpoint UUID string. Required
         function_id : uuid str
             Function UUID string. Required
-        asynchronous : bool
-            Whether or not to run the function asynchronously
 
         Returns
         -------
         task_id : str
-        UUID string that identifies the task if asynchronous is False
-
-        Globus Compute Task: asyncio.Task
-        A future that will eventually resolve into the function's result if
-        asynchronous is True
+        UUID string that identifies the task
         """
-        assert endpoint_id is not None, "endpoint_id key-word argument must be set"
-        assert function_id is not None, "function_id key-word argument must be set"
-
-        batch = self.create_batch(create_websocket_queue=self.asynchronous)
-        batch.add(function_id, endpoint_id, args, kwargs)
-        r = self.batch_run(batch)
+        batch = self.create_batch()
+        batch.add(function_id, args, kwargs)
+        r = self.batch_run(endpoint_id, batch)
 
-        return r[0]
+        return r["tasks"][function_id][0]
 
-    def create_batch(self, task_group_id=None, create_websocket_queue=False) -> Batch:
+    def create_batch(
+        self,
+        task_group_id: UUID_LIKE_T | None = None,
+        user_endpoint_config: dict[str, t.Any] | None = None,
+        create_websocket_queue: bool = False,
+    ) -> Batch:
         """
         Create a Batch instance to handle batch submission in Globus Compute
 
         Parameters
         ----------
 
-        task_group_id : str
-            Override the session wide session_task_group_id with a different
-            task_group_id for this batch.
-            If task_group_id is not specified, it will default to using the client's
-            session_task_group_id
+        endpoint_id : UUID-like
+            ID of the endpoint where the tasks in this batch will be executed
+
+        task_group_id : UUID-like (optional)
+            Associate this batch with a pre-existing Task Group. If there is no Task
+            Group associated with the given ID, or the user is not authorized to use
+            it, the services will respond with an error.
+            If task_group_id is not specified, the services will create a Task Group.
+
+        user_endpoint_config: dict (optional)
+            User endpoint configuration values as described and allowed by endpoint
+            administrators
 
         create_websocket_queue : bool
             Whether to create a websocket queue for the task_group_id if
             it isn't already created
 
         Returns
         -------
         Batch instance
-            Status block containing "status" key.
         """
-        if not task_group_id:
-            task_group_id = self.session_task_group_id
-
         return Batch(
-            task_group_id=task_group_id, create_websocket_queue=create_websocket_queue
+            task_group_id,
+            user_endpoint_config,
+            create_websocket_queue,
+            serializer=self.fx_serializer,
         )
 
     @requires_login
-    def batch_run(self, batch) -> t.List[str]:
-        """Initiate a batch of tasks to Globus Compute
+    def batch_run(
+        self, endpoint_id: UUID_LIKE_T, batch: Batch
+    ) -> dict[str, str | dict[str, list[str]]]:
+        """
+        Initiate a batch of tasks to Globus Compute
 
-        Parameters
-        ----------
-        batch: a Batch object
+        :param endpoint_id: The endpoint identifier to which to send the batch
+        :param batch: a Batch object
 
         Returns
         -------
-        task_ids : a list of UUID strings that identify the tasks
+        dictionary with the following keys:
+            tasks: a mapping of function IDs to lists of task IDs
+            request_id: arbitrary unique string the web-service assigns this request
+                (only intended for help with support requests)
+            task_group_id: the task group identifier associated with the submitted tasks
+            endpoint_id: the endpoint the tasks were submitted to
         """
-        assert isinstance(batch, Batch), "Requires a Batch object as input"
-        assert len(batch.tasks) > 0, "Requires a non-empty batch"
-
-        data = batch.prepare()
+        if not batch:
+            raise ValueError("No tasks specified for batch run")
 
         # Send the data to Globus Compute
-        r = self.web_client.submit(data)
-
-        task_uuids: t.List[str] = []
-        for result in r["results"]:
-            task_id = result["task_uuid"]
-            task_uuids.append(task_id)
-            if not (200 <= result["http_status_code"] < 300):
-                # this method of handling errors for a batch response is not
-                # ideal, as it will raise any error in the multi-response,
-                # but it will do until batch_run is deprecated in favor of Executer
-                # Note that some errors may already be caught and raised
-                # by globus_compute_sdk.sdk.client.request as GlobusAPIError
-
-                # Checking for 'Failed' is how FuncxResponseError.unpack
-                # originally checked for errors.
-
-                # All errors should have 'reason' but just in case
-                error_reason = result.get("reason", "Unknown execution failure")
-                raise TaskExecutionFailed(error_reason)
-
-        if self.asynchronous:
-            task_group_id = r["task_group_id"]
-            asyncio_tasks = []
-            for task_id in task_uuids:
-                funcx_task = ComputeTask(task_id)
-                asyncio_task = self.loop.create_task(funcx_task.get_result())
-                asyncio_tasks.append(asyncio_task)
-
-                self.ws_polling_task.add_task(funcx_task)
-            self.ws_polling_task.put_task_group_id(task_group_id)
-            return asyncio_tasks
-
-        return task_uuids
+        return self.web_client.submit(endpoint_id, batch.prepare()).data
 
     @requires_login
     def register_endpoint(
         self,
         name,
         endpoint_id,
         metadata=None,
@@ -822,7 +732,23 @@
 
         Returns
         -------
         json
             The response of the request
         """
         return self.web_client.delete_endpoint(endpoint_id)
+
+    @requires_login
+    def delete_function(self, function_id: str):
+        """Delete a function
+
+        Parameters
+        ----------
+        function_id : str
+            The UUID of the function
+
+        Returns
+        -------
+        json
+            The response of the request
+        """
+        return self.web_client.delete_function(function_id)
```

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/container_spec.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/container_spec.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/executor.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/executor.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from __future__ import annotations
 
 import concurrent.futures
+import json
 import logging
 import os
 import queue
 import random
 import sys
 import threading
 import time
 import typing as t
 import uuid
 import warnings
+from collections import defaultdict
 
 if sys.version_info >= (3, 8):
     from concurrent.futures import InvalidStateError
 else:
 
     class InvalidStateError(Exception):
         pass
@@ -23,14 +25,19 @@
 import pika
 from globus_compute_common import messagepack
 from globus_compute_common.messagepack.message_types import Result
 from globus_compute_sdk.errors import TaskExecutionFailed
 from globus_compute_sdk.sdk.asynchronous.compute_future import ComputeFuture
 from globus_compute_sdk.sdk.client import Client
 from globus_compute_sdk.sdk.utils import chunk_by
+from globus_compute_sdk.sdk.utils.uuid_like import (
+    UUID_LIKE_T,
+    as_optional_uuid,
+    as_uuid,
+)
 
 log = logging.getLogger(__name__)
 
 if t.TYPE_CHECKING:
     import pika.exceptions
     from pika.channel import Channel
     from pika.frame import Method
@@ -47,104 +54,87 @@
         gce = to_shutdown.pop()
         gce.shutdown()
 
 
 threading.Thread(target=__executor_atexit).start()
 
 
-class TaskSubmissionInfo:
+class _TaskSubmissionInfo:
+    __slots__ = (
+        "task_num",
+        "task_group_uuid",
+        "endpoint_uuid",
+        "function_uuid",
+        "user_endpoint_config",
+        "args",
+        "kwargs",
+    )
+
     def __init__(
         self,
         *,
         task_num: int,
-        function_id: str,
-        endpoint_id: str,
+        task_group_id: UUID_LIKE_T | None,
+        endpoint_id: UUID_LIKE_T,
+        function_id: UUID_LIKE_T,
+        user_endpoint_config: dict[str, t.Any] | None,
         args: tuple,
         kwargs: dict,
     ):
         self.task_num = task_num
-        self.function_id = function_id
-        self.endpoint_id = endpoint_id
+        self.task_group_uuid = as_optional_uuid(task_group_id)
+        self.function_uuid = as_uuid(function_id)
+        self.endpoint_uuid = as_uuid(endpoint_id)
+        self.user_endpoint_config = user_endpoint_config
         self.args = args
         self.kwargs = kwargs
 
     def __repr__(self):
-        return (
-            "TaskSubmissionInfo("
-            f"task_num={self.task_num}, "
-            f"function_id='{self.function_id}', "
-            f"endpoint_id='{self.endpoint_id}', "
-            "args=..., kwargs=...)"
+        attrs = (
+            f"task_num={self.task_num}",
+            f"task_group_uuid='{self.task_group_uuid}'",
+            f"endpoint_uuid='{self.endpoint_uuid}'",
+            f"function_uuid='{self.function_uuid}'",
+            f"user_endpoint_config={{{len(self.user_endpoint_config or {})}}}",
+            f"args=[{len(self.args)}]",
+            f"kwargs=[{len(self.kwargs)}]",
         )
-
-
-class AtomicController:
-    """This is used to synchronize between the Executor which starts
-    WebSocketPollingTasks and the WebSocketPollingTask which closes itself when there
-    are 0 tasks.
-    """
-
-    def __init__(self, start_callback, stop_callback):
-        self._value = 0
-        self._lock = threading.Lock()
-        self.start_callback = start_callback
-        self.stop_callback = stop_callback
-
-    def reset(self):
-        """Reset the counter to 0; this method does not call callbacks"""
-        with self._lock:
-            self._value = 0
-
-    def increment(self, val: int = 1):
-        with self._lock:
-            if self._value == 0:
-                self.start_callback()
-            self._value += val
-
-    def decrement(self):
-        with self._lock:
-            self._value -= 1
-            if self._value == 0:
-                self.stop_callback()
-            return self._value
-
-    def value(self):
-        with self._lock:
-            return self._value
-
-    def __repr__(self):
-        return f"AtomicController value:{self._value}"
+        return f"{type(self).__name__}({'; '.join(attrs)})"
 
 
 class Executor(concurrent.futures.Executor):
     """
     Extend Python's |Executor|_ base class for Globus Compute's purposes.
 
     .. |Executor| replace:: ``Executor``
     .. _Executor: https://docs.python.org/3/library/concurrent.futures.html#executor-objects
     """  # noqa
 
     def __init__(
         self,
-        endpoint_id: str | None = None,
-        container_id: str | None = None,
+        endpoint_id: UUID_LIKE_T | None = None,
+        container_id: UUID_LIKE_T | None = None,
         funcx_client: Client | None = None,
-        task_group_id: str | None = None,
+        task_group_id: UUID_LIKE_T | None = None,
+        user_endpoint_config: dict[str, t.Any] | None = None,
         label: str = "",
         batch_size: int = 128,
         **kwargs,
     ):
         """
         :param endpoint_id: id of the endpoint to which to submit tasks
         :param container_id: id of the container in which to execute tasks
         :param funcx_client: instance of Client to be used by the
             executor.  If not provided, the executor will instantiate one with default
             arguments.
         :param task_group_id: The Task Group to which to associate tasks.  If not set,
             one will be instantiated.
+        :param user_endpoint_config: User endpoint configuration values as described
+            and allowed by endpoint administrators. Must be a JSON-serializable dict
+            or None.
         :param label: a label to name the executor; mainly utilized for
             logging and advanced needs with multiple executors.
         :param batch_size: the maximum number of tasks to coalesce before
             sending upstream [min: 1, default: 128]
         :param batch_interval: [DEPRECATED; unused] number of seconds to coalesce tasks
             before submitting upstream
         :param batch_enabled: [DEPRECATED; unused] whether to batch results
@@ -161,23 +151,30 @@
             raise TypeError(msg)
 
         if not funcx_client:
             funcx_client = Client()
         self.funcx_client = funcx_client
 
         self.endpoint_id = endpoint_id
-        self.container_id = container_id
+
+        # mypy ... sometimes you just ain't too bright
+        self.container_id = container_id  # type: ignore[assignment]
+
+        self._task_group_id: uuid.UUID | None = None  # help mypy out
+        self.task_group_id = task_group_id
+
+        self.user_endpoint_config = user_endpoint_config
+
         self.label = label
         self.batch_size = max(1, batch_size)
 
         self.task_count_submitted = 0
         self._task_counter: int = 0
-        self._task_group_id: str = task_group_id or str(uuid.uuid4())
         self._tasks_to_send: queue.Queue[
-            tuple[ComputeFuture, TaskSubmissionInfo] | tuple[None, None]
+            tuple[ComputeFuture, _TaskSubmissionInfo] | tuple[None, None]
         ] = queue.Queue()
         self._function_registry: dict[tuple[t.Callable, str | None], str] = {}
 
         self._stopped = False
         self._stopped_in_error = False
         self._shutdown_lock = threading.RLock()
         self._result_watcher: _ResultWatcher | None = None
@@ -187,45 +184,122 @@
             target=self._task_submitter_impl, name="TaskSubmitter"
         )
         self._task_submitter.start()
         _REGISTERED_FXEXECUTORS[id(self)] = self
 
     def __repr__(self) -> str:
         name = self.__class__.__name__
-        label = self.label and f"{self.label}, " or ""
-        ep_id = self.endpoint_id and f", ep_id:{self.endpoint_id}" or ""
-        c_id = self.container_id and f", c_id:{self.container_id}" or ""
-        tg_id = f", tg_id:{self.task_group_id}"
-        return f"{name}<{label}{self.batch_size}{ep_id}{c_id}{tg_id}>"
+        label = self.label and f"{self.label}; " or ""
+        ep_id = self.endpoint_id and f"ep_id:{self.endpoint_id}; " or ""
+        c_id = self.container_id and f"c_id:{self.container_id}; " or ""
+        tg_id = f"tg_id:{self.task_group_id}; "
+        bs = f"bs:{self.batch_size}"
+        return f"{name}<{label}{ep_id}{c_id}{tg_id}{bs}>"
 
     @property
-    def task_group_id(self) -> str:
+    def task_group_id(self):
         """
         The Task Group with which this instance is currently associated.  New tasks will
         be sent to this Task Group upstream, and the result listener will only listen
         for results for this group.
 
-        Must be a string.  Set by simple assignment::
+        Must be a UUID, valid uuid-like string, or None.  Set by simple assignment::
+
+            >>> import uuid
+            >>> from globus_compute_sdk import Executor
+            >>> tg_id = uuid.uuid4()  # IRL: some *known* taskgroup id
+            >>> gce = Executor(task_group_id=tg_id)
+
+            # Alternatively, may use a stringified uuid:
+            >>> gce = Executor(task_group_id=str(tg_id))
+
+            # May also alter after construction:
+            >>> gce.task_group_id = tg_id
+            >>> gce.task_group_id = str(tg_id)
+
+            # Internally, it is always stored as a UUID (or None):
+            >>> gce.task_group_id
+            UUID('11111111-2222-4444-8888-000000000000')
 
-            gce = Executor(endpoint_id="...")
-            gce.task_group_id = "Some-stored-id"
+        This is typically used when reattaching to a previously initiated set
+        of tasks.  See `reload_tasks()`_ for more information.
 
-        This is typically used when reattaching to a previously initiated set of tasks.
-        See `reload_tasks()`_ for more information.
+        If not set manually, this will be set automatically on `submit()`_, to
+        a Task Group ID supplied by the services.
 
-        [default: ``None``, which translates to the Client task group id]
+        [default: ``None``]
         """
         return self._task_group_id
 
     @task_group_id.setter
-    def task_group_id(self, task_group_id: str):
-        self._task_group_id = task_group_id
+    def task_group_id(self, task_group_id: UUID_LIKE_T | None):
+        self._task_group_id = as_optional_uuid(task_group_id)
+
+    @property
+    def user_endpoint_config(self) -> dict[str, t.Any] | None:
+        """
+        The endpoint configuration values, as described and allowed by endpoint
+        administrators, that this instance is currently associated with.
+
+        Must be a JSON-serializable dict or None. Set by simple assignment::
+
+            >>> from globus_compute_sdk import Executor
+            >>> uep_config = {"foo": "bar"}
+            >>> gce = Executor(user_endpoint_config=uep_config)
+
+            # May also alter after construction:
+            >>> gce.user_endpoint_config = uep_config
+        """
+        return self._user_endpoint_config
+
+    @user_endpoint_config.setter
+    def user_endpoint_config(self, val: dict | None):
+        if val is not None:
+            if not isinstance(val, dict):
+                raise TypeError(
+                    f"Config must be of type dict, not {type(val).__name__}"
+                )
+            try:
+                json.dumps(val)
+            except TypeError:
+                raise TypeError("Configuration must be JSON-serializable")
+        self._user_endpoint_config = val
+
+    @property
+    def container_id(self) -> uuid.UUID | None:
+        """
+        The container id with which this Executor instance is currently associated.
+        Tasks submitted after this is set will use this container.
+
+        Must be a UUID, valid uuid-like string, or None.  Set by simple assignment::
+
+            >>> import uuid
+            >>> from globus_compute_sdk import Executor
+            >>> c_id = "00000000-0000-0000-0000-000000000000"  # some known container id
+            >>> c_as_uuid = uuid.UUID(c_id)
+            >>> gce = Executor(container_id=c_id)
+
+            # May also alter after construction:
+            >>> gce.container_id = c_id
+            >>> gce.container_id = c_as_uuid  # also accepts a UUID object
+
+            # Internally, it is always stored as a UUID (or None):
+            >>> gce.container_id
+            UUID('00000000-0000-0000-0000-000000000000')
+
+        [default: ``None``]
+        """
+        return self._container_id
+
+    @container_id.setter
+    def container_id(self, c_id: UUID_LIKE_T | None):
+        self._container_id = as_optional_uuid(c_id)
 
     def _fn_cache_key(self, fn: t.Callable):
-        return (fn, self.container_id)
+        return fn, self.container_id
 
     def register_function(
         self, fn: t.Callable, function_id: str | None = None, **func_register_kwargs
     ) -> str:
         """
         Register a task function with this Executor's cache.
 
@@ -397,18 +471,20 @@
         if args is None:
             args = ()
         if kwargs is None:
             kwargs = {}
 
         self._task_counter += 1
 
-        task = TaskSubmissionInfo(
+        task = _TaskSubmissionInfo(
             task_num=self._task_counter,  # unnecessary; maybe useful for debugging?
-            function_id=function_id,
+            task_group_id=self.task_group_id,
             endpoint_id=self.endpoint_id,
+            user_endpoint_config=self.user_endpoint_config,
+            function_id=function_id,
             args=args,
             kwargs=kwargs,
         )
 
         fut = ComputeFuture()
         self._tasks_to_send.put((fut, task))
         return fut
@@ -431,39 +507,51 @@
         Raises
         ------
         NotImplementedError
           always raised
         """  # noqa
         raise NotImplementedError()
 
-    def reload_tasks(self) -> t.Iterable[ComputeFuture]:
+    def reload_tasks(
+        self, task_group_id: UUID_LIKE_T | None = None
+    ) -> t.Iterable[ComputeFuture]:
         """
         .. _reload_tasks():
 
         Load the set of tasks associated with this Executor's Task Group from the
         web services and return a list of futures, one for each task.  This is
         nominally intended to "reattach" to a previously initiated session, based on
         the Task Group ID.
 
+        :param task_group_id: Optionally specify a task_group_id to use. If present,
+            will overwrite the Executor's task_group_id
         :returns: An iterable of futures.
         :raises ValueError: if the server response is incorrect or invalid
         :raises KeyError: the server did not return an expected response
         :raises various: the usual (unhandled) request errors (e.g., no connection;
             invalid authorization)
 
         Notes
         -----
         Any previous futures received from this executor will be cancelled.
         """  # noqa
+        if task_group_id is not None:
+            self.task_group_id = task_group_id
+
+        if self.task_group_id is None:
+            raise ValueError("must specify a task_group_id in order to reload tasks")
+
         # step 1: cleanup!
         if self._result_watcher:
             self._result_watcher.shutdown(wait=False, cancel_futures=True)
             self._result_watcher = None
 
         task_group_id = self.task_group_id  # snapshot
+        assert task_group_id is not None  # mypy: we _just_ proved this
+
         # step 2: from server, acquire list of related task ids and make futures
         r = self.funcx_client.web_client.get_taskgroup_tasks(task_group_id)
         if r["taskgroup_id"] != task_group_id:
             msg = (
                 "Server did not respond with requested TaskGroup Tasks.  "
                 f"(Requested tasks for {task_group_id} but received "
                 f"tasks for {r['taskgroup_id']}"
@@ -567,59 +655,102 @@
         This thread stops when it receives a poison-pill of ``(None, None)``
         in the queue.  (See ``shutdown()``.)
         """
         log.debug(
             "%s: task submission thread started (%s)", self, threading.get_ident()
         )
         to_send = self._tasks_to_send  # cache lookup
-        futs: list[ComputeFuture] = []  # for mypy/the exception branch
+
+        # Alias types -- this awkward typing is all about the dict we use
+        # internally to make sure we appropriately group tasks for upstream
+        # submission.  For example, if the user submitted to two different
+        # endpoints, we separate the tasks by the dictionary key.
+        class SubmitGroup(t.NamedTuple):
+            task_group_uuid: uuid.UUID | None
+            endpoint_uuid: uuid.UUID
+            user_endpoint_config: str
+
+        SubmitGroupFutures = t.Dict[
+            SubmitGroup,
+            t.List[ComputeFuture],
+        ]
+        SubmitGroupTasks = t.Dict[
+            SubmitGroup,
+            t.List[_TaskSubmissionInfo],
+        ]
+
         try:
             fut: ComputeFuture | None = ComputeFuture()  # just start the loop; please
             while fut is not None:
-                futs = []
-                tasks: list[TaskSubmissionInfo] = []
+                futs: SubmitGroupFutures = defaultdict(list)
+                tasks: SubmitGroupTasks = defaultdict(list)
                 task_count = 0
                 try:
                     fut, task = to_send.get()  # Block; wait for first result ...
                     task_count += 1
                     bs = max(1, self.batch_size)  # May have changed while waiting
                     while task is not None:
                         assert fut is not None  # Come on mypy; contextually clear!
-                        tasks.append(task)
-                        futs.append(fut)
-                        if not (len(tasks) < bs):
+                        submit_group = SubmitGroup(
+                            task.task_group_uuid,
+                            task.endpoint_uuid,
+                            # dict type is unhashable
+                            json.dumps(task.user_endpoint_config, sort_keys=True),
+                        )
+                        tasks[submit_group].append(task)
+                        futs[submit_group].append(fut)
+                        if any(len(tl) >= bs for tl in tasks.values()):
                             break
                         fut, task = to_send.get(block=False)  # ... don't block again
                         task_count += 1
                 except queue.Empty:
                     pass
 
                 if not tasks:
                     continue
 
-                log.info(f"Submitting tasks to Globus Compute: {len(tasks)}")
-                self._submit_tasks(futs, tasks)
+                for submit_group, task_list in tasks.items():
+                    fut_list = futs[submit_group]
+
+                    tg_uuid, ep_uuid, uep_config = submit_group
+                    uep_config = json.loads(uep_config)
+                    # Needed for mypy
+                    assert uep_config is None or isinstance(uep_config, dict)
+                    log.info(
+                        f"Submitting tasks for Task Group {tg_uuid} to"
+                        f" Endpoint {ep_uuid}: {len(task_list):,}"
+                    )
+
+                    self._submit_tasks(
+                        tg_uuid, ep_uuid, uep_config, fut_list, task_list
+                    )
 
-                with self._shutdown_lock:
-                    if self._stopped:
+                    to_watch = [f for f in fut_list if f.task_id and not f.done()]
+                    if not to_watch:
                         continue
 
-                    if not (self._result_watcher and self._result_watcher.is_alive()):
-                        # Don't initialize the result watcher unless at least
-                        # one batch has been sent
-                        self._result_watcher = _ResultWatcher(self)
-                        self._result_watcher.start()
-                    try:
-                        self._result_watcher.watch_for_task_results(futs)
-                    except self._result_watcher.__class__.ShuttingDownError:
-                        log.debug("Waiting for previous ResultWatcher to shutdown")
-                        self._result_watcher.join()
-                        self._result_watcher = _ResultWatcher(self)
-                        self._result_watcher.start()
-                        self._result_watcher.watch_for_task_results(futs)
+                    with self._shutdown_lock:
+                        if self._stopped:
+                            continue
+
+                        if not (
+                            self._result_watcher and self._result_watcher.is_alive()
+                        ):
+                            # Don't initialize the result watcher unless at least
+                            # one batch has been sent
+                            self._result_watcher = _ResultWatcher(self)
+                            self._result_watcher.start()
+                        try:
+                            self._result_watcher.watch_for_task_results(to_watch)
+                        except self._result_watcher.__class__.ShuttingDownError:
+                            log.debug("Waiting for previous ResultWatcher to shutdown")
+                            self._result_watcher.join()
+                            self._result_watcher = _ResultWatcher(self)
+                            self._result_watcher.start()
+                            self._result_watcher.watch_for_task_results(to_watch)
 
                 # important to clear futures; else a legitimately early-shutdown
                 # request (e.g., __exit__()) can cancel these (finally block,
                 # below) before the result comes back, even though _result_watcher
                 # is already watching them.
                 futs.clear()
 
@@ -645,58 +776,120 @@
             raise
         finally:
             if sys.exc_info() != (None, None, None):
                 time.sleep(0.1)  # give any in-flight Futures a chance to be .put() ...
             while not self._tasks_to_send.empty():
                 fut, _task = self._tasks_to_send.get()
                 if fut:
-                    futs.append(fut)
-
-            for fut in futs:
-                fut.cancel()
-                fut.set_running_or_notify_cancel()
+                    fut.cancel()
+                    fut.set_running_or_notify_cancel()
             try:
                 while True:
                     self._tasks_to_send.task_done()
             except ValueError:
                 pass
             log.debug("%s: task submission thread complete", self)
 
-    def _submit_tasks(self, futs: list[ComputeFuture], tasks: list[TaskSubmissionInfo]):
+    def _submit_tasks(
+        self,
+        taskgroup_uuid: uuid.UUID | None,
+        endpoint_uuid: uuid.UUID,
+        user_endpoint_config: dict | None,
+        futs: list[ComputeFuture],
+        tasks: list[_TaskSubmissionInfo],
+    ):
         """
         Submit a batch of tasks to the webservice, destined for self.endpoint_id.
         Upon success, update the futures with their associated task_id.
 
+        :param endpoint_uuid: UUID of the Endpoint on which to execute this batch.
+        :param taskgroup_uuid: UUID of the task group
+        :param user_endpoint_config: User endpoint configuration values as described and
+            allowed by endpoint administrators
         :param futs: a list of ComputeFutures; will have their task_id attribute
             set when function completes successfully.
         :param tasks: a list of tasks to submit upstream in a batch.
         """
+        if taskgroup_uuid is None and self.task_group_id:
+            taskgroup_uuid = self.task_group_id
+
         batch = self.funcx_client.create_batch(
-            task_group_id=self.task_group_id,
-            create_websocket_queue=True,
+            taskgroup_uuid, user_endpoint_config, create_websocket_queue=True
         )
-        for task in tasks:
-            batch.add(task.function_id, task.endpoint_id, task.args, task.kwargs)
+        submitted_futs_by_fn: t.DefaultDict[str, list[ComputeFuture]] = defaultdict(
+            list
+        )
+        for fut, task in zip(futs, tasks):
+            f_uuid_str = str(task.function_uuid)
+            submitted_futs_by_fn[f_uuid_str].append(fut)
+            batch.add(f_uuid_str, task.args, task.kwargs)
             log.debug("Added task to Globus Compute batch: %s", task)
 
         try:
-            batch_tasks = self.funcx_client.batch_run(batch)
-        except Exception:
-            log.error(f"Error submitting {len(tasks)} tasks to Globus Compute")
+            batch_response = self.funcx_client.batch_run(endpoint_uuid, batch)
+        except Exception as e:
+            log.exception(f"Error submitting {len(tasks)} tasks to Globus Compute")
+            for fut_list in submitted_futs_by_fn.values():
+                for fut in fut_list:
+                    fut.set_exception(e)
+            raise
+
+        try:
+            received_tasks_by_fn: dict[str, list[str]] = batch_response["tasks"]
+            new_tg_id: str = batch_response["task_group_id"]
+        except Exception as e:
+            log.exception(
+                f"Server response ({batch_response}) missing an expected field"
+            )
+            for fut_list in submitted_futs_by_fn.values():
+                for fut in fut_list:
+                    fut.set_exception(e)
             raise
 
-        self.task_count_submitted += len(batch_tasks)
+        if str(self.task_group_id) != new_tg_id:
+            log.info(f"Updating task_group_id from {self.task_group_id} to {new_tg_id}")
+            self.task_group_id = new_tg_id
+
+        batch_count = sum(len(x) for x in received_tasks_by_fn.values())
+        self.task_count_submitted += batch_count
         log.debug(
-            "Batch submitted to task_group: %s - %s",
+            "Batch submitted to task_group: %s - %s (total: %s)",
             self.task_group_id,
+            batch_count,
             self.task_count_submitted,
         )
 
-        for fut, task_uuid in zip(futs, batch_tasks):
-            fut.task_id = task_uuid
+        for fn_id, fut_list in submitted_futs_by_fn.items():
+            task_uuids = received_tasks_by_fn.get(fn_id)
+
+            if task_uuids is None:
+                fut_exc = Exception(
+                    f"The Globus Compute Service ignored tasks for function {fn_id}!"
+                    "  This 'should not happen,' so please reach out to the Globus"
+                    " Compute team if you are able to recreate this behavior."
+                )
+                for fut in fut_list:
+                    fut.set_exception(fut_exc)
+                continue
+
+            if len(fut_list) != len(task_uuids):
+                fut_exc = Exception(
+                    "The Globus Compute Service only partially initiated requested"
+                    f" tasks for function {fn_id}!  It is unclear which tasks it"
+                    " honored, so marking all futures as failed.  Please reach out"
+                    " to the Globus Compute team if you are able to recreate this"
+                    " behavior."
+                )
+                for fut in fut_list:
+                    fut.set_exception(fut_exc)
+                continue
+
+            # Happy -- expected -- path
+            for fut, task_id in zip(fut_list, task_uuids):
+                fut.task_id = task_id
 
 
 class _ResultWatcher(threading.Thread):
     """
     _ResultWatcher is an internal SDK class meant for consumption by the
     Executor.  It is a standard async AMQP consumer implementation
     using the Pika library that matches futures from the Executor against
@@ -902,15 +1095,17 @@
             if self._closed:
                 msg = "Unable to watch futures: %s is shutting down."
                 raise self.__class__.ShuttingDownError(msg % self.__class__.__name__)
 
             to_watch = {
                 f.task_id: f
                 for f in futures
-                if f.task_id and f.task_id not in self._open_futures
+                if f.task_id
+                if not f.done()
+                if f.task_id not in self._open_futures
             }
             self._open_futures.update(to_watch)
 
             if self._open_futures:  # futures as an empty list is acceptable
                 self._open_futures_empty.clear()
                 if self._received_results:
                     # no sense is setting the event if there are not yet
```

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/client_login.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/client_login.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/decorators.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/decorators.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/login_flow.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/login_flow.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/manager.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/protocol.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/protocol.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/tokenstore.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/tokenstore.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/login_manager/whoami.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/login_manager/whoami.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/utils/printing.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/utils/printing.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/sdk/web_client.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/sdk/web_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 Globus Compute web service.
 
 It also implements data helpers for building complex payloads. Most notably,
 `FunctionRegistrationData` which can be constructed from an arbitrary callable.
 """
 import json
 import typing as t
-import uuid
 
 import globus_sdk
 from globus_compute_common.sdk_version_sharing import user_agent_substring
 from globus_compute_sdk.sdk._environments import get_web_service_url, remove_url_path
+from globus_compute_sdk.sdk.utils.uuid_like import UUID_LIKE_T
 from globus_compute_sdk.serialize import ComputeSerializer
 from globus_compute_sdk.version import __version__
 from globus_sdk.exc.api import GlobusAPIError
 
-ID_PARAM_T = t.Union[uuid.UUID, str]
-
 
 def _get_packed_code(
     func: t.Callable, serializer: t.Optional[ComputeSerializer] = None
 ) -> str:
     serializer = serializer if serializer else ComputeSerializer()
     return serializer.pack_buffers([serializer.serialize(func)])
 
@@ -29,15 +27,15 @@
 class FunctionRegistrationData:
     def __init__(
         self,
         *,
         function: t.Optional[t.Callable] = None,
         function_name: t.Optional[str] = None,
         function_code: t.Optional[str] = None,
-        container_uuid: t.Optional[ID_PARAM_T] = None,
+        container_uuid: t.Optional[UUID_LIKE_T] = None,
         description: t.Optional[str] = None,
         public: bool = False,
         group: t.Optional[str] = None,
         serializer: t.Optional[ComputeSerializer] = None,
     ):
         if function is not None:
             function_name = function.__name__
@@ -98,24 +96,24 @@
         self._user_app_name = None
         self.user_app_name = app_name
 
     def get_version(self, *, service: str = "all") -> globus_sdk.GlobusHTTPResponse:
         return self.get("/v2/version", query_params={"service": service})
 
     def get_taskgroup_tasks(
-        self, task_group_id: ID_PARAM_T
+        self, task_group_id: UUID_LIKE_T
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.get(f"/v2/taskgroup/{task_group_id}")
 
-    def get_task(self, task_id: ID_PARAM_T) -> globus_sdk.GlobusHTTPResponse:
+    def get_task(self, task_id: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
         return self.get(f"/v2/tasks/{task_id}")
 
     def get_batch_status(
         self,
-        task_ids: t.Iterable[ID_PARAM_T],
+        task_ids: t.Iterable[UUID_LIKE_T],
         *,
         additional_fields: t.Optional[t.Dict[str, t.Any]] = None,
     ) -> globus_sdk.GlobusHTTPResponse:
         if isinstance(task_ids, str):
             task_ids = [task_ids]
         data = {"task_ids": [str(t) for t in task_ids]}
         if additional_fields is not None:
@@ -142,21 +140,23 @@
     def user_app_name(self, value):
         self._user_app_name = value
         app_name = user_agent_substring(__version__)
         if value is not None:
             app_name += f"/{value}"
         globus_sdk.BaseClient.app_name.fset(self, app_name)
 
-    def submit(self, batch: t.Dict[str, t.Any]) -> globus_sdk.GlobusHTTPResponse:
-        return self.post("/v2/submit", data=batch)
+    def submit(
+        self, endpoint_id: UUID_LIKE_T, batch: t.Dict[str, t.Any]
+    ) -> globus_sdk.GlobusHTTPResponse:
+        return self.post(f"/v3/endpoints/{endpoint_id}/submit", data=batch)
 
     def register_endpoint(
         self,
         endpoint_name: str,
-        endpoint_id: ID_PARAM_T,
+        endpoint_id: UUID_LIKE_T,
         *,
         metadata: t.Optional[dict] = None,
         multi_tenant: t.Optional[bool] = None,
         display_name: t.Optional[str] = None,
         additional_fields: t.Optional[t.Dict[str, t.Any]] = None,
     ) -> globus_sdk.GlobusHTTPResponse:
         data: t.Dict[str, t.Any] = {
@@ -181,20 +181,20 @@
             data.update(additional_fields)
         return self.post("/v2/endpoints", data=data)
 
     def get_result_amqp_url(self) -> globus_sdk.GlobusHTTPResponse:
         return self.get("/v2/get_amqp_result_connection_url")
 
     def get_endpoint_status(
-        self, endpoint_id: ID_PARAM_T
+        self, endpoint_id: UUID_LIKE_T
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.get(f"/v2/endpoints/{endpoint_id}/status")
 
     def get_endpoint_metadata(
-        self, endpoint_id: ID_PARAM_T
+        self, endpoint_id: UUID_LIKE_T
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.get(f"/v2/endpoints/{endpoint_id}")
 
     def get_endpoints(self) -> globus_sdk.GlobusHTTPResponse:
         return self.get("/v2/endpoints")
 
     def register_function(
@@ -206,28 +206,35 @@
         data = (
             function_registration_data.to_dict()
             if isinstance(function_registration_data, FunctionRegistrationData)
             else function_registration_data
         )
         return self.post("/v2/functions", data=data)
 
-    def get_whitelist(self, endpoint_id: ID_PARAM_T) -> globus_sdk.GlobusHTTPResponse:
+    def get_whitelist(self, endpoint_id: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
         return self.get(f"/v2/endpoints/{endpoint_id}/whitelist")
 
     def whitelist_add(
-        self, endpoint_id: ID_PARAM_T, function_ids: t.Iterable[ID_PARAM_T]
+        self, endpoint_id: UUID_LIKE_T, function_ids: t.Iterable[UUID_LIKE_T]
     ) -> globus_sdk.GlobusHTTPResponse:
         if isinstance(function_ids, str):
             function_ids = [function_ids]
         data = {"func": [str(f) for f in function_ids]}
         return self.post(f"/v2/endpoints/{endpoint_id}/whitelist", data=data)
 
     def whitelist_remove(
-        self, endpoint_id: ID_PARAM_T, function_id: ID_PARAM_T
+        self, endpoint_id: UUID_LIKE_T, function_id: UUID_LIKE_T
     ) -> globus_sdk.GlobusHTTPResponse:
         return self.delete(f"/v2/endpoints/{endpoint_id}/whitelist/{function_id}")
 
-    def stop_endpoint(self, endpoint_id: ID_PARAM_T) -> globus_sdk.GlobusHTTPResponse:
+    def stop_endpoint(self, endpoint_id: UUID_LIKE_T) -> globus_sdk.GlobusHTTPResponse:
         return self.post(f"/v2/endpoints/{endpoint_id}/lock", data={})
 
-    def delete_endpoint(self, endpoint_id: ID_PARAM_T) -> globus_sdk.GlobusHTTPResponse:
+    def delete_endpoint(
+        self, endpoint_id: UUID_LIKE_T
+    ) -> globus_sdk.GlobusHTTPResponse:
         return self.delete(f"/v2/endpoints/{endpoint_id}")
+
+    def delete_function(
+        self, function_id: UUID_LIKE_T
+    ) -> globus_sdk.GlobusHTTPResponse:
+        return self.delete(f"/v2/functions/{function_id}")
```

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/__init__.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/base.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/concretes.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/concretes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/serialize/facade.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/serialize/facade.py`

 * *Files identical despite different names*

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk/version.py` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from globus_compute_sdk.errors import VersionMismatch
 from packaging.version import Version
 
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.2.4a0"
+__version__ = "2.3.0a0"
 
 
 def compare_versions(
     current: str, min_version: str, *, package_name: str = "globus-compute-sdk"
 ) -> None:
     current_v = Version(current)
     min_v = Version(min_version)
```

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk.egg-info/PKG-INFO` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-sdk
-Version: 2.2.4a0
+Version: 2.3.0a0
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Project-URL: Changelog, https://globus-compute.readthedocs.io/en/latest/changelog.html
 Project-URL: Upgrade to Globus Compute, https://globus-compute.readthedocs.io/en/latest/funcx_upgrade.html
```

### Comparing `globus-compute-sdk-2.2.4a0/globus_compute_sdk.egg-info/SOURCES.txt` & `globus-compute-sdk-2.3.0a0/globus_compute_sdk.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -19,23 +19,26 @@
 globus_compute_sdk/sdk/client.py
 globus_compute_sdk/sdk/container_spec.py
 globus_compute_sdk/sdk/executor.py
 globus_compute_sdk/sdk/web_client.py
 globus_compute_sdk/sdk/asynchronous/__init__.py
 globus_compute_sdk/sdk/asynchronous/compute_future.py
 globus_compute_sdk/sdk/asynchronous/compute_task.py
-globus_compute_sdk/sdk/asynchronous/ws_polling_task.py
 globus_compute_sdk/sdk/login_manager/__init__.py
 globus_compute_sdk/sdk/login_manager/client_login.py
 globus_compute_sdk/sdk/login_manager/decorators.py
 globus_compute_sdk/sdk/login_manager/globus_auth.py
 globus_compute_sdk/sdk/login_manager/login_flow.py
 globus_compute_sdk/sdk/login_manager/manager.py
 globus_compute_sdk/sdk/login_manager/protocol.py
 globus_compute_sdk/sdk/login_manager/tokenstore.py
 globus_compute_sdk/sdk/login_manager/whoami.py
 globus_compute_sdk/sdk/utils/__init__.py
 globus_compute_sdk/sdk/utils/printing.py
+globus_compute_sdk/sdk/utils/uuid_like.py
 globus_compute_sdk/serialize/__init__.py
 globus_compute_sdk/serialize/base.py
 globus_compute_sdk/serialize/concretes.py
-globus_compute_sdk/serialize/facade.py
+globus_compute_sdk/serialize/facade.py
+tests/__init__.py
+tests/conftest.py
+tests/utils.py
```

### Comparing `globus-compute-sdk-2.2.4a0/setup.py` & `globus-compute-sdk-2.3.0a0/setup.py`

 * *Files identical despite different names*

