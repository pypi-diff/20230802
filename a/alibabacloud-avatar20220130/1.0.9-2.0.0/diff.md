# Comparing `tmp/alibabacloud_avatar20220130-1.0.9.tar.gz` & `tmp/alibabacloud_avatar20220130-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_avatar20220130-1.0.9.tar", last modified: Mon Nov 28 06:56:37 2022, max compression
+gzip compressed data, was "dist/alibabacloud_avatar20220130-2.0.0.tar", last modified: Wed Aug  2 02:42:53 2023, max compression
```

## Comparing `alibabacloud_avatar20220130-1.0.9.tar` & `alibabacloud_avatar20220130-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/
--rw-r--r--   0 root         (0) root         (0)      517 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1031 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1116 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/
--rw-r--r--   0 root         (0) root         (0)       21 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44582 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/client.py
--rw-r--r--   0 root         (0) root         (0)    96120 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      444 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      156 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2625 2022-11-28 06:56:37.000000 alibabacloud_avatar20220130-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1719 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1031 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1116 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95528 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130/client.py
+-rw-r--r--   0 root         (0) root         (0)   204962 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2346 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      444 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      157 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-08-02 02:42:53.000000 alibabacloud_avatar20220130-2.0.0/setup.py
```

### Comparing `alibabacloud_avatar20220130-1.0.9/LICENSE` & `alibabacloud_avatar20220130-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130-1.0.9/PKG-INFO` & `alibabacloud_avatar20220130-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_avatar20220130
-Version: 1.0.9
+Version: 2.0.0
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130-1.0.9/README-CN.md` & `alibabacloud_avatar20220130-2.0.0/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130-1.0.9/README.md` & `alibabacloud_avatar20220130-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_avatar20220130-1.0.9/alibabacloud_avatar20220130.egg-info/PKG-INFO` & `alibabacloud_avatar20220130-2.0.0/alibabacloud_avatar20220130.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-avatar20220130
-Version: 1.0.9
+Version: 2.0.0
 Summary: Alibaba Cloud avatar (20220130) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_avatar20220130-1.0.9/setup.py` & `alibabacloud_avatar20220130-2.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,30 +20,30 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_avatar20220130.
 
-Created on 28/11/2022
+Created on 02/08/2023
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_avatar20220130"
 NAME = "alibabacloud_avatar20220130" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud avatar (20220130) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.8, <1.0.0",
+    "alibabacloud_tea_util>=0.3.11, <1.0.0",
     "alibabacloud_tea_openapi>=0.3.6, <1.0.0",
-    "alibabacloud_openapi_util>=0.2.0, <1.0.0",
+    "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
         LONG_DESCRIPTION = fp.read()
```

