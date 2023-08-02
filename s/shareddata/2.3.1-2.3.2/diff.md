# Comparing `tmp/shareddata-2.3.1.tar.gz` & `tmp/shareddata-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.3.1.tar", last modified: Wed Aug  2 08:23:34 2023, max compression
+gzip compressed data, was "shareddata-2.3.2.tar", last modified: Wed Aug  2 09:04:15 2023, max compression
```

## Comparing `shareddata-2.3.1.tar` & `shareddata-2.3.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:23:34.166602 shareddata-2.3.1/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.3.1/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 08:23:34.166602 shareddata-2.3.1/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.3.1/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.3.1/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-02 08:23:34.166602 shareddata-2.3.1/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:23:34.166602 shareddata-2.3.1/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:23:34.166602 shareddata-2.3.1/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4050 2023-08-02 07:32:52.000000 shareddata-2.3.1/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/RealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9165 2023-08-02 08:23:09.000000 shareddata-2.3.1/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30167 2023-08-02 08:21:31.000000 shareddata-2.3.1/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.3.1/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.3.1/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:23:34.166602 shareddata-2.3.1/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:04:15.857180 shareddata-2.3.2/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.3.2/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 09:04:15.857180 shareddata-2.3.2/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.3.2/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.3.2/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-02 09:04:15.857180 shareddata-2.3.2/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:04:15.853180 shareddata-2.3.2/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:04:15.857180 shareddata-2.3.2/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4251 2023-08-02 08:56:01.000000 shareddata-2.3.2/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/RealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9165 2023-08-02 08:55:08.000000 shareddata-2.3.2/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30167 2023-08-02 08:55:08.000000 shareddata-2.3.2/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-2.3.2/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.3.2/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.3.2/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 09:04:15.857180 shareddata-2.3.2/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-02 09:04:15.000000 shareddata-2.3.2/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.3.1/LICENSE` & `shareddata-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/PKG-INFO` & `shareddata-2.3.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.3.1
+Version: 2.3.2
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.3.1/README.md` & `shareddata-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/setup.cfg` & `shareddata-2.3.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.3.1
+version = 2.3.2
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.3.1/src/SharedData/AWSKinesis.py` & `shareddata-2.3.2/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/AWSS3.py` & `shareddata-2.3.2/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/DataFrame.py` & `shareddata-2.3.2/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/Defaults.py` & `shareddata-2.3.2/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/Logger.py` & `shareddata-2.3.2/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.3.2/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/Metadata.py` & `shareddata-2.3.2/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/MultiProc.py` & `shareddata-2.3.2/src/SharedData/MultiProc.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,83 +32,90 @@
 #     end = iteration[2]
 #     calendars = args[0]
 #     idx = (calendars[cal]>=start) & ((calendars[cal]<=end))
 #     return [np.count_nonzero(idx)]
 
 
 # load all files in a directory into memory
-def io_bound(thread_func, iterator, args, \
-    maxproc=multiprocessing.cpu_count() - 2, maxthreads=10):
-    
-    results = []
+def io_bound(thread_func, iterator, args, maxproc=None, maxthreads=10):
+    results = []    
     # determine chunksize
     niterator = len(iterator)
     if niterator>0:
         n_workers = multiprocessing.cpu_count() - 2
         n_workers = min(n_workers,niterator)
         if not maxproc is None:
             n_workers = min(n_workers,maxproc)
         chunksize = round(niterator / n_workers)
         # create the process pool
         with ProcessPoolExecutor(n_workers) as executor:        
-            futures = []
+            futures = list()
             # split the load operations into chunks
             for i in range(0, niterator, chunksize):
                 # select a chunk of filenames
                 proc_iterator = iterator[i:(i + chunksize)]
                 # submit the task
-                future = executor.submit(io_bound_process, thread_func, proc_iterator, args, maxthreads)
-                futures.extend(future)
+                future = executor.submit(io_bound_process, \
+                    thread_func, proc_iterator, args, maxthreads)
+                futures.append(future)
             # process all results
-            for future in futures:                
-                results.extend(future.result())
+            for future in futures:
+                # open the file and load the data
+                res = future.result()
+                results = [*results, *res]                
     return results
 
 # return the contents of many files
 def io_bound_process(thread_func, proc_iterator, args, maxthreads):
     results = []
     # create a thread pool
     nthreads = len(proc_iterator)
     nthreads = min(nthreads,maxthreads)
     if nthreads>0:
         with ThreadPoolExecutor(nthreads) as exe:
             # load files
-            futures = [exe.submit(thread_func, iteration, args) for iteration in proc_iterator]
+            futures = [exe.submit(thread_func, iteration, args) \
+                for iteration in proc_iterator]
             # collect data
             for future in futures:
-                results.extend(future.result())                        
+                res = future.result()
+                results = [*results, *res]
+        
     return results
  
+
 def cpu_bound(thread_func, iterator, args, maxproc = None):
     results = []    
     # determine chunksize
     niterator = len(iterator)
     if niterator>0:
         n_workers = multiprocessing.cpu_count() - 2    
         n_workers = min(n_workers,niterator)
         if not maxproc is None:
             n_workers = min(n_workers,maxproc)
         chunksize = round(niterator / n_workers)
         # create the process pool
         with ProcessPoolExecutor(n_workers) as executor:        
-            futures = []
+            futures = list()
             # split the load operations into chunks
             for i in range(0, niterator, chunksize):
                 # select a chunk of filenames
                 proc_iterator = iterator[i:(i + chunksize)]
                 # submit the task
                 future = executor.submit(cpu_bound_process, thread_func, proc_iterator, args)
-                futures.extend(future)                                 
+                futures.append(future)                                 
             # process all results
-            for future in futures:                
-                results.extend(future.result())                
+            for future in futures:
+                # open the file and load the data
+                res = future.result()
+                results = [*results, *res]    
     return results
 
+
 # return the contents of many files
 def cpu_bound_process(thread_func, proc_iterator, args):
     results = []
     for iteration in proc_iterator:
-        results.extend(thread_func(iteration, args))
+        res = thread_func(iteration, args)
+        results = [*results, *res]              
     return results
-
-
```

### Comparing `shareddata-2.3.1/src/SharedData/RealTime.py` & `shareddata-2.3.2/src/SharedData/RealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/RealTimeProcess.py` & `shareddata-2.3.2/src/SharedData/RealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/SharedData.py` & `shareddata-2.3.2/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/SharedNumpy.py` & `shareddata-2.3.2/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/Table.py` & `shareddata-2.3.2/src/SharedData/Table.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/TableIndex.py` & `shareddata-2.3.2/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/TableIndexJit.py` & `shareddata-2.3.2/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/TimeSeries.py` & `shareddata-2.3.2/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/TimeseriesContainer.py` & `shareddata-2.3.2/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/SharedData/Utils.py` & `shareddata-2.3.2/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.1/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.3.2/src/shareddata.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.3.1
+Version: 2.3.2
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.3.1/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.3.2/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

