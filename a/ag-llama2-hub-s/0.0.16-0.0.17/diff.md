# Comparing `tmp/ag_llama2_hub_s-0.0.16.tar.gz` & `tmp/ag_llama2_hub_s-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ag_llama2_hub_s-0.0.16.tar", last modified: Wed Aug  2 08:40:41 2023, max compression
+gzip compressed data, was "dist\ag_llama2_hub_s-0.0.17.tar", last modified: Wed Aug  2 10:47:26 2023, max compression
```

## Comparing `ag_llama2_hub_s-0.0.16.tar` & `ag_llama2_hub_s-0.0.17.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:40:41.114855 ag_llama2_hub_s-0.0.16/
--rw-rw-rw-   0        0        0      837 2023-08-02 08:40:41.113882 ag_llama2_hub_s-0.0.16/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 08:40:41.098897 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/
--rw-rw-rw-   0        0        0     2116 2023-08-01 15:48:31.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/__init__.py
--rw-rw-rw-   0        0        0     3643 2023-07-30 09:17:59.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/__main__.py
--rw-rw-rw-   0        0        0     5492 2023-08-02 08:40:31.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/model.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:40:41.107874 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/
--rw-rw-rw-   0        0        0      837 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      317 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      251 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-08-02 08:40:40.000000 ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 08:40:41.114855 ag_llama2_hub_s-0.0.16/setup.cfg
--rw-rw-rw-   0        0        0     2571 2023-08-01 15:46:58.000000 ag_llama2_hub_s-0.0.16/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:40:41.111863 ag_llama2_hub_s-0.0.16/utils/
--rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.16/utils/download.py
--rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.16/utils/render.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:47:26.767189 ag_llama2_hub_s-0.0.17/
+-rw-rw-rw-   0        0        0      837 2023-08-02 10:47:26.765055 ag_llama2_hub_s-0.0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 10:47:26.751093 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/
+-rw-rw-rw-   0        0        0     2116 2023-08-01 15:48:31.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/__init__.py
+-rw-rw-rw-   0        0        0     3683 2023-08-02 10:47:01.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/__main__.py
+-rw-rw-rw-   0        0        0     5492 2023-08-02 08:40:31.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/model.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:47:26.759072 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/
+-rw-rw-rw-   0        0        0      837 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      251 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-08-02 10:47:26.000000 ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 10:47:26.767189 ag_llama2_hub_s-0.0.17/setup.cfg
+-rw-rw-rw-   0        0        0     2571 2023-08-01 15:46:58.000000 ag_llama2_hub_s-0.0.17/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 10:47:26.763062 ag_llama2_hub_s-0.0.17/utils/
+-rw-rw-rw-   0        0        0     1238 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.17/utils/download.py
+-rw-rw-rw-   0        0        0      595 2023-06-10 04:41:23.000000 ag_llama2_hub_s-0.0.17/utils/render.py
```

### Comparing `ag_llama2_hub_s-0.0.16/PKG-INFO` & `ag_llama2_hub_s-0.0.17/ag_llama2_hub_s.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ag_llama2_hub_s
-Version: 0.0.16
+Name: ag-llama2-hub-s
+Version: 0.0.17
 Summary: ag_llama2_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/__init__.py` & `ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/__init__.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/__main__.py` & `ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
     except Exception as e:
         logger.exception(traceback.TracebackException.from_exception(e))
         logger.error(f"Error generating completion: {e}", exc_info=True)
         return str({"error": str(e)})
 
 def main():
     """Start serving API requests."""
+    logger.info(f"Running from main()")
     load_stream_model()
     
 
 
 if __name__ == "__main__":
     logger.info(f"Running from __main__")
     main()
```

### Comparing `ag_llama2_hub_s-0.0.16/ag_llama2_hub_s/model.py` & `ag_llama2_hub_s-0.0.17/ag_llama2_hub_s/model.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.16/ag_llama2_hub_s.egg-info/PKG-INFO` & `ag_llama2_hub_s-0.0.17/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ag-llama2-hub-s
-Version: 0.0.16
+Name: ag_llama2_hub_s
+Version: 0.0.17
 Summary: ag_llama2_hub Test Package for Somthing
 Home-page: UNKNOWN
 Author: AA
 License: UNKNOWN
 Description: long_description
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ag_llama2_hub_s-0.0.16/setup.py` & `ag_llama2_hub_s-0.0.17/setup.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.16/utils/download.py` & `ag_llama2_hub_s-0.0.17/utils/download.py`

 * *Files identical despite different names*

### Comparing `ag_llama2_hub_s-0.0.16/utils/render.py` & `ag_llama2_hub_s-0.0.17/utils/render.py`

 * *Files identical despite different names*

