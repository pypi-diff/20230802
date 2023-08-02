# Comparing `tmp/testflows.github.runners-1.3.230801.1235756.tar.gz` & `tmp/testflows.github.runners-1.3.230802.1011544.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230801.1235756.tar", last modified: Tue Aug  1 23:57:57 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230802.1011544.tar", last modified: Wed Aug  2 01:15:44 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230801.1235756.tar` & `testflows.github.runners-1.3.230802.1011544.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.068637 testflows.github.runners-1.3.230801.1235756/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    58949 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    58357 2023-08-01 23:57:22.000000 testflows.github.runners-1.3.230801.1235756/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-01 23:57:57.068637 testflows.github.runners-1.3.230801.1235756/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-01 23:57:56.000000 testflows.github.runners-1.3.230801.1235756/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-01 23:57:56.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25252 2023-08-01 23:26:46.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4210 2023-08-01 21:03:13.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    19139 2023-08-01 23:44:19.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5322 2023-08-01 21:06:23.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    58949 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    59560 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    58968 2023-08-02 01:12:25.000000 testflows.github.runners-1.3.230802.1011544/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.384858 testflows.github.runners-1.3.230802.1011544/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.384858 testflows.github.runners-1.3.230802.1011544/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    25597 2023-08-02 01:01:56.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4237 2023-08-02 01:04:45.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19572 2023-08-02 01:04:27.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5403 2023-08-02 01:05:02.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.384858 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    59560 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230801.1235756/LICENSE` & `testflows.github.runners-1.3.230802.1011544/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/PKG-INFO` & `testflows.github.runners-1.3.230802.1011544/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230801.1235756
+Version: 1.3.230802.1011544
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -438,14 +438,32 @@
 
 :✋ Note:
    Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
    workflow run takes to complete it jobs, if number of jobs in the workflow
    is greater than the value of this option, as compared to the case if all available runners
    would be allowed.
 
+=============
+Skipping Jobs
+=============
+
+By default, a runner will be created for any **queued** job.
+
+If needed, you can skip creating runners if a job does not have some specified label
+using the **--with-label** option.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners --with-label on-demand
+
+will only create runners for jobs that contain **on-demand** label and skip any job that is missing
+that label.
+
 ===============================
 Jobs That Require Docker Engine
 ===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
@@ -772,14 +790,15 @@
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
    * **ssh_key: str**
    * **max_runners: count**
    * **max_runners_in_workflow_run: count**
+   * **with_label: str**
    * **default_image: image**
    * **default_server_type: server_type**
    * **default_location: location**
    * **workers: count**
    * **setup_script: path**
    * **startup_x64_script: path**
    * **startup_arm64_script: path**
@@ -1556,14 +1575,18 @@
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **--max-runners-in-workflow-run count**
   maximum number of runners allowed in a workflow run, default: not set
 
+* **--with-label label**
+  only create runners for jobs that have the specified label,
+  by default jobs are not skipped and runners will be created for any queued job
+
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
```

### Comparing `testflows.github.runners-1.3.230801.1235756/README.rst` & `testflows.github.runners-1.3.230802.1011544/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -421,14 +421,32 @@
 
 :✋ Note:
    Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
    workflow run takes to complete it jobs, if number of jobs in the workflow
    is greater than the value of this option, as compared to the case if all available runners
    would be allowed.
 
+=============
+Skipping Jobs
+=============
+
+By default, a runner will be created for any **queued** job.
+
+If needed, you can skip creating runners if a job does not have some specified label
+using the **--with-label** option.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners --with-label on-demand
+
+will only create runners for jobs that contain **on-demand** label and skip any job that is missing
+that label.
+
 ===============================
 Jobs That Require Docker Engine
 ===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
@@ -755,14 +773,15 @@
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
    * **ssh_key: str**
    * **max_runners: count**
    * **max_runners_in_workflow_run: count**
+   * **with_label: str**
    * **default_image: image**
    * **default_server_type: server_type**
    * **default_location: location**
    * **workers: count**
    * **setup_script: path**
    * **startup_x64_script: path**
    * **startup_arm64_script: path**
@@ -1539,14 +1558,18 @@
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **--max-runners-in-workflow-run count**
   maximum number of runners allowed in a workflow run, default: not set
 
+* **--with-label label**
+  only create runners for jobs that have the specified label,
+  by default jobs are not skipped and runners will be created for any queued job
+
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
```

### Comparing `testflows.github.runners-1.3.230801.1235756/setup.py` & `testflows.github.runners-1.3.230802.1011544/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230801.1235756",
+    version="1.3.230802.1011544",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.3.230801.1235756"
+__version__ = "1.3.230802.1011544"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -129,14 +129,24 @@
         "--max-runners-in-workflow-run",
         metavar="count",
         type=args.count_type,
         help="maximum number of runners allowed for a workflow run, default: not set",
     )
 
     parser.add_argument(
+        "--with-label",
+        metavar="label",
+        type=str,
+        help=(
+            "only create runners for jobs that have the specified label,\n"
+            "by default jobs are not filtered and runners will be created for any queued job"
+        ),
+    )
+
+    parser.add_argument(
         "--default-image",
         metavar="architecture:type:name_or_description",
         type=args.image_type,
         help=(
             "default runner server image type and name or description,\n"
             "where the architecture is either: 'x86' or 'arm' and\n"
             "the type is either: 'system','snapshot','backup','app',\n"
@@ -641,14 +651,15 @@
                     )
 
         try:
             with Action("Creating scale up service"):
                 scale_up_service: Future = worker_pool.submit(
                     scale_up,
                     terminate=terminate,
+                    with_label=config.with_label,
                     scripts=scripts,
                     ssh_key=ssh_key,
                     default_server_type=config.default_server_type,
                     default_image=config.default_image,
                     default_location=config.default_location,
                     worker_pool=worker_pool,
                     hetzner_token=config.hetzner_token,
```

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 class Config:
     """Program configuration class."""
 
     github_token: str = os.getenv("GITHUB_TOKEN")
     github_repository: str = os.getenv("GITHUB_REPOSITORY")
     hetzner_token: str = os.getenv("HETZNER_TOKEN")
     ssh_key: str = os.path.expanduser("~/.ssh/id_rsa.pub")
+    with_label: str = None
     max_runners: count = 10
     max_runners_in_workflow_run: count = None
     default_image: image = image("x86:system:ubuntu-22.04")
     default_server_type: server_type = server_type("cx11")
     default_location: location = None
     workers: count = 10
     setup_script: path = None
```

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scale_up.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,14 +279,15 @@
             ):
                 return True
     return False
 
 
 def scale_up(
     terminate: threading.Event,
+    with_label: str,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
     hetzner_token: str,
     ssh_key: SSHKey,
     default_server_type: ServerType,
@@ -444,14 +445,21 @@
                                         if max_servers_in_workflow_run_reached(
                                             run_id=run.id,
                                             servers=servers,
                                             max_servers_in_workflow_run=max_servers_in_workflow_run,
                                         ):
                                             break
 
+                                    if with_label is not None:
+                                        if not with_label in labels:
+                                            with Action(
+                                                f"Skipping {job} with {labels} as it is missing label '{with_label}'"
+                                            ):
+                                                continue
+
                                     with Action(f"Creating new server for {job}"):
                                         create_runner_server(
                                             name=server_name,
                                             labels=labels,
                                             setup_worker_pool=setup_worker_pool,
                                             futures=futures,
                                             servers=servers,
```

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     --ssh-key
     """
     command = ""
     command += f" --github-token $GITHUB_TOKEN"
     command += f" --github-repository $GITHUB_REPOSITORY"
     command += f" --hetzner-token $HETZNER_TOKEN"
     command += f" --config {config.config_file}" if config.config_file else ""
+    command += f" --with-label {config.with_label}" if config.with_label else ""
     command += f" --workers {config.workers}"
     command += f" --default-type {config.default_server_type.name}"
     command += (
         f" --default-location {config.default_location.name}"
         if config.default_location
         else ""
     )
```

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230801.1235756
+Version: 1.3.230802.1011544
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -438,14 +438,32 @@
 
 :✋ Note:
    Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
    workflow run takes to complete it jobs, if number of jobs in the workflow
    is greater than the value of this option, as compared to the case if all available runners
    would be allowed.
 
+=============
+Skipping Jobs
+=============
+
+By default, a runner will be created for any **queued** job.
+
+If needed, you can skip creating runners if a job does not have some specified label
+using the **--with-label** option.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners --with-label on-demand
+
+will only create runners for jobs that contain **on-demand** label and skip any job that is missing
+that label.
+
 ===============================
 Jobs That Require Docker Engine
 ===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
@@ -772,14 +790,15 @@
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
    * **ssh_key: str**
    * **max_runners: count**
    * **max_runners_in_workflow_run: count**
+   * **with_label: str**
    * **default_image: image**
    * **default_server_type: server_type**
    * **default_location: location**
    * **workers: count**
    * **setup_script: path**
    * **startup_x64_script: path**
    * **startup_arm64_script: path**
@@ -1556,14 +1575,18 @@
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
 * **--max-runners-in-workflow-run count**
   maximum number of runners allowed in a workflow run, default: not set
 
+* **--with-label label**
+  only create runners for jobs that have the specified label,
+  by default jobs are not skipped and runners will be created for any queued job
+
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
```

### Comparing `testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

