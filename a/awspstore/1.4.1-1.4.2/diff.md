# Comparing `tmp/awspstore-1.4.1.tar.gz` & `tmp/awspstore-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awspstore-1.4.1.tar", last modified: Tue Aug  1 10:54:00 2023, max compression
+gzip compressed data, was "awspstore-1.4.2.tar", last modified: Wed Aug  2 04:44:04 2023, max compression
```

## Comparing `awspstore-1.4.1.tar` & `awspstore-1.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:54:00.065133 awspstore-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-01 10:53:39.000000 awspstore-1.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 10:54:00.065133 awspstore-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-01 10:53:39.000000 awspstore-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:54:00.065133 awspstore-1.4.1/awspstore/
--rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-08-01 10:53:39.000000 awspstore-1.4.1/awspstore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:54:00.065133 awspstore-1.4.1/awspstore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-01 10:54:00.000000 awspstore-1.4.1/awspstore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-01 10:54:00.000000 awspstore-1.4.1/awspstore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 10:54:00.000000 awspstore-1.4.1/awspstore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-01 10:54:00.000000 awspstore-1.4.1/awspstore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-01 10:54:00.000000 awspstore-1.4.1/awspstore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 10:54:00.065133 awspstore-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-01 10:53:39.000000 awspstore-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 10:54:00.065133 awspstore-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-01 10:53:39.000000 awspstore-1.4.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:44:04.410004 awspstore-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-08-02 04:43:52.000000 awspstore-1.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-02 04:44:04.410004 awspstore-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-02 04:43:52.000000 awspstore-1.4.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:44:04.406003 awspstore-1.4.2/awspstore/
+-rw-r--r--   0 runner    (1001) docker     (123)     3706 2023-08-02 04:43:52.000000 awspstore-1.4.2/awspstore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:44:04.406003 awspstore-1.4.2/awspstore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-08-02 04:44:04.000000 awspstore-1.4.2/awspstore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-08-02 04:44:04.000000 awspstore-1.4.2/awspstore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 04:44:04.000000 awspstore-1.4.2/awspstore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 04:44:04.000000 awspstore-1.4.2/awspstore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-02 04:44:04.000000 awspstore-1.4.2/awspstore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 04:44:04.410004 awspstore-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-08-02 04:43:52.000000 awspstore-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 04:44:04.410004 awspstore-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-08-02 04:43:52.000000 awspstore-1.4.2/tests/test_utils.py
```

### Comparing `awspstore-1.4.1/LICENSE` & `awspstore-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `awspstore-1.4.1/PKG-INFO` & `awspstore-1.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awspstore
-Version: 1.4.1
+Version: 1.4.2
 Summary: Vault for your software project using AWS Parameter Store
 Home-page: https://github.com/eldad1221/aws-vault
 Author: Eldad Bishari
 Author-email: eldad@1221tlv.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `awspstore-1.4.1/README.md` & `awspstore-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `awspstore-1.4.1/awspstore/__init__.py` & `awspstore-1.4.2/awspstore/__init__.py`

 * *Files identical despite different names*

### Comparing `awspstore-1.4.1/awspstore.egg-info/PKG-INFO` & `awspstore-1.4.2/awspstore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: awspstore
-Version: 1.4.1
+Version: 1.4.2
 Summary: Vault for your software project using AWS Parameter Store
 Home-page: https://github.com/eldad1221/aws-vault
 Author: Eldad Bishari
 Author-email: eldad@1221tlv.org
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `awspstore-1.4.1/setup.py` & `awspstore-1.4.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="awspstore",
-    version="1.4.1",
+    version="1.4.2",
     author="Eldad Bishari",
     author_email="eldad@1221tlv.org",
     description="Vault for your software project using AWS Parameter Store",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/eldad1221/aws-vault",
     packages=setuptools.find_packages(),
     install_requires=[
-        'boto3==1.26.3',
-        'quickbelog~=1.1.0',
+        'boto3>=1.26.3',
+        'quickbelog>=1.1.0',
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.7',
```

### Comparing `awspstore-1.4.1/tests/test_utils.py` & `awspstore-1.4.2/tests/test_utils.py`

 * *Files identical despite different names*

