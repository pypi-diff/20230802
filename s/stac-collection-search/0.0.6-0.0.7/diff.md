# Comparing `tmp/stac_collection_search-0.0.6.tar.gz` & `tmp/stac_collection_search-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_collection_search-0.0.6.tar", last modified: Thu Jun 22 14:04:30 2023, max compression
+gzip compressed data, was "stac_collection_search-0.0.7.tar", last modified: Wed Aug  2 09:56:01 2023, max compression
```

## Comparing `stac_collection_search-0.0.6.tar` & `stac_collection_search-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-22 14:04:30.237640 stac_collection_search-0.0.6/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1094 2023-06-21 21:29:21.000000 stac_collection_search-0.0.6/LICENSE.md
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1450 2023-06-22 14:04:30.237640 stac_collection_search-0.0.6/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      946 2023-06-21 17:54:21.000000 stac_collection_search-0.0.6/README.md
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-06-22 14:04:30.237640 stac_collection_search-0.0.6/setup.cfg
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1302 2023-06-22 14:03:00.000000 stac_collection_search-0.0.6/setup.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-22 14:04:30.237640 stac_collection_search-0.0.6/stac_collection_search/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       83 2023-06-21 18:14:31.000000 stac_collection_search-0.0.6/stac_collection_search/__init__.py
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     5005 2023-06-22 14:02:53.000000 stac_collection_search-0.0.6/stac_collection_search/utils.py
-drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-06-22 14:04:30.237640 stac_collection_search-0.0.6/stac_collection_search.egg-info/
--rw-rw-r--   0 ivica     (1000) ivica     (1000)     1450 2023-06-22 14:04:30.000000 stac_collection_search-0.0.6/stac_collection_search.egg-info/PKG-INFO
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      325 2023-06-22 14:04:30.000000 stac_collection_search-0.0.6/stac_collection_search.egg-info/SOURCES.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-06-22 14:04:30.000000 stac_collection_search-0.0.6/stac_collection_search.egg-info/dependency_links.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)      115 2023-06-22 14:04:30.000000 stac_collection_search-0.0.6/stac_collection_search.egg-info/requires.txt
--rw-rw-r--   0 ivica     (1000) ivica     (1000)       23 2023-06-22 14:04:30.000000 stac_collection_search-0.0.6/stac_collection_search.egg-info/top_level.txt
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-02 09:56:01.893578 stac_collection_search-0.0.7/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1094 2023-06-21 21:29:21.000000 stac_collection_search-0.0.7/LICENSE.md
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1778 2023-08-02 09:56:01.893578 stac_collection_search-0.0.7/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1025 2023-06-23 09:51:47.000000 stac_collection_search-0.0.7/README.md
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       38 2023-08-02 09:56:01.893578 stac_collection_search-0.0.7/setup.cfg
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1302 2023-08-02 09:55:43.000000 stac_collection_search-0.0.7/setup.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-02 09:56:01.893578 stac_collection_search-0.0.7/stac_collection_search/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       83 2023-06-21 18:14:31.000000 stac_collection_search-0.0.7/stac_collection_search/__init__.py
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     5271 2023-08-02 09:53:45.000000 stac_collection_search-0.0.7/stac_collection_search/utils.py
+drwxrwxr-x   0 ivica     (1000) ivica     (1000)        0 2023-08-02 09:56:01.893578 stac_collection_search-0.0.7/stac_collection_search.egg-info/
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)     1778 2023-08-02 09:56:01.000000 stac_collection_search-0.0.7/stac_collection_search.egg-info/PKG-INFO
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      325 2023-08-02 09:56:01.000000 stac_collection_search-0.0.7/stac_collection_search.egg-info/SOURCES.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)        1 2023-08-02 09:56:01.000000 stac_collection_search-0.0.7/stac_collection_search.egg-info/dependency_links.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)      115 2023-08-02 09:56:01.000000 stac_collection_search-0.0.7/stac_collection_search.egg-info/requires.txt
+-rw-rw-r--   0 ivica     (1000) ivica     (1000)       23 2023-08-02 09:56:01.000000 stac_collection_search-0.0.7/stac_collection_search.egg-info/top_level.txt
```

### Comparing `stac_collection_search-0.0.6/LICENSE.md` & `stac_collection_search-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `stac_collection_search-0.0.6/PKG-INFO` & `stac_collection_search-0.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 Metadata-Version: 2.1
 Name: stac_collection_search
-Version: 0.0.6
+Version: 0.0.7
 Summary: STAC Collection Search helper utility
+Home-page: UNKNOWN
 Author: Ivica Matic
 Author-email: <ivica.matic@spatialdays.com>
+License: UNKNOWN
+Description: 
+        # STAC Collection Search
+        Quick utility which enables you to search for STAC collections with a given bbox and datetime extent.
+        
+        ## How to use
+        
+        ``` python
+          import requests
+          import datetime
+          import shapely
+          from stac_collection_search import search_collections
+        
+          url ="https://planetarycomputer.microsoft.com/api/stac/v1/collections"
+          headers = {
+            "Content-Type": "application/geo+json",
+          }
+          response = requests.get(url, headers=headers)
+          collection_list_json_dict = response.json()
+          temporal_extent_start = datetime.datetime(2019, 1, 1)
+          temporal_extent_end = datetime.datetime(2021, 1, 1)
+          spatial_extent = shapely.geometry.box(50, 0, 51, 1)
+          collection_list = search_collections(collection_list_json_dict, spatial_extent=spatial_extent,
+                                              temporal_extent_start=temporal_extent_start,
+                                              temporal_extent_end=temporal_extent_end)
+          print(collection_list, len(collection_list)) """ -> ['3dep-seamless', 'sentinel-1-rtc', '...'], 66 """
+        
+        ```
 Keywords: python,azure,stac,fastapi,eo,earth observation,spatial,search,collection
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-
-# STAC Collection Search
-Quick utility which enables you to search for STAC collections with a given bbox and datetime extent.
-
-## How to use
-
-``` python
-  import requests
-  import datetime
-  import shapely
-  from stac_collection_search import search_collections
-
-  url ="https://planetarycomputer.microsoft.com/api/stac/v1/collections"
-  response = requests.get(url)
-  collection_list_json_dict = response.json()
-  temporal_extent_start = datetime.datetime(2019, 1, 1)
-  temporal_extent_end = datetime.datetime(2021, 1, 1)
-  spatial_extent = shapely.geometry.box(50, 0, 51, 1)
-  collection_list = search_collections(collection_list_json_dict, spatial_extent=spatial_extent,
-                                      temporal_extent_start=temporal_extent_start,
-                                      temporal_extent_end=temporal_extent_end)
-  print(collection_list, len(collection_list)) """ -> ['3dep-seamless', 'sentinel-1-rtc', '...'], 66 """
-
-```
```

### Comparing `stac_collection_search-0.0.6/README.md` & `stac_collection_search-0.0.7/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 ``` python
   import requests
   import datetime
   import shapely
   from stac_collection_search import search_collections
 
   url ="https://planetarycomputer.microsoft.com/api/stac/v1/collections"
-  response = requests.get(url)
+  headers = {
+    "Content-Type": "application/geo+json",
+  }
+  response = requests.get(url, headers=headers)
   collection_list_json_dict = response.json()
   temporal_extent_start = datetime.datetime(2019, 1, 1)
   temporal_extent_end = datetime.datetime(2021, 1, 1)
   spatial_extent = shapely.geometry.box(50, 0, 51, 1)
   collection_list = search_collections(collection_list_json_dict, spatial_extent=spatial_extent,
                                       temporal_extent_start=temporal_extent_start,
                                       temporal_extent_end=temporal_extent_end)
```

### Comparing `stac_collection_search-0.0.6/setup.py` & `stac_collection_search-0.0.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'STAC Collection Search helper utility'
 LONG_DESCRIPTION = 'STAC Collection Search helper which enables a collection search on the stac-fastapi'
 
 requirements = []
 requirements_file = "./requirements.txt"
 if os.path.isfile(requirements_file):
     with open(requirements_file) as f:
```

### Comparing `stac_collection_search-0.0.6/stac_collection_search/utils.py` & `stac_collection_search-0.0.7/stac_collection_search/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,30 +16,39 @@
 
 
 def _get_shapely_object_from_bbox_list(bbox_list: List) -> shapely.geometry.Polygon:
     return shapely.geometry.box(*bbox_list)
 
 
 def _get_collections(collection_list_json: dict) -> List[CollectionInfo]:
-    return [
-        CollectionInfo(
-            id=i["id"],
-            spatial_extent=shapely.geometry.MultiPolygon(
-                [
-                    _get_shapely_object_from_bbox_list(spatial_extent)
-                    for spatial_extent in i["extent"]["spatial"]["bbox"]
-                ]
-            ),
-            temporal_extent=TemporalExtent(
-                start=_process_timestamp(i["extent"]["temporal"]["interval"][0][0]),
-                end=_process_timestamp(i["extent"]["temporal"]["interval"][-1][1]),
-            ),
-        )
-        for i in collection_list_json["collections"]
-    ]
+    collections_info = []
+    for i in collection_list_json.get("collections", []):
+        try:
+            spatial_extent = i["extent"]["spatial"]["bbox"]
+            temporal_extent = i["extent"]["temporal"]["interval"]
+
+            shapely_objects = [
+                _get_shapely_object_from_bbox_list(spatial_bbox)
+                for spatial_bbox in spatial_extent
+            ]
+
+            collection = CollectionInfo(
+                id=i["id"],
+                spatial_extent=shapely.geometry.MultiPolygon(shapely_objects),
+                temporal_extent=TemporalExtent(
+                    start=_process_timestamp(temporal_extent[0][0]),
+                    end=_process_timestamp(temporal_extent[-1][1]),
+                ),
+            )
+            collections_info.append(collection)
+        except KeyError:
+            continue
+
+    return collections_info
+
 
 
 def _process_timestamp(timestamp: str) -> datetime:
     """
     Process a timestamp string into a datetime object.
     """
     if timestamp is None:
```

