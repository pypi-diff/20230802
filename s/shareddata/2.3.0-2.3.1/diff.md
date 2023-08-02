# Comparing `tmp/shareddata-2.3.0.tar.gz` & `tmp/shareddata-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shareddata-2.3.0.tar", last modified: Wed Aug  2 08:15:34 2023, max compression
+gzip compressed data, was "shareddata-2.3.1.tar", last modified: Wed Aug  2 08:23:34 2023, max compression
```

## Comparing `shareddata-2.3.0.tar` & `shareddata-2.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:15:34.725597 shareddata-2.3.0/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.3.0/LICENSE
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 08:15:34.725597 shareddata-2.3.0/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.3.0/README.md
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.3.0/pyproject.toml
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-02 08:15:34.725597 shareddata-2.3.0/setup.cfg
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:15:34.725597 shareddata-2.3.0/src/
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:15:34.725597 shareddata-2.3.0/src/SharedData/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/AWSKinesis.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/AWSS3.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/DataFrame.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/Defaults.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/Logger.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/LoggerConsumerProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/Metadata.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4050 2023-08-02 07:32:52.000000 shareddata-2.3.0/src/SharedData/MultiProc.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/RealTime.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/RealTimeProcess.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/SharedData.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9030 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/SharedNumpy.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30596 2023-08-02 08:12:48.000000 shareddata-2.3.0/src/SharedData/Table.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/TableIndex.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/TableIndexJit.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/TimeSeries.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-2.3.0/src/SharedData/TimeseriesContainer.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.3.0/src/SharedData/Utils.py
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.3.0/src/SharedData/__init__.py
-drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:15:34.725597 shareddata-2.3.0/src/shareddata.egg-info/
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/PKG-INFO
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/SOURCES.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/dependency_links.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/requires.txt
--rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-02 08:15:34.000000 shareddata-2.3.0/src/shareddata.egg-info/top_level.txt
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:23:34.166602 shareddata-2.3.1/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    35149 2023-06-24 22:46:48.000000 shareddata-2.3.1/LICENSE
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 08:23:34.166602 shareddata-2.3.1/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      611 2023-06-25 11:52:46.000000 shareddata-2.3.1/README.md
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      103 2023-06-24 22:46:48.000000 shareddata-2.3.1/pyproject.toml
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      894 2023-08-02 08:23:34.166602 shareddata-2.3.1/setup.cfg
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:23:34.166602 shareddata-2.3.1/src/
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:23:34.166602 shareddata-2.3.1/src/SharedData/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    14294 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/AWSKinesis.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     5533 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/AWSS3.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    10837 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/DataFrame.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1514 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/Defaults.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4284 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/Logger.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1272 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/LoggerConsumerProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    11236 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/Metadata.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     4050 2023-08-02 07:32:52.000000 shareddata-2.3.1/src/SharedData/MultiProc.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     3389 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/RealTime.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     2476 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/RealTimeProcess.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     7535 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/SharedData.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     9165 2023-08-02 08:23:09.000000 shareddata-2.3.1/src/SharedData/SharedNumpy.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    30167 2023-08-02 08:21:31.000000 shareddata-2.3.1/src/SharedData/Table.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     8672 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/TableIndex.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    18035 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/TableIndexJit.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    13509 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/TimeSeries.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)    16371 2023-08-01 11:14:58.000000 shareddata-2.3.1/src/SharedData/TimeseriesContainer.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1391 2023-07-29 18:49:47.000000 shareddata-2.3.1/src/SharedData/Utils.py
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        0 2023-06-24 22:46:48.000000 shareddata-2.3.1/src/SharedData/__init__.py
+drwxrwxr-x   0 jcooloj   (1000) jcooloj   (1000)        0 2023-08-02 08:23:34.166602 shareddata-2.3.1/src/shareddata.egg-info/
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)     1166 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/PKG-INFO
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      782 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/SOURCES.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)        1 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/dependency_links.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)      183 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/requires.txt
+-rw-rw-r--   0 jcooloj   (1000) jcooloj   (1000)       11 2023-08-02 08:23:34.000000 shareddata-2.3.1/src/shareddata.egg-info/top_level.txt
```

### Comparing `shareddata-2.3.0/LICENSE` & `shareddata-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/PKG-INFO` & `shareddata-2.3.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.3.0
+Version: 2.3.1
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.3.0/README.md` & `shareddata-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/setup.cfg` & `shareddata-2.3.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = shareddata
-version = 2.3.0
+version = 2.3.1
 author = Jose Carlito de Oliveira Filho
 author_email = jcarlitooliveira@gmail.com
 description = Shared Memory Database with S3 repository
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/jcarlitooliveira/SharedData
 project_urls =
```

### Comparing `shareddata-2.3.0/src/SharedData/AWSKinesis.py` & `shareddata-2.3.1/src/SharedData/AWSKinesis.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/AWSS3.py` & `shareddata-2.3.1/src/SharedData/AWSS3.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/DataFrame.py` & `shareddata-2.3.1/src/SharedData/DataFrame.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/Defaults.py` & `shareddata-2.3.1/src/SharedData/Defaults.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/Logger.py` & `shareddata-2.3.1/src/SharedData/Logger.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/LoggerConsumerProcess.py` & `shareddata-2.3.1/src/SharedData/LoggerConsumerProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/Metadata.py` & `shareddata-2.3.1/src/SharedData/Metadata.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/MultiProc.py` & `shareddata-2.3.1/src/SharedData/MultiProc.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/RealTime.py` & `shareddata-2.3.1/src/SharedData/RealTime.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/RealTimeProcess.py` & `shareddata-2.3.1/src/SharedData/RealTimeProcess.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/SharedData.py` & `shareddata-2.3.1/src/SharedData/SharedData.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/SharedNumpy.py` & `shareddata-2.3.1/src/SharedData/SharedNumpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 
     def __new__(cls, shape, dtype=None, buffer=None, offset=0, strides=None, order=None):
         obj = np.ndarray.__new__(
             cls, shape, dtype, buffer, offset, strides, order)
         obj.table = None
         return obj
 
+    def preallocate(self):
+        arr = super().__getitem__(slice(0, self.size))
+        arr['mtime'][:] = np.datetime64('NaT')
     ############################## KEYLESS OPERATIONS ########################################
 
     def insert(self, new_records):
         self.table.acquire()
 
         try:
             nrec = new_records.size
@@ -201,14 +204,16 @@
         return [dtiniid,dtendid+1]
     
     def get_index_date_portfolio(self,keys):    
         if not self.keys.initialized:
             self.keys.initialize()    
         return self.keys.get_index_date_portfolio_func(self[:], keys, self.pkey, self.keys.portiniidx,self.keys.portlist)
         
+
+    
     ############################## GETTERS / SETTERS ##############################
 
     def __getitem__(self, key):
         if hasattr(self, 'table'):
             arr = super().__getitem__(slice(0, self.count))  # slice arr
             if self.count > 0:                
                 return arr.__getitem__(key)
```

### Comparing `shareddata-2.3.0/src/SharedData/Table.py` & `shareddata-2.3.1/src/SharedData/Table.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,35 +193,24 @@
             self.shareddata.malloc(shm_name,create=True,size=total_size,overwrite=True)
         if not ismalloc:
             raise Exception('Could not allocate shared memory!')
 
         # allocate header
         self.hdr['semaphore']=1 # lock semaphore memory
         self.shm.buf[0:nb_hdr] = self.hdr.tobytes()
-        self.hdr = np.ndarray((1,),dtype=self.hdrdtype,buffer=self.shm.buf)[0]
-        # TODO: allow tail size to change
-        # set tail 10% of total file size in 100MB steps
-        # sizemb = (self.hdr['recordssize'] * self.hdr['itemsize'])/10**6
-        # if sizemb<=1000:
-        #     self.maxtailbytes = int(100*10**6)
-        # elif sizemb<=2000:
-        #     self.maxtailbytes = int(200*10**6)
-        # elif sizemb<=5000:
-        #     self.maxtailbytes = int(500*10**6)
-        # else:
-        #     self.maxtailbytes = int(1000*10**6)
-                
+        self.hdr = np.ndarray((1,),dtype=self.hdrdtype,buffer=self.shm.buf)[0]                        
         # allocate table data
         descr = self.hdr['descr'].decode(encoding='UTF-8',errors='ignore')
         self.recnames = descr.split(';')[0].split(',')
         self.recformats = descr.split(';')[1].split(',')
         self.recdtype = np.dtype({'names':self.recnames,'formats':self.recformats})
         self.records = SharedNumpy((self.hdr['recordssize'],),\
             dtype=self.recdtype,buffer=self.shm.buf, offset=nb_hdr)
         self.records.table = self
+        self.records.preallocate()
         
     def read(self,size=None):
         success = False
         path, shm_name = self.get_path()
         head_io = None
         head_io_remote_isnewer = False
         tail_io = None
```

### Comparing `shareddata-2.3.0/src/SharedData/TableIndex.py` & `shareddata-2.3.1/src/SharedData/TableIndex.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/TableIndexJit.py` & `shareddata-2.3.1/src/SharedData/TableIndexJit.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/TimeSeries.py` & `shareddata-2.3.1/src/SharedData/TimeSeries.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/TimeseriesContainer.py` & `shareddata-2.3.1/src/SharedData/TimeseriesContainer.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/SharedData/Utils.py` & `shareddata-2.3.1/src/SharedData/Utils.py`

 * *Files identical despite different names*

### Comparing `shareddata-2.3.0/src/shareddata.egg-info/PKG-INFO` & `shareddata-2.3.1/src/shareddata.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shareddata
-Version: 2.3.0
+Version: 2.3.1
 Summary: Shared Memory Database with S3 repository
 Home-page: https://github.com/jcarlitooliveira/SharedData
 Author: Jose Carlito de Oliveira Filho
 Author-email: jcarlitooliveira@gmail.com
 Project-URL: Bug Tracker, https://github.com/jcarlitooliveira/SharedData/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `shareddata-2.3.0/src/shareddata.egg-info/SOURCES.txt` & `shareddata-2.3.1/src/shareddata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

