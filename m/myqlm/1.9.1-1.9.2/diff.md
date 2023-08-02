# Comparing `tmp/myqlm-1.9.1-py3-none-any.whl.zip` & `tmp/myqlm-1.9.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2032 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2589 b- defN 23-Jul-31 23:26 myqlm-1.9.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-31 23:26 myqlm-1.9.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jul-31 23:26 myqlm-1.9.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      289 b- defN 23-Jul-31 23:26 myqlm-1.9.1.dist-info/RECORD
-4 files, 2971 bytes uncompressed, 1466 bytes compressed:  50.7%
+Zip file size: 2033 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2589 b- defN 23-Aug-01 23:09 myqlm-1.9.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-01 23:09 myqlm-1.9.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Aug-01 23:09 myqlm-1.9.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      289 b- defN 23-Aug-01 23:09 myqlm-1.9.2.dist-info/RECORD
+4 files, 2971 bytes uncompressed, 1467 bytes compressed:  50.6%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: myqlm-1.9.1.dist-info/METADATA
+Filename: myqlm-1.9.2.dist-info/METADATA
 Comment: 
 
-Filename: myqlm-1.9.1.dist-info/WHEEL
+Filename: myqlm-1.9.2.dist-info/WHEEL
 Comment: 
 
-Filename: myqlm-1.9.1.dist-info/top_level.txt
+Filename: myqlm-1.9.2.dist-info/top_level.txt
 Comment: 
 
-Filename: myqlm-1.9.1.dist-info/RECORD
+Filename: myqlm-1.9.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `myqlm-1.9.1.dist-info/METADATA` & `myqlm-1.9.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myqlm
-Version: 1.9.1
+Version: 1.9.2
 Summary: myQLM package
 Home-page: https://atos.net/en/lp/myqlm
 Author: Atos Quantum Lab
 Author-email: myqlm@atos.net
 License: Atos myQLM EULA
 Project-URL: Documentation, https://myqlm.github.io
 Project-URL: Bug Tracker, https://github.com/myQLM/myqlm-issues/issues
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: qat-comm (==1.4.3)
 Requires-Dist: qat-core (==1.8.0)
 Requires-Dist: qat-lang (==3.0.0)
 Requires-Dist: qat-devices (==0.2.1)
-Requires-Dist: qat-variational (==1.4.0)
+Requires-Dist: qat-variational (==1.4.1)
 Requires-Dist: qlmaas (==1.9.1)
 Requires-Dist: myqlm-clinalg (==0.1.0)
 Requires-Dist: myqlm-contrib (==1.9.1)
 Requires-Dist: myqlm-fermion (==1.1.0)
 Requires-Dist: myqlm-simulators (==1.9.1)
 
 # Module myQLM
```

