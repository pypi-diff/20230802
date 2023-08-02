# Comparing `tmp/naruno_api-0.60.2.tar.gz` & `tmp/naruno_api-0.60.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_api-0.60.2.tar", last modified: Tue Aug  1 14:28:26 2023, max compression
+gzip compressed data, was "naruno_api-0.60.3.tar", last modified: Wed Aug  2 15:08:31 2023, max compression
```

## Comparing `naruno_api-0.60.2.tar` & `naruno_api-0.60.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:26.539884 naruno_api-0.60.2/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-01 14:28:26.535884 naruno_api-0.60.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 14:28:26.535884 naruno_api-0.60.2/naruno_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-01 14:28:26.000000 naruno_api-0.60.2/naruno_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-01 14:28:26.000000 naruno_api-0.60.2/naruno_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:28:26.000000 naruno_api-0.60.2/naruno_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:28:26.000000 naruno_api-0.60.2/naruno_api.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-01 14:28:26.000000 naruno_api-0.60.2/naruno_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 14:28:26.000000 naruno_api-0.60.2/naruno_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-01 14:28:26.539884 naruno_api-0.60.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-01 14:28:12.000000 naruno_api-0.60.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:31.666722 naruno_api-0.60.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-02 15:08:31.666722 naruno_api-0.60.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 15:08:31.666722 naruno_api-0.60.3/naruno_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-08-02 15:08:31.000000 naruno_api-0.60.3/naruno_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-08-02 15:08:31.000000 naruno_api-0.60.3/naruno_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:08:31.000000 naruno_api-0.60.3/naruno_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:08:31.000000 naruno_api-0.60.3/naruno_api.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-08-02 15:08:31.000000 naruno_api-0.60.3/naruno_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 15:08:31.000000 naruno_api-0.60.3/naruno_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 15:08:31.666722 naruno_api-0.60.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-08-02 15:08:12.000000 naruno_api-0.60.3/setup.py
```

### Comparing `naruno_api-0.60.2/setup.py` & `naruno_api-0.60.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from setuptools import setup
 
 setup(
     name="naruno_api",
-    version="0.60.2",
+    version="0.60.3",
     description="""This is API mode installer for Naruno""",
     url="https://docs.naruno.org/",
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     license="MPL-2.0",
     install_requires="""
 flask==2.0.0
```

