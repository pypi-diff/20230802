# Comparing `tmp/alibabacloud_arms20190808-2.0.2.tar.gz` & `tmp/alibabacloud_arms20190808-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_arms20190808-2.0.2.tar", last modified: Tue Aug  1 02:15:34 2023, max compression
+gzip compressed data, was "dist/alibabacloud_arms20190808-2.0.3.tar", last modified: Wed Aug  2 03:51:18 2023, max compression
```

## Comparing `alibabacloud_arms20190808-2.0.2.tar` & `alibabacloud_arms20190808-2.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/
--rw-r--r--   0 root         (0) root         (0)      371 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2370 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1025 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1110 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808/
--rw-r--r--   0 root         (0) root         (0)       21 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808/__init__.py
--rw-r--r--   0 root         (0) root         (0)   600601 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808/client.py
--rw-r--r--   0 root         (0) root         (0)  1428058 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2370 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      428 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      157 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       26 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2023-08-01 02:15:34.000000 alibabacloud_arms20190808-2.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2652 2023-08-01 02:15:33.000000 alibabacloud_arms20190808-2.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/
+-rw-r--r--   0 root         (0) root         (0)      412 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1110 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   600601 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808/client.py
+-rw-r--r--   0 root         (0) root         (0)  1428058 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2370 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      428 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       26 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 03:51:18.000000 alibabacloud_arms20190808-2.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2652 2023-08-02 03:51:17.000000 alibabacloud_arms20190808-2.0.3/setup.py
```

### Comparing `alibabacloud_arms20190808-2.0.2/LICENSE` & `alibabacloud_arms20190808-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_arms20190808-2.0.2/PKG-INFO` & `alibabacloud_arms20190808-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_arms20190808
-Version: 2.0.2
+Version: 2.0.3
 Summary: Alibaba Cloud Application Real-Time Monitoring Service (20190808) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_arms20190808-2.0.2/README-CN.md` & `alibabacloud_arms20190808-2.0.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_arms20190808-2.0.2/README.md` & `alibabacloud_arms20190808-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808/client.py` & `alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808/client.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808/models.py` & `alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808/models.py`

 * *Files identical despite different names*

### Comparing `alibabacloud_arms20190808-2.0.2/alibabacloud_arms20190808.egg-info/PKG-INFO` & `alibabacloud_arms20190808-2.0.3/alibabacloud_arms20190808.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-arms20190808
-Version: 2.0.2
+Version: 2.0.3
 Summary: Alibaba Cloud Application Real-Time Monitoring Service (20190808) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_arms20190808-2.0.2/setup.py` & `alibabacloud_arms20190808-2.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_arms20190808.
 
-Created on 01/08/2023
+Created on 02/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_arms20190808"
 NAME = "alibabacloud_arms20190808" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud Application Real-Time Monitoring Service (20190808) SDK Library for Python"
```

