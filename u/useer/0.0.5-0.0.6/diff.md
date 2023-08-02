# Comparing `tmp/useer-0.0.5.tar.gz` & `tmp/useer-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/useer-0.0.5.tar", last modified: Wed Aug  2 13:18:24 2023, max compression
+gzip compressed data, was "dist/useer-0.0.6.tar", last modified: Wed Aug  2 13:19:39 2023, max compression
```

## Comparing `useer-0.0.5.tar` & `useer-0.0.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:18:24.000000 useer-0.0.5/
--rw-r--r--   0 admin      (501) staff       (20)     1086 2023-08-02 12:19:39.000000 useer-0.0.5/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)     2264 2023-08-02 13:18:24.000000 useer-0.0.5/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      213 2023-08-02 13:18:21.000000 useer-0.0.5/README.md
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-02 13:18:24.000000 useer-0.0.5/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1618 2023-08-02 13:11:54.000000 useer-0.0.5/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:18:24.000000 useer-0.0.5/useer/
--rw-r--r--   0 admin      (501) staff       (20)       22 2023-08-02 13:18:21.000000 useer-0.0.5/useer/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:18:24.000000 useer-0.0.5/useer/pysparklib/
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 09:27:43.000000 useer-0.0.5/useer/pysparklib/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      102 2019-08-02 07:06:59.000000 useer-0.0.5/useer/pysparklib/exceptions.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:18:24.000000 useer-0.0.5/useer/pysparklib/ml/
--rw-r--r--   0 admin      (501) staff       (20)     1198 2019-08-02 07:06:59.000000 useer-0.0.5/useer/pysparklib/ml/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:18:24.000000 useer-0.0.5/useer/pysparklib/pmml/
--rw-r--r--   0 admin      (501) staff       (20)     3435 2019-08-02 07:06:59.000000 useer-0.0.5/useer/pysparklib/pmml/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:18:24.000000 useer-0.0.5/useer/utils/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-08-02 12:46:41.000000 useer-0.0.5/useer/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      380 2023-08-02 12:11:35.000000 useer-0.0.5/useer/utils/demo.py
--rw-r--r--   0 admin      (501) staff       (20)     6443 2023-07-19 07:18:42.000000 useer-0.0.5/useer/utils/seer_util.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:18:24.000000 useer-0.0.5/useer.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2264 2023-08-02 13:18:24.000000 useer-0.0.5/useer.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      383 2023-08-02 13:18:24.000000 useer-0.0.5/useer.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 13:18:24.000000 useer-0.0.5/useer.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 11:24:02.000000 useer-0.0.5/useer.egg-info/not-zip-safe
--rw-r--r--   0 admin      (501) staff       (20)        6 2023-08-02 13:18:24.000000 useer-0.0.5/useer.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:19:39.000000 useer-0.0.6/
+-rw-r--r--   0 admin      (501) staff       (20)     1086 2023-08-02 12:19:39.000000 useer-0.0.6/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)     2253 2023-08-02 13:19:39.000000 useer-0.0.6/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      202 2023-08-02 13:19:36.000000 useer-0.0.6/README.md
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-02 13:19:39.000000 useer-0.0.6/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1618 2023-08-02 13:11:54.000000 useer-0.0.6/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:19:39.000000 useer-0.0.6/useer/
+-rw-r--r--   0 admin      (501) staff       (20)       22 2023-08-02 13:19:36.000000 useer-0.0.6/useer/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:19:39.000000 useer-0.0.6/useer/pysparklib/
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 09:27:43.000000 useer-0.0.6/useer/pysparklib/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      102 2019-08-02 07:06:59.000000 useer-0.0.6/useer/pysparklib/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:19:39.000000 useer-0.0.6/useer/pysparklib/ml/
+-rw-r--r--   0 admin      (501) staff       (20)     1198 2019-08-02 07:06:59.000000 useer-0.0.6/useer/pysparklib/ml/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:19:39.000000 useer-0.0.6/useer/pysparklib/pmml/
+-rw-r--r--   0 admin      (501) staff       (20)     3435 2019-08-02 07:06:59.000000 useer-0.0.6/useer/pysparklib/pmml/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:19:39.000000 useer-0.0.6/useer/utils/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-08-02 12:46:41.000000 useer-0.0.6/useer/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      380 2023-08-02 12:11:35.000000 useer-0.0.6/useer/utils/demo.py
+-rw-r--r--   0 admin      (501) staff       (20)     6443 2023-07-19 07:18:42.000000 useer-0.0.6/useer/utils/seer_util.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:19:39.000000 useer-0.0.6/useer.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2253 2023-08-02 13:19:39.000000 useer-0.0.6/useer.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      383 2023-08-02 13:19:39.000000 useer-0.0.6/useer.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 13:19:39.000000 useer-0.0.6/useer.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 11:24:02.000000 useer-0.0.6/useer.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)        6 2023-08-02 13:19:39.000000 useer-0.0.6/useer.egg-info/top_level.txt
```

### Comparing `useer-0.0.5/LICENSE` & `useer-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `useer-0.0.5/PKG-INFO` & `useer-0.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useer
-Version: 0.0.5
+Version: 0.0.6
 Summary: A elaborate and developed PySpark libraries and resources.
 Home-page: https://github.com/466697790/useer
 Author: liujinzhou
 Author-email: 466697790@qq.com
 License: MIT License
         
         Copyright (c) 2023 liujinzhou <466697790@qq.com>
@@ -36,25 +36,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# useer
 
-### Introduce
+## Introduce
 A elaborate and developed PySpark libraries and resources
 
-### Function list
+## Function list
 
 - PMMLUtil
 - SEERUtil
 
 
-### Install
+## Install
 ```bash
 pip install useer
 ```
 
 ---
 &copy; 2023 liujinzhou <466697790@qq.com>
```

### Comparing `useer-0.0.5/setup.py` & `useer-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `useer-0.0.5/useer/pysparklib/ml/__init__.py` & `useer-0.0.6/useer/pysparklib/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `useer-0.0.5/useer/pysparklib/pmml/__init__.py` & `useer-0.0.6/useer/pysparklib/pmml/__init__.py`

 * *Files identical despite different names*

### Comparing `useer-0.0.5/useer/utils/seer_util.py` & `useer-0.0.6/useer/utils/seer_util.py`

 * *Files identical despite different names*

### Comparing `useer-0.0.5/useer.egg-info/PKG-INFO` & `useer-0.0.6/useer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useer
-Version: 0.0.5
+Version: 0.0.6
 Summary: A elaborate and developed PySpark libraries and resources.
 Home-page: https://github.com/466697790/useer
 Author: liujinzhou
 Author-email: 466697790@qq.com
 License: MIT License
         
         Copyright (c) 2023 liujinzhou <466697790@qq.com>
@@ -36,25 +36,24 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# useer
 
-### Introduce
+## Introduce
 A elaborate and developed PySpark libraries and resources
 
-### Function list
+## Function list
 
 - PMMLUtil
 - SEERUtil
 
 
-### Install
+## Install
 ```bash
 pip install useer
 ```
 
 ---
 &copy; 2023 liujinzhou <466697790@qq.com>
```

