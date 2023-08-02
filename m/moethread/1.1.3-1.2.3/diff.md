# Comparing `tmp/moethread-1.1.3.tar.gz` & `tmp/moethread-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\moethread-1.1.3.tar", last modified: Sun Apr 30 06:02:37 2023, max compression
+gzip compressed data, was "dist\moethread-1.2.3.tar", last modified: Wed Aug  2 08:18:34 2023, max compression
```

## Comparing `moethread-1.1.3.tar` & `moethread-1.2.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 06:02:37.000000 moethread-1.1.3/
--rw-rw-rw-   0        0        0     7855 2023-04-30 06:02:37.000000 moethread-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     5823 2022-11-06 03:31:44.000000 moethread-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread/
--rw-rw-rw-   0        0        0      134 2023-02-22 01:29:53.000000 moethread-1.1.3/moethread/__init__.py
--rw-rw-rw-   0        0        0     3529 2023-04-30 05:57:01.000000 moethread-1.1.3/moethread/main.py
--rw-rw-rw-   0        0        0     1196 2023-04-30 05:59:40.000000 moethread-1.1.3/moethread/version.py
-drwxrwxrwx   0        0        0        0 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/
--rw-rw-rw-   0        0        0     7855 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      211 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-04-30 06:02:37.000000 moethread-1.1.3/moethread.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 06:02:37.000000 moethread-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1166 2023-04-30 06:02:33.000000 moethread-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:18:34.000000 moethread-1.2.3/
+-rw-rw-rw-   0        0        0     7855 2023-08-02 08:18:34.000000 moethread-1.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     5823 2022-11-06 03:31:44.000000 moethread-1.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 08:18:34.000000 moethread-1.2.3/moethread/
+-rw-rw-rw-   0        0        0      146 2023-08-02 08:12:11.000000 moethread-1.2.3/moethread/__init__.py
+-rw-rw-rw-   0        0        0     4259 2023-08-02 08:09:13.000000 moethread-1.2.3/moethread/main.py
+-rw-rw-rw-   0        0        0     1196 2023-08-02 06:29:14.000000 moethread-1.2.3/moethread/version.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:18:34.000000 moethread-1.2.3/moethread.egg-info/
+-rw-rw-rw-   0        0        0     7855 2023-08-02 08:18:34.000000 moethread-1.2.3/moethread.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-08-02 08:18:34.000000 moethread-1.2.3/moethread.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:18:34.000000 moethread-1.2.3/moethread.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 08:18:34.000000 moethread-1.2.3/moethread.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 08:18:34.000000 moethread-1.2.3/moethread.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:18:34.000000 moethread-1.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1501 2023-08-02 08:12:00.000000 moethread-1.2.3/setup.py
```

### Comparing `moethread-1.1.3/PKG-INFO` & `moethread-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moethread
-Version: 1.1.3
+Version: 1.2.3
 Summary: Python wrapper for ThreadPoolExecutor to easily multithread resource bound tasks
 Home-page: https://github.com/mhamdan91/moethread
 Author: mhamdan91 (Hamdan, Muhammad)
 Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Moethread
         =======================================
```

### Comparing `moethread-1.1.3/README.md` & `moethread-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `moethread-1.1.3/moethread/main.py` & `moethread-1.2.3/moethread/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -20,58 +20,76 @@
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
 import time
 import sys
 import math
+from moecolor import print
+from moecolor import FormatText as ft
 from concurrent.futures import ThreadPoolExecutor
 
-def parallel_call(func):
-    def eta_estimator(completed_percent, current_time):
-        rem =  (100.0 * current_time)/ completed_percent -  current_time
-        return rem
+def func_status(func):
+    def _wrapper(*args, **kwargs):
+        print('********************* MultiThreading Start *********************', color='#FFFF99')
+        result = func(*args, **kwargs)
+        print('********************* MultiThreading End *********************', color='#FFFF99')
+        return result
+    return _wrapper
+
+def progress(count, total, st, return_str=False):
+        elapsed_time = time.perf_counter() - st
+        completed = count / total
+        completed_percent = completed * 100
+        eta = (100.0 * elapsed_time)/ completed_percent -  elapsed_time
+        msg = f"\r[ STATUS ] Progress: {completed:0.2%} | Processed: {count}/{total} | " \
+              f"Elapsed-time: {elapsed_time:0.2f}s | ETA: {eta:0.3f}s"
+        if return_str:
+            return msg
+        else:
+            sys.stdout.write(ft(msg, color='lime').text)
+            sys.stdout.flush()
+            if count >= total:
+                print("") # Needed after completing job...
 
+def parallel_call(func):
     def processor(*args, **kwargs):
         global count, st
         total = kwargs.get('total')
         # Before call
         func(*args, **kwargs)
         # After call
         count += 1
-        et = time.perf_counter()
-        lapsed_time = et-st
-        completed = count/total
-        eta = eta_estimator(completed * 100, lapsed_time)
-        msg = f"\r[ STATUS ] Progress: {completed:0.2%} | Processed: {count}/{total} | Elapsed-time: {lapsed_time:0.2f}s | ETA: {eta:0.3f}s"
-        sys.stdout.write(msg)
-        sys.stdout.flush()
+        progress(count, total, st)
 
+    @func_status
     def wrapper(*args, **kwargs):
         # Parallelize task...
-        global count, st
-        count = 0
-        _data = kwargs.get('data')
-        total = len(list(_data.values())[0])
-        print('********************* MultiThreading Start *********************')
-        if not total:
-            print("[  WARN  ] Recieved empty list. Early termination...")
-            print('********************* MultiThreading End *********************')
+        try:
+            global count, st
+            count = 0
+            _data = kwargs.get('data')
+            if not _data:
+                print("[  WARN  ] Recieved empty list or invalid argument. Make sure to "\
+                      "provide data as a kwarg [data=your_data_dict]. Early termination...", color='orange')
+                return
+            total = len(list(_data.values())[0])
+            _threads = kwargs.get('threads', -1) or kwargs.get('thread', -1)
+            thread_limit = kwargs.get('thread_limit', 0)
+            thread_count = (int(math.sqrt(total)) + 1) * int(math.log(total, 10)) if math.log(total, 10) >= 1 else 1
+            thread = thread_count if _threads < 1 else _threads
+            threads = min(4096, thread) if thread_limit == 0 else thread
+            print(f"[  INFO  ] Launching: {threads} threads...", color='blue')
+            # Check if all values have the same length, and raise exception if not...
+            for key in _data:
+                if total != len(_data[key]):
+                    raise Exception("Dictionary values are inconsistent. All values must have the same length...")
+                st = time.perf_counter()
+            with ThreadPoolExecutor(threads) as exe:
+                # Iterate over data...
+                for i in range(total):
+                    data = {key: list(_data[key])[i] for key in _data}
+                    exe.submit(processor, *args, data=data, total=total)
+        except Exception as e:
+            print(f"[ ERROR ] {e}.", color='red')
             return
-        _threads = kwargs.get('threads', -1) or kwargs.get('thread', -1)
-        thread_limit = kwargs.get('thread_limit', 0)
-        thread_count = (int(math.sqrt(total)) + 1) * int(math.log(total, 10)) if math.log(total, 10) >= 1 else 1
-        thread = thread_count if _threads < 1 else _threads
-        threads = min(4096, thread) if thread_limit == 0 else thread
-        print(f"[  INFO  ] Launching: {threads} threads...")
-        # Check if all values have the same length, and raise exception if not...
-        for key in _data:
-            if total != len(_data[key]):
-                raise "Dictionary values are inconsistent. All values must have the same length..."
-        st = time.perf_counter()
-        with ThreadPoolExecutor(threads) as exe:
-            # Iterate over data...
-            for i in range(total):
-                data = {key: list(_data[key])[i] for key in _data}
-                exe.submit(processor, *args, data=data, total=total)
-        print('\n********************* MultiThreading End *********************')
     return wrapper
```

### Comparing `moethread-1.1.3/moethread/version.py` & `moethread-1.2.3/moethread/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.1.3"
+__version__ = "1.2.3"
 __author__ = "Muhammad Hamdan <mhamdan.dev@gmail.com>"
 __copyright__ = """
 MIT License
 
 Copyright (c) 2022 Muhammad Hamdan
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `moethread-1.1.3/moethread.egg-info/PKG-INFO` & `moethread-1.2.3/moethread.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moethread
-Version: 1.1.3
+Version: 1.2.3
 Summary: Python wrapper for ThreadPoolExecutor to easily multithread resource bound tasks
 Home-page: https://github.com/mhamdan91/moethread
 Author: mhamdan91 (Hamdan, Muhammad)
 Author-email: <mhamdan.dev@gmail.com>
 License: UNKNOWN
 Description: Moethread
         =======================================
```

### Comparing `moethread-1.1.3/setup.py` & `moethread-1.2.3/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,25 +1,29 @@
-from setuptools import setup, find_packages
 import os
-
+from setuptools import setup, find_packages
+from pip._internal.network.session import PipSession
+from pip._internal.req.req_file import parse_requirements
 from moethread.version import __version__
+VERSION = __version__
+PROJECT_DIR = os.path.dirname(os.path.realpath(__file__))
+REQUIREMENTS = parse_requirements(os.path.join(PROJECT_DIR, 'requirements.txt'), session=PipSession())
 DESCRIPTION = 'Python wrapper for ThreadPoolExecutor to easily multithread resource bound tasks'
 LONG_DESCRIPTION = open('README.md').read()
 # Setting up
 setup(
     name="moethread",
-    version=__version__,
+    version=VERSION,
     author="mhamdan91 (Hamdan, Muhammad)",
     author_email="<mhamdan.dev@gmail.com>",
     url='https://github.com/mhamdan91/moethread',
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=[str(ir.requirement) for ir in REQUIREMENTS],
     keywords=['python', 'multithreading', 'wrappers', 'decorator', 'pool', 'multitasking',
               'easy multithreading', 'thread', 'parallel', 'concurrent'],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
```

