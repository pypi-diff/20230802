# Comparing `tmp/syscolouringsaddV2-1.0.0.tar.gz` & `tmp/syscolouringsaddV2-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syscolouringsaddV2-1.0.0.tar", last modified: Tue Aug  1 23:14:59 2023, max compression
+gzip compressed data, was "syscolouringsaddV2-1.1.0.tar", last modified: Tue Aug  1 23:17:04 2023, max compression
```

## Comparing `syscolouringsaddV2-1.0.0.tar` & `syscolouringsaddV2-1.1.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 23:14:59.056645 syscolouringsaddV2-1.0.0/
--rw-r--r--   0 root         (0) root         (0)      351 2023-08-01 23:14:59.056645 syscolouringsaddV2-1.0.0/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 23:14:59.056645 syscolouringsaddV2-1.0.0/pipcolortoolsV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 syscolouringsaddV2-1.0.0/pipcolortoolsV2/__init__.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 23:14:59.056645 syscolouringsaddV2-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      564 2023-08-01 23:14:58.000000 syscolouringsaddV2-1.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 23:14:59.056645 syscolouringsaddV2-1.0.0/syscolouringsaddV2/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-01 23:14:58.000000 syscolouringsaddV2-1.0.0/syscolouringsaddV2/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 23:14:59.056645 syscolouringsaddV2-1.0.0/syscolouringsaddV2.egg-info/
--rw-r--r--   0 root         (0) root         (0)      351 2023-08-01 23:14:58.000000 syscolouringsaddV2-1.0.0/syscolouringsaddV2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      235 2023-08-01 23:14:59.000000 syscolouringsaddV2-1.0.0/syscolouringsaddV2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 23:14:58.000000 syscolouringsaddV2-1.0.0/syscolouringsaddV2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-08-01 23:14:58.000000 syscolouringsaddV2-1.0.0/syscolouringsaddV2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 23:17:04.854283 syscolouringsaddV2-1.1.0/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-08-01 23:17:04.854283 syscolouringsaddV2-1.1.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 23:17:04.854283 syscolouringsaddV2-1.1.0/pipcolortoolsV2/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-24 21:14:28.000000 syscolouringsaddV2-1.1.0/pipcolortoolsV2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 23:17:04.854283 syscolouringsaddV2-1.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      564 2023-08-01 23:17:04.000000 syscolouringsaddV2-1.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 23:17:04.854283 syscolouringsaddV2-1.1.0/syscolouringsaddV2/
+-rw-r--r--   0 root         (0) root         (0)    96773 2023-08-01 23:17:04.000000 syscolouringsaddV2-1.1.0/syscolouringsaddV2/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 23:17:04.854283 syscolouringsaddV2-1.1.0/syscolouringsaddV2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      351 2023-08-01 23:17:04.000000 syscolouringsaddV2-1.1.0/syscolouringsaddV2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      235 2023-08-01 23:17:04.000000 syscolouringsaddV2-1.1.0/syscolouringsaddV2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 23:17:04.000000 syscolouringsaddV2-1.1.0/syscolouringsaddV2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-08-01 23:17:04.000000 syscolouringsaddV2-1.1.0/syscolouringsaddV2.egg-info/top_level.txt
```

### Comparing `syscolouringsaddV2-1.0.0/setup.py` & `syscolouringsaddV2-1.1.0/setup.py`

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
     name="syscolouringsaddV2",
     version=VERSION,
```

