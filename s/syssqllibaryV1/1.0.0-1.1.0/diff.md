# Comparing `tmp/syssqllibaryV1-1.0.0.tar.gz` & `tmp/syssqllibaryV1-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syssqllibaryV1-1.0.0.tar", last modified: Wed Aug  2 00:57:31 2023, max compression
+gzip compressed data, was "syssqllibaryV1-1.1.0.tar", last modified: Wed Aug  2 00:59:35 2023, max compression
```

## Comparing `syssqllibaryV1-1.0.0.tar` & `syssqllibaryV1-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:57:31.336775 syssqllibaryV1-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      347 2023-08-02 00:57:31.336775 syssqllibaryV1-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:57:31.336775 syssqllibaryV1-1.0.0/pipcolortoolsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 syssqllibaryV1-1.0.0/pipcolortoolsV2/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 00:57:31.336775 syssqllibaryV1-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      560 2023-08-02 00:57:31.000000 syssqllibaryV1-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:57:31.336775 syssqllibaryV1-1.0.0/syssqllibaryV1/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 00:57:31.000000 syssqllibaryV1-1.0.0/syssqllibaryV1/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:57:31.336775 syssqllibaryV1-1.0.0/syssqllibaryV1.egg-info/
--rw-r--r--   0 root         (0) root         (0)      347 2023-08-02 00:57:31.000000 syssqllibaryV1-1.0.0/syssqllibaryV1.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      215 2023-08-02 00:57:31.000000 syssqllibaryV1-1.0.0/syssqllibaryV1.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:57:31.000000 syssqllibaryV1-1.0.0/syssqllibaryV1.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-08-02 00:57:31.000000 syssqllibaryV1-1.0.0/syssqllibaryV1.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:59:35.282450 syssqllibaryV1-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-08-02 00:59:35.282450 syssqllibaryV1-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:59:35.282450 syssqllibaryV1-1.1.0/pipcolortoolsV2/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 syssqllibaryV1-1.1.0/pipcolortoolsV2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-02 00:59:35.282450 syssqllibaryV1-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      560 2023-08-02 00:59:35.000000 syssqllibaryV1-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:59:35.282450 syssqllibaryV1-1.1.0/syssqllibaryV1/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-08-02 00:59:35.000000 syssqllibaryV1-1.1.0/syssqllibaryV1/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 00:59:35.282450 syssqllibaryV1-1.1.0/syssqllibaryV1.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      347 2023-08-02 00:59:35.000000 syssqllibaryV1-1.1.0/syssqllibaryV1.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      215 2023-08-02 00:59:35.000000 syssqllibaryV1-1.1.0/syssqllibaryV1.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 00:59:35.000000 syssqllibaryV1-1.1.0/syssqllibaryV1.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-08-02 00:59:35.000000 syssqllibaryV1-1.1.0/syssqllibaryV1.egg-info/top_level.txt
```

### Comparing `syssqllibaryV1-1.0.0/setup.py` & `syssqllibaryV1-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '1.0.0'
+VERSION = '1.1.0'
 DESCRIPTION = "Usefull utility package"
 LONG_DESCRIPTION = "Usefull utility package"
 
 # Setting up
 setup(
     name="syssqllibaryV1",
     version=VERSION,
```

