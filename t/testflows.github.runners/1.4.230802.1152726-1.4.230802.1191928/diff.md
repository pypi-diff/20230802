# Comparing `tmp/testflows.github.runners-1.4.230802.1152726.tar.gz` & `tmp/testflows.github.runners-1.4.230802.1191928.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.4.230802.1152726.tar", last modified: Wed Aug  2 15:27:26 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.4.230802.1191928.tar", last modified: Wed Aug  2 19:19:28 2023, max compression
```

## Comparing `testflows.github.runners-1.4.230802.1152726.tar` & `testflows.github.runners-1.4.230802.1191928.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.905244 testflows.github.runners-1.4.230802.1152726/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    62884 2023-08-02 15:27:26.905244 testflows.github.runners-1.4.230802.1152726/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    62292 2023-08-02 13:51:26.000000 testflows.github.runners-1.4.230802.1152726/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 15:27:26.905244 testflows.github.runners-1.4.230802.1152726/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2783 2023-08-02 12:21:36.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25924 2023-08-02 14:19:56.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4262 2023-08-02 12:20:43.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    15538 2023-08-02 11:42:31.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    25858 2023-08-02 12:11:44.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2561 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-08-02 12:20:19.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1152726/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 15:27:26.901244 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    62884 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 15:27:26.000000 testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 19:19:28.729530 testflows.github.runners-1.4.230802.1191928/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1191928/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    63278 2023-08-02 19:19:28.729530 testflows.github.runners-1.4.230802.1191928/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    62686 2023-08-02 19:07:12.000000 testflows.github.runners-1.4.230802.1191928/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 19:19:28.729530 testflows.github.runners-1.4.230802.1191928/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 19:19:28.000000 testflows.github.runners-1.4.230802.1191928/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 19:19:28.725530 testflows.github.runners-1.4.230802.1191928/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 19:19:28.725530 testflows.github.runners-1.4.230802.1191928/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 19:19:28.729530 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 19:19:28.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 15:26:55.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     3019 2023-08-02 18:47:51.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 19:19:28.729530 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    26311 2023-08-02 19:06:07.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13654 2023-08-02 19:18:14.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4326 2023-08-02 18:55:05.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15802 2023-08-02 18:59:59.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25858 2023-08-02 12:11:44.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 19:19:28.729530 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 19:19:28.729530 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2561 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5553 2023-08-02 18:56:43.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1191928/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 19:19:28.729530 testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    63278 2023-08-02 19:19:28.000000 testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 19:19:28.000000 testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 19:19:28.000000 testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 19:19:28.000000 testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 19:19:28.000000 testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.4.230802.1152726/LICENSE` & `testflows.github.runners-1.4.230802.1191928/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/PKG-INFO` & `testflows.github.runners-1.4.230802.1191928/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.4.230802.1152726
+Version: 1.4.230802.1191928
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -455,19 +455,21 @@
 Therefore, it is inefficient to delete a server if it only executed a job
 that runs for a few minutes. Instead, the after completing a job the server is powered off
 and if it can be recycled it is rebuild from scratch by reinstalling the image
 thus providing a clean environment for the next job.
 
 Powered off servers are marked as recyclable by changing their name to **github-runner-recycle-{uuid}**.
 
-Recyclable servers are deleted *10* minutes before they reach their end of life, if they were not
-recycled before that. The end of life is calculated on per hour basis.
-
-For example, if the server is running for 2 hours and 50 minutes, then it will be
-considered end of life and deleted as it has *10* minutes or less of useful life.
+Recyclable servers are deleted when they reach their end of life period
+which is defined by the **--end-of-life** option, and by default is set to *50* minutes.
+The end of life is calculated on hourly basis and must be greater than *0* and less than *60*.
+
+For example, with the default value of the **--end-of-life** option set to the *50* minutes,
+if the server is running for 2 hours and 50 minutes, then it will be
+considered to have reached its end of life and is deleted because it has only *10* minutes or less of useful life.
 However, if the server is running for 2 hours and 30 minutes, then it potentially
 has 30 minutes of life left and it will be kept around to potentially be recycled.
 
 Sometimes a job might need a server that does not match any recyclable servers,
 if the maximum number of runners has been reached **then one of the recyclable servers
 will be picked at random to be deleted** to make room for a new server.
 
@@ -1606,14 +1608,18 @@
 
 * **--license**
   show program's license and exit
 
 * **-r {on,off}, --recycle {on,off}**
   turn on or off recycling of powered off servers, either 'on' or 'off', default: *on*
 
+* **--end-of-life minutes**
+  number of minutes in 1 hour (60 minutes) period after which a recyclable server
+  is considered to have reached its end of life and thus is deleted, default: *50*
+
 * **-c path, --config path**
   program configuration file
 
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
```

### Comparing `testflows.github.runners-1.4.230802.1152726/README.rst` & `testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.4.230802.1191928
+Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
+Home-page: https://github.com/testflows/github-runners
+Author: Vitaliy Zakaznikov
+Author-email: vzakaznikov@testflows.com
+License: Apache-2.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: POSIX :: Linux
+Requires-Python: >=3.8
+Description-Content-Type: text/x-rst
+Provides-Extra: dev
+License-File: LICENSE
+
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 300px
    :align: center
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
@@ -438,19 +455,21 @@
 Therefore, it is inefficient to delete a server if it only executed a job
 that runs for a few minutes. Instead, the after completing a job the server is powered off
 and if it can be recycled it is rebuild from scratch by reinstalling the image
 thus providing a clean environment for the next job.
 
 Powered off servers are marked as recyclable by changing their name to **github-runner-recycle-{uuid}**.
 
-Recyclable servers are deleted *10* minutes before they reach their end of life, if they were not
-recycled before that. The end of life is calculated on per hour basis.
-
-For example, if the server is running for 2 hours and 50 minutes, then it will be
-considered end of life and deleted as it has *10* minutes or less of useful life.
+Recyclable servers are deleted when they reach their end of life period
+which is defined by the **--end-of-life** option, and by default is set to *50* minutes.
+The end of life is calculated on hourly basis and must be greater than *0* and less than *60*.
+
+For example, with the default value of the **--end-of-life** option set to the *50* minutes,
+if the server is running for 2 hours and 50 minutes, then it will be
+considered to have reached its end of life and is deleted because it has only *10* minutes or less of useful life.
 However, if the server is running for 2 hours and 30 minutes, then it potentially
 has 30 minutes of life left and it will be kept around to potentially be recycled.
 
 Sometimes a job might need a server that does not match any recyclable servers,
 if the maximum number of runners has been reached **then one of the recyclable servers
 will be picked at random to be deleted** to make room for a new server.
 
@@ -1589,14 +1608,18 @@
 
 * **--license**
   show program's license and exit
 
 * **-r {on,off}, --recycle {on,off}**
   turn on or off recycling of powered off servers, either 'on' or 'off', default: *on*
 
+* **--end-of-life minutes**
+  number of minutes in 1 hour (60 minutes) period after which a recyclable server
+  is considered to have reached its end of life and thus is deleted, default: *50*
+
 * **-c path, --config path**
   program configuration file
 
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
```

### Comparing `testflows.github.runners-1.4.230802.1152726/setup.py` & `testflows.github.runners-1.4.230802.1191928/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.4.230802.1152726",
+    version="1.4.230802.1191928",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/__init__.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.4.230802.1152726"
+__version__ = "1.4.230802.1191928"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/actions.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/args.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/args.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,24 @@
 from hcloud.images.domain import Image
 from hcloud.locations.domain import Location
 from hcloud.server_types.domain import ServerType
 
 from argparse import ArgumentTypeError
 
 
+def end_of_life_type(v):
+    """Server end of life type."""
+    try:
+        v = int(v)
+        assert v > 0 and v < 60, f"{v} must be > 0 and < 60"
+    except AssertionError as e:
+        raise ArgumentTypeError(str(e))
+    return v
+
+
 def switch_type(v):
     """Switch argument type."""
     if v == "on":
         return True
     elif v == "off":
         return False
     raise ArgumentTypeError(f"invalid value {v}")
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,24 @@
         "-r",
         "--recycle",
         type=args.switch_type,
         help="turn on recycling of powered off servers, either 'on' or 'off', default: on",
     )
 
     parser.add_argument(
+        "--end-of-life",
+        metavar="minutes",
+        type=args.end_of_life_type,
+        help=(
+            "number of minutes in 1 hour (60 minutes) period after which a recyclable server\n"
+            "is considered to have reached its end of life and thus is deleted, default: 50"
+        ),
+    )
+
+    parser.add_argument(
         "--max-runners-in-workflow-run",
         metavar="count",
         type=args.count_type,
         help="maximum number of runners allowed for a workflow run, default: not set",
     )
 
     parser.add_argument(
@@ -681,14 +691,15 @@
                     standby_runners=config.standby_runners,
                 )
 
             with Action("Creating scale down service"):
                 scale_down_service: Future = worker_pool.submit(
                     scale_down,
                     recycle=config.recycle,
+                    end_of_life=config.end_of_life,
                     ssh_key=ssh_key,
                     hetzner_token=config.hetzner_token,
                     github_token=config.github_token,
                     github_repository=config.github_repository,
                     terminate=terminate,
                     max_powered_off_time=config.max_powered_off_time,
                     max_unused_runner_time=config.max_unused_runner_time,
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/cloud.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/cloud.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,16 +60,17 @@
         )
 
         if args.force:
             with Action(
                 f"Checking if server {server_name} already exists", ignore_fail=True
             ):
                 server: BoundServer = client.servers.get_by_name(server_name)
-                with Action(f"Deleting server {server_name}"):
-                    server.delete()
+                if server is not None:
+                    with Action(f"Deleting server {server_name}"):
+                        server.delete()
 
         with Action("Checking if default image exists"):
             config.default_image = check_image(
                 client=client, image=config.default_image
             )
 
         with Action("Checking if server image exists"):
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/config.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 
 path = args.path_type
 count = args.count_type
 image = args.image_type
 location = args.location_type
 server_type = args.server_type
+end_of_life = args.end_of_life_type
 
 
 @dataclass
 class standby_runner:
     labels: list[str]
     count: count = 1
     replenish_immediately: bool = True
@@ -47,14 +48,15 @@
 
     github_token: str = os.getenv("GITHUB_TOKEN")
     github_repository: str = os.getenv("GITHUB_REPOSITORY")
     hetzner_token: str = os.getenv("HETZNER_TOKEN")
     ssh_key: str = os.path.expanduser("~/.ssh/id_rsa.pub")
     with_label: str = None
     recycle: bool = True
+    end_of_life: count = 50
     max_runners: count = 10
     max_runners_in_workflow_run: count = None
     default_image: image = image("x86:system:ubuntu-22.04")
     default_server_type: server_type = server_type("cx11")
     default_location: location = None
     workers: count = 10
     setup_script: path = None
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/delete.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/logger.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/request.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scale_down.py`

 * *Files 3% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     """Unused self-hosted runner."""
 
     time: float
     runner: SelfHostedActionsRunner
     observed_interval: float
 
 
-def recycle_server(reason: str, server: BoundServer, ssh_key: SSHKey, margin=10):
+def recycle_server(reason: str, server: BoundServer, ssh_key: SSHKey, end_of_life: int):
     """Recycle server."""
     now = datetime.now(timezone.utc)
     used = now - server.created
     days = used.days
     hours, remainder = divmod(used.seconds, 3600)
     minutes, _ = divmod(remainder, 60)
 
@@ -98,15 +98,15 @@
             ignore_fail=True,
         ):
             try:
                 server.delete()
             finally:
                 return
 
-    if minutes > (60 - margin):
+    if minutes >= end_of_life:
         with Action(
             f"Try deleting {reason} server {server.name} "
             f"used {days}d{hours}h{minutes}m "
             "as it is end of life",
             stacklevel=3,
             ignore_fail=True,
         ):
@@ -129,14 +129,15 @@
 
 def scale_down(
     terminate: threading.Event,
     hetzner_token: str,
     github_token: str,
     github_repository: str,
     recycle: bool,
+    end_of_life: int,
     max_powered_off_time: int,
     max_unused_runner_time: int,
     max_runner_registration_time: int,
     interval: int,
     ssh_key: SSHKey,
     debug: bool = False,
     standby_runners: list[StandbyRunner] = None,
@@ -276,14 +277,15 @@
                     else:
                         if time.time() - powered_off_server.time > max_powered_off_time:
                             if recycle:
                                 recycle_server(
                                     reason="powered off",
                                     server=powered_off_server.server,
                                     ssh_key=ssh_key,
+                                    end_of_life=end_of_life,
                                 )
                             else:
                                 with Action(
                                     f"Deleting powered off server {server_name}",
                                     ignore_fail=True,
                                 ) as action:
                                     powered_off_server.server.delete()
@@ -305,14 +307,15 @@
                             > max_runner_registration_time
                         ):
                             if recycle:
                                 recycle_server(
                                     reason="zombie",
                                     server=zombie_server.server,
                                     ssh_key=ssh_key,
+                                    end_of_life=end_of_life,
                                 )
                             else:
                                 with Action(
                                     f"Deleting zombie server {server_name}",
                                     ignore_fail=True,
                                 ) as action:
                                     zombie_server.server.delete()
@@ -342,14 +345,15 @@
 
                             if runner_server is not None:
                                 if recycle:
                                     recycle_server(
                                         reason="unused runner",
                                         server=runner_server,
                                         ssh_key=ssh_key,
+                                        end_of_life=end_of_life,
                                     )
                                 else:
                                     with Action(
                                         f"Deleting unused runner server {runner_server.name}",
                                         ignore_fail=True,
                                     ):
                                         runner_server.delete()
@@ -368,14 +372,15 @@
             ):
                 for server_name in list(recyclable_servers.keys()):
                     recyclable_server = recyclable_servers[server_name]
                     recycle_server(
                         reason="unused recyclable",
                         server=recyclable_server,
                         ssh_key=ssh_key,
+                        end_of_life=end_of_life,
                     )
 
         except Exception as exc:
             msg = f"❗ Error: {type(exc).__name__} {exc}"
             if debug:
                 logger.exception(f"{msg}\n{exc}")
             else:
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scale_up.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/server.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/service.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/service.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     """
     command = ""
     command += f" --github-token $GITHUB_TOKEN"
     command += f" --github-repository $GITHUB_REPOSITORY"
     command += f" --hetzner-token $HETZNER_TOKEN"
     command += f" --config {config.config_file}" if config.config_file else ""
     command += f" --recycle " + "on" if config.recycle else "off"
+    command += f" --end-of-life {config.end_of_life}" if config.end_of_life else ""
     command += f" --with-label {config.with_label}" if config.with_label else ""
     command += f" --workers {config.workers}"
     command += f" --default-type {config.default_server_type.name}"
     command += (
         f" --default-location {config.default_location.name}"
         if config.default_location
         else ""
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows/github/runners/shell.py` & `testflows.github.runners-1.4.230802.1191928/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.4.230802.1191928/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.4.230802.1152726
-Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
-Home-page: https://github.com/testflows/github-runners
-Author: Vitaliy Zakaznikov
-Author-email: vzakaznikov@testflows.com
-License: Apache-2.0
-Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: POSIX :: Linux
-Requires-Python: >=3.8
-Description-Content-Type: text/x-rst
-Provides-Extra: dev
-License-File: LICENSE
-
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-ArtWork/master/images/logo.png
    :width: 300px
    :align: center
    :target: https://testflows.com
    :alt: TestFlows Open-source Testing Framework
 
 ----
@@ -455,19 +438,21 @@
 Therefore, it is inefficient to delete a server if it only executed a job
 that runs for a few minutes. Instead, the after completing a job the server is powered off
 and if it can be recycled it is rebuild from scratch by reinstalling the image
 thus providing a clean environment for the next job.
 
 Powered off servers are marked as recyclable by changing their name to **github-runner-recycle-{uuid}**.
 
-Recyclable servers are deleted *10* minutes before they reach their end of life, if they were not
-recycled before that. The end of life is calculated on per hour basis.
-
-For example, if the server is running for 2 hours and 50 minutes, then it will be
-considered end of life and deleted as it has *10* minutes or less of useful life.
+Recyclable servers are deleted when they reach their end of life period
+which is defined by the **--end-of-life** option, and by default is set to *50* minutes.
+The end of life is calculated on hourly basis and must be greater than *0* and less than *60*.
+
+For example, with the default value of the **--end-of-life** option set to the *50* minutes,
+if the server is running for 2 hours and 50 minutes, then it will be
+considered to have reached its end of life and is deleted because it has only *10* minutes or less of useful life.
 However, if the server is running for 2 hours and 30 minutes, then it potentially
 has 30 minutes of life left and it will be kept around to potentially be recycled.
 
 Sometimes a job might need a server that does not match any recyclable servers,
 if the maximum number of runners has been reached **then one of the recyclable servers
 will be picked at random to be deleted** to make room for a new server.
 
@@ -1606,14 +1591,18 @@
 
 * **--license**
   show program's license and exit
 
 * **-r {on,off}, --recycle {on,off}**
   turn on or off recycling of powered off servers, either 'on' or 'off', default: *on*
 
+* **--end-of-life minutes**
+  number of minutes in 1 hour (60 minutes) period after which a recyclable server
+  is considered to have reached its end of life and thus is deleted, default: *50*
+
 * **-c path, --config path**
   program configuration file
 
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
```

### Comparing `testflows.github.runners-1.4.230802.1152726/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.4.230802.1191928/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

