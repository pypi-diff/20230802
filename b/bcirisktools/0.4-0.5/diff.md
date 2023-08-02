# Comparing `tmp/bcirisktools-0.4.tar.gz` & `tmp/bcirisktools-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcirisktools-0.4.tar", last modified: Wed Aug  2 19:04:32 2023, max compression
+gzip compressed data, was "bcirisktools-0.5.tar", last modified: Wed Aug  2 19:15:30 2023, max compression
```

## Comparing `bcirisktools-0.4.tar` & `bcirisktools-0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:04:32.457000 bcirisktools-0.4/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.4/LICENCE
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-08-02 19:04:32.450000 bcirisktools-0.4/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.4/README.md
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:04:32.339000 bcirisktools-0.4/bcirisktools/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      308 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/__init__.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/input_filters.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/metrics_bci.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/modeling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    16808 2023-08-02 19:01:12.000000 bcirisktools-0.4/bcirisktools/profiling.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/shapley_report.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/stability.py
--rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.4/bcirisktools/tree_crt.py
-drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:04:32.430000 bcirisktools-0.4/bcirisktools.egg-info/
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/PKG-INFO
--rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/SOURCES.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/dependency_links.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/requires.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-02 19:04:31.000000 bcirisktools-0.4/bcirisktools.egg-info/top_level.txt
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.4/pyproject.toml
--rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-02 19:04:32.464000 bcirisktools-0.4/setup.cfg
--rw-r--r--   0 sagemaker-user  (1000) users      (100)     1016 2023-08-02 19:04:18.000000 bcirisktools-0.4/setup.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:15:30.033000 bcirisktools-0.5/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1063 2023-07-27 13:56:43.000000 bcirisktools-0.5/LICENCE
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-08-02 19:15:30.026000 bcirisktools-0.5/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     4265 2023-07-27 13:56:43.000000 bcirisktools-0.5/README.md
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:15:29.902000 bcirisktools-0.5/bcirisktools/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      385 2023-08-02 19:08:07.000000 bcirisktools-0.5/bcirisktools/__init__.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     3382 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/input_filters.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1480 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/metrics_bci.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     7528 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/modeling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    16808 2023-08-02 19:01:12.000000 bcirisktools-0.5/bcirisktools/profiling.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     9991 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/shapley_report.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     5705 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/stability.py
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)    18972 2023-07-27 13:56:43.000000 bcirisktools-0.5/bcirisktools/tree_crt.py
+drwxr-xr-x   0 sagemaker-user  (1000) users      (100)        0 2023-08-02 19:15:30.000000 bcirisktools-0.5/bcirisktools.egg-info/
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      571 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/PKG-INFO
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)      436 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/SOURCES.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)        1 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/dependency_links.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       78 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/requires.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       13 2023-08-02 19:15:29.000000 bcirisktools-0.5/bcirisktools.egg-info/top_level.txt
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       62 2023-07-27 13:56:43.000000 bcirisktools-0.5/pyproject.toml
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)       38 2023-08-02 19:15:30.036000 bcirisktools-0.5/setup.cfg
+-rw-r--r--   0 sagemaker-user  (1000) users      (100)     1016 2023-08-02 19:15:11.000000 bcirisktools-0.5/setup.py
```

### Comparing `bcirisktools-0.4/LICENCE` & `bcirisktools-0.5/LICENCE`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/PKG-INFO` & `bcirisktools-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.4
+Version: 0.5
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.4/README.md` & `bcirisktools-0.5/README.md`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/bcirisktools/input_filters.py` & `bcirisktools-0.5/bcirisktools/input_filters.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/bcirisktools/metrics_bci.py` & `bcirisktools-0.5/bcirisktools/metrics_bci.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/bcirisktools/modeling.py` & `bcirisktools-0.5/bcirisktools/modeling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/bcirisktools/profiling.py` & `bcirisktools-0.5/bcirisktools/profiling.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/bcirisktools/shapley_report.py` & `bcirisktools-0.5/bcirisktools/shapley_report.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/bcirisktools/stability.py` & `bcirisktools-0.5/bcirisktools/stability.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/bcirisktools/tree_crt.py` & `bcirisktools-0.5/bcirisktools/tree_crt.py`

 * *Files identical despite different names*

### Comparing `bcirisktools-0.4/bcirisktools.egg-info/PKG-INFO` & `bcirisktools-0.5/bcirisktools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcirisktools
-Version: 0.4
+Version: 0.5
 Summary: BCI risks tools
 Author: Mezosky
 Author-email: <imezadelajara@gmail.com>
 Keywords: python,risk,tools,bci
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bcirisktools-0.4/setup.py` & `bcirisktools-0.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import find_packages, setup
 
-VERSION = "0.4"
+VERSION = "0.5"
 DESCRIPTION = "BCI risks tools"
 LONG_DESCRIPTION = "A package that compiles different risk tools used by BCI bank."
 
 # Setting up
 setup(
     name="bcirisktools",
     version=VERSION,
```

