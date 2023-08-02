# Comparing `tmp/operatorio-0.2.1.tar.gz` & `tmp/operatorio-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "operatorio-0.2.1.tar", last modified: Wed Aug  2 15:30:41 2023, max compression
+gzip compressed data, was "operatorio-0.2.2.tar", last modified: Wed Aug  2 15:35:33 2023, max compression
```

## Comparing `operatorio-0.2.1.tar` & `operatorio-0.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:30:41.774871 operatorio-0.2.1/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:30:41.774638 operatorio-0.2.1/PKG-INFO
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:30:41.772803 operatorio-0.2.1/operatorio/
--rw-r--r--   0 david      (501) staff       (20)      125 2023-07-21 18:45:08.000000 operatorio-0.2.1/operatorio/__init__.py
--rw-r--r--   0 david      (501) staff       (20)     2635 2023-08-02 15:30:28.000000 operatorio-0.2.1/operatorio/main.py
-drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:30:41.774385 operatorio-0.2.1/operatorio.egg-info/
--rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/PKG-INFO
--rw-r--r--   0 david      (501) staff       (20)      219 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/SOURCES.txt
--rw-r--r--   0 david      (501) staff       (20)        1 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/dependency_links.txt
--rw-r--r--   0 david      (501) staff       (20)        9 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/requires.txt
--rw-r--r--   0 david      (501) staff       (20)       11 2023-08-02 15:30:41.000000 operatorio-0.2.1/operatorio.egg-info/top_level.txt
--rw-r--r--   0 david      (501) staff       (20)       38 2023-08-02 15:30:41.774936 operatorio-0.2.1/setup.cfg
--rw-r--r--   0 david      (501) staff       (20)      532 2023-08-02 15:30:33.000000 operatorio-0.2.1/setup.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:35:33.671547 operatorio-0.2.2/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:35:33.671327 operatorio-0.2.2/PKG-INFO
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:35:33.669687 operatorio-0.2.2/operatorio/
+-rw-r--r--   0 david      (501) staff       (20)      221 2023-08-02 15:35:00.000000 operatorio-0.2.2/operatorio/__init__.py
+-rw-r--r--   0 david      (501) staff       (20)     2635 2023-08-02 15:30:28.000000 operatorio-0.2.2/operatorio/main.py
+drwxr-xr-x   0 david      (501) staff       (20)        0 2023-08-02 15:35:33.670961 operatorio-0.2.2/operatorio.egg-info/
+-rw-r--r--   0 david      (501) staff       (20)      331 2023-08-02 15:35:33.000000 operatorio-0.2.2/operatorio.egg-info/PKG-INFO
+-rw-r--r--   0 david      (501) staff       (20)      219 2023-08-02 15:35:33.000000 operatorio-0.2.2/operatorio.egg-info/SOURCES.txt
+-rw-r--r--   0 david      (501) staff       (20)        1 2023-08-02 15:35:33.000000 operatorio-0.2.2/operatorio.egg-info/dependency_links.txt
+-rw-r--r--   0 david      (501) staff       (20)        9 2023-08-02 15:35:33.000000 operatorio-0.2.2/operatorio.egg-info/requires.txt
+-rw-r--r--   0 david      (501) staff       (20)       11 2023-08-02 15:35:33.000000 operatorio-0.2.2/operatorio.egg-info/top_level.txt
+-rw-r--r--   0 david      (501) staff       (20)       38 2023-08-02 15:35:33.671609 operatorio-0.2.2/setup.cfg
+-rw-r--r--   0 david      (501) staff       (20)      532 2023-08-02 15:35:31.000000 operatorio-0.2.2/setup.py
```

### Comparing `operatorio-0.2.1/operatorio/main.py` & `operatorio-0.2.2/operatorio/main.py`

 * *Files identical despite different names*

### Comparing `operatorio-0.2.1/setup.py` & `operatorio-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="operatorio",
-    version="0.2.1",
+    version="0.2.2",
     description="A Python SDK for the Operator Search API.",
     author="David Shi",
     author_email="david@operator.io",
     url="https://github.com/operatorlabs/sdk/python",
     packages=['operatorio'],  
     install_requires=[
         'requests',
```

