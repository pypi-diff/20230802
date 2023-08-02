# Comparing `tmp/flxtrd-0.2.4.tar.gz` & `tmp/flxtrd-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flxtrd-0.2.4.tar", max compression
+gzip compressed data, was "flxtrd-0.2.5.tar", max compression
```

## Comparing `flxtrd-0.2.4.tar` & `flxtrd-0.2.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.4/LICENSE
--rw-r--r--   0        0        0     8726 2023-07-04 12:36:56.071698 flxtrd-0.2.4/README.md
--rw-r--r--   0        0        0     2211 2023-07-31 11:11:53.329826 flxtrd-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/__init__.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/__init__.py
--rw-r--r--   0        0        0     7470 2023-07-04 06:14:54.745883 flxtrd-0.2.4/src/flxtrd/core/api_client.py
--rw-r--r--   0        0        0      580 2023-07-04 11:24:10.475838 flxtrd-0.2.4/src/flxtrd/core/logger.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/plugins/__init__.py
--rw-r--r--   0        0        0     4911 2023-07-03 13:51:39.979348 flxtrd-0.2.4/src/flxtrd/core/plugins/auth.py
--rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/plugins/base.py
--rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/plugins/devices.py
--rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/core/plugins/log.py
--rw-r--r--   0        0        0     5261 2023-07-03 13:51:39.979348 flxtrd-0.2.4/src/flxtrd/core/types.py
--rw-r--r--   0        0        0     1788 2023-07-31 07:51:31.956598 flxtrd-0.2.4/src/flxtrd/core/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/protocols/__init__.py
--rw-r--r--   0        0        0    10790 2023-07-31 11:10:01.081832 flxtrd-0.2.4/src/flxtrd/protocols/ampq.py
--rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/protocols/base.py
--rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.4/src/flxtrd/protocols/restapi.py
--rw-r--r--   0        0        0     9468 1970-01-01 00:00:00.000000 flxtrd-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     9136 2023-06-28 18:33:40.555857 flxtrd-0.2.5/LICENSE
+-rw-r--r--   0        0        0     8976 2023-08-02 06:47:57.890817 flxtrd-0.2.5/README.md
+-rw-r--r--   0        0        0     2211 2023-08-02 06:48:28.710815 flxtrd-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      730 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/core/__init__.py
+-rw-r--r--   0        0        0     7470 2023-07-04 06:14:54.745883 flxtrd-0.2.5/src/flxtrd/core/api_client.py
+-rw-r--r--   0        0        0      580 2023-07-04 11:24:10.475838 flxtrd-0.2.5/src/flxtrd/core/logger.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/core/plugins/__init__.py
+-rw-r--r--   0        0        0     4911 2023-07-03 13:51:39.979348 flxtrd-0.2.5/src/flxtrd/core/plugins/auth.py
+-rw-r--r--   0        0        0      441 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/core/plugins/base.py
+-rw-r--r--   0        0        0     1248 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/core/plugins/devices.py
+-rw-r--r--   0        0        0      501 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/core/plugins/log.py
+-rw-r--r--   0        0        0     5271 2023-08-02 06:48:17.258816 flxtrd-0.2.5/src/flxtrd/core/types.py
+-rw-r--r--   0        0        0     2210 2023-08-02 06:48:43.750815 flxtrd-0.2.5/src/flxtrd/core/utils.py
+-rw-r--r--   0        0        0        0 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/protocols/__init__.py
+-rw-r--r--   0        0        0    10790 2023-08-02 06:48:17.258816 flxtrd-0.2.5/src/flxtrd/protocols/ampq.py
+-rw-r--r--   0        0        0      257 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/protocols/base.py
+-rw-r--r--   0        0        0     1545 2023-06-28 18:33:40.555857 flxtrd-0.2.5/src/flxtrd/protocols/restapi.py
+-rw-r--r--   0        0        0     9718 1970-01-01 00:00:00.000000 flxtrd-0.2.5/PKG-INFO
```

### Comparing `flxtrd-0.2.4/LICENSE` & `flxtrd-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.4/README.md` & `flxtrd-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,20 +39,40 @@
     MyClient --> CustomPlugins
     FlexAPIClient --> APIProtocols
     FlexAPIClient --> FlexPlugins
 ```
 
 ## Quickstart Guide
 
+Create virtual environment
+
+```sh
+python3 -m venv venv
+```
+
+Activate virtual environment
+
+```sh
+source venv/bin/activate
+```
+
 Install GLocalFlexTrade Python package
 
 ```sh
 pip install flxtrd
 ```
 
+Update GLocalFlexTrade Python package to latest version
+
+```sh
+pip install --upgrade flxtrd
+# or
+pip install -U flxtrd
+```
+
 ### Basic trading client example
 
 ```py
 """Example usage of the trading client using AMPQ protocol"""
 from logging import ERROR, INFO
 import sys
```

### Comparing `flxtrd-0.2.4/pyproject.toml` & `flxtrd-0.2.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flxtrd"
-version = "0.2.4"
+version = "0.2.5"
 description = "Public client API for the flexible energy trading market GLocalFlex."
 authors = ["glocalflex"]
 repository = "https://github.com/glocalflex/GLocalFlexTrade"
 documentation = "https://glocalflex.github.io/GLocalFlexTrade/"
 readme = "README.md"
 # packages = [
 #   {include = "src"},
```

### Comparing `flxtrd-0.2.4/src/flxtrd/__init__.py` & `flxtrd-0.2.5/src/flxtrd/__init__.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.4/src/flxtrd/core/api_client.py` & `flxtrd-0.2.5/src/flxtrd/core/api_client.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.4/src/flxtrd/core/logger.py` & `flxtrd-0.2.5/src/flxtrd/core/logger.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.4/src/flxtrd/core/plugins/auth.py` & `flxtrd-0.2.5/src/flxtrd/core/plugins/auth.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.4/src/flxtrd/core/plugins/devices.py` & `flxtrd-0.2.5/src/flxtrd/core/plugins/devices.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.4/src/flxtrd/core/types.py` & `flxtrd-0.2.5/src/flxtrd/core/types.py`

 * *Files 11% similar despite different names*

```diff
@@ -64,17 +64,17 @@
     def __str__(self) -> str:
         return json.dumps(self._format_human_readable(), indent=4)
 
     def _format_human_readable(self) -> dict:
         return {
             "power_w": round(self.power_w, 3),
             "energy_wh": round(self.energy_wh, 3),
-            "start_time": utils.get_formatted_time(self.start_time_epoch_ms),
+            "start_time": utils.epoch_time_to_isoformat(self.start_time_epoch_ms),
             "duration_min": self.duration_min,
-            "expiration_time": utils.get_formatted_time(self.expiration_time_epoch_ms),
+            "expiration_time": utils.epoch_time_to_isoformat(self.expiration_time_epoch_ms),
         }
 
     @property
     def as_dict_human_readable(self):
         return self._format_human_readable()
```

### Comparing `flxtrd-0.2.4/src/flxtrd/core/utils.py` & `flxtrd-0.2.5/src/flxtrd/core/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,23 +2,37 @@
 from logging import ERROR
 
 from flxtrd.core.logger import log
 
 MILLI = 1000
 
 
-def get_formatted_time(milliseconds: int) -> datetime:
+def epoch_time_to_isoformat(epoch_time: int) -> datetime:
     """
     Converts milliseconds to a human-readable string with milliseconds
     :param milliseconds: milliseconds to convert
-    :return: human-readable string with milliseconds
+    :return: human-readable date string in iso format
     """
-
-    dt = datetime.fromtimestamp(milliseconds / MILLI, tz=timezone.utc)
-    return dt.strftime("%Y-%m-%d %H:%M:%S.%f")[:-3]
+    
+    EPOCH_SEC_LENGTH = 10
+    milliseconds = "000"
+
+    if not isinstance(epoch_time, str):
+        epoch_time = str(epoch_time)
+
+    if len(epoch_time) > EPOCH_SEC_LENGTH:
+        milliseconds = epoch_time[EPOCH_SEC_LENGTH:13]
+        epoch_time = epoch_time[:EPOCH_SEC_LENGTH]
+    elif len(epoch_time) == EPOCH_SEC_LENGTH:
+        pass
+    else:
+        raise ValueError("Epoch time is too short")
+    
+    dt = datetime.fromtimestamp(int(epoch_time), tz=timezone.utc)
+    return dt.strftime("%Y-%m-%dT%H:%M:%S") + f".{milliseconds}Z"
 
 
 def seconds_to_min(seconds: int):
     """Convert seconds to minutes"""
     if seconds == 0:
         log(ERROR, "Duration is zero")
         return 0
```

### Comparing `flxtrd-0.2.4/src/flxtrd/protocols/ampq.py` & `flxtrd-0.2.5/src/flxtrd/protocols/ampq.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.4/src/flxtrd/protocols/restapi.py` & `flxtrd-0.2.5/src/flxtrd/protocols/restapi.py`

 * *Files identical despite different names*

### Comparing `flxtrd-0.2.4/PKG-INFO` & `flxtrd-0.2.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flxtrd
-Version: 0.2.4
+Version: 0.2.5
 Summary: Public client API for the flexible energy trading market GLocalFlex.
 Home-page: https://github.com/glocalflex/GLocalFlexTrade
 Author: glocalflex
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -57,20 +57,40 @@
     MyClient --> CustomPlugins
     FlexAPIClient --> APIProtocols
     FlexAPIClient --> FlexPlugins
 ```
 
 ## Quickstart Guide
 
+Create virtual environment
+
+```sh
+python3 -m venv venv
+```
+
+Activate virtual environment
+
+```sh
+source venv/bin/activate
+```
+
 Install GLocalFlexTrade Python package
 
 ```sh
 pip install flxtrd
 ```
 
+Update GLocalFlexTrade Python package to latest version
+
+```sh
+pip install --upgrade flxtrd
+# or
+pip install -U flxtrd
+```
+
 ### Basic trading client example
 
 ```py
 """Example usage of the trading client using AMPQ protocol"""
 from logging import ERROR, INFO
 import sys
```

