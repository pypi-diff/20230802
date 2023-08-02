# Comparing `tmp/voicemeeter_api-2.3.7.tar.gz` & `tmp/voicemeeter_api-2.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicemeeter_api-2.3.7.tar", max compression
+gzip compressed data, was "voicemeeter_api-2.4.0.tar", max compression
```

## Comparing `voicemeeter_api-2.3.7.tar` & `voicemeeter_api-2.4.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.3.7/LICENSE
--rw-r--r--   0        0        0     1102 2023-08-01 17:12:17.142993 voicemeeter_api-2.3.7/pyproject.toml
--rw-r--r--   0        0        0    18957 2023-08-01 15:15:42.523592 voicemeeter_api-2.3.7/README.md
--rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.3.7/voicemeeterlib/__init__.py
--rw-r--r--   0        0        0     8226 2023-07-18 12:50:39.247222 voicemeeter_api-2.3.7/voicemeeterlib/bus.py
--rw-r--r--   0        0        0     4618 2023-07-23 07:05:02.003142 voicemeeter_api-2.3.7/voicemeeterlib/cbindings.py
--rw-r--r--   0        0        0     1194 2023-07-25 17:25:27.080618 voicemeeter_api-2.3.7/voicemeeterlib/command.py
--rw-r--r--   0        0        0     6050 2023-08-01 16:48:00.788867 voicemeeter_api-2.3.7/voicemeeterlib/config.py
--rw-r--r--   0        0        0     1748 2023-07-25 17:25:30.796461 voicemeeter_api-2.3.7/voicemeeterlib/device.py
--rw-r--r--   0        0        0      575 2023-07-10 12:27:38.707424 voicemeeter_api-2.3.7/voicemeeterlib/error.py
--rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.3.7/voicemeeterlib/event.py
--rw-r--r--   0        0        0     7792 2023-07-28 09:25:54.751960 voicemeeter_api-2.3.7/voicemeeterlib/factory.py
--rw-r--r--   0        0        0     1091 2023-07-25 17:25:27.080618 voicemeeter_api-2.3.7/voicemeeterlib/inst.py
--rw-r--r--   0        0        0     1800 2023-07-25 17:25:30.842924 voicemeeter_api-2.3.7/voicemeeterlib/iremote.py
--rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.3.7/voicemeeterlib/kinds.py
--rw-r--r--   0        0        0     1512 2023-07-25 17:25:30.885025 voicemeeter_api-2.3.7/voicemeeterlib/macrobutton.py
--rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.3.7/voicemeeterlib/meta.py
--rw-r--r--   0        0        0     6485 2023-07-28 09:25:54.753959 voicemeeter_api-2.3.7/voicemeeterlib/misc.py
--rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.3.7/voicemeeterlib/recorder.py
--rw-r--r--   0        0        0    12341 2023-08-01 15:15:42.523592 voicemeeter_api-2.3.7/voicemeeterlib/remote.py
--rw-r--r--   0        0        0    15352 2023-07-22 11:42:06.374784 voicemeeter_api-2.3.7/voicemeeterlib/strip.py
--rw-r--r--   0        0        0     2277 2023-08-01 15:15:42.525096 voicemeeter_api-2.3.7/voicemeeterlib/subject.py
--rw-r--r--   0        0        0     2930 2023-07-18 13:06:02.678934 voicemeeter_api-2.3.7/voicemeeterlib/updater.py
--rw-r--r--   0        0        0     2436 2023-07-21 11:41:24.422287 voicemeeter_api-2.3.7/voicemeeterlib/util.py
--rw-r--r--   0        0        0     6055 2023-07-20 10:04:33.726657 voicemeeter_api-2.3.7/voicemeeterlib/vban.py
--rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1091 2022-06-16 12:51:04.818279 voicemeeter_api-2.4.0/LICENSE
+-rw-r--r--   0        0        0     1102 2023-08-02 14:42:32.480639 voicemeeter_api-2.4.0/pyproject.toml
+-rw-r--r--   0        0        0    18957 2023-08-01 15:15:42.523592 voicemeeter_api-2.4.0/README.md
+-rw-r--r--   0        0        0       69 2022-07-31 06:38:44.483821 voicemeeter_api-2.4.0/voicemeeterlib/__init__.py
+-rw-r--r--   0        0        0     8226 2023-07-18 12:50:39.247222 voicemeeter_api-2.4.0/voicemeeterlib/bus.py
+-rw-r--r--   0        0        0     4618 2023-08-02 14:26:03.847115 voicemeeter_api-2.4.0/voicemeeterlib/cbindings.py
+-rw-r--r--   0        0        0     1194 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.0/voicemeeterlib/command.py
+-rw-r--r--   0        0        0     6050 2023-08-01 16:48:00.788867 voicemeeter_api-2.4.0/voicemeeterlib/config.py
+-rw-r--r--   0        0        0     1748 2023-07-25 17:25:30.796461 voicemeeter_api-2.4.0/voicemeeterlib/device.py
+-rw-r--r--   0        0        0      666 2023-08-02 14:34:34.328692 voicemeeter_api-2.4.0/voicemeeterlib/error.py
+-rw-r--r--   0        0        0     2099 2023-06-22 08:38:58.271443 voicemeeter_api-2.4.0/voicemeeterlib/event.py
+-rw-r--r--   0        0        0     7792 2023-07-28 09:25:54.751960 voicemeeter_api-2.4.0/voicemeeterlib/factory.py
+-rw-r--r--   0        0        0     1091 2023-07-25 17:25:27.080618 voicemeeter_api-2.4.0/voicemeeterlib/inst.py
+-rw-r--r--   0        0        0     1800 2023-07-25 17:25:30.842924 voicemeeter_api-2.4.0/voicemeeterlib/iremote.py
+-rw-r--r--   0        0        0     2628 2023-07-18 13:00:26.971422 voicemeeter_api-2.4.0/voicemeeterlib/kinds.py
+-rw-r--r--   0        0        0     1512 2023-07-25 17:25:30.885025 voicemeeter_api-2.4.0/voicemeeterlib/macrobutton.py
+-rw-r--r--   0        0        0     1130 2023-06-21 12:24:03.433043 voicemeeter_api-2.4.0/voicemeeterlib/meta.py
+-rw-r--r--   0        0        0     6485 2023-07-28 09:25:54.753959 voicemeeter_api-2.4.0/voicemeeterlib/misc.py
+-rw-r--r--   0        0        0     6739 2023-07-01 18:30:01.004734 voicemeeter_api-2.4.0/voicemeeterlib/recorder.py
+-rw-r--r--   0        0        0    12341 2023-08-01 15:15:42.523592 voicemeeter_api-2.4.0/voicemeeterlib/remote.py
+-rw-r--r--   0        0        0    15352 2023-07-22 11:42:06.374784 voicemeeter_api-2.4.0/voicemeeterlib/strip.py
+-rw-r--r--   0        0        0     2277 2023-08-01 15:15:42.525096 voicemeeter_api-2.4.0/voicemeeterlib/subject.py
+-rw-r--r--   0        0        0     2930 2023-07-18 13:06:02.678934 voicemeeter_api-2.4.0/voicemeeterlib/updater.py
+-rw-r--r--   0        0        0     2436 2023-07-21 11:41:24.422287 voicemeeter_api-2.4.0/voicemeeterlib/util.py
+-rw-r--r--   0        0        0     6055 2023-07-20 10:04:33.726657 voicemeeter_api-2.4.0/voicemeeterlib/vban.py
+-rw-r--r--   0        0        0    18745 1970-01-01 00:00:00.000000 voicemeeter_api-2.4.0/PKG-INFO
```

### Comparing `voicemeeter_api-2.3.7/LICENSE` & `voicemeeter_api-2.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/pyproject.toml` & `voicemeeter_api-2.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "voicemeeter-api"
-version = "2.3.7"
+version = "2.4.0"
 description = "A Python wrapper for the Voiceemeter API"
 authors = ["onyx-and-iris <code@onyxandiris.online>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/onyx-and-iris/voicemeeter-api-python"
 
 packages = [{ include = "voicemeeterlib" }]
```

### Comparing `voicemeeter_api-2.3.7/README.md` & `voicemeeter_api-2.4.0/README.md`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/bus.py` & `voicemeeter_api-2.4.0/voicemeeterlib/bus.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/cbindings.py` & `voicemeeter_api-2.4.0/voicemeeterlib/cbindings.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/command.py` & `voicemeeter_api-2.4.0/voicemeeterlib/command.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/config.py` & `voicemeeter_api-2.4.0/voicemeeterlib/config.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/device.py` & `voicemeeter_api-2.4.0/voicemeeterlib/device.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/error.py` & `voicemeeter_api-2.4.0/voicemeeterlib/error.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-class InstallError(Exception):
-    """Exception raised when installation errors occur"""
-
-
-class CAPIError(Exception):
-    """Exception raised when the C-API returns error values"""
+class VMError(Exception):
+    """Base VM Exception class. Raised when general errors occur."""
 
-    def __init__(self, fn_name, code, msg=None):
-        self.fn_name = fn_name
-        self.code = code
-        self.message = msg if msg else f"{fn_name} returned {code}"
+    def __init__(self, msg):
+        self.message = msg
         super().__init__(self.message)
 
     def __str__(self):
         return f"{type(self).__name__}: {self.message}"
 
 
-class VMError(Exception):
-    """Exception raised when general errors occur"""
+class InstallError(VMError):
+    """Exception raised when installation errors occur"""
+
+
+class CAPIError(VMError):
+    """Exception raised when the C-API returns an error code"""
+
+    def __init__(self, fn_name, code, msg=None):
+        self.fn_name = fn_name
+        self.code = code
+        super(CAPIError, self).__init__(msg if msg else f"{fn_name} returned {code}")
```

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/event.py` & `voicemeeter_api-2.4.0/voicemeeterlib/event.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/factory.py` & `voicemeeter_api-2.4.0/voicemeeterlib/factory.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/inst.py` & `voicemeeter_api-2.4.0/voicemeeterlib/inst.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/iremote.py` & `voicemeeter_api-2.4.0/voicemeeterlib/iremote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/kinds.py` & `voicemeeter_api-2.4.0/voicemeeterlib/kinds.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/macrobutton.py` & `voicemeeter_api-2.4.0/voicemeeterlib/macrobutton.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/meta.py` & `voicemeeter_api-2.4.0/voicemeeterlib/meta.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/misc.py` & `voicemeeter_api-2.4.0/voicemeeterlib/misc.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/recorder.py` & `voicemeeter_api-2.4.0/voicemeeterlib/recorder.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/remote.py` & `voicemeeter_api-2.4.0/voicemeeterlib/remote.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/strip.py` & `voicemeeter_api-2.4.0/voicemeeterlib/strip.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/subject.py` & `voicemeeter_api-2.4.0/voicemeeterlib/subject.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/updater.py` & `voicemeeter_api-2.4.0/voicemeeterlib/updater.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/util.py` & `voicemeeter_api-2.4.0/voicemeeterlib/util.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/voicemeeterlib/vban.py` & `voicemeeter_api-2.4.0/voicemeeterlib/vban.py`

 * *Files identical despite different names*

### Comparing `voicemeeter_api-2.3.7/PKG-INFO` & `voicemeeter_api-2.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicemeeter-api
-Version: 2.3.7
+Version: 2.4.0
 Summary: A Python wrapper for the Voiceemeter API
 Home-page: https://github.com/onyx-and-iris/voicemeeter-api-python
 License: MIT
 Author: onyx-and-iris
 Author-email: code@onyxandiris.online
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

