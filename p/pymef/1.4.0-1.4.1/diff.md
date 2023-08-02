# Comparing `tmp/pymef-1.4.0-cp39-cp39-win_amd64.whl.zip` & `tmp/pymef-1.4.1-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 100439 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat       35 b- defN 23-Jul-31 12:56 pymef/__init__.py
--rw-rw-rw-  2.0 fat    11416 b- defN 23-Jul-31 12:56 pymef/mef_constants.py
--rw-rw-rw-  2.0 fat    68120 b- defN 23-Jul-31 12:56 pymef/mef_session.py
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-31 12:56 pymef/mef_file/__init__.py
--rw-rw-rw-  2.0 fat   196608 b- defN 23-Jul-31 12:59 pymef/mef_file/pymef3_file.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Jul-31 12:59 pymef-1.4.0.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      781 b- defN 23-Jul-31 12:59 pymef-1.4.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-31 12:59 pymef-1.4.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-Jul-31 12:59 pymef-1.4.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      793 b- defN 23-Jul-31 12:59 pymef-1.4.0.dist-info/RECORD
-10 files, 278953 bytes uncompressed, 99091 bytes compressed:  64.5%
+Zip file size: 100315 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat       35 b- defN 23-Aug-02 08:18 pymef/__init__.py
+-rw-rw-rw-  2.0 fat    11416 b- defN 23-Aug-02 08:18 pymef/mef_constants.py
+-rw-rw-rw-  2.0 fat    68120 b- defN 23-Aug-02 08:18 pymef/mef_session.py
+-rw-rw-rw-  2.0 fat        0 b- defN 23-Aug-02 08:18 pymef/mef_file/__init__.py
+-rw-rw-rw-  2.0 fat   196608 b- defN 23-Aug-02 08:20 pymef/mef_file/pymef3_file.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Aug-02 08:20 pymef-1.4.1.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      781 b- defN 23-Aug-02 08:20 pymef-1.4.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 23-Aug-02 08:20 pymef-1.4.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Aug-02 08:20 pymef-1.4.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      793 b- defN 23-Aug-02 08:20 pymef-1.4.1.dist-info/RECORD
+10 files, 278953 bytes uncompressed, 98967 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: pymef/mef_file/__init__.py
 Comment: 
 
 Filename: pymef/mef_file/pymef3_file.cp39-win_amd64.pyd
 Comment: 
 
-Filename: pymef-1.4.0.dist-info/LICENSE.txt
+Filename: pymef-1.4.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pymef-1.4.0.dist-info/METADATA
+Filename: pymef-1.4.1.dist-info/METADATA
 Comment: 
 
-Filename: pymef-1.4.0.dist-info/WHEEL
+Filename: pymef-1.4.1.dist-info/WHEEL
 Comment: 
 
-Filename: pymef-1.4.0.dist-info/top_level.txt
+Filename: pymef-1.4.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pymef-1.4.0.dist-info/RECORD
+Filename: pymef-1.4.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pymef-1.4.0.dist-info/LICENSE.txt` & `pymef-1.4.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pymef-1.4.0.dist-info/METADATA` & `pymef-1.4.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymef
-Version: 1.4.0
+Version: 1.4.1
 Summary: Wrapper for MEF (multiscale electrophysiology format)
 Home-page: https://github.com/msel-source/pymef
 Author: Jan Cimbalnik
 Author-email: jan.cimbalnik@fnusa.cz, jan.cimbalnik@mayo.edu
 License: Apache 2.0
 Keywords: MEF Mayo electrophysiology
 Platform: Linux
```

## Comparing `pymef-1.4.0.dist-info/RECORD` & `pymef-1.4.1.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pymef/__init__.py,sha256=1kbpvlJLskk6yXEzWWp_1GMkivt-reEwM9z57ohq87E,35
 pymef/mef_constants.py,sha256=lwecPdOx5sGP_9ueW5KDKT0lX0ds0FKhhpTxfZgmrTg,11416
 pymef/mef_session.py,sha256=l19E3CWqpbXO66fzWq8ppf5kFZBiq01F-jAdtXqXxE4,68120
 pymef/mef_file/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pymef/mef_file/pymef3_file.cp39-win_amd64.pyd,sha256=g1PUBu7TywgbQB6UaRp1RatHk5KbFD1fQksbbu5pnRM,196608
-pymef-1.4.0.dist-info/LICENSE.txt,sha256=MNaQiBd4P07-eYH_tzjMXycxKMeVO5u6i7Af6rjwYlk,1094
-pymef-1.4.0.dist-info/METADATA,sha256=5sK-E0aagSQWBuhF3n9F-0hWw3w96s_gmbH7nvoTHSo,781
-pymef-1.4.0.dist-info/WHEEL,sha256=NZXutxp9x3iJrMA3rHv3QSs0Fcg3h-CxsoGzMpYH3vg,100
-pymef-1.4.0.dist-info/top_level.txt,sha256=tdTwUbmCnT-Ua1bHfuMrg0l_wJ76REhL5ffyVx04gHg,6
-pymef-1.4.0.dist-info/RECORD,,
+pymef/mef_file/pymef3_file.cp39-win_amd64.pyd,sha256=0RjvUCehk8SUV0MWJxWu5cMZHdrAJMWex6saefASOzg,196608
+pymef-1.4.1.dist-info/LICENSE.txt,sha256=MNaQiBd4P07-eYH_tzjMXycxKMeVO5u6i7Af6rjwYlk,1094
+pymef-1.4.1.dist-info/METADATA,sha256=nmRUrZ8XLxtyNdeYa7fvj5PHCN-pG6_Nh9tQ0GrBMco,781
+pymef-1.4.1.dist-info/WHEEL,sha256=NZXutxp9x3iJrMA3rHv3QSs0Fcg3h-CxsoGzMpYH3vg,100
+pymef-1.4.1.dist-info/top_level.txt,sha256=tdTwUbmCnT-Ua1bHfuMrg0l_wJ76REhL5ffyVx04gHg,6
+pymef-1.4.1.dist-info/RECORD,,
```

