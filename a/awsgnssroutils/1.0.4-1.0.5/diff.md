# Comparing `tmp/awsgnssroutils-1.0.4.tar.gz` & `tmp/awsgnssroutils-1.0.5.tar.gz`

## Comparing `awsgnssroutils-1.0.4.tar` & `awsgnssroutils-1.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/src/awsgnssroutils/__init__.py
--rw-r--r--   0        0        0    38941 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/src/awsgnssroutils/database.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/LICENSE
--rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/README.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.5/src/awsgnssroutils/__init__.py
+-rw-r--r--   0        0        0    39812 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.5/src/awsgnssroutils/database.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.5/LICENSE
+-rw-r--r--   0        0        0     7751 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.5/README.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8422 2020-02-02 00:00:00.000000 awsgnssroutils-1.0.5/PKG-INFO
```

### Comparing `awsgnssroutils-1.0.4/src/awsgnssroutils/database.py` & `awsgnssroutils-1.0.5/src/awsgnssroutils/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """database.py
 
 Authors: Amy McVey (amcvey@aer.com) and Stephen Leroy (sleroy@aer.com)
-Date: 29 June 2023
+Date: 2 Aug 2023
 
 ================================================================================
 
 This module contains utilities to query the AWS Registry of Open Data repository
 of GNSS radio occultation data. It does so using database files posted in the
 AWS repository.
 
@@ -49,23 +49,23 @@
 import numpy as np
 import s3fs
 import json
 import re
 import time
 from botocore import UNSIGNED
 
-#  Usefule parameters.
+#  Update valid processing centers as they appear in the AWS Registry of Open Data.
 
-
-#Update valid processing centers based on open data bucket listing
 s3 = s3fs.S3FileSystem( client_kwargs={ 'region_name': AWSregion },
-                                 config_kwargs={ 'signature_version': UNSIGNED }
-#lists processing_centers on open data bucket
+                                 config_kwargs={ 'signature_version': UNSIGNED } )
+
 initial_prefix_array = s3.ls( os.path.join( databaseS3bucket, f'contributed/v1.1/' ) )
-valid_processing_centers = [os.path.basename(prefix) for prefix in initial_prefix_array ]
+valid_processing_centers = [ os.path.basename(prefix) for prefix in initial_prefix_array ]
+
+#  Define valid file types.
 
 valid_file_types = [ "calibratedPhase", "refractivityRetrieval", "atmosphericRetrieval" ]
 
 #  Exception handling.
 
 class Error( Exception ):
     pass
@@ -637,20 +637,37 @@
 
             local_file_list.append( local_file )
 
         print( "Download took {:} seconds.".format( round((time.time()-sTime),1 ) ) )
         return local_file_list
 
     def values( self, field ):
-        """Return an ndarray of values of a requested field for the data in the
-        OccList. Valid fields are "longitude", "latitude", "datetime", "localtime".
-        Longitudes and latitudes are in degrees; datetime is an ISO format time;
-        and local times are in hours."""
+        """Return an array of values of a requested field for the data in the
+        OccList. Valid fields are "longitude", "latitude", "datetime", "localtime",
+        in which case ndarrays are returned. Longitudes and latitudes are in degrees;
+        datetime is an ISO format time; and local times are in hours. Valid values
+        also include paths to data files. If the requested field is "ucar_calibratedPhase",
+        then a list of strings is returned, each element being the path to a ucar_calibratedPhase
+        file, for example."""
 
-        if field == "longitude":
+        m = re.search( "^([a-z]+)_([a-zA-Z]+)$", field )
+
+        if m:
+            processing_center, file_type = m.group(1), m.group(2)
+            if processing_center in valid_processing_centers and file_type in valid_file_types:
+                x = []
+                for item in self._data:
+                    if field in item.keys():
+                        if item[field] == "":
+                            x.append( None )
+                        else:
+                            x.append( "s3://" + os.path.join( databaseS3bucket, item[field] ) )
+                    else:
+                        x.append( None )
+        elif field == "longitude":
             x = np.ma.masked_equal( [ item['longitude'] for item in self._data ], float_fill_value )
 
         elif field == "latitude":
             x = np.ma.masked_equal( [ item['latitude'] for item in self._data ], float_fill_value )
 
         elif field == "localtime":
             x = np.ma.masked_equal( [ item['local_time'] for item in self._data ], float_fill_value )
```

### Comparing `awsgnssroutils-1.0.4/LICENSE` & `awsgnssroutils-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.0.4/README.md` & `awsgnssroutils-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `awsgnssroutils-1.0.4/pyproject.toml` & `awsgnssroutils-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "hatchling", "s3fs", "numpy" ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awsgnssroutils"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
 	{ name="Stephen Leroy", email="sleroy@aer.com" },
 	{ name="Amy McVey", email="amcvey@aer.com" }
 	]
 description = "Utilities for access and manipulation of GNSS radio occultation in the AWS Registry of Open Data"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `awsgnssroutils-1.0.4/PKG-INFO` & `awsgnssroutils-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awsgnssroutils
-Version: 1.0.4
+Version: 1.0.5
 Summary: Utilities for access and manipulation of GNSS radio occultation in the AWS Registry of Open Data
 Project-URL: Homepage, https://github.com/gnss-ro/aws-opendata
 Project-URL: Bug Tracker, https://github.com/gnss-ro/aws-opendata/issues
 Author-email: Stephen Leroy <sleroy@aer.com>, Amy McVey <amcvey@aer.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

