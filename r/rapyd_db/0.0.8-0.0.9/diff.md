# Comparing `tmp/rapyd_db-0.0.8.tar.gz` & `tmp/rapyd_db-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/rapyd_db-0.0.8.tar", last modified: Fri Jan 15 18:00:06 2021, max compression
+gzip compressed data, was "dist/rapyd_db-0.0.9.tar", last modified: Tue Aug  1 22:21:50 2023, max compression
```

## Comparing `rapyd_db-0.0.8.tar` & `rapyd_db-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 karthicr (809502784) karthicr (809502784)        0 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)    11348 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/LICENSE
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)    16009 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/PKG-INFO
-drwxrwxr-x   0 karthicr (809502784) karthicr (809502784)        0 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db/
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)      454 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/rapyd_db/utils.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)       79 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/rapyd_db/__init__.py
-drwxrwxr-x   0 karthicr (809502784) karthicr (809502784)        0 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db/backends/
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)     7101 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/rapyd_db/backends/mongo.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)     5707 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/rapyd_db/backends/mssql.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)      967 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/rapyd_db/backends/__init__.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)     5107 2021-01-15 17:55:46.000000 rapyd_db-0.0.8/rapyd_db/backends/mysql.py
-drwxrwxr-x   0 karthicr (809502784) karthicr (809502784)        0 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db/tests/
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)     2948 2021-01-15 17:55:46.000000 rapyd_db-0.0.8/rapyd_db/tests/test_mssql.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)     2074 2021-01-15 17:55:46.000000 rapyd_db-0.0.8/rapyd_db/tests/test_mongo.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)        0 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/rapyd_db/tests/__init__.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)     3033 2021-01-15 17:55:46.000000 rapyd_db-0.0.8/rapyd_db/tests/test_mysql.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)      497 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/rapyd_db/loggingadapter.py
-drwxrwxr-x   0 karthicr (809502784) karthicr (809502784)        0 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db.egg-info/
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)      489 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db.egg-info/SOURCES.txt
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)    16009 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db.egg-info/PKG-INFO
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)        1 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db.egg-info/dependency_links.txt
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)        9 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db.egg-info/top_level.txt
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)       66 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/rapyd_db.egg-info/requires.txt
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)     3092 2021-01-15 17:55:46.000000 rapyd_db-0.0.8/README.rst
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)     1128 2021-01-15 17:55:46.000000 rapyd_db-0.0.8/setup.py
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)       38 2021-01-15 18:00:06.000000 rapyd_db-0.0.8/setup.cfg
--rw-rw-r--   0 karthicr (809502784) karthicr (809502784)       35 2021-01-15 17:05:15.000000 rapyd_db-0.0.8/MANIFEST.in
+drwxr-xr-x   0 karthicr (809502784) staff       (20)        0 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/
+drwxr-xr-x   0 karthicr (809502784) staff       (20)        0 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db.egg-info/
+-rw-r--r--   0 karthicr (809502784) staff       (20)    16009 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db.egg-info/PKG-INFO
+-rw-r--r--   0 karthicr (809502784) staff       (20)      489 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db.egg-info/SOURCES.txt
+-rw-r--r--   0 karthicr (809502784) staff       (20)       66 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db.egg-info/requires.txt
+-rw-r--r--   0 karthicr (809502784) staff       (20)        9 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db.egg-info/top_level.txt
+-rw-r--r--   0 karthicr (809502784) staff       (20)        1 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db.egg-info/dependency_links.txt
+-rw-r--r--   0 karthicr (809502784) staff       (20)    16009 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/PKG-INFO
+-rw-r--r--   0 karthicr (809502784) staff       (20)    11348 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/LICENSE
+-rw-r--r--   0 karthicr (809502784) staff       (20)       35 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/MANIFEST.in
+-rw-r--r--   0 karthicr (809502784) staff       (20)     1128 2023-08-01 22:12:04.000000 rapyd_db-0.0.9/setup.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)       38 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/setup.cfg
+drwxr-xr-x   0 karthicr (809502784) staff       (20)        0 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db/
+drwxr-xr-x   0 karthicr (809502784) staff       (20)        0 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db/backends/
+-rw-r--r--   0 karthicr (809502784) staff       (20)     5707 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/backends/mssql.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)     7107 2023-08-01 22:12:04.000000 rapyd_db-0.0.9/rapyd_db/backends/mongo.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)      967 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/backends/__init__.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)     5107 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/backends/mysql.py
+drwxr-xr-x   0 karthicr (809502784) staff       (20)        0 2023-08-01 22:21:50.000000 rapyd_db-0.0.9/rapyd_db/tests/
+-rw-r--r--   0 karthicr (809502784) staff       (20)        0 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/tests/__init__.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)     3033 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/tests/test_mysql.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)     2948 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/tests/test_mssql.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)     2074 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/tests/test_mongo.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)       79 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/__init__.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)      454 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/utils.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)      497 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/rapyd_db/loggingadapter.py
+-rw-r--r--   0 karthicr (809502784) staff       (20)     3092 2023-08-01 22:06:20.000000 rapyd_db-0.0.9/README.rst
```

### Comparing `rapyd_db-0.0.8/LICENSE` & `rapyd_db-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rapyd_db-0.0.8/PKG-INFO` & `rapyd_db-0.0.9/rapyd_db.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapyd_db
-Version: 0.0.8
+Name: rapyd-db
+Version: 0.0.9
 Summary: An opinionated lightweight wrapper around various DB backend drivers.
 Home-page: https://github.com/karthicraghupathi/rapyd_db
 Author: Karthic Raghupathi
 Author-email: karthicr@gmail.com
 License:                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
@@ -326,10 +326,10 @@
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Provides-Extra: mssql
 Provides-Extra: mongo
+Provides-Extra: mssql
 Provides-Extra: mysql
```

### Comparing `rapyd_db-0.0.8/rapyd_db/backends/mongo.py` & `rapyd_db-0.0.9/rapyd_db/backends/mongo.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,8 +160,8 @@
             execution_end = datetime.now()
             adapter.info(
                 "Executed in {} second(s)".format(
                     (execution_end - execution_start).seconds
                 )
             )
             adapter.info("Ended {} execution at {}".format(operation, execution_end))
-            return result
+            return list(result)
```

### Comparing `rapyd_db-0.0.8/rapyd_db/backends/mssql.py` & `rapyd_db-0.0.9/rapyd_db/backends/mssql.py`

 * *Files identical despite different names*

### Comparing `rapyd_db-0.0.8/rapyd_db/backends/__init__.py` & `rapyd_db-0.0.9/rapyd_db/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyd_db-0.0.8/rapyd_db/backends/mysql.py` & `rapyd_db-0.0.9/rapyd_db/backends/mysql.py`

 * *Files identical despite different names*

### Comparing `rapyd_db-0.0.8/rapyd_db/tests/test_mssql.py` & `rapyd_db-0.0.9/rapyd_db/tests/test_mssql.py`

 * *Files identical despite different names*

### Comparing `rapyd_db-0.0.8/rapyd_db/tests/test_mongo.py` & `rapyd_db-0.0.9/rapyd_db/tests/test_mongo.py`

 * *Files identical despite different names*

### Comparing `rapyd_db-0.0.8/rapyd_db/tests/test_mysql.py` & `rapyd_db-0.0.9/rapyd_db/tests/test_mysql.py`

 * *Files identical despite different names*

### Comparing `rapyd_db-0.0.8/rapyd_db.egg-info/PKG-INFO` & `rapyd_db-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: rapyd-db
-Version: 0.0.8
+Name: rapyd_db
+Version: 0.0.9
 Summary: An opinionated lightweight wrapper around various DB backend drivers.
 Home-page: https://github.com/karthicraghupathi/rapyd_db
 Author: Karthic Raghupathi
 Author-email: karthicr@gmail.com
 License:                                  Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
@@ -326,10 +326,10 @@
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
-Provides-Extra: mssql
 Provides-Extra: mongo
+Provides-Extra: mssql
 Provides-Extra: mysql
```

### Comparing `rapyd_db-0.0.8/README.rst` & `rapyd_db-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `rapyd_db-0.0.8/setup.py` & `rapyd_db-0.0.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     readme = f.read()
 
 with open("LICENSE") as f:
     license = f.read()
 
 setup(
     name="rapyd_db",
-    version="0.0.8",
+    version="0.0.9",
     description="An opinionated lightweight wrapper around various DB backend drivers.",
     long_description=readme,
     author="Karthic Raghupathi",
     author_email="karthicr@gmail.com",
     url="https://github.com/karthicraghupathi/rapyd_db",
     license=license,
     packages=find_packages(exclude=("tests", "docs")),
```

