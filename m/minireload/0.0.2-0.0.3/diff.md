# Comparing `tmp/minireload-0.0.2.tar.gz` & `tmp/minireload-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minireload-0.0.2.tar", last modified: Wed Aug  2 08:02:18 2023, max compression
+gzip compressed data, was "minireload-0.0.3.tar", last modified: Wed Aug  2 08:52:57 2023, max compression
```

## Comparing `minireload-0.0.2.tar` & `minireload-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:02:18.538319 minireload-0.0.2/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 minireload-0.0.2/LICENSE
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1207 2023-08-02 08:02:18.538319 minireload-0.0.2/PKG-INFO
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      778 2023-03-31 07:55:26.000000 minireload-0.0.2/README.md
--rw-rw-r--   0 ruof      (1000) ruof      (1000)      513 2023-08-02 08:01:32.000000 minireload-0.0.2/pyproject.toml
--rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-08-02 08:02:18.538319 minireload-0.0.2/setup.cfg
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:02:18.538319 minireload-0.0.2/src/
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:02:18.538319 minireload-0.0.2/src/minireload/
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1570 2023-05-26 09:29:53.000000 minireload-0.0.2/src/minireload/__init__.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)    12173 2023-08-02 07:59:39.000000 minireload-0.0.2/src/minireload/autoreload.py
--rw-rw-r--   0 ruof      (1000) ruof      (1000)     1226 2023-03-31 10:16:14.000000 minireload-0.0.2/src/minireload/main.py
-drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:02:18.538319 minireload-0.0.2/src/minireload.egg-info/
--rw-r--r--   0 ruof      (1000) ruof      (1000)     1207 2023-08-02 08:02:18.000000 minireload-0.0.2/src/minireload.egg-info/PKG-INFO
--rw-r--r--   0 ruof      (1000) ruof      (1000)      263 2023-08-02 08:02:18.000000 minireload-0.0.2/src/minireload.egg-info/SOURCES.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-08-02 08:02:18.000000 minireload-0.0.2/src/minireload.egg-info/dependency_links.txt
--rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-08-02 08:02:18.000000 minireload-0.0.2/src/minireload.egg-info/top_level.txt
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:52:57.678904 minireload-0.0.3/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1496 2023-03-31 07:55:26.000000 minireload-0.0.3/LICENSE
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     1270 2023-08-02 08:52:57.678904 minireload-0.0.3/PKG-INFO
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      841 2023-08-02 08:51:26.000000 minireload-0.0.3/README.md
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)      513 2023-08-02 08:52:33.000000 minireload-0.0.3/pyproject.toml
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       38 2023-08-02 08:52:57.678904 minireload-0.0.3/setup.cfg
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:52:57.678904 minireload-0.0.3/src/
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:52:57.678904 minireload-0.0.3/src/minireload/
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1623 2023-08-02 08:48:12.000000 minireload-0.0.3/src/minireload/__init__.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)    12213 2023-08-02 08:50:45.000000 minireload-0.0.3/src/minireload/autoreload.py
+-rw-rw-r--   0 ruof      (1000) ruof      (1000)     1226 2023-03-31 10:16:14.000000 minireload-0.0.3/src/minireload/main.py
+drwxr-xr-x   0 ruof      (1000) ruof      (1000)        0 2023-08-02 08:52:57.678904 minireload-0.0.3/src/minireload.egg-info/
+-rw-r--r--   0 ruof      (1000) ruof      (1000)     1270 2023-08-02 08:52:57.000000 minireload-0.0.3/src/minireload.egg-info/PKG-INFO
+-rw-r--r--   0 ruof      (1000) ruof      (1000)      263 2023-08-02 08:52:57.000000 minireload-0.0.3/src/minireload.egg-info/SOURCES.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)        1 2023-08-02 08:52:57.000000 minireload-0.0.3/src/minireload.egg-info/dependency_links.txt
+-rw-r--r--   0 ruof      (1000) ruof      (1000)       11 2023-08-02 08:52:57.000000 minireload-0.0.3/src/minireload.egg-info/top_level.txt
```

### Comparing `minireload-0.0.2/LICENSE` & `minireload-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `minireload-0.0.2/PKG-INFO` & `minireload-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minireload
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hot code reloading for python scripts with a main loop
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/minireload
 Project-URL: Bug Tracker, https://github.com/joruof/minireload/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,14 +12,22 @@
 
 # minireload
 
 Hot code reloading for python scripts with a main loop.
 Basically just a nicer front-end for superreload + exception handling.
 Requires only the python standard library and no external dependencies. 
 
+
+## Setup
+
+Available via pip:
+```
+pip3 install minireload
+```
+
 ## Usage
 
 ```python
 import minireload as mr
 
 class Main:
```

### Comparing `minireload-0.0.2/README.md` & `minireload-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # minireload
 
 Hot code reloading for python scripts with a main loop.
 Basically just a nicer front-end for superreload + exception handling.
 Requires only the python standard library and no external dependencies. 
 
+
+## Setup
+
+Available via pip:
+```
+pip3 install minireload
+```
+
 ## Usage
 
 ```python
 import minireload as mr
 
 class Main:
```

### Comparing `minireload-0.0.2/pyproject.toml` & `minireload-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "minireload"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Jona Ruof", email="jona.ruof@uni-ulm.de" },
 ]
 description = "Hot code reloading for python scripts with a main loop"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `minireload-0.0.2/src/minireload/__init__.py` & `minireload-0.0.3/src/minireload/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,12 +55,14 @@
                 func()
             elif exc_func is not None:
                 if exc_func(exc) == True:
                     exc = None
             else:
                 # backoff time to reduce cpu usage
                 time.sleep(0.1)
+        except KeyboardInterrupt:
+            return
         except SystemExit:
             return
         except Exception as e:
             traceback.print_exc()
             exc = e
```

### Comparing `minireload-0.0.2/src/minireload/autoreload.py` & `minireload-0.0.3/src/minireload/autoreload.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,56 +72,55 @@
 import queue
 import weakref
 
 from importlib import reload
 
 import multiprocessing as mp
 
-
 # ------------------------------------------------------------------------------
 # Autoreload functionality
 # ------------------------------------------------------------------------------
 
 
 def scan_modules(requests, results):
 
     while True:
-
         try:
-            mtime_table, req = requests.get(timeout=2.0)
-        except KeyboardInterrupt:
-            return
-        except queue.Empty:
-            return
-
-        needs_reload = []
-
-        for name, origin in req.items():
-
-            if name in [None, "__mp_main__", "__main__"]:
-                # we cannot reload(__main__) or reload(__mp_main__)
-                continue
-
-            if origin in [None, "built-in", "frozen"]:
-                # builtins or frozen modules will likely not change
-                continue
-
-            try:
-                mtime = os.stat(origin).st_mtime
-            except OSError:
-                continue
-
             try:
-                if mtime_table[name] < mtime:
-                    needs_reload.append(name)
+                mtime_table, req = requests.get(timeout=2.0)
+            except queue.Empty:
+                return
+
+            needs_reload = []
+
+            for name, origin in req.items():
+
+                if name in [None, "__mp_main__", "__main__"]:
+                    # we cannot reload(__main__) or reload(__mp_main__)
+                    continue
+
+                if origin in [None, "built-in", "frozen"]:
+                    # builtins or frozen modules will likely not change
+                    continue
+
+                try:
+                    mtime = os.stat(origin).st_mtime
+                except OSError:
+                    continue
+
+                try:
+                    if mtime_table[name] < mtime:
+                        needs_reload.append(name)
+                        mtime_table[name] = mtime
+                except KeyError:
                     mtime_table[name] = mtime
-            except KeyError:
-                mtime_table[name] = mtime
 
-        results.put((mtime_table, needs_reload))
+            results.put((mtime_table, needs_reload))
+        except KeyboardInterrupt:
+            return
 
 
 class ModuleReloader:
 
     def __init__(self):
 
         self.waiting_for_scan = False
@@ -129,18 +128,14 @@
         self.init_subproc()
 
         # (module-name, name) -> weakref, for replacing old code objects
         self.old_objects = {}
 
         self.mtime_table = {}
 
-    def __del__(self):
-
-        self.scan_process.terminate()
-
     def init_subproc(self):
 
         self.waiting_for_scan = False
 
         self.scan_requests = mp.Queue(1)
         self.scan_results = mp.Queue(1)
```

### Comparing `minireload-0.0.2/src/minireload/main.py` & `minireload-0.0.3/src/minireload/main.py`

 * *Files identical despite different names*

### Comparing `minireload-0.0.2/src/minireload.egg-info/PKG-INFO` & `minireload-0.0.3/src/minireload.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minireload
-Version: 0.0.2
+Version: 0.0.3
 Summary: Hot code reloading for python scripts with a main loop
 Author-email: Jona Ruof <jona.ruof@uni-ulm.de>
 Project-URL: Homepage, https://github.com/joruof/minireload
 Project-URL: Bug Tracker, https://github.com/joruof/minireload/issues
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -12,14 +12,22 @@
 
 # minireload
 
 Hot code reloading for python scripts with a main loop.
 Basically just a nicer front-end for superreload + exception handling.
 Requires only the python standard library and no external dependencies. 
 
+
+## Setup
+
+Available via pip:
+```
+pip3 install minireload
+```
+
 ## Usage
 
 ```python
 import minireload as mr
 
 class Main:
```

