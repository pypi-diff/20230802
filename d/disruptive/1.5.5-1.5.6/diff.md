# Comparing `tmp/disruptive-1.5.5.tar.gz` & `tmp/disruptive-1.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "disruptive-1.5.5.tar", last modified: Tue Feb  7 11:39:37 2023, max compression
+gzip compressed data, was "disruptive-1.5.6.tar", last modified: Wed Aug  2 11:14:38 2023, max compression
```

## Comparing `disruptive-1.5.5.tar` & `disruptive-1.5.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:39:37.126349 disruptive-1.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-02-07 11:39:26.000000 disruptive-1.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-02-07 11:39:37.126349 disruptive-1.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-02-07 11:39:26.000000 disruptive-1.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:39:37.126349 disruptive-1.5.5/disruptive/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:39:37.126349 disruptive-1.5.5/disruptive/events/
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    61763 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/events/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:39:37.126349 disruptive-1.5.5/disruptive/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/claim.py
--rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    20350 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/emulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/eventhistory.py
--rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/organization.py
--rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/role.py
--rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/resources/stream.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-02-07 11:39:26.000000 disruptive-1.5.5/disruptive/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 11:39:37.126349 disruptive-1.5.5/disruptive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-02-07 11:39:37.000000 disruptive-1.5.5/disruptive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-02-07 11:39:37.000000 disruptive-1.5.5/disruptive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 11:39:37.000000 disruptive-1.5.5/disruptive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-02-07 11:39:37.000000 disruptive-1.5.5/disruptive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-07 11:39:37.000000 disruptive-1.5.5/disruptive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-07 11:39:26.000000 disruptive-1.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-02-07 11:39:37.126349 disruptive-1.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-07 11:39:26.000000 disruptive-1.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.829436 disruptive-1.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-08-02 11:14:21.000000 disruptive-1.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-02 11:14:38.829436 disruptive-1.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-08-02 11:14:21.000000 disruptive-1.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.817436 disruptive-1.5.6/disruptive/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11704 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.817436 disruptive-1.5.6/disruptive/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    61763 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/events/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4900 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.829436 disruptive-1.5.6/disruptive/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9193 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/claim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19270 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20380 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/emulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/eventhistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11192 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/organization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17641 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3201 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/role.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17110 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3982 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/resources/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-08-02 11:14:21.000000 disruptive-1.5.6/disruptive/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:14:38.817436 disruptive-1.5.6/disruptive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 11:14:38.000000 disruptive-1.5.6/disruptive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 11:14:21.000000 disruptive-1.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-02 11:14:38.829436 disruptive-1.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-02 11:14:21.000000 disruptive-1.5.6/setup.py
```

### Comparing `disruptive-1.5.5/LICENSE` & `disruptive-1.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/PKG-INFO` & `disruptive-1.5.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disruptive
-Version: 1.5.5
+Version: 1.5.6
 Summary: Disruptive Technologies Python API.
 Home-page: https://github.com/disruptive-technologies/disruptive-python
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Project-URL: Documentation, https://developer.disruptive-technologies.com/api/libraries/python/
 Project-URL: Developers Page, https://developer.disruptive-technologies.com/docs/
 Keywords: disruptive,technologies,dt,rest,api
```

### Comparing `disruptive-1.5.5/README.md` & `disruptive-1.5.6/README.md`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/__init__.py` & `disruptive-1.5.6/disruptive/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Metadata
-__version__ = '1.5.5'
+__version__ = '1.5.6'
 
 # If set, logs of chosen level and higher are printed to console.
 # Default value None results in no logs at any level.
 log_level = None
 
 # REST API base URLs of which all endpoints are an expansion.
 base_url = 'https://api.disruptive-technologies.com/v2'
```

### Comparing `disruptive-1.5.5/disruptive/authentication.py` & `disruptive-1.5.6/disruptive/authentication.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/errors.py` & `disruptive-1.5.6/disruptive/errors.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/events/__init__.py` & `disruptive-1.5.6/disruptive/events/__init__.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/events/events.py` & `disruptive-1.5.6/disruptive/events/events.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/logging.py` & `disruptive-1.5.6/disruptive/logging.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/outputs.py` & `disruptive-1.5.6/disruptive/outputs.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/requests.py` & `disruptive-1.5.6/disruptive/requests.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/claim.py` & `disruptive-1.5.6/disruptive/resources/claim.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/data_connector.py` & `disruptive-1.5.6/disruptive/resources/data_connector.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/device.py` & `disruptive-1.5.6/disruptive/resources/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,20 @@
     TOUCH = 'touch'
     HUMIDITY = 'humidity'
     PROXIMITY_COUNTER = 'proximityCounter'
     TOUCH_COUNTER = 'touchCounter'
     WATER_DETECTOR = 'waterDetector'
     CLOUD_CONNECTOR = 'ccon'
     CO2 = 'co2'
+    MOTION = 'motion'
     DESK_OCCUPANCY = 'deskOccupancy'
     DEVICE_TYPES = [
         TEMPERATURE, PROXIMITY, TOUCH, HUMIDITY,
         PROXIMITY_COUNTER, TOUCH_COUNTER, WATER_DETECTOR,
-        CLOUD_CONNECTOR, CO2, DESK_OCCUPANCY,
+        CLOUD_CONNECTOR, CO2, MOTION, DESK_OCCUPANCY,
     ]
 
     def __init__(self, device: dict) -> None:
         """
         Constructs the Device object by unpacking the raw device response.
 
         Parameters
```

### Comparing `disruptive-1.5.5/disruptive/resources/emulator.py` & `disruptive-1.5.6/disruptive/resources/emulator.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/eventhistory.py` & `disruptive-1.5.6/disruptive/resources/eventhistory.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/organization.py` & `disruptive-1.5.6/disruptive/resources/organization.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/project.py` & `disruptive-1.5.6/disruptive/resources/project.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/role.py` & `disruptive-1.5.6/disruptive/resources/role.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/service_account.py` & `disruptive-1.5.6/disruptive/resources/service_account.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/resources/stream.py` & `disruptive-1.5.6/disruptive/resources/stream.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive/transforms.py` & `disruptive-1.5.6/disruptive/transforms.py`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/disruptive.egg-info/PKG-INFO` & `disruptive-1.5.6/disruptive.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: disruptive
-Version: 1.5.5
+Version: 1.5.6
 Summary: Disruptive Technologies Python API.
 Home-page: https://github.com/disruptive-technologies/disruptive-python
 Author: Disruptive Technologies Research AS
 Author-email: developer-support@disruptive-technologies.com
 Project-URL: Documentation, https://developer.disruptive-technologies.com/api/libraries/python/
 Project-URL: Developers Page, https://developer.disruptive-technologies.com/docs/
 Keywords: disruptive,technologies,dt,rest,api
```

### Comparing `disruptive-1.5.5/disruptive.egg-info/SOURCES.txt` & `disruptive-1.5.6/disruptive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `disruptive-1.5.5/setup.cfg` & `disruptive-1.5.6/setup.cfg`

 * *Files identical despite different names*

