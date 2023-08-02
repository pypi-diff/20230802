# Comparing `tmp/arrayqueues-1.3.1.tar.gz` & `tmp/arrayqueues-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayqueues-1.3.1.tar", last modified: Wed Feb 17 21:43:55 2021, max compression
+gzip compressed data, was "arrayqueues-1.4.1.tar", last modified: Wed Aug  2 14:11:06 2023, max compression
```

## Comparing `arrayqueues-1.3.1.tar` & `arrayqueues-1.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 21:43:55.331509 arrayqueues-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 21:43:55.323509 arrayqueues-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 21:43:55.327509 arrayqueues-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1994 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1283 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1054 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/NEWS.md
--rw-r--r--   0 runner    (1001) docker     (116)     2838 2021-02-17 21:43:55.331509 arrayqueues-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1786 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 21:43:55.327509 arrayqueues-1.3.1/arrayqueues/
--rw-r--r--   0 runner    (1001) docker     (116)      242 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/arrayqueues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3045 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/arrayqueues/portable_queue.py
--rw-r--r--   0 runner    (1001) docker     (116)     5683 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/arrayqueues/shared_arrays.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 21:43:55.327509 arrayqueues-1.3.1/arrayqueues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     2838 2021-02-17 21:43:54.000000 arrayqueues-1.3.1/arrayqueues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      471 2021-02-17 21:43:55.000000 arrayqueues-1.3.1/arrayqueues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-17 21:43:54.000000 arrayqueues-1.3.1/arrayqueues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       80 2021-02-17 21:43:54.000000 arrayqueues-1.3.1/arrayqueues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-02-17 21:43:54.000000 arrayqueues-1.3.1/arrayqueues.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      332 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)        5 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       66 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (116)      429 2021-02-17 21:43:55.331509 arrayqueues-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1229 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-17 21:43:55.331509 arrayqueues-1.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1014 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/tests/test_portable_queue.py
--rw-r--r--   0 runner    (1001) docker     (116)     3421 2021-02-17 21:43:44.000000 arrayqueues-1.3.1/tests/test_shared_arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:11:06.298292 arrayqueues-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:11:06.298292 arrayqueues-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:11:06.298292 arrayqueues-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/NEWS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-02 14:11:06.298292 arrayqueues-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:11:06.298292 arrayqueues-1.4.1/arrayqueues/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/arrayqueues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/arrayqueues/portable_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5681 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/arrayqueues/shared_arrays.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:11:06.298292 arrayqueues-1.4.1/arrayqueues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3010 2023-08-02 14:11:06.000000 arrayqueues-1.4.1/arrayqueues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-08-02 14:11:06.000000 arrayqueues-1.4.1/arrayqueues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 14:11:06.000000 arrayqueues-1.4.1/arrayqueues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-02 14:11:06.000000 arrayqueues-1.4.1/arrayqueues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-02 14:11:06.000000 arrayqueues-1.4.1/arrayqueues.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-08-02 14:11:06.298292 arrayqueues-1.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 14:11:06.298292 arrayqueues-1.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/tests/test_portable_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-08-02 14:10:56.000000 arrayqueues-1.4.1/tests/test_shared_arrays.py
```

### Comparing `arrayqueues-1.3.1/.github/workflows/main.yml` & `arrayqueues-1.4.1/.github/workflows/main.yml`

 * *Files 15% similar despite different names*

```diff
@@ -23,15 +23,15 @@
           flake8
   test:
     needs: lint
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-latest, macos-latest, windows-latest]
-        python-version: [3.7, 3.8.6]
+        python-version: ['3.7', '3.8', '3.9', '3.10', '3.11']
         exclude:
           - os: macos-latest
             python-version: 3.7
           - os: windows-latest
             python-version: 3.7
     steps:
       - uses: actions/checkout@v2
```

### Comparing `arrayqueues-1.3.1/.gitignore` & `arrayqueues-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `arrayqueues-1.3.1/LICENSE.txt` & `arrayqueues-1.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arrayqueues-1.3.1/PKG-INFO` & `arrayqueues-1.4.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 Metadata-Version: 2.1
 Name: arrayqueues
-Version: 1.3.1
+Version: 1.4.1
 Summary: Multiprocessing queues for numpy arrays using shared memory
 Home-page: https://github.com/portugueslab/arrayqueues
 Author: Vilim Stih @portugueslab
 Author-email: vilim@neuro.mpg.de
 License: MIT
-Description: # ArrayQueues
-        
-        [![Build Status](https://travis-ci.org/portugueslab/arrayqueues.svg?branch=master)](https://travis-ci.org/portugueslab/arrayqueues)
-        [![Coverage Status](https://coveralls.io/repos/github/portugueslab/arrayqueues/badge.svg?branch=master)](https://coveralls.io/github/portugueslab/arrayqueues?branch=master)
-        [![PyPI version](https://badge.fury.io/py/arrayqueues.svg)](https://badge.fury.io/py/arrayqueues)
-        
-        This package provides a drop-in replacement for the Python multiprocessing Queue class which handles transport of large numpy arrays.
-        It avoids pickling and uses the multiprocessing Array class in the background.
-        The major difference between this implementation and the normal queue is that the maximal amount of memory that the queue can have must be specified beforehand.
-        
-        Attempting to send an array of a different shape or datatype of the previously inserted one resets the queue.
-        Only passing of numpy arrays is supported, optionally annotated with timestamps if using the TimestampedArrayQueue class,
-        but other object types can be supported by extending the class.
-        
-        The package has been tested on Python 3.6/3/7 on Windows and MacOS and Linux with Travis. Python 2.7 is not supported.
-        
-        # Usage example
-        ```python
-        from arrayqueues.shared_arrays import ArrayQueue
-        from multiprocessing import Process
-        import numpy as np
-        
-        class ReadProcess(Process):
-            def __init__(self, source_queue):
-                super().__init__()
-                self.source_queue = source_queue
-              
-            def run(self):
-                print(self.source_queue.get())
-        
-        if __name__ == "__main__":
-            q = ArrayQueue(1) # intitialises an ArrayQueue which can hold 1MB of data
-            n = np.full((5,5), 5)
-            q.put(n)
-            r = ReadProcess(q)
-            r.start()
-            r.join()
-            
-        ```
-        
-        Further examples can be found in tests.
-        
 Keywords: multiprocessing queues arrays
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+# ArrayQueues
+
+[![Python Version](https://img.shields.io/pypi/pyversions/arrayqueues.svg)](https://pypi.org/project/arrayqueues)
+[![Tests](https://img.shields.io/github/workflow/status/portugueslab/arrayqueues/tests)](
+    https://github.com/portugueslab/arrayqueues/actions)
+[![Coverage Status](https://coveralls.io/repos/github/portugueslab/arrayqueues/badge.svg?branch=master)](https://coveralls.io/github/portugueslab/arrayqueues?branch=master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/arrayqueues.svg)](https://badge.fury.io/py/arrayqueues)
+
+This package provides a drop-in replacement for the Python multiprocessing Queue class which handles transport of large numpy arrays.
+It avoids pickling and uses the multiprocessing Array class in the background.
+The major difference between this implementation and the normal queue is that the maximal amount of memory that the queue can have must be specified beforehand.
+
+Attempting to send an array of a different shape or datatype of the previously inserted one resets the queue.
+Only passing of numpy arrays is supported, optionally annotated with timestamps if using the TimestampedArrayQueue class,
+but other object types can be supported by extending the class.
+
+The package has been tested on Python 3.6/3/7 on Windows and MacOS and Linux with Travis. Python 2.7 is not supported.
+
+# Usage example
+```python
+from arrayqueues.shared_arrays import ArrayQueue
+from multiprocessing import Process
+import numpy as np
+
+class ReadProcess(Process):
+    def __init__(self, source_queue):
+        super().__init__()
+        self.source_queue = source_queue
+      
+    def run(self):
+        print(self.source_queue.get())
+
+if __name__ == "__main__":
+    q = ArrayQueue(1) # intitialises an ArrayQueue which can hold 1MB of data
+    n = np.full((5,5), 5)
+    q.put(n)
+    r = ReadProcess(q)
+    r.start()
+    r.join()
+    
+```
+
+Further examples can be found in tests.
```

### Comparing `arrayqueues-1.3.1/README.md` & `arrayqueues-1.4.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # ArrayQueues
 
-[![Build Status](https://travis-ci.org/portugueslab/arrayqueues.svg?branch=master)](https://travis-ci.org/portugueslab/arrayqueues)
+[![Python Version](https://img.shields.io/pypi/pyversions/arrayqueues.svg)](https://pypi.org/project/arrayqueues)
+[![Tests](https://img.shields.io/github/workflow/status/portugueslab/arrayqueues/tests)](
+    https://github.com/portugueslab/arrayqueues/actions)
 [![Coverage Status](https://coveralls.io/repos/github/portugueslab/arrayqueues/badge.svg?branch=master)](https://coveralls.io/github/portugueslab/arrayqueues?branch=master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![PyPI version](https://badge.fury.io/py/arrayqueues.svg)](https://badge.fury.io/py/arrayqueues)
 
 This package provides a drop-in replacement for the Python multiprocessing Queue class which handles transport of large numpy arrays.
 It avoids pickling and uses the multiprocessing Array class in the background.
 The major difference between this implementation and the normal queue is that the maximal amount of memory that the queue can have must be specified beforehand.
 
 Attempting to send an array of a different shape or datatype of the previously inserted one resets the queue.
```

### Comparing `arrayqueues-1.3.1/arrayqueues/portable_queue.py` & `arrayqueues-1.4.1/arrayqueues/portable_queue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """The code below has been entirely taken from the following GitHub gist:
 https://gist.github.com/FanchenBao/d8577599c46eab1238a81857bb7277c9
 """
 
+import sys
 from multiprocessing import Value, get_context, queues
 
 
 class SharedCounter(object):
     """A synchronized shared counter.
 
     The locking done by multiprocessing.Value ensures that only a single
@@ -20,21 +21,21 @@
 
     """
 
     def __init__(self, n=0):
         self.count = Value("i", n)
 
     def increment(self, n=1):
-        """ Increment the counter by n (default = 1) """
+        """Increment the counter by n (default = 1)"""
         with self.count.get_lock():
             self.count.value += n
 
     @property
     def value(self):
-        """ Return the value of the counter """
+        """Return the value of the counter"""
         return self.count.value
 
 
 class PortableQueue(queues.Queue):
     """A portable implementation of multiprocessing.Queue.
 
     Because of multithreading / multiprocessing semantics, Queue.qsize() may
@@ -64,25 +65,28 @@
             self._writer,
             self._rlock,
             self._wlock,
             self._sem,
             self._opid,
             self.size,
         ) = state
-        super(PortableQueue, self)._after_fork()
+        if sys.version_info >= (3, 9):
+            super(PortableQueue, self)._reset()
+        else:
+            super(PortableQueue, self)._after_fork()
 
     def put(self, *args, **kwargs):
         super(PortableQueue, self).put(*args, **kwargs)
         self.size.increment(1)
 
     def get(self, *args, **kwargs):
         retrived_val = super(PortableQueue, self).get(*args, **kwargs)
         self.size.increment(-1)
         return retrived_val
 
     def qsize(self):
-        """ Reliable implementation of multiprocessing.Queue.qsize() """
+        """Reliable implementation of multiprocessing.Queue.qsize()"""
         return self.size.value
 
     def empty(self):
-        """ Reliable implementation of multiprocessing.Queue.empty() """
+        """Reliable implementation of multiprocessing.Queue.empty()"""
         return not self.qsize()
```

### Comparing `arrayqueues-1.3.1/arrayqueues/shared_arrays.py` & `arrayqueues-1.4.1/arrayqueues/shared_arrays.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,14 @@
         return self.queue.qsize()
 
 
 class TimestampedArrayQueue(ArrayQueue):
     """A small extension to support timestamps saved alongside arrays"""
 
     def put(self, element, timestamp=None):
-
         if self.view is None or not self.view.fits(element):
             self.view = ArrayView(
                 self.array.get_obj(), self.maxbytes, element.dtype, element.shape
             )
         else:
             self.check_full()
 
@@ -153,15 +152,14 @@
     """A small extension to support timestamps saved alongside arrays"""
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.counter = 0
 
     def put(self, element, timestamp=None):
-
         if self.view is None or not self.view.fits(element):
             self.view = ArrayView(
                 self.array.get_obj(), self.maxbytes, element.dtype, element.shape
             )
         else:
             self.check_full()
```

### Comparing `arrayqueues-1.3.1/arrayqueues.egg-info/PKG-INFO` & `arrayqueues-1.4.1/arrayqueues.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,68 @@
 Metadata-Version: 2.1
 Name: arrayqueues
-Version: 1.3.1
+Version: 1.4.1
 Summary: Multiprocessing queues for numpy arrays using shared memory
 Home-page: https://github.com/portugueslab/arrayqueues
 Author: Vilim Stih @portugueslab
 Author-email: vilim@neuro.mpg.de
 License: MIT
-Description: # ArrayQueues
-        
-        [![Build Status](https://travis-ci.org/portugueslab/arrayqueues.svg?branch=master)](https://travis-ci.org/portugueslab/arrayqueues)
-        [![Coverage Status](https://coveralls.io/repos/github/portugueslab/arrayqueues/badge.svg?branch=master)](https://coveralls.io/github/portugueslab/arrayqueues?branch=master)
-        [![PyPI version](https://badge.fury.io/py/arrayqueues.svg)](https://badge.fury.io/py/arrayqueues)
-        
-        This package provides a drop-in replacement for the Python multiprocessing Queue class which handles transport of large numpy arrays.
-        It avoids pickling and uses the multiprocessing Array class in the background.
-        The major difference between this implementation and the normal queue is that the maximal amount of memory that the queue can have must be specified beforehand.
-        
-        Attempting to send an array of a different shape or datatype of the previously inserted one resets the queue.
-        Only passing of numpy arrays is supported, optionally annotated with timestamps if using the TimestampedArrayQueue class,
-        but other object types can be supported by extending the class.
-        
-        The package has been tested on Python 3.6/3/7 on Windows and MacOS and Linux with Travis. Python 2.7 is not supported.
-        
-        # Usage example
-        ```python
-        from arrayqueues.shared_arrays import ArrayQueue
-        from multiprocessing import Process
-        import numpy as np
-        
-        class ReadProcess(Process):
-            def __init__(self, source_queue):
-                super().__init__()
-                self.source_queue = source_queue
-              
-            def run(self):
-                print(self.source_queue.get())
-        
-        if __name__ == "__main__":
-            q = ArrayQueue(1) # intitialises an ArrayQueue which can hold 1MB of data
-            n = np.full((5,5), 5)
-            q.put(n)
-            r = ReadProcess(q)
-            r.start()
-            r.join()
-            
-        ```
-        
-        Further examples can be found in tests.
-        
 Keywords: multiprocessing queues arrays
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Software Development :: Libraries
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE.txt
+
+# ArrayQueues
+
+[![Python Version](https://img.shields.io/pypi/pyversions/arrayqueues.svg)](https://pypi.org/project/arrayqueues)
+[![Tests](https://img.shields.io/github/workflow/status/portugueslab/arrayqueues/tests)](
+    https://github.com/portugueslab/arrayqueues/actions)
+[![Coverage Status](https://coveralls.io/repos/github/portugueslab/arrayqueues/badge.svg?branch=master)](https://coveralls.io/github/portugueslab/arrayqueues?branch=master)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/arrayqueues.svg)](https://badge.fury.io/py/arrayqueues)
+
+This package provides a drop-in replacement for the Python multiprocessing Queue class which handles transport of large numpy arrays.
+It avoids pickling and uses the multiprocessing Array class in the background.
+The major difference between this implementation and the normal queue is that the maximal amount of memory that the queue can have must be specified beforehand.
+
+Attempting to send an array of a different shape or datatype of the previously inserted one resets the queue.
+Only passing of numpy arrays is supported, optionally annotated with timestamps if using the TimestampedArrayQueue class,
+but other object types can be supported by extending the class.
+
+The package has been tested on Python 3.6/3/7 on Windows and MacOS and Linux with Travis. Python 2.7 is not supported.
+
+# Usage example
+```python
+from arrayqueues.shared_arrays import ArrayQueue
+from multiprocessing import Process
+import numpy as np
+
+class ReadProcess(Process):
+    def __init__(self, source_queue):
+        super().__init__()
+        self.source_queue = source_queue
+      
+    def run(self):
+        print(self.source_queue.get())
+
+if __name__ == "__main__":
+    q = ArrayQueue(1) # intitialises an ArrayQueue which can hold 1MB of data
+    n = np.full((5,5), 5)
+    q.put(n)
+    r = ReadProcess(q)
+    r.start()
+    r.join()
+    
+```
+
+Further examples can be found in tests.
```

### Comparing `arrayqueues-1.3.1/setup.py` & `arrayqueues-1.4.1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,32 @@
     requirements = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="arrayqueues",
-    version="1.3.1",
+    version="1.4.1",
     author="Vilim Stih @portugueslab",
     author_email="vilim@neuro.mpg.de",
     license="MIT",
     packages=find_namespace_packages(exclude=("docs", "tests*")),
     install_requires=requirements,
     extras_require=dict(dev=requirements_dev),
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Multimedia :: Video",
         "Topic :: Software Development :: Libraries",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
     keywords="multiprocessing queues arrays",
     description="Multiprocessing queues for numpy arrays using shared memory",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/portugueslab/arrayqueues",
 )
```

### Comparing `arrayqueues-1.3.1/tests/test_portable_queue.py` & `arrayqueues-1.4.1/tests/test_portable_queue.py`

 * *Files identical despite different names*

### Comparing `arrayqueues-1.3.1/tests/test_shared_arrays.py` & `arrayqueues-1.4.1/tests/test_shared_arrays.py`

 * *Files identical despite different names*

