# Comparing `tmp/pybarb-0.3.9.tar.gz` & `tmp/pybarb-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybarb-0.3.9.tar", last modified: Tue Aug  1 14:03:26 2023, max compression
+gzip compressed data, was "pybarb-0.4.tar", last modified: Wed Aug  2 09:27:58 2023, max compression
```

## Comparing `pybarb-0.3.9.tar` & `pybarb-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:03:26.198536 pybarb-0.3.9/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-01 14:03:26.198536 pybarb-0.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-01 14:03:18.000000 pybarb-0.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:03:26.198536 pybarb-0.3.9/pybarb/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-01 14:03:18.000000 pybarb-0.3.9/pybarb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33050 2023-08-01 14:03:18.000000 pybarb-0.3.9/pybarb/pybarb.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:03:26.198536 pybarb-0.3.9/pybarb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-01 14:03:26.000000 pybarb-0.3.9/pybarb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:03:26.198536 pybarb-0.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-01 14:03:18.000000 pybarb-0.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:27:58.212223 pybarb-0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 09:27:58.212223 pybarb-0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-08-02 09:27:50.000000 pybarb-0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:27:58.212223 pybarb-0.4/pybarb/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-02 09:27:50.000000 pybarb-0.4/pybarb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33060 2023-08-02 09:27:50.000000 pybarb-0.4/pybarb/pybarb.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 09:27:58.212223 pybarb-0.4/pybarb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-08-02 09:27:58.000000 pybarb-0.4/pybarb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-02 09:27:58.000000 pybarb-0.4/pybarb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 09:27:58.000000 pybarb-0.4/pybarb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-02 09:27:58.000000 pybarb-0.4/pybarb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-02 09:27:58.000000 pybarb-0.4/pybarb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 09:27:58.212223 pybarb-0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-08-02 09:27:50.000000 pybarb-0.4/setup.py
```

### Comparing `pybarb-0.3.9/README.md` & `pybarb-0.4/README.md`

 * *Files identical despite different names*

### Comparing `pybarb-0.3.9/pybarb/pybarb.py` & `pybarb-0.4/pybarb/pybarb.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,15 +184,15 @@
                 AdvertisingSpotsResultSet: The advertising spots result set.
         """
 
         # The query parameters
         params = {"min_transmission_date": min_transmission_date, "max_transmission_date": max_transmission_date,
                   "station_code": None if station is None else self.get_station_code(station), 
                   "panel_code": None if panel is None else self.get_panel_code(panel),
-                  "advertiser": advertiser, "buyer": buyer, "consolidated": consolidated,
+                  "advertiser_name": advertiser, "buyer_name": buyer, "consolidated": consolidated,
                   "standardise_audiences": standardise_audiences, "use_reporting_days": use_reporting_days, "last_updated_greater_than": last_updated_greater_than,
                   "limit": limit}
 
         api_response_data = self.query_event_endpoint(
             "advertising_spots", params)
 
         return AdvertisingSpotsResultSet(api_response_data)
```

