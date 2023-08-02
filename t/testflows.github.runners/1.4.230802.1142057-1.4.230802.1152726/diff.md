# Comparing `tmp/testflows.github.runners-1.4.230802.1142057.tar.gz` & `tmp/testflows.github.runners-1.4.230802.1152726.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.4.230802.1142057.tar", last modified: Wed Aug  2 14:20:58 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.4.230802.1152726.tar", last modified: Wed Aug  2 15:27:26 2023, max compression
```

## Comparing `testflows.github.runners-1.4.230802.1142057.tar` & `testflows.github.runners-1.4.230802.1152726.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1142057/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    62884 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    62292 2023-08-02 13:51:26.000000 testflows.github.runners-1.4.230802.1142057/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 14:20:57.000000 testflows.github.runners-1.4.230802.1142057/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 14:20:57.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 12:06:55.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2783 2023-08-02 12:21:36.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25924 2023-08-02 14:19:56.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4262 2023-08-02 12:20:43.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    15538 2023-08-02 11:42:31.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    25858 2023-08-02 12:11:44.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2561 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-08-02 12:20:19.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1142057/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 14:20:58.194688 testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    62884 2023-08-02 14:20:58.000000 testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 14:20:58.000000 testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 14:20:58.000000 testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 14:20:58.000000 testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 14:20:58.000000 testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.905244 testflows.github.runners-1.4.230802.1152726/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    62884 2023-08-02 15:27:26.905244 testflows.github.runners-1.4.230802.1152726/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    62292 2023-08-02 13:51:26.000000 testflows.github.runners-1.4.230802.1152726/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 15:27:26.905244 testflows.github.runners-1.4.230802.1152726/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2783 2023-08-02 12:21:36.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    25924 2023-08-02 14:19:56.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4262 2023-08-02 12:20:43.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15538 2023-08-02 11:42:31.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25858 2023-08-02 12:11:44.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2561 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-08-02 12:20:19.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    62884 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.4.230802.1142057/LICENSE` & `testflows.github.runners-1.4.230802.1152726/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/PKG-INFO` & `testflows.github.runners-1.4.230802.1152726/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230802.1142057
+Version: 1.4.230802.1152726
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.4.230802.1142057/README.rst` & `testflows.github.runners-1.4.230802.1152726/README.rst`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/setup.py` & `testflows.github.runners-1.4.230802.1152726/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.4.230802.1142057",
+    version="1.4.230802.1152726",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/__init__.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.4.230802.1142057"
+__version__ = "1.4.230802.1152726"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/actions.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/api_watch.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,14 @@
                 github = Github(login_or_token=github_token)
                 github.get_rate_limit
             with Action("Checking current API calls consumption rate"):
                 current, total = github.rate_limiting
                 next_resettime = github.rate_limiting_resettime
 
                 with Action(
-                    f"Consumed {(calls-current) if not calls < current else {total-current}} calls in {interval} sec, {current} calls left, reset in {int(next_resettime - time.time())} sec"
+                    f"Consumed {(calls-current) if not calls < current else (total-current)} calls in {interval} sec, {current} calls left, reset in {int(next_resettime - time.time())} sec"
                 ):
                     calls = current
             i = 0
 
         time.sleep(1)
         i += 1
```

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/args.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/bin/github-runners`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/cloud.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/config.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/config.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/delete.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/logger.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/request.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/server.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/service.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/service.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows/github/runners/shell.py` & `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230802.1142057
+Version: 1.4.230802.1152726
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testflows.github.runners-1.4.230802.1142057/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

