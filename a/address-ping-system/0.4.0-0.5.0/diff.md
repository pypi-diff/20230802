# Comparing `tmp/address_ping_system-0.4.0.tar.gz` & `tmp/address_ping_system-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "address_ping_system-0.4.0.tar", last modified: Thu Jul 27 17:50:27 2023, max compression
+gzip compressed data, was "address_ping_system-0.5.0.tar", last modified: Wed Aug  2 12:10:46 2023, max compression
```

## Comparing `address_ping_system-0.4.0.tar` & `address_ping_system-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:50:27.538057 address_ping_system-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-27 17:50:13.000000 address_ping_system-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-27 17:50:27.538057 address_ping_system-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-07-27 17:50:13.000000 address_ping_system-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:50:27.538057 address_ping_system-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-27 17:50:13.000000 address_ping_system-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:50:27.530057 address_ping_system-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:50:27.534057 address_ping_system-0.4.0/src/address_ping_system/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-27 17:50:13.000000 address_ping_system-0.4.0/src/address_ping_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-27 17:50:13.000000 address_ping_system-0.4.0/src/address_ping_system/address_ping_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 17:50:27.538057 address_ping_system-0.4.0/src/address_ping_system.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-07-27 17:50:27.000000 address_ping_system-0.4.0/src/address_ping_system.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-27 17:50:27.000000 address_ping_system-0.4.0/src/address_ping_system.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:50:27.000000 address_ping_system-0.4.0/src/address_ping_system.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-27 17:50:27.000000 address_ping_system-0.4.0/src/address_ping_system.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 17:50:27.000000 address_ping_system-0.4.0/src/address_ping_system.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 17:50:27.000000 address_ping_system-0.4.0/src/address_ping_system.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-27 17:50:27.000000 address_ping_system-0.4.0/src/address_ping_system.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:10:46.714576 address_ping_system-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-08-02 12:10:35.000000 address_ping_system-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-02 12:10:46.714576 address_ping_system-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-08-02 12:10:35.000000 address_ping_system-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:10:46.714576 address_ping_system-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-08-02 12:10:35.000000 address_ping_system-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:10:46.714576 address_ping_system-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:10:46.714576 address_ping_system-0.5.0/src/address_ping_system/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-02 12:10:35.000000 address_ping_system-0.5.0/src/address_ping_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2658 2023-08-02 12:10:35.000000 address_ping_system-0.5.0/src/address_ping_system/address_ping_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:10:46.714576 address_ping_system-0.5.0/src/address_ping_system.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-08-02 12:10:46.000000 address_ping_system-0.5.0/src/address_ping_system.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-08-02 12:10:46.000000 address_ping_system-0.5.0/src/address_ping_system.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:10:46.000000 address_ping_system-0.5.0/src/address_ping_system.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-08-02 12:10:46.000000 address_ping_system-0.5.0/src/address_ping_system.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:10:46.000000 address_ping_system-0.5.0/src/address_ping_system.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-02 12:10:46.000000 address_ping_system-0.5.0/src/address_ping_system.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-02 12:10:46.000000 address_ping_system-0.5.0/src/address_ping_system.egg-info/top_level.txt
```

### Comparing `address_ping_system-0.4.0/LICENSE` & `address_ping_system-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `address_ping_system-0.4.0/PKG-INFO` & `address_ping_system-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: address_ping_system
-Version: 0.4.0
+Version: 0.5.0
 Summary: Mapping Addresses to Dynamic IPs, Simplified
 Home-page: https://github.com/Naruno/Address-Ping-System
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MIT
 Description: # Address Ping System (APS) for Naruno
         Address Ping System (APS) is a tool designed to check the online status of servers associated with blockchain addresses in Naruno. With APS, you can ensure that the servers you want to communicate with are online and reachable before sending any messages or making any transactions.
```

### Comparing `address_ping_system-0.4.0/README.md` & `address_ping_system-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `address_ping_system-0.4.0/setup.py` & `address_ping_system-0.5.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from setuptools import setup
 
 
 setup(name='address_ping_system',
-version='0.4.0',
+version='0.5.0',
 description="""Mapping Addresses to Dynamic IPs, Simplified""",
 long_description_content_type="text/markdown",
 include_package_data=True,
 long_description="".join(open("README.md", encoding="utf-8").readlines()),
 url='https://github.com/Naruno/Address-Ping-System',
 author="Naruno Developers",
 author_email='onur.atakan.ulusoy@naruno.org',
 license='MIT',
 packages=["address_ping_system"],
 package_dir={'':'src'},
 install_requires=[
     "fire==0.5.0",
-    "naruno_remote_app==0.59.0"
+    "naruno_remote_app",
+    "naruno"
 ],
 entry_points = {
     'console_scripts': ['aps=address_ping_system.address_ping_system:main'],
 },
 python_requires=">= 3",
 zip_safe=False)
```

### Comparing `address_ping_system-0.4.0/src/address_ping_system/address_ping_system.py` & `address_ping_system-0.5.0/src/address_ping_system/address_ping_system.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,17 @@
 import time
 import fire
 import pickle
 import contextlib
 
 class aps:
     command_line = False
-    def __init__(self, password, timeout=180, cache_time=120, trusted_users=[], port=8000):
+    def __init__(self, password, timeout=180, cache_time=120, trusted_users=[], port=8000, host="localhost"):
         self.trusted_users = trusted_users
-        self.integration = Integration("APS", password=password, port=port)
+        self.integration = Integration("APS", password=password, port=port host=host)
         self.timeout = timeout + self.integration.wait_amount
         self.cache_time = cache_time + self.integration.wait_amount
         self.last_ping_time = 0
 
         self.load_cache()
 
     def last_ping_time_save(self):
```

### Comparing `address_ping_system-0.4.0/src/address_ping_system.egg-info/PKG-INFO` & `address_ping_system-0.5.0/src/address_ping_system.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: address-ping-system
-Version: 0.4.0
+Version: 0.5.0
 Summary: Mapping Addresses to Dynamic IPs, Simplified
 Home-page: https://github.com/Naruno/Address-Ping-System
 Author: Naruno Developers
 Author-email: onur.atakan.ulusoy@naruno.org
 License: MIT
 Description: # Address Ping System (APS) for Naruno
         Address Ping System (APS) is a tool designed to check the online status of servers associated with blockchain addresses in Naruno. With APS, you can ensure that the servers you want to communicate with are online and reachable before sending any messages or making any transactions.
```

