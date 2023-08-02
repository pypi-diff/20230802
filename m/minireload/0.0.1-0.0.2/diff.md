# Comparing `tmp/minireload-0.0.1.tar.gz` & `tmp/minireload-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minireload-0.0.1.tar", last modified: Fri Mar 31 08:06:42 2023, max compression
+gzip compressed data, was "minireload-0.0.2.tar", last modified: Wed Aug  2 08:02:18 2023, max compression
```

## Comparing `minireload-0.0.1.tar` & `minireload-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-03-31 08:06:42.826295 minireload-0.0.1/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 minireload-0.0.1/LICENSE
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1207 2023-03-31 08:06:42.826295 minireload-0.0.1/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      778 2023-03-31 07:55:26.000000 minireload-0.0.1/README.md
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      513 2023-03-31 07:55:26.000000 minireload-0.0.1/pyproject.toml
--rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-03-31 08:06:42.826295 minireload-0.0.1/setup.cfg
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-03-31 08:06:42.822296 minireload-0.0.1/src/
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-03-31 08:06:42.826295 minireload-0.0.1/src/minireload/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1570 2023-03-31 07:59:05.000000 minireload-0.0.1/src/minireload/__init__.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    12057 2023-03-31 07:55:26.000000 minireload-0.0.1/src/minireload/autoreload.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1226 2023-03-31 08:05:27.000000 minireload-0.0.1/src/minireload/main.py
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-03-31 08:06:42.826295 minireload-0.0.1/src/minireload.egg-info/
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1207 2023-03-31 08:06:42.000000 minireload-0.0.1/src/minireload.egg-info/PKG-INFO
--rw-r--r--   0 ruof      (1000) ruof      (1000)      263 2023-03-31 08:06:42.000000 minireload-0.0.1/src/minireload.egg-info/SOURCES.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-03-31 08:06:42.000000 minireload-0.0.1/src/minireload.egg-info/dependency_links.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-03-31 08:06:42.000000 minireload-0.0.1/src/minireload.egg-info/top_level.txt
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:02:18.538319 minireload-0.0.2/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 minireload-0.0.2/LICENSE
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     1207 2023-08-02 08:02:18.538319 minireload-0.0.2/PKG-INFO
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      778 2023-03-31 07:55:26.000000 minireload-0.0.2/README.md
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      513 2023-08-02 08:01:32.000000 minireload-0.0.2/pyproject.toml
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-08-02 08:02:18.538319 minireload-0.0.2/setup.cfg
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:02:18.538319 minireload-0.0.2/src/
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:02:18.538319 minireload-0.0.2/src/minireload/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1570 2023-05-26 09:29:53.000000 minireload-0.0.2/src/minireload/__init__.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    12173 2023-08-02 07:59:39.000000 minireload-0.0.2/src/minireload/autoreload.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1226 2023-03-31 10:16:14.000000 minireload-0.0.2/src/minireload/main.py
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:02:18.538319 minireload-0.0.2/src/minireload.egg-info/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     1207 2023-08-02 08:02:18.000000 minireload-0.0.2/src/minireload.egg-info/PKG-INFO
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      263 2023-08-02 08:02:18.000000 minireload-0.0.2/src/minireload.egg-info/SOURCES.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-08-02 08:02:18.000000 minireload-0.0.2/src/minireload.egg-info/dependency_links.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-08-02 08:02:18.000000 minireload-0.0.2/src/minireload.egg-info/top_level.txt
```

### Comparing `minireload-0.0.1/LICENSE` & `minireload-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `minireload-0.0.1/PKG-INFO` & `minireload-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minireload
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hot code reloading for python scripts with a main loop
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/minireload
 Project-URL: Bug Tracker, https://github.com/joruof/minireload/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `minireload-0.0.1/README.md` & `minireload-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `minireload-0.0.1/pyproject.toml` & `minireload-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "minireload"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Jona Ruof", email="jona.ruof@uni-ulm.de" },
 ]
 description = "Hot code reloading for python scripts with a main loop"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `minireload-0.0.1/src/minireload/__init__.py` & `minireload-0.0.2/src/minireload/__init__.py`

 * *Files identical despite different names*

### Comparing `minireload-0.0.1/src/minireload/autoreload.py` & `minireload-0.0.2/src/minireload/autoreload.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,16 @@
 
 def scan_modules(requests, results):
 
     while True:
 
         try:
             mtime_table, req = requests.get(timeout=2.0)
+        except KeyboardInterrupt:
+            return
         except queue.Empty:
             return
 
         needs_reload = []
 
         for name, origin in req.items():
 
@@ -127,14 +129,18 @@
         self.init_subproc()
 
         # (module-name, name) -> weakref, for replacing old code objects
         self.old_objects = {}
 
         self.mtime_table = {}
 
+    def __del__(self):
+
+        self.scan_process.terminate()
+
     def init_subproc(self):
 
         self.waiting_for_scan = False
 
         self.scan_requests = mp.Queue(1)
         self.scan_results = mp.Queue(1)
```

### Comparing `minireload-0.0.1/src/minireload/main.py` & `minireload-0.0.2/src/minireload/main.py`

 * *Files identical despite different names*

### Comparing `minireload-0.0.1/src/minireload.egg-info/PKG-INFO` & `minireload-0.0.2/src/minireload.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minireload
-Version: 0.0.1
+Version: 0.0.2
 Summary: Hot code reloading for python scripts with a main loop
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/minireload
 Project-URL: Bug Tracker, https://github.com/joruof/minireload/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

