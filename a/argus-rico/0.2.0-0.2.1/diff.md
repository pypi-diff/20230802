# Comparing `tmp/argus_rico-0.2.0.tar.gz` & `tmp/argus_rico-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argus_rico-0.2.0.tar", max compression
+gzip compressed data, was "argus_rico-0.2.1.tar", max compression
```

## Comparing `argus_rico-0.2.0.tar` & `argus_rico-0.2.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     1071 2023-05-24 01:07:47.899290 argus_rico-0.2.0/LICENSE
--rw-r--r--   0        0        0     1345 2023-08-02 03:41:31.806139 argus_rico-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3619 2023-08-01 15:17:21.804082 argus_rico-0.2.0/src/argus_rico/__init__.py
--rw-r--r--   0        0        0       67 2023-07-19 01:08:54.295571 argus_rico-0.2.0/src/argus_rico/catalogs/__init__.py
--rw-r--r--   0        0        0     8750 2023-07-21 00:21:26.572087 argus_rico-0.2.0/src/argus_rico/catalogs/atlas.py
--rw-r--r--   0        0        0     2728 2023-08-02 03:34:16.263004 argus_rico-0.2.0/src/argus_rico/cli.py
--rw-r--r--   0        0        0     1162 2023-08-01 16:33:55.909016 argus_rico-0.2.0/src/argus_rico/consumer.py
--rw-r--r--   0        0        0      388 2023-08-02 03:34:16.263244 argus_rico-0.2.0/src/argus_rico/efte/__init__.py
--rw-r--r--   0        0        0     3735 2023-07-19 01:08:54.295934 argus_rico-0.2.0/src/argus_rico/efte/db.py
--rw-r--r--   0        0        0      878 2023-07-21 00:32:52.766382 argus_rico-0.2.0/src/argus_rico/efte/efte_runner.py
--rw-r--r--   0        0        0     1848 2023-08-02 03:34:16.263454 argus_rico-0.2.0/src/argus_rico/efte/processor.py
--rw-r--r--   0        0        0      659 2023-07-21 06:16:58.642198 argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.alert.avsc
--rw-r--r--   0        0        0     3700 2023-08-02 03:34:16.263689 argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.candidate.avsc
--rw-r--r--   0        0        0      895 2023-07-21 06:16:58.642438 argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.xmatch.avsc
--rw-r--r--   0        0        0     3616 2023-07-21 06:16:58.642565 argus_rico-0.2.0/src/argus_rico/efte/schemas/raw_candidate.avsc
--rw-r--r--   0        0        0     7282 2023-08-02 03:34:16.263896 argus_rico-0.2.0/src/argus_rico/efte/stream.py
--rw-r--r--   0        0        0     4175 2023-08-01 16:38:21.655761 argus_rico-0.2.0/src/argus_rico/efte/vetnet.py
--rw-r--r--   0        0        0     1978 2023-08-02 03:34:16.264112 argus_rico-0.2.0/src/argus_rico/efte/watchdog.py
--rw-r--r--   0        0        0     2060 2023-06-12 16:35:31.667549 argus_rico-0.2.0/src/argus_rico/heartbeat.py
--rw-r--r--   0        0        0     5049 2023-07-19 01:08:54.296496 argus_rico-0.2.0/src/argus_rico/images.py
--rw-r--r--   0        0        0      379 2023-08-02 03:41:12.508808 argus_rico-0.2.0/src/argus_rico/models/__init__.py
--rw-r--r--   0        0        0     1727 2023-08-02 03:34:16.264367 argus_rico-0.2.0/src/argus_rico/models/efte_alert.py
--rw-r--r--   0        0        0     8111 2023-06-12 16:35:31.667921 argus_rico-0.2.0/src/argus_rico/models/evr_image.py
--rw-r--r--   0        0        0     2740 2023-06-12 16:35:31.668047 argus_rico-0.2.0/src/argus_rico/producer.py
--rw-r--r--   0        0        0        0 2023-06-12 16:35:31.668081 argus_rico-0.2.0/src/argus_rico/py.typed
--rw-r--r--   0        0        0     2845 2023-07-19 23:57:27.800686 argus_rico-0.2.0/src/argus_rico/s3.py
--rw-r--r--   0        0        0     9139 2023-07-25 22:16:36.634429 argus_rico-0.2.0/src/argus_rico/slack.py
--rw-r--r--   0        0        0      828 2023-08-02 03:34:16.264530 argus_rico-0.2.0/src/argus_rico/utils.py
--rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 argus_rico-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-24 01:07:47.899290 argus_rico-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1345 2023-08-02 04:18:54.661480 argus_rico-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3619 2023-08-01 15:17:21.804082 argus_rico-0.2.1/src/argus_rico/__init__.py
+-rw-r--r--   0        0        0       67 2023-07-19 01:08:54.295571 argus_rico-0.2.1/src/argus_rico/catalogs/__init__.py
+-rw-r--r--   0        0        0     8750 2023-07-21 00:21:26.572087 argus_rico-0.2.1/src/argus_rico/catalogs/atlas.py
+-rw-r--r--   0        0        0     2728 2023-08-02 03:34:16.263004 argus_rico-0.2.1/src/argus_rico/cli.py
+-rw-r--r--   0        0        0     1162 2023-08-01 16:33:55.909016 argus_rico-0.2.1/src/argus_rico/consumer.py
+-rw-r--r--   0        0        0      388 2023-08-02 03:34:16.263244 argus_rico-0.2.1/src/argus_rico/efte/__init__.py
+-rw-r--r--   0        0        0     3735 2023-07-19 01:08:54.295934 argus_rico-0.2.1/src/argus_rico/efte/db.py
+-rw-r--r--   0        0        0      878 2023-07-21 00:32:52.766382 argus_rico-0.2.1/src/argus_rico/efte/efte_runner.py
+-rw-r--r--   0        0        0     1848 2023-08-02 03:34:16.263454 argus_rico-0.2.1/src/argus_rico/efte/processor.py
+-rw-r--r--   0        0        0      659 2023-07-21 06:16:58.642198 argus_rico-0.2.1/src/argus_rico/efte/schemas/efte.alert.avsc
+-rw-r--r--   0        0        0     3700 2023-08-02 03:34:16.263689 argus_rico-0.2.1/src/argus_rico/efte/schemas/efte.candidate.avsc
+-rw-r--r--   0        0        0      895 2023-07-21 06:16:58.642438 argus_rico-0.2.1/src/argus_rico/efte/schemas/efte.xmatch.avsc
+-rw-r--r--   0        0        0     3616 2023-07-21 06:16:58.642565 argus_rico-0.2.1/src/argus_rico/efte/schemas/raw_candidate.avsc
+-rw-r--r--   0        0        0     7426 2023-08-02 04:18:30.043574 argus_rico-0.2.1/src/argus_rico/efte/stream.py
+-rw-r--r--   0        0        0     4175 2023-08-01 16:38:21.655761 argus_rico-0.2.1/src/argus_rico/efte/vetnet.py
+-rw-r--r--   0        0        0     1978 2023-08-02 03:34:16.264112 argus_rico-0.2.1/src/argus_rico/efte/watchdog.py
+-rw-r--r--   0        0        0     2060 2023-06-12 16:35:31.667549 argus_rico-0.2.1/src/argus_rico/heartbeat.py
+-rw-r--r--   0        0        0     5049 2023-07-19 01:08:54.296496 argus_rico-0.2.1/src/argus_rico/images.py
+-rw-r--r--   0        0        0      379 2023-08-02 03:41:12.508808 argus_rico-0.2.1/src/argus_rico/models/__init__.py
+-rw-r--r--   0        0        0     1727 2023-08-02 03:34:16.264367 argus_rico-0.2.1/src/argus_rico/models/efte_alert.py
+-rw-r--r--   0        0        0     8111 2023-06-12 16:35:31.667921 argus_rico-0.2.1/src/argus_rico/models/evr_image.py
+-rw-r--r--   0        0        0     2740 2023-06-12 16:35:31.668047 argus_rico-0.2.1/src/argus_rico/producer.py
+-rw-r--r--   0        0        0        0 2023-06-12 16:35:31.668081 argus_rico-0.2.1/src/argus_rico/py.typed
+-rw-r--r--   0        0        0     2845 2023-07-19 23:57:27.800686 argus_rico-0.2.1/src/argus_rico/s3.py
+-rw-r--r--   0        0        0     9139 2023-07-25 22:16:36.634429 argus_rico-0.2.1/src/argus_rico/slack.py
+-rw-r--r--   0        0        0      828 2023-08-02 03:34:16.264530 argus_rico-0.2.1/src/argus_rico/utils.py
+-rw-r--r--   0        0        0     1529 1970-01-01 00:00:00.000000 argus_rico-0.2.1/PKG-INFO
```

### Comparing `argus_rico-0.2.0/LICENSE` & `argus_rico-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/pyproject.toml` & `argus_rico-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "argus-rico"
-version = "0.2.0"
+version = "0.2.1"
 description = "Transient alert generation and database interaction for Argus and Evryscope"
 authors = ["Hank Corbett"]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.11"
 python-dotenv = "^0.19.0"
 fastavro = "^1.4.12"
```

### Comparing `argus_rico-0.2.0/src/argus_rico/__init__.py` & `argus_rico-0.2.1/src/argus_rico/__init__.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/catalogs/atlas.py` & `argus_rico-0.2.1/src/argus_rico/catalogs/atlas.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/cli.py` & `argus_rico-0.2.1/src/argus_rico/cli.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/consumer.py` & `argus_rico-0.2.1/src/argus_rico/consumer.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/db.py` & `argus_rico-0.2.1/src/argus_rico/efte/db.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/efte_runner.py` & `argus_rico-0.2.1/src/argus_rico/efte/efte_runner.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/processor.py` & `argus_rico-0.2.1/src/argus_rico/efte/processor.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.alert.avsc` & `argus_rico-0.2.1/src/argus_rico/efte/schemas/efte.alert.avsc`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.candidate.avsc` & `argus_rico-0.2.1/src/argus_rico/efte/schemas/efte.candidate.avsc`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/schemas/efte.xmatch.avsc` & `argus_rico-0.2.1/src/argus_rico/efte/schemas/efte.xmatch.avsc`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/schemas/raw_candidate.avsc` & `argus_rico-0.2.1/src/argus_rico/efte/schemas/raw_candidate.avsc`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/stream.py` & `argus_rico-0.2.1/src/argus_rico/efte/stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 __all__ = ["EFTEAlertReceiver", "EFTEAlertStreamer"]
 
 import base64
 import io
 import os
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any, Dict, List, Optional
 from uuid import uuid4
 
 import astropy.table as tbl
 import blosc
 import fastavro as fa
 import orjson
 import pandas as pd
@@ -206,16 +206,20 @@
         """
         if self.filter_path is not None:
             with open(self.filter_path, "r") as file:
                 filter_conditions = file.read().splitlines()
             filter_conditions = [f for f in filter_conditions if len(f) > 3]
 
         for alert in alerts:
-            if len(alert["xmatch"]) > 0 and self.filter_path is not None:
-                xmatch = pd.DataFrame.from_records(alert["xmatch"])
-                for condition in filter_conditions:
-                    column_name, operator, value = condition.split()
-                    xmatch = xmatch.query(f"{column_name} {operator} {value}")
-                if len(xmatch) > 0:
-                    self._write_candidate(alert)
+            if self.filter_path is not None:
+                if len(alert["xmatch"]) > 0:
+                    xmatch = pd.DataFrame.from_records(alert["xmatch"])
+                    xmatch["g-r"] = xmatch["g"] - xmatch["r"]
+                    for condition in filter_conditions:
+                        column_name, operator, value = condition.split()
+                        xmatch = xmatch.query(f"{column_name} {operator} {value}")
+                    if len(xmatch) > 0:
+                        self._write_candidate(alert)
+                else:
+                    return
             else:
                 self._write_candidate(alert)
```

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/vetnet.py` & `argus_rico-0.2.1/src/argus_rico/efte/vetnet.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/efte/watchdog.py` & `argus_rico-0.2.1/src/argus_rico/efte/watchdog.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/heartbeat.py` & `argus_rico-0.2.1/src/argus_rico/heartbeat.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/images.py` & `argus_rico-0.2.1/src/argus_rico/images.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/models/efte_alert.py` & `argus_rico-0.2.1/src/argus_rico/models/efte_alert.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/models/evr_image.py` & `argus_rico-0.2.1/src/argus_rico/models/evr_image.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/producer.py` & `argus_rico-0.2.1/src/argus_rico/producer.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/s3.py` & `argus_rico-0.2.1/src/argus_rico/s3.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/slack.py` & `argus_rico-0.2.1/src/argus_rico/slack.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/src/argus_rico/utils.py` & `argus_rico-0.2.1/src/argus_rico/utils.py`

 * *Files identical despite different names*

### Comparing `argus_rico-0.2.0/PKG-INFO` & `argus_rico-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argus-rico
-Version: 0.2.0
+Version: 0.2.1
 Summary: Transient alert generation and database interaction for Argus and Evryscope
 Author: Hank Corbett
 Requires-Python: >=3.9,<3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: astropy (>=5.3,<6.0)
```

