# Comparing `tmp/openmodule_commands-12.1.2.tar.gz` & `tmp/openmodule_commands-12.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openmodule_commands-12.1.2.tar", last modified: Tue Aug  1 10:20:01 2023, max compression
+gzip compressed data, was "openmodule_commands-12.1.3.tar", last modified: Wed Aug  2 14:26:22 2023, max compression
```

## Comparing `openmodule_commands-12.1.2.tar` & `openmodule_commands-12.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:20:01.096619 openmodule_commands-12.1.2/
--rw-r--r--   0 root         (0) root         (0)      302 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/AUTHORS
--rw-r--r--   0 root         (0) root         (0)     8267 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/ChangeLog
--rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 10:20:01.096619 openmodule_commands-12.1.2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2826 2023-08-01 10:19:48.000000 openmodule_commands-12.1.2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 10:20:01.096619 openmodule_commands-12.1.2/openmodule_commands.egg-info/
--rw-r--r--   0 root         (0) root         (0)      618 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      232 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       46 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/pbr.json
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-01 10:20:01.000000 openmodule_commands-12.1.2/openmodule_commands.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      850 2023-08-01 10:20:01.096619 openmodule_commands-12.1.2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-08-01 10:19:48.000000 openmodule_commands-12.1.2/setup.py
--rw-rw-rw-   0 root         (0) root         (0)     8162 2023-08-01 10:19:48.000000 openmodule_commands-12.1.2/translate.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:26:22.250930 openmodule_commands-12.1.3/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/AUTHORS
+-rw-r--r--   0 root         (0) root         (0)     8235 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/ChangeLog
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-02 14:26:22.250930 openmodule_commands-12.1.3/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2826 2023-08-02 14:26:08.000000 openmodule_commands-12.1.3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 14:26:22.250930 openmodule_commands-12.1.3/openmodule_commands.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      618 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/openmodule_commands.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/openmodule_commands.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/openmodule_commands.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      232 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/openmodule_commands.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/openmodule_commands.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       46 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/openmodule_commands.egg-info/pbr.json
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-02 14:26:22.000000 openmodule_commands-12.1.3/openmodule_commands.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      850 2023-08-02 14:26:22.250930 openmodule_commands-12.1.3/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-08-02 14:26:08.000000 openmodule_commands-12.1.3/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)     8162 2023-08-02 14:26:08.000000 openmodule_commands-12.1.3/translate.py
```

### Comparing `openmodule_commands-12.1.2/ChangeLog` & `openmodule_commands-12.1.3/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 CHANGES
 =======
 
+v12.1.3
+-------
+
+* docs
+* use hashlib to compute hash
+
 v12.1.2
 -------
 
 * databox changed to rpc\_no\_blocking -> no exceptions and no waiting added immediate\_callbacks to MockRPCClient
 
 v12.1.1
 -------
@@ -229,12 +235,7 @@
 * drop support for python 3.7
 * cleanup and docs
 * testcases for the new test method
 * better logging for rpc requests, and added a function to the test framework to receive rpc responses async
 * moved config yaml path guesser to separate function, removed GUID again because its not a great idea after all
 * reduced warnings in the testcases
 * GUID type and rpc server changes to better support all pydantic models, in this case Union Types. DEVICE-891
-* fixes an issue in rpc server logging, and adds more debug log output
-
-v7.0.0
-------
-
```

### Comparing `openmodule_commands-12.1.2/PKG-INFO` & `openmodule_commands-12.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule_commands
-Version: 12.1.2
+Version: 12.1.3
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-12.1.2/__init__.py` & `openmodule_commands-12.1.3/__init__.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.2/openmodule_commands.egg-info/PKG-INFO` & `openmodule_commands-12.1.3/openmodule_commands.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openmodule-commands
-Version: 12.1.2
+Version: 12.1.3
 Summary: Commands for openmodule services
 Home-page: https://gitlab.com/arivo-public/device-python/openmodule.git
 Author: ARIVO
 Author-email: support@arivo.co
 License: GNU General Public License v2 (GPLv2)
 Keywords: arivo openmodule openmodule_commands commands
 Platform: UNKNOWN
```

### Comparing `openmodule_commands-12.1.2/setup.cfg` & `openmodule_commands-12.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.2/setup.py` & `openmodule_commands-12.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `openmodule_commands-12.1.2/translate.py` & `openmodule_commands-12.1.3/translate.py`

 * *Files identical despite different names*

