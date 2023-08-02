# Comparing `tmp/shareddata-2.2.7.tar.gz` & `tmp/shareddata-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.2.7.tar", last modified: Tue Aug  1 10:28:45 2023, max compression
+gzip compressed data, was "shareddata-2.3.0.tar", last modified: Wed Aug  2 08:15:34 2023, max compression
```

## Comparing `shareddata-2.2.7.tar` & `shareddata-2.3.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-01 10:28:45.418496 shareddata-2.2.7/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.2.7/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-01 10:28:45.418496 shareddata-2.2.7/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.2.7/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.2.7/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-01 10:28:45.418496 shareddata-2.2.7/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-01 10:28:45.418496 shareddata-2.2.7/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-01 10:28:45.418496 shareddata-2.2.7/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-06-30 13:42:45.000000 shareddata-2.2.7/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-06-24 22:46:48.000000 shareddata-2.2.7/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-07-29 20:08:59.000000 shareddata-2.2.7/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-07-29 18:19:38.000000 shareddata-2.2.7/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-07-29 20:09:03.000000 shareddata-2.2.7/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-07-31 11:49:07.000000 shareddata-2.2.7/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 10:28:18.000000 shareddata-2.2.7/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4472 2023-07-08 20:55:15.000000 shareddata-2.2.7/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-07-29 20:09:00.000000 shareddata-2.2.7/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-07-31 11:51:47.000000 shareddata-2.2.7/src/SharedData/RealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-07-31 09:53:00.000000 shareddata-2.2.7/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9030 2023-07-31 12:46:43.000000 shareddata-2.2.7/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    28818 2023-07-31 10:09:34.000000 shareddata-2.2.7/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-07-31 12:53:11.000000 shareddata-2.2.7/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-06-25 22:48:17.000000 shareddata-2.2.7/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-07-31 10:19:55.000000 shareddata-2.2.7/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-07-31 17:38:51.000000 shareddata-2.2.7/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.2.7/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.2.7/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-01 10:28:45.418496 shareddata-2.2.7/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-01 10:28:45.000000 shareddata-2.2.7/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:15:34.725597 shareddata-2.3.0/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.3.0/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 08:15:34.725597 shareddata-2.3.0/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.3.0/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.3.0/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-02 08:15:34.725597 shareddata-2.3.0/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:15:34.725597 shareddata-2.3.0/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:15:34.725597 shareddata-2.3.0/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4050 2023-08-02 07:32:52.000000 shareddata-2.3.0/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/RealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9030 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30596 2023-08-02 08:12:48.000000 shareddata-2.3.0/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.3.0/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.3.0/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:15:34.725597 shareddata-2.3.0/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.2.7/LICENSE` & `shareddata-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/PKG-INFO` & `shareddata-2.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.2.7
+Version: 2.3.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.2.7/README.md` & `shareddata-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/setup.cfg` & `shareddata-2.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.2.7
+version = 2.3.0
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.2.7/src/SharedData/AWSKinesis.py` & `shareddata-2.3.0/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/AWSS3.py` & `shareddata-2.3.0/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/DataFrame.py` & `shareddata-2.3.0/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/Defaults.py` & `shareddata-2.3.0/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/Logger.py` & `shareddata-2.3.0/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.3.0/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/Metadata.py` & `shareddata-2.3.0/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/MultiProc.py` & `shareddata-2.3.0/src/SharedData/MultiProc.py`

 * *Files 12% similar despite different names*

```diff
@@ -32,97 +32,83 @@
 #     end = iteration[2]
 #     calendars = args[0]
 #     idx = (calendars[cal]>=start) & ((calendars[cal]<=end))
 #     return [np.count_nonzero(idx)]
 
 
 # load all files in a directory into memory
-def io_bound(thread_func, iterator, args, maxproc=None, maxthreads=10):
-    results = []    
+def io_bound(thread_func, iterator, args, \
+    maxproc=multiprocessing.cpu_count() - 2, maxthreads=10):
+    
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
-            futures = list()
+            futures = []
             # split the load operations into chunks
             for i in range(0, niterator, chunksize):
                 # select a chunk of filenames
                 proc_iterator = iterator[i:(i + chunksize)]
                 # submit the task
                 future = executor.submit(io_bound_process, thread_func, proc_iterator, args, maxthreads)
-                futures.append(future)
+                futures.extend(future)
             # process all results
-            for future in futures:
-                # open the file and load the data
-                res = future.result()
-                results = [*results, *res]                
+            for future in futures:                
+                results.extend(future.result())
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
             futures = [exe.submit(thread_func, iteration, args) for iteration in proc_iterator]
             # collect data
             for future in futures:
-                res = future.result()
-                results = [*results, *res]
-        
+                results.extend(future.result())                        
     return results
  
-
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
-            futures = list()
+            futures = []
             # split the load operations into chunks
             for i in range(0, niterator, chunksize):
                 # select a chunk of filenames
                 proc_iterator = iterator[i:(i + chunksize)]
                 # submit the task
                 future = executor.submit(cpu_bound_process, thread_func, proc_iterator, args)
-                futures.append(future)                                 
+                futures.extend(future)                                 
             # process all results
-            for future in futures:
-                # open the file and load the data
-                res = future.result()
-                results = [*results, *res]    
+            for future in futures:                
+                results.extend(future.result())                
     return results
 
-
 # return the contents of many files
 def cpu_bound_process(thread_func, proc_iterator, args):
     results = []
     for iteration in proc_iterator:
-        res = thread_func(iteration, args)
-        results = [*results, *res]              
+        results.extend(thread_func(iteration, args))
     return results
 
-def progressbar_thread(progress,niterations):
-    pbar = tqdm(total=niterations,desc='Running multi proc...')
-    while True:        
-        pbar.update(progress - pbar.n)
-        if progress >= niterations:
-            break
-        time.sleep(0.2)
```

### Comparing `shareddata-2.2.7/src/SharedData/RealTime.py` & `shareddata-2.3.0/src/SharedData/RealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/RealTimeProcess.py` & `shareddata-2.3.0/src/SharedData/RealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/SharedData.py` & `shareddata-2.3.0/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/SharedNumpy.py` & `shareddata-2.3.0/src/SharedData/SharedNumpy.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/Table.py` & `shareddata-2.3.0/src/SharedData/Table.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,28 +86,31 @@
                     formats = [item[1] for item in descr]
                     size = int(records.size*1.25)
                     self.create(names,formats,size)
                     self.records.insert(records)
 
                 elif (records is None):
                     # create new shared memory read value
-                    tini = time.time()            
-                    self.read(size)
+                    tini = time.time()                                
+                    if not self.read(size):
+                        raise Exception('%s/%s does not exist!' % (self.source,self.tablename))
                     te = time.time()-tini+0.000001
                     datasize = self.hdr['count']*self.hdr['itemsize']/1000000
                     Logger.log.debug('read %s/%s %.2fMB in %.2fs %.2fMBps ' % \
                         (self.source,self.tablename,datasize,te,datasize/te))
                     
             elif (self.create_map == 'map'):
                 # map existing shared memory
                 self.malloc_map()
         except Exception as e:
             path, shm_name = self.get_path()
             Logger.log.error('Error initalizing %s!\n%s' % (shm_name,e))
             self.free()
+            raise Exception('Error initalizing %s!\n%s' % (shm_name,e))
+            
 
         self.init_time = time.time() - self.init_time
         
     def get_path(self):
         shm_name = self.user + '/' + self.database + '/' \
             + self.period + '/' + self.source + '/table/' + self.tablename
         if os.name=='posix':
@@ -213,14 +216,15 @@
         self.recformats = descr.split(';')[1].split(',')
         self.recdtype = np.dtype({'names':self.recnames,'formats':self.recformats})
         self.records = SharedNumpy((self.hdr['recordssize'],),\
             dtype=self.recdtype,buffer=self.shm.buf, offset=nb_hdr)
         self.records.table = self
         
     def read(self,size=None):
+        success = False
         path, shm_name = self.get_path()
         head_io = None
         head_io_remote_isnewer = False
         tail_io = None
         tail_io_remote_isnewer = False
         headpath = path / 'head.bin'
         tailpath = path / 'tail.bin'
@@ -230,28 +234,30 @@
         # download remote head if its newer than local
         if self.shareddata.s3read:
             force_download= (not self.shareddata.save_local)     
             tini = time.time()
             [head_io_gzip, head_local_mtime, head_remote_mtime] = \
                 S3Download(str(headpath),str(headpath)+'.gzip',force_download)            
             if not head_io_gzip is None:
+                success=True
                 te = time.time()-tini+0.000001
                 datasize = head_io_gzip.getbuffer().nbytes/1000000
                 Logger.log.debug('download head %s/%s %.2fMB in %.2fs %.2fMBps ' % \
                     (self.source,self.tablename,datasize,te,datasize/te))
                 
                 head_io_remote_isnewer = True
                 head_io_gzip.seek(0)
                 head_io = gzip.GzipFile(fileobj=head_io_gzip, mode='rb')                
                 unzip_head = True
                 
         # open head_io to read header
         if self.shareddata.save_local:
             if head_io is None:
                 if headpath.exists():
+                    success=True
                     head_io = open(headpath, 'rb')
 
         # read header
         if not head_io is None:
             head_io.seek(0)
             nbhdrdescr = int.from_bytes(head_io.read(8),byteorder='little')
             hdrdescr_b = head_io.read(nbhdrdescr)
@@ -398,14 +404,16 @@
                         self.write_tail(path,nb_header,nb_head,nb_tail,tail_remote_mtime)
                         UpdateModTime(path/'tail.bin',tail_remote_mtime)
                 except Exception as e:
                     Logger.log.error('Could not save local %s\n%s!' % (path,e))
                 
                 self.release()
 
+        return success
+
     def malloc_map(self):
         # Read the header
         nbhdrdescr = int.from_bytes(self.shm.buf[0:8],byteorder='little')
         hdrdescr_b = self.shm.buf[8:8+nbhdrdescr].tobytes()
         hdrdescr = hdrdescr_b.decode(encoding='UTF-8',errors='ignore')
         hdrdescr = hdrdescr.replace('\x00','')
         self.hdrnames = hdrdescr.split(';')[0].split(',')
@@ -457,24 +465,31 @@
             self.release()
             return False
         
         self.release()
         return True
 
     def fill_header(self,md5hash=None):
-        maxtailsize = int(self.maxtailbytes / self.hdr['itemsize'])
-        if self.hdr['count']<=maxtailsize:
+
+        partdate = pd.Timestamp(datetime(datetime.now().year,1,1))
+        idx = self.records['date']>=partdate
+        if np.any(idx):
+            if np.all(idx):                
+                headsize = self.hdr['count']
+                tailsize = 0
+                self.hdr['hastail']=0
+            else:
+                partid = np.where(idx)[0][0]
+                headsize = partid
+                tailsize = self.hdr['count'] - partid            
+                self.hdr['hastail']=1
+        else:
             tailsize = 0
             headsize = self.hdr['count']            
             self.hdr['hastail']=0
-        else:
-            tailsize = self.hdr['count'] % maxtailsize            
-            headsize = self.hdr['count'] - tailsize
-            self.hdr['hastail']=1
-        
         
         headsize_chg = (headsize != self.hdr['headsize'])
         self.hdr['headsize'] = headsize
 
         head_modified = (self.hdr['minchgid']<=self.hdr['headsize'])
         write_head = (head_modified) | (headsize_chg)
 
@@ -482,16 +497,35 @@
         nb_head = int(self.hdr['headsize']*self.hdr['itemsize'])
         nb_tail = int(tailsize*self.hdr['itemsize'])
         
         self.tailhdr['mtime'] = self.hdr['mtime']
         self.tailhdr['tailsize'] = tailsize
 
         if md5hash is None:
-            self.hdr['md5hash']=0 # reset the hash value        
-            m = hashlib.md5(self.shm.buf[nb_header:nb_header+nb_head+nb_tail])
+            self.hdr['md5hash']=0 # reset the hash value
+            nb_records_mb = (nb_header+nb_head+nb_tail)/(1024*1024)
+            if nb_records_mb<=100:
+                m = hashlib.md5(self.shm.buf[nb_header:nb_header+nb_head+nb_tail])
+            else:
+                message = 'Creating md5 hash:%iMB %s/%s' % (nb_records_mb,self.source,self.tablename)
+                block_size = 100 * 1024 * 1024 # or any other block size that you prefer
+                nb_total = nb_header+nb_head+nb_tail
+                read_bytes = nb_header
+                m = hashlib.md5()                    
+                # Use a with block to manage the progress bar
+                with tqdm(total=nb_total, unit='B',unit_scale=True, desc=message) as pbar:                    
+                    # Loop until we have read all the data                    
+                    while read_bytes < nb_total:
+                        # Read a block of data
+                        chunk_size = min(block_size, nb_total-read_bytes)
+                        # Update the shared memory buffer with the newly read data
+                        m.update(self.shm.buf[read_bytes:read_bytes+chunk_size])
+                        read_bytes += chunk_size # update the total number of bytes read so far
+                        # Update the progress bar
+                        pbar.update( chunk_size )
             self.hdr['md5hash'] = m.digest()
         else:
             self.hdr['md5hash'] = md5hash
         self.tailhdr['md5hash'] = self.hdr['md5hash']
 
         return [write_head,nb_header,nb_head,nb_tail]
     
@@ -604,15 +638,15 @@
             tini = time.time()
             hdrptr = self.hdr.__array_interface__['data'][0]
             semseek = 258        
             while cpp.bool_compare_and_swap(hdrptr, semseek, 0, 1)==0:
                 telapsed = time.time() - tini
                 if telapsed>timeout:
                     raise TimeoutError('Timeout waiting for semaphore')
-                time.sleep(0.0001)
+                time.sleep(0.000001)
         else:
             while self.hdr['semaphore']!=0:
                 telapsed = time.time() - tini
                 if telapsed>timeout:
                     raise TimeoutError('Timeout waiting for semaphore')
                 time.sleep(0.0001)
             self.hdr['semaphore'] = 1
```

### Comparing `shareddata-2.2.7/src/SharedData/TableIndex.py` & `shareddata-2.3.0/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/TableIndexJit.py` & `shareddata-2.3.0/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/TimeSeries.py` & `shareddata-2.3.0/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/TimeseriesContainer.py` & `shareddata-2.3.0/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/SharedData/Utils.py` & `shareddata-2.3.0/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.2.7/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.3.0/src/shareddata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.2.7
+Version: 2.3.0
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.2.7/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.3.0/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

