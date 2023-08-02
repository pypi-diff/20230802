# Comparing `tmp/useer-0.0.3.tar.gz` & `tmp/useer-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/useer-0.0.3.tar", last modified: Wed Aug  2 12:55:43 2023, max compression
+gzip compressed data, was "dist/useer-0.0.4.tar", last modified: Wed Aug  2 13:12:13 2023, max compression
```

## Comparing `useer-0.0.3.tar` & `useer-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 12:55:43.000000 useer-0.0.3/
--rw-r--r--   0 admin      (501) staff       (20)     1086 2023-08-02 12:19:39.000000 useer-0.0.3/LICENSE
--rw-r--r--   0 admin      (501) staff       (20)     2009 2023-08-02 12:55:43.000000 useer-0.0.3/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      209 2023-08-02 10:45:47.000000 useer-0.0.3/README.md
--rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-02 12:55:43.000000 useer-0.0.3/setup.cfg
--rw-r--r--   0 admin      (501) staff       (20)     1502 2023-08-02 12:17:26.000000 useer-0.0.3/setup.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 12:55:43.000000 useer-0.0.3/useer/
--rw-r--r--   0 admin      (501) staff       (20)       22 2023-08-02 12:37:44.000000 useer-0.0.3/useer/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 12:55:43.000000 useer-0.0.3/useer/pysparklib/
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 09:27:43.000000 useer-0.0.3/useer/pysparklib/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      102 2019-08-02 07:06:59.000000 useer-0.0.3/useer/pysparklib/exceptions.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 12:55:43.000000 useer-0.0.3/useer/pysparklib/ml/
--rw-r--r--   0 admin      (501) staff       (20)     1198 2019-08-02 07:06:59.000000 useer-0.0.3/useer/pysparklib/ml/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 12:55:43.000000 useer-0.0.3/useer/pysparklib/pmml/
--rw-r--r--   0 admin      (501) staff       (20)     3435 2019-08-02 07:06:59.000000 useer-0.0.3/useer/pysparklib/pmml/__init__.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 12:55:43.000000 useer-0.0.3/useer/utils/
--rw-r--r--   0 admin      (501) staff       (20)        0 2023-08-02 12:46:41.000000 useer-0.0.3/useer/utils/__init__.py
--rw-r--r--   0 admin      (501) staff       (20)      380 2023-08-02 12:11:35.000000 useer-0.0.3/useer/utils/demo.py
--rw-r--r--   0 admin      (501) staff       (20)     6443 2023-07-19 07:18:42.000000 useer-0.0.3/useer/utils/seer_util.py
-drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 12:55:43.000000 useer-0.0.3/useer.egg-info/
--rw-r--r--   0 admin      (501) staff       (20)     2009 2023-08-02 12:55:43.000000 useer-0.0.3/useer.egg-info/PKG-INFO
--rw-r--r--   0 admin      (501) staff       (20)      383 2023-08-02 12:55:43.000000 useer-0.0.3/useer.egg-info/SOURCES.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 12:55:43.000000 useer-0.0.3/useer.egg-info/dependency_links.txt
--rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 11:24:02.000000 useer-0.0.3/useer.egg-info/not-zip-safe
--rw-r--r--   0 admin      (501) staff       (20)        6 2023-08-02 12:55:43.000000 useer-0.0.3/useer.egg-info/top_level.txt
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:12:13.000000 useer-0.0.4/
+-rw-r--r--   0 admin      (501) staff       (20)     1086 2023-08-02 12:19:39.000000 useer-0.0.4/LICENSE
+-rw-r--r--   0 admin      (501) staff       (20)     2260 2023-08-02 13:12:13.000000 useer-0.0.4/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      209 2023-08-02 10:45:47.000000 useer-0.0.4/README.md
+-rw-r--r--   0 admin      (501) staff       (20)       38 2023-08-02 13:12:13.000000 useer-0.0.4/setup.cfg
+-rw-r--r--   0 admin      (501) staff       (20)     1618 2023-08-02 13:11:54.000000 useer-0.0.4/setup.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:12:13.000000 useer-0.0.4/useer/
+-rw-r--r--   0 admin      (501) staff       (20)       22 2023-08-02 13:05:02.000000 useer-0.0.4/useer/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:12:13.000000 useer-0.0.4/useer/pysparklib/
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 09:27:43.000000 useer-0.0.4/useer/pysparklib/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      102 2019-08-02 07:06:59.000000 useer-0.0.4/useer/pysparklib/exceptions.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:12:13.000000 useer-0.0.4/useer/pysparklib/ml/
+-rw-r--r--   0 admin      (501) staff       (20)     1198 2019-08-02 07:06:59.000000 useer-0.0.4/useer/pysparklib/ml/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:12:13.000000 useer-0.0.4/useer/pysparklib/pmml/
+-rw-r--r--   0 admin      (501) staff       (20)     3435 2019-08-02 07:06:59.000000 useer-0.0.4/useer/pysparklib/pmml/__init__.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:12:13.000000 useer-0.0.4/useer/utils/
+-rw-r--r--   0 admin      (501) staff       (20)        0 2023-08-02 12:46:41.000000 useer-0.0.4/useer/utils/__init__.py
+-rw-r--r--   0 admin      (501) staff       (20)      380 2023-08-02 12:11:35.000000 useer-0.0.4/useer/utils/demo.py
+-rw-r--r--   0 admin      (501) staff       (20)     6443 2023-07-19 07:18:42.000000 useer-0.0.4/useer/utils/seer_util.py
+drwxr-xr-x   0 admin      (501) staff       (20)        0 2023-08-02 13:12:13.000000 useer-0.0.4/useer.egg-info/
+-rw-r--r--   0 admin      (501) staff       (20)     2260 2023-08-02 13:12:13.000000 useer-0.0.4/useer.egg-info/PKG-INFO
+-rw-r--r--   0 admin      (501) staff       (20)      383 2023-08-02 13:12:13.000000 useer-0.0.4/useer.egg-info/SOURCES.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 13:12:13.000000 useer-0.0.4/useer.egg-info/dependency_links.txt
+-rw-r--r--   0 admin      (501) staff       (20)        1 2023-08-02 11:24:02.000000 useer-0.0.4/useer.egg-info/not-zip-safe
+-rw-r--r--   0 admin      (501) staff       (20)        6 2023-08-02 13:12:13.000000 useer-0.0.4/useer.egg-info/top_level.txt
```

### Comparing `useer-0.0.3/LICENSE` & `useer-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `useer-0.0.3/PKG-INFO` & `useer-0.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A elaborate and developed PySpark libraries and resources.
 Home-page: https://github.com/466697790/useer
 Author: liujinzhou
 Author-email: 466697790@qq.com
 License: MIT License
         
         Copyright (c) 2023 liujinzhou <466697790@qq.com>
@@ -33,8 +33,28 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# pysparklib
+
+### A elaborate and developed PySpark libraries and resources
+
+
+### Function list
+
+- PMMLUtil
+- SEERUtil
+
+
+### Install
+```bash
+pip install useer
+```
+
+---
+&copy; 2023 liujinzhou <466697790@qq.com>
```

### Comparing `useer-0.0.3/setup.py` & `useer-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,14 +16,16 @@
         but you're trying to install it on Python {CURRENT_PYTHON[0]}.{CURRENT_PYTHON[1]}.""")
     sys.exit(1)
 
 setup(
     name=name,
     version=version,
     description='A elaborate and developed PySpark libraries and resources.',
+    long_description=open('README.md', encoding='utf-8').read(),
+    long_description_content_type="text/markdown",
     author='liujinzhou',
     author_email='466697790@qq.com',
     url='https://github.com/466697790/useer',
     license=open('LICENSE', encoding='utf-8').read(),
     packages=find_packages(),
     include_package_data=True,
     install_requires=[],
```

### Comparing `useer-0.0.3/useer/pysparklib/ml/__init__.py` & `useer-0.0.4/useer/pysparklib/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `useer-0.0.3/useer/pysparklib/pmml/__init__.py` & `useer-0.0.4/useer/pysparklib/pmml/__init__.py`

 * *Files identical despite different names*

### Comparing `useer-0.0.3/useer/utils/seer_util.py` & `useer-0.0.4/useer/utils/seer_util.py`

 * *Files identical despite different names*

### Comparing `useer-0.0.3/useer.egg-info/PKG-INFO` & `useer-0.0.4/useer.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: useer
-Version: 0.0.3
+Version: 0.0.4
 Summary: A elaborate and developed PySpark libraries and resources.
 Home-page: https://github.com/466697790/useer
 Author: liujinzhou
 Author-email: 466697790@qq.com
 License: MIT License
         
         Copyright (c) 2023 liujinzhou <466697790@qq.com>
@@ -33,8 +33,28 @@
 Classifier: Natural Language :: Chinese (Simplified)
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
+Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# pysparklib
+
+### A elaborate and developed PySpark libraries and resources
+
+
+### Function list
+
+- PMMLUtil
+- SEERUtil
+
+
+### Install
+```bash
+pip install useer
+```
+
+---
+&copy; 2023 liujinzhou <466697790@qq.com>
```

