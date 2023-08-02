# Comparing `tmp/testflows.github.runners-1.3.230802.1011544.tar.gz` & `tmp/testflows.github.runners-1.4.230802.1135328.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230802.1011544.tar", last modified: Wed Aug  2 01:15:44 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.4.230802.1135328.tar", last modified: Wed Aug  2 13:53:28 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230802.1011544.tar` & `testflows.github.runners-1.4.230802.1135328.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    59560 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    58968 2023-08-02 01:12:25.000000 testflows.github.runners-1.3.230802.1011544/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.384858 testflows.github.runners-1.3.230802.1011544/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.384858 testflows.github.runners-1.3.230802.1011544/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    25597 2023-08-02 01:01:56.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4237 2023-08-02 01:04:45.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    19572 2023-08-02 01:04:27.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.388858 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5403 2023-08-02 01:05:02.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230802.1011544/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 01:15:44.384858 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    59560 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 01:15:44.000000 testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 13:53:28.495075 testflows.github.runners-1.4.230802.1135328/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1135328/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    62884 2023-08-02 13:53:28.495075 testflows.github.runners-1.4.230802.1135328/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    62292 2023-08-02 13:51:26.000000 testflows.github.runners-1.4.230802.1135328/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-02 13:53:28.495075 testflows.github.runners-1.4.230802.1135328/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-02 13:53:28.000000 testflows.github.runners-1.4.230802.1135328/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 13:53:28.491075 testflows.github.runners-1.4.230802.1135328/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 13:53:28.491075 testflows.github.runners-1.4.230802.1135328/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 13:53:28.495075 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-02 13:53:28.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1741 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1995 2023-08-02 12:06:55.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2783 2023-08-02 12:21:36.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 13:53:28.495075 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    25955 2023-08-02 12:19:07.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4262 2023-08-02 12:20:43.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    15538 2023-08-02 11:42:31.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    25858 2023-08-02 12:11:44.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 13:53:28.495075 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 13:53:28.495075 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2561 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5469 2023-08-02 12:20:19.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1512 2023-08-02 11:42:30.000000 testflows.github.runners-1.4.230802.1135328/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-02 13:53:28.495075 testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    62884 2023-08-02 13:53:28.000000 testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-02 13:53:28.000000 testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-02 13:53:28.000000 testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-02 13:53:28.000000 testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-02 13:53:28.000000 testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230802.1011544/LICENSE` & `testflows.github.runners-1.4.230802.1135328/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/PKG-INFO` & `testflows.github.runners-1.4.230802.1135328/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230802.1011544
+Version: 1.4.230802.1135328
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -64,14 +64,15 @@
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
 ========
 Features
 ========
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+* supports server recycling to minimize costs
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
@@ -438,14 +439,74 @@
 
 :✋ Note:
    Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
    workflow run takes to complete it jobs, if number of jobs in the workflow
    is greater than the value of this option, as compared to the case if all available runners
    would be allowed.
 
+
+=============================
+Recycling Powered Off Servers
+=============================
+
+By default, recycling of powered off servers that has completed executing a job is turned on.
+
+Recycling allows to minimize costs by allowing multiple runners to be brought up on
+the same server instance as Hetzner Cloud bills servers in 1 hour increments.
+Therefore, it is inefficient to delete a server if it only executed a job
+that runs for a few minutes. Instead, the after completing a job the server is powered off
+and if it can be recycled it is rebuild from scratch by reinstalling the image
+thus providing a clean environment for the next job.
+
+Powered off servers are marked as recyclable by changing their name to **github-runner-recycle-{uuid}**.
+
+Recyclable servers are deleted *10* minutes before they reach their end of life, if they were not
+recycled before that. The end of life is calculated on per hour basis.
+
+For example, if the server is running for 2 hours and 50 minutes, then it will be
+considered end of life and deleted as it has *10* minutes or less of useful life.
+However, if the server is running for 2 hours and 30 minutes, then it potentially
+has 30 minutes of life left and it will be kept around to potentially be recycled.
+
+Sometimes a job might need a server that does not match any recyclable servers,
+if the maximum number of runners has been reached **then one of the recyclable servers
+will be picked at random to be deleted** to make room for a new server.
+
+:✋ Note:
+   Randomly deleting a potentially recyclable server is not the most optimal choice,
+   as we could be deleting a server that has higher cost per hour as compared to the others.
+   However, this strategy provides a good-enough behavior in most cases without building
+   server cost comparison analysis into the program as Hetzner Cloud server costs
+   could change at any time.
+
+A recyclable server is recycled for a new job if it matches the following:
+
+* server type matches exactly what the job required or the default type
+* server location matches exactly if job requested a runner in a specific location or the default location is specified
+* server has matching SSH keys
+
+:✋ Note:
+   **Matching server type exactly means that even if a bigger more expensive server type
+   could be potentially recycled it is not used, even though a job that actually requires
+   that expensive server might not be queued before the server's end of life.**
+
+   This is intensional, as we can't predict when a job that actually requires the more expensive
+   server type could be queued. If the program would allow recycling higher server types
+   than actually requested by a job, then we could run into cases when a job
+   that requires smaller and a less expensive server runs on a bigger more expensive server instead.
+   In this case, a job that actually requires the bigger server would force a new expensive server to be created
+   and thus causing more expensive servers to be created than actually necessary.
+
+If needed, you can turn recycling off using the **--recycle {on,off}** option.
+
+.. code-block:: bash
+
+   github-runners --recycle off
+
+
 =============
 Skipping Jobs
 =============
 
 By default, a runner will be created for any **queued** job.
 
 If needed, you can skip creating runners if a job does not have some specified label
@@ -1542,14 +1603,17 @@
 
 * **-v, --version**
   show program's version number and exit
 
 * **--license**
   show program's license and exit
 
+* **-r {on,off}, --recycle {on,off}**
+  turn on or off recycling of powered off servers, either 'on' or 'off', default: *on*
+
 * **-c path, --config path**
   program configuration file
 
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
@@ -1561,15 +1625,15 @@
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
-  default runner server location name, default: not specified
+  default runner server location name, default: *not specified*
 
 * **--default-image architecture:type:name_or_description**
   default runner server image type and name or description,
   where the architecture is either: 'x86' or 'arm',
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
```

### Comparing `testflows.github.runners-1.3.230802.1011544/README.rst` & `testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.4.230802.1135328
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
@@ -47,14 +64,15 @@
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
 ========
 Features
 ========
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+* supports server recycling to minimize costs
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
@@ -421,14 +439,74 @@
 
 :✋ Note:
    Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
    workflow run takes to complete it jobs, if number of jobs in the workflow
    is greater than the value of this option, as compared to the case if all available runners
    would be allowed.
 
+
+=============================
+Recycling Powered Off Servers
+=============================
+
+By default, recycling of powered off servers that has completed executing a job is turned on.
+
+Recycling allows to minimize costs by allowing multiple runners to be brought up on
+the same server instance as Hetzner Cloud bills servers in 1 hour increments.
+Therefore, it is inefficient to delete a server if it only executed a job
+that runs for a few minutes. Instead, the after completing a job the server is powered off
+and if it can be recycled it is rebuild from scratch by reinstalling the image
+thus providing a clean environment for the next job.
+
+Powered off servers are marked as recyclable by changing their name to **github-runner-recycle-{uuid}**.
+
+Recyclable servers are deleted *10* minutes before they reach their end of life, if they were not
+recycled before that. The end of life is calculated on per hour basis.
+
+For example, if the server is running for 2 hours and 50 minutes, then it will be
+considered end of life and deleted as it has *10* minutes or less of useful life.
+However, if the server is running for 2 hours and 30 minutes, then it potentially
+has 30 minutes of life left and it will be kept around to potentially be recycled.
+
+Sometimes a job might need a server that does not match any recyclable servers,
+if the maximum number of runners has been reached **then one of the recyclable servers
+will be picked at random to be deleted** to make room for a new server.
+
+:✋ Note:
+   Randomly deleting a potentially recyclable server is not the most optimal choice,
+   as we could be deleting a server that has higher cost per hour as compared to the others.
+   However, this strategy provides a good-enough behavior in most cases without building
+   server cost comparison analysis into the program as Hetzner Cloud server costs
+   could change at any time.
+
+A recyclable server is recycled for a new job if it matches the following:
+
+* server type matches exactly what the job required or the default type
+* server location matches exactly if job requested a runner in a specific location or the default location is specified
+* server has matching SSH keys
+
+:✋ Note:
+   **Matching server type exactly means that even if a bigger more expensive server type
+   could be potentially recycled it is not used, even though a job that actually requires
+   that expensive server might not be queued before the server's end of life.**
+
+   This is intensional, as we can't predict when a job that actually requires the more expensive
+   server type could be queued. If the program would allow recycling higher server types
+   than actually requested by a job, then we could run into cases when a job
+   that requires smaller and a less expensive server runs on a bigger more expensive server instead.
+   In this case, a job that actually requires the bigger server would force a new expensive server to be created
+   and thus causing more expensive servers to be created than actually necessary.
+
+If needed, you can turn recycling off using the **--recycle {on,off}** option.
+
+.. code-block:: bash
+
+   github-runners --recycle off
+
+
 =============
 Skipping Jobs
 =============
 
 By default, a runner will be created for any **queued** job.
 
 If needed, you can skip creating runners if a job does not have some specified label
@@ -1525,14 +1603,17 @@
 
 * **-v, --version**
   show program's version number and exit
 
 * **--license**
   show program's license and exit
 
+* **-r {on,off}, --recycle {on,off}**
+  turn on or off recycling of powered off servers, either 'on' or 'off', default: *on*
+
 * **-c path, --config path**
   program configuration file
 
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
@@ -1544,15 +1625,15 @@
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
-  default runner server location name, default: not specified
+  default runner server location name, default: *not specified*
 
 * **--default-image architecture:type:name_or_description**
   default runner server image type and name or description,
   where the architecture is either: 'x86' or 'arm',
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
```

### Comparing `testflows.github.runners-1.3.230802.1011544/setup.py` & `testflows.github.runners-1.4.230802.1135328/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230802.1011544",
+    version="1.4.230802.1135328",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/__init__.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 __author__ = "Vitaliy Zakaznikov"
-__version__ = "1.3.230802.1011544"
+__version__ = "1.4.230802.1135328"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/actions.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/actions.py`

 * *Files 11% similar despite different names*

```diff
@@ -23,29 +23,31 @@
     debug = False
 
     def __init__(
         self,
         name: str,
         ignore_fail: bool = False,
         level: int = logging.INFO,
+        stacklevel: int = 2,
     ):
         self.name = name
         self.ignore_fail = ignore_fail
         self.level = level
+        self.stacklevel = stacklevel
 
     def __enter__(self):
-        logger.log(msg=f"🍀 {self.name}", stacklevel=2, level=self.level)
+        logger.log(msg=f"🍀 {self.name}", stacklevel=self.stacklevel, level=self.level)
         return self
 
     def note(self, message):
-        logger.log(msg=f"   {message}", stacklevel=2, level=self.level)
+        logger.log(msg=f"   {message}", stacklevel=self.stacklevel, level=self.level)
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         if exc_value is not None:
             msg = f"❌ Error: {exc_type.__name__} {exc_value}"
             if not self.debug:
-                logger.log(msg=msg, stacklevel=2, level=logging.ERROR)
+                logger.log(msg=msg, stacklevel=self.stacklevel, level=logging.ERROR)
             else:
-                logger.exception(msg=msg, stacklevel=3)
+                logger.exception(msg=msg, stacklevel=self.stacklevel + 1)
             if self.ignore_fail:
                 return True
             raise
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/api_watch.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,14 +42,14 @@
                 github = Github(login_or_token=github_token)
                 github.get_rate_limit
             with Action("Checking current API calls consumption rate"):
                 current, total = github.rate_limiting
                 next_resettime = github.rate_limiting_resettime
 
                 with Action(
-                    f"Consumed {calls - current} calls in {interval} sec, {current} calls left, reset in {int(next_resettime - time.time())} sec"
+                    f"Consumed {(calls-current) if not calls < current else {total-current}} calls in {interval} sec, {current} calls left, reset in {int(next_resettime - time.time())} sec"
                 ):
                     calls = current
             i = 0
 
         time.sleep(1)
         i += 1
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/args.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/args.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,23 @@
 from hcloud.images.domain import Image
 from hcloud.locations.domain import Location
 from hcloud.server_types.domain import ServerType
 
 from argparse import ArgumentTypeError
 
 
+def switch_type(v):
+    """Switch argument type."""
+    if v == "on":
+        return True
+    elif v == "off":
+        return False
+    raise ArgumentTypeError(f"invalid value {v}")
+
+
 def path_type(v):
     """Path argument type."""
     try:
         v = os.path.abspath(os.path.expanduser(v))
         os.path.exists(v)
     except Exception as e:
         raise ArgumentTypeError(str(e))
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/bin/github-runners`

 * *Files 2% similar despite different names*

```diff
@@ -122,14 +122,22 @@
         "--max-runners",
         metavar="count",
         type=args.count_type,
         help="maximum number of active runners, default: 10",
     )
 
     parser.add_argument(
+        "-r",
+        "--recycle",
+        type=args.switch_type,
+        choices=["on", "off"],
+        help="turn on recycling of powered off servers, either 'on' or 'off', default: on",
+    )
+
+    parser.add_argument(
         "--max-runners-in-workflow-run",
         metavar="count",
         type=args.count_type,
         help="maximum number of runners allowed for a workflow run, default: not set",
     )
 
     parser.add_argument(
@@ -198,15 +206,15 @@
         help="path to custom ARM64 server startup script",
     )
 
     parser.add_argument(
         "--max-powered-off-time",
         metavar="sec",
         type=args.count_type,
-        help="maximum time after which a powered off server is deleted, default: 60 sec",
+        help="maximum time after which a powered off server is recycled or deleted, default: 60 sec",
     )
 
     parser.add_argument(
         "--max-unused-runner-time",
         metavar="sec",
         type=args.count_type,
         help="maximum time after which an unused runner is removed and its server deleted, default: 120 sec",
@@ -651,14 +659,15 @@
                     )
 
         try:
             with Action("Creating scale up service"):
                 scale_up_service: Future = worker_pool.submit(
                     scale_up,
                     terminate=terminate,
+                    recycle=config.recycle,
                     with_label=config.with_label,
                     scripts=scripts,
                     ssh_key=ssh_key,
                     default_server_type=config.default_server_type,
                     default_image=config.default_image,
                     default_location=config.default_location,
                     worker_pool=worker_pool,
@@ -672,14 +681,16 @@
                     debug=config.debug,
                     standby_runners=config.standby_runners,
                 )
 
             with Action("Creating scale down service"):
                 scale_down_service: Future = worker_pool.submit(
                     scale_down,
+                    recycle=config.recycle,
+                    ssh_key=ssh_key,
                     hetzner_token=config.hetzner_token,
                     github_token=config.github_token,
                     github_repository=config.github_repository,
                     terminate=terminate,
                     max_powered_off_time=config.max_powered_off_time,
                     max_unused_runner_time=config.max_unused_runner_time,
                     max_runner_registration_time=config.max_runner_registration_time,
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/cloud.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/config.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     """Program configuration class."""
 
     github_token: str = os.getenv("GITHUB_TOKEN")
     github_repository: str = os.getenv("GITHUB_REPOSITORY")
     hetzner_token: str = os.getenv("HETZNER_TOKEN")
     ssh_key: str = os.path.expanduser("~/.ssh/id_rsa.pub")
     with_label: str = None
+    recycle: bool = True
     max_runners: count = 10
     max_runners_in_workflow_run: count = None
     default_image: image = image("x86:system:ubuntu-22.04")
     default_server_type: server_type = server_type("cx11")
     default_location: location = None
     workers: count = 10
     setup_script: path = None
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/delete.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/logger.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/request.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scale_down.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,31 +13,36 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import time
 import copy
 import logging
 import threading
 
+from datetime import datetime, timezone
 from dataclasses import dataclass
 
 from .actions import Action
 from .scale_up import (
     server_name_prefix,
     runner_name_prefix,
     standby_runner_name_prefix,
+    recycle_server_name_prefix,
+    server_ssh_key_label,
+    uid,
     StandbyRunner,
 )
 from .logger import logger
 
 from github import Github
 from github.Repository import Repository
 from github.SelfHostedActionsRunner import SelfHostedActionsRunner
 
 from hcloud import Client
 from hcloud.servers.client import BoundServer
+from hcloud.ssh_keys.domain import SSHKey
 
 
 @dataclass
 class PoweredOffServer:
     """Powered off server."""
 
     time: float
@@ -59,23 +64,84 @@
     """Unused self-hosted runner."""
 
     time: float
     runner: SelfHostedActionsRunner
     observed_interval: float
 
 
+def recycle_server(reason: str, server: BoundServer, ssh_key: SSHKey, margin=10):
+    """Recycle server."""
+    now = datetime.now(timezone.utc)
+    used = now - server.created
+    days = used.days
+    hours, remainder = divmod(used.seconds, 3600)
+    minutes, _ = divmod(remainder, 60)
+
+    if not server_ssh_key_label in server.labels:
+        with Action(
+            f"Try deleting {reason} server {server.name} "
+            f"used {days}d{hours}h{minutes}m "
+            "as it has no SSH key label",
+            stacklevel=3,
+            ignore_fail=True,
+        ):
+            try:
+                server.delete()
+            finally:
+                return
+
+    if server.labels[server_ssh_key_label] != ssh_key.name:
+        with Action(
+            f"Try deleting {reason} server {server.name} "
+            f"used {days}d{hours}h{minutes}m "
+            "as it has a different SSH key",
+            stacklevel=3,
+            ignore_fail=True,
+        ):
+            try:
+                server.delete()
+            finally:
+                return
+
+    if minutes > (60 - margin):
+        with Action(
+            f"Try deleting {reason} server {server.name} "
+            f"used {days}d{hours}h{minutes}m "
+            "as it is end of life",
+            stacklevel=3,
+            ignore_fail=True,
+        ):
+            try:
+                server.delete()
+            finally:
+                return
+
+    if not server.name.startswith(recycle_server_name_prefix):
+        with Action(
+            f"Marking server {server.name} "
+            f"used {days}d{hours}h{minutes}m "
+            f"for recycling with {60 - minutes}m of life",
+            stacklevel=3,
+            ignore_fail=True,
+        ):
+            server.power_off()
+            server.update(name=f"{recycle_server_name_prefix}{uid()}")
+
+
 def scale_down(
     terminate: threading.Event,
     hetzner_token: str,
     github_token: str,
     github_repository: str,
+    recycle: bool,
     max_powered_off_time: int,
     max_unused_runner_time: int,
     max_runner_registration_time: int,
     interval: int,
+    ssh_key: SSHKey,
     debug: bool = False,
     standby_runners: list[StandbyRunner] = None,
 ):
     """Scale down service by deleting any powered off server,
     any server that has unused runner, or any server that failed to register its
     runner (zombie server).
     """
@@ -90,14 +156,15 @@
         github = Github(login_or_token=github_token, per_page=100)
 
     with Action(f"Getting repository {github_repository}"):
         repo: Repository = github.get_repo(github_repository)
 
     while True:
         current_interval = time.time()
+        recyclable_servers: dict[str] = {}
 
         if terminate.is_set():
             with Action("Terminating scale down service"):
                 break
 
         try:
             with Action("Getting list of servers", level=logging.DEBUG):
@@ -107,30 +174,41 @@
                     for server in servers
                     if server.name.startswith(server_name_prefix)
                 ]
 
             with Action("Getting list of self-hosted runners", level=logging.DEBUG):
                 runners: list[SelfHostedActionsRunner] = repo.get_self_hosted_runners()
 
+            if recycle:
+                with Action("Looking for recyclable servers", level=logging.DEBUG):
+                    for server in servers:
+                        if server.status == server.STATUS_OFF:
+                            if server.name.startswith(recycle_server_name_prefix):
+                                if server.name not in recyclable_servers:
+                                    recyclable_servers[server.name] = server
+
             with Action(
                 "Looking for powered off or zombie servers", level=logging.DEBUG
             ):
                 for server in servers:
                     if server.status == server.STATUS_OFF:
-                        if server.name not in powered_off_servers:
-                            with Action(f"Found new powered off server {server.name}"):
-                                powered_off_servers[server.name] = PoweredOffServer(
-                                    time=time.time(),
-                                    server=server,
-                                    observed_interval=current_interval,
-                                )
-                        powered_off_servers[server.name].server = server
-                        powered_off_servers[
-                            server.name
-                        ].observed_interval = current_interval
+                        if not server.name.startswith(recycle_server_name_prefix):
+                            if server.name not in powered_off_servers:
+                                with Action(
+                                    f"Found new powered off server {server.name}"
+                                ):
+                                    powered_off_servers[server.name] = PoweredOffServer(
+                                        time=time.time(),
+                                        server=server,
+                                        observed_interval=current_interval,
+                                    )
+                            powered_off_servers[server.name].server = server
+                            powered_off_servers[
+                                server.name
+                            ].observed_interval = current_interval
 
                     elif server.status == server.STATUS_RUNNING:
                         if server.name not in [runner.name for runner in runners]:
                             if server.name not in zombie_servers:
                                 with Action(
                                     f"Found new potential zombie server {server.name}"
                                 ):
@@ -193,20 +271,27 @@
                         with Action(
                             f"Forgetting about powered off server {server.name}"
                         ):
                             powered_off_servers.pop(server_name)
 
                     else:
                         if time.time() - powered_off_server.time > max_powered_off_time:
-                            with Action(
-                                f"Deleting powered off server {server_name}",
-                                ignore_fail=True,
-                            ) as action:
-                                powered_off_server.server.delete()
-                                powered_off_servers.pop(server_name)
+                            if recycle:
+                                recycle_server(
+                                    reason="powered off",
+                                    server=powered_off_server.server,
+                                    ssh_key=ssh_key,
+                                )
+                            else:
+                                with Action(
+                                    f"Deleting powered off server {server_name}",
+                                    ignore_fail=True,
+                                ) as action:
+                                    powered_off_server.server.delete()
+                            powered_off_servers.pop(server_name)
 
             with Action(
                 "Checking which zombie servers need to be deleted", level=logging.DEBUG
             ):
                 for server_name in list(zombie_servers.keys()):
                     zombie_server = zombie_servers[server_name]
 
@@ -215,20 +300,27 @@
                             zombie_servers.pop(server_name)
 
                     else:
                         if (
                             time.time() - zombie_server.time
                             > max_runner_registration_time
                         ):
-                            with Action(
-                                f"Deleting zombie server {server_name}",
-                                ignore_fail=True,
-                            ) as action:
-                                zombie_server.server.delete()
-                                zombie_servers.pop(server_name)
+                            if recycle:
+                                recycle_server(
+                                    reason="zombie",
+                                    server=zombie_server.server,
+                                    ssh_key=ssh_key,
+                                )
+                            else:
+                                with Action(
+                                    f"Deleting zombie server {server_name}",
+                                    ignore_fail=True,
+                                ) as action:
+                                    zombie_server.server.delete()
+                            zombie_servers.pop(server_name)
 
             with Action(
                 "Checking which unused runners need to be removed",
                 level=logging.DEBUG,
             ):
 
                 for runner_name in list(unused_runners.keys()):
@@ -245,28 +337,47 @@
                             with Action(
                                 f"Try to find server for the runner {runner_name}",
                                 ignore_fail=True,
                             ):
                                 runner_server = client.servers.get_by_name(runner_name)
 
                             if runner_server is not None:
-                                with Action(
-                                    f"Deleting unused runner server {runner_server.name}",
-                                    ignore_fail=True,
-                                ):
-                                    runner_server.delete()
-                                    runner_server = None
+                                if recycle:
+                                    recycle_server(
+                                        reason="unused runner",
+                                        server=runner_server,
+                                        ssh_key=ssh_key,
+                                    )
+                                else:
+                                    with Action(
+                                        f"Deleting unused runner server {runner_server.name}",
+                                        ignore_fail=True,
+                                    ):
+                                        runner_server.delete()
+                                runner_server = None
 
                             if runner_server is None:
                                 with Action(
                                     f"Removing self-hosted runner {runner_name}",
                                     ignore_fail=True,
                                 ):
                                     repo.remove_self_hosted_runner(unused_runner.runner)
 
+            with Action(
+                "Checking which recyclable servers need to be deleted",
+                level=logging.DEBUG,
+            ):
+                for server_name in list(recyclable_servers.keys()):
+                    recyclable_server = recyclable_servers[server_name]
+                    recycle_server(
+                        reason="unused recyclable",
+                        server=recyclable_server,
+                        ssh_key=ssh_key,
+                    )
+
         except Exception as exc:
             msg = f"❗ Error: {type(exc).__name__} {exc}"
             if debug:
                 logger.exception(f"{msg}\n{exc}")
             else:
                 logger.error(msg)
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scale_up.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import os
 import time
 import uuid
+import random
 import logging
 import threading
 
 from dataclasses import dataclass
 
 from .actions import Action
 from .scripts import Scripts
@@ -47,22 +48,32 @@
 
 from concurrent.futures import ThreadPoolExecutor, Future
 
 server_name_prefix = "github-runner-"
 runner_name_prefix = server_name_prefix
 standby_server_name_prefix = f"{server_name_prefix}standby-"
 standby_runner_name_prefix = standby_server_name_prefix
+recycle_server_name_prefix = f"{server_name_prefix}recycle-"
+server_ssh_key_label = "github-runner-ssh-key"
 
 
 @dataclass
 class RunnerServer:
     name: str
     labels: set[str]
+    server_type: ServerType
+    server_location: Location
     server_status: str = Server.STATUS_STARTING
     status: str = "initializing"  # busy, ready
+    server: BoundServer = None
+
+
+def uid():
+    """Return unique id."""
+    return str(uuid.uuid1()).replace("-", "")
 
 
 def server_setup(
     server: BoundServer,
     setup_script: str,
     startup_script: str,
     github_token: str,
@@ -87,25 +98,26 @@
         )
         GITHUB_RUNNER_TOKEN = content["token"]
 
     with Action("Getting current directory"):
         current_dir = os.path.dirname(__file__)
 
     with Action("Executing setup.sh script"):
-        ssh(server, f"bash -s  < {setup_script}")
+        ssh(server, f"bash -s  < {setup_script}", stacklevel=3)
 
     with Action("Executing startup.sh script"):
         ssh(
             server,
             f"'sudo -u ubuntu "
             f"GITHUB_REPOSITORY=\"{os.getenv('GITHUB_REPOSITORY')}\" "
             f'GITHUB_RUNNER_TOKEN="{GITHUB_RUNNER_TOKEN}" '
             f"GITHUB_RUNNER_GROUP=Default "
             f'GITHUB_RUNNER_LABELS="{runner_labels}" '
             f"bash -s' < {startup_script}",
+            stacklevel=3,
         )
 
 
 def get_server_type(labels: set[str], default: ServerType, label_prefix="type-"):
     """Get server type for the specified job."""
     server_type = None
 
@@ -174,37 +186,33 @@
 
 
 def create_server(
     hetzner_token: str,
     setup_worker_pool: ThreadPoolExecutor,
     labels: set[str],
     name: str,
-    default_server_type: ServerType,
-    default_location: Location,
-    default_image: Image,
-    scripts: Scripts,
+    server_type: ServerType,
+    server_location: Location,
+    server_image: Image,
+    startup_script: str,
+    setup_script: str,
     github_token: str,
     github_repository: str,
     ssh_key: SSHKey,
     timeout=60,
 ):
     """Create specified number of server instances."""
-
     client = Client(token=hetzner_token)
 
-    server_type = get_server_type(labels=labels, default=default_server_type)
-    server_location = get_server_location(labels=labels, default=default_location)
-    server_image = get_server_image(client=client, labels=labels, default=default_image)
-    startup_script = get_startup_script(server_type=server_type, scripts=scripts)
-
     server_labels = {
         f"github-runner-label-{i}": value for i, value in enumerate(labels)
     }
+    server_labels[server_ssh_key_label] = ssh_key.name
 
-    with Action("Validating server labels"):
+    with Action(f"Validating server {name} labels"):
         valid, error_msg = LabelValidator.validate_verbose(labels=server_labels)
         if not valid:
             raise ValueError(f"invalid server labels {server_labels}: {error_msg}")
 
     with Action(f"Creating server {name} with labels {labels}"):
         response = client.servers.create(
             name=name,
@@ -218,15 +226,66 @@
 
     with Action(f"Waiting for server {server.name} to be ready") as action:
         wait_ready(server=server, timeout=timeout, action=action)
 
     setup_worker_pool.submit(
         server_setup,
         server=response.server,
-        setup_script=scripts.setup,
+        setup_script=setup_script,
+        startup_script=startup_script,
+        github_token=github_token,
+        github_repository=github_repository,
+        runner_labels=",".join(labels),
+        timeout=timeout,
+    )
+
+
+def recycle_server(
+    server_name: str,
+    hetzner_token: str,
+    setup_worker_pool: ThreadPoolExecutor,
+    labels: set[str],
+    name: str,
+    server_image: Image,
+    startup_script: str,
+    setup_script: str,
+    github_token: str,
+    github_repository: str,
+    ssh_key: SSHKey,
+    timeout=60,
+):
+    """Create specified number of server instances."""
+    client = Client(token=hetzner_token, poll_interval=1)
+
+    server_labels = {
+        f"github-runner-label-{i}": value for i, value in enumerate(labels)
+    }
+    server_labels[server_ssh_key_label] = ssh_key.name
+
+    with Action(f"Validating server {name} labels"):
+        valid, error_msg = LabelValidator.validate_verbose(labels=server_labels)
+        if not valid:
+            raise ValueError(f"invalid server labels {server_labels}: {error_msg}")
+
+    with Action(f"Get recyclable server {server_name}"):
+        server: BoundServer = client.servers.get_by_name(name=server_name)
+
+    with Action(f"Recycling server {server_name} to make {name}"):
+        server = server.update(name=name, labels=server_labels)
+
+    with Action(f"Rebuilding recycled server {server.name} image"):
+        server.rebuild(image=server_image).wait_until_finished(max_retries=timeout)
+
+    with Action(f"Waiting for server {server.name} to be ready") as action:
+        wait_ready(server=server, timeout=timeout, action=action)
+
+    setup_worker_pool.submit(
+        server_setup,
+        server=server,
+        setup_script=setup_script,
         startup_script=startup_script,
         github_token=github_token,
         github_repository=github_repository,
         runner_labels=",".join(labels),
         timeout=timeout,
     )
 
@@ -279,14 +338,15 @@
             ):
                 return True
     return False
 
 
 def scale_up(
     terminate: threading.Event,
+    recycle: bool,
     with_label: str,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
     hetzner_token: str,
     ssh_key: SSHKey,
@@ -298,51 +358,150 @@
     max_servers_in_workflow_run: int,
     max_server_ready_time: int,
     debug: bool = False,
     standby_runners: list[StandbyRunner] = None,
 ):
     """Scale up service."""
 
+    with Action("Logging in to Hetzner Cloud"):
+        client = Client(token=hetzner_token)
+
     def create_runner_server(
         name: str,
         labels: set[str],
         setup_worker_pool: ThreadPoolExecutor,
         futures: list[Future],
         servers: list[RunnerServer],
     ):
         """Create new server that would provide a runner with given labels."""
+        recyclable_servers: list[BoundServer] = []
+
+        server_type = get_server_type(labels=labels, default=default_server_type)
+        server_location = get_server_location(labels=labels, default=default_location)
+        server_image = get_server_image(
+            client=client, labels=labels, default=default_image
+        )
+        startup_script = get_startup_script(server_type=server_type, scripts=scripts)
+
+        with Action(
+            f"Trying to create server {name}, "
+            f"type: {server_type.name}, "
+            f"location: {server_location.name if server_location else 'any'}, "
+            f"ssh-key: {ssh_key.name}",
+            stacklevel=3,
+            level=logging.DEBUG,
+        ):
+            pass
+
+        if recycle:
+            for server in servers:
+                if server.name.startswith(recycle_server_name_prefix):
+                    recyclable_servers.append(server)
+                    with Action(
+                        f"Trying to see if we can recycle {server.name}, "
+                        f"type: {server.server_type.name}, "
+                        f"location: {server.server_location.name}, "
+                        f"labels: {server.server.labels}",
+                        stacklevel=3,
+                        level=logging.DEBUG,
+                    ):
+                        pass
+
+                    if (
+                        (server.server_type.name == server_type.name)
+                        and (
+                            server_location is None
+                            or server.server_location.name == server_location.name
+                        )
+                        and (
+                            server.server.labels.get("github-runner-ssh-key")
+                            == ssh_key.name
+                        )
+                    ):
+                        future = worker_pool.submit(
+                            recycle_server,
+                            server_name=server.name,
+                            hetzner_token=hetzner_token,
+                            setup_worker_pool=setup_worker_pool,
+                            labels=labels,
+                            name=name,
+                            server_image=server_image,
+                            startup_script=startup_script,
+                            setup_script=scripts.setup,
+                            github_token=github_token,
+                            github_repository=github_repository,
+                            ssh_key=ssh_key,
+                            timeout=max_server_ready_time,
+                        )
+                        future.server_name = name
+                        futures.append(future)
+                        servers.pop(servers.index(server))
+                        servers.append(
+                            RunnerServer(
+                                name=name,
+                                server_type=server_type,
+                                server_location=server_location,
+                                labels=labels,
+                            )
+                        )
+                        return
+                    else:
+                        with Action(
+                            f"Recyclable server {server.name} did not match {name}",
+                            stacklevel=3,
+                            level=logging.DEBUG,
+                        ):
+                            pass
+
         if max_servers is not None:
             if len(servers) >= max_servers:
                 with Action(
-                    f"Maximum number of servers {max_servers} has been reached"
+                    f"Maximum number of servers {max_servers} has been reached",
+                    stacklevel=3,
                 ):
-                    raise StopIteration("maximum number of servers reached")
+                    if recyclable_servers:
+                        random.shuffle(recyclable_servers)
+                        recyclable_server = recyclable_servers.pop()
+
+                        with Action(
+                            f"Deleting randomly picked recyclable server {recyclable_server.name}",
+                            stacklevel=3,
+                            ignore_fail=True,
+                        ):
+                            recyclable_server.server.delete()
+                        servers.pop(servers.index(recyclable_server))
+                    else:
+                        raise StopIteration("maximum number of servers reached")
 
         future = worker_pool.submit(
             create_server,
             hetzner_token=hetzner_token,
             setup_worker_pool=setup_worker_pool,
             labels=labels,
             name=name,
-            default_server_type=default_server_type,
-            default_location=default_location,
-            default_image=default_image,
-            scripts=scripts,
+            server_type=server_type,
+            server_location=server_location,
+            server_image=server_image,
+            setup_script=scripts.setup,
+            startup_script=startup_script,
             github_token=github_token,
             github_repository=github_repository,
             ssh_key=ssh_key,
             timeout=max_server_ready_time,
         )
         future.server_name = name
-
         futures.append(future)
-        servers.append(RunnerServer(name=name, labels=labels))
-
-    with Action("Logging in to Hetzner Cloud"):
-        client = Client(token=hetzner_token)
+        servers.append(
+            RunnerServer(
+                name=name,
+                server_type=server_type,
+                server_location=server_location,
+                labels=labels,
+            )
+        )
 
     with Action("Logging in to GitHub"):
         github = Github(login_or_token=github_token, per_page=100)
 
     with Action(f"Getting repository {github_repository}"):
         repo: Repository = github.get_repo(github_repository)
 
@@ -371,27 +530,33 @@
                             labels=set(
                                 [
                                     value
                                     for name, value in server.labels.items()
                                     if name.startswith("github-runner-label")
                                 ]
                             ),
+                            server_type=server.server_type,
+                            server_location=server.datacenter.location,
+                            server=server,
                         )
                         for server in client.servers.get_all()
                         if server.name.startswith(server_name_prefix)
                     ]
 
                 with Action("Getting list of self-hosted runners", level=logging.DEBUG):
                     runners: list[SelfHostedActionsRunner] = [
                         runner
                         for runner in repo.get_self_hosted_runners()
                         if runner.name.startswith(runner_name_prefix)
                     ]
 
-                with Action("Setting status of servers based on the runner status"):
+                with Action(
+                    "Setting status of servers based on the runner status",
+                    level=logging.DEBUG,
+                ):
                     for runner in runners:
                         for server in servers:
                             if server.name == runner.name:
                                 if runner.status == "online":
                                     server.status = "busy" if runner.busy else "ready"
 
                 with Action("Looking for queued jobs", level=logging.DEBUG):
@@ -419,15 +584,15 @@
                                         with Action(
                                             f"Server already exists for {job.status} {job}",
                                             level=logging.DEBUG,
                                         ):
                                             continue
 
                                     if job.status == "in_progress":
-                                        # check we job is running on a standby runner
+                                        # check if the job is running on a standby runner
                                         if job.raw_data["runner_name"].startswith(
                                             standby_runner_name_prefix
                                         ):
                                             continue
 
                                         with Action(
                                             f"Finding labels for the job from which {job} stole the runner"
@@ -482,15 +647,15 @@
                             if available < standby_runner.count:
                                 for _ in range(standby_runner.count - available):
                                     try:
                                         with Action(
                                             f"Replenishing{' immediately' if replenish_immediately else ''} standby server with {labels}"
                                         ):
                                             create_runner_server(
-                                                name=f"{standby_server_name_prefix}{str(uuid.uuid1()).replace('-','')}",
+                                                name=f"{standby_server_name_prefix}{uid()}",
                                                 labels=labels,
                                                 setup_worker_pool=setup_worker_pool,
                                                 futures=futures,
                                                 servers=servers,
                                             )
                                     except StopIteration:
                                         break
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/server.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,17 @@
 
     attempt = -1
     start_time = time.time()
 
     while True:
         attempt += 1
         with Action(
-            f"Trying to connect to {server.name}@{ip}...{attempt}", ignore_fail=True
+            f"Trying to connect to {server.name}@{ip}...{attempt}",
+            ignore_fail=True,
+            stacklevel=3,
         ):
             returncode = ssh(server, "hostname", check=False)
             if returncode == 0:
                 break
         if time.time() - start_time >= timeout:
             ssh(server, "hostname")
         else:
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/service.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/service.py`

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
+    command += f" --recycle " + "on" if config.recycle else "off"
     command += f" --with-label {config.with_label}" if config.with_label else ""
     command += f" --workers {config.workers}"
     command += f" --default-type {config.default_server_type.name}"
     command += (
         f" --default-location {config.default_location.name}"
         if config.default_location
         else ""
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows/github/runners/shell.py` & `testflows.github.runners-1.4.230802.1135328/testflows/github/runners/shell.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,17 @@
 import time
 import logging
 import subprocess
 
 logger = logging.getLogger("testflows.github.runners")
 
 
-def shell(cmd: str, shell: bool = True, check: bool = True, use_logger=True):
+def shell(
+    cmd: str, shell: bool = True, check: bool = True, use_logger=True, stacklevel=2
+):
     """Execute command."""
     p = subprocess.Popen(
         cmd,
         shell=shell,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         bufsize=1,
@@ -33,15 +35,15 @@
     )
 
     for line in iter(p.stdout.readline, ""):
         if line == "":
             time.sleep(0.1)
             continue
         if use_logger:
-            logger.info(f"   > {line.rstrip()}", stacklevel=2)
+            logger.info(f"   > {line.rstrip()}", stacklevel=stacklevel)
         else:
             print(line.rstrip())
 
     p.wait()
 
     if check:
         assert p.returncode == 0, f"{cmd} returned non-zero exit code {p.returncode}"
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.4.230802.1135328/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.3.230802.1011544
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
@@ -64,14 +47,15 @@
    for any job is the cost of the server for 1 hour plus the cost for one public IPv4 address.
 
 ========
 Features
 ========
 
 * cost efficient on-demand runners using `Hetzner Cloud <https://www.hetzner.com/cloud>`_
+* supports server recycling to minimize costs
 * simple configuration, no Webhooks, no need for AWS lambdas, and no need to setup any GitHub application
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
@@ -438,14 +422,74 @@
 
 :✋ Note:
    Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
    workflow run takes to complete it jobs, if number of jobs in the workflow
    is greater than the value of this option, as compared to the case if all available runners
    would be allowed.
 
+
+=============================
+Recycling Powered Off Servers
+=============================
+
+By default, recycling of powered off servers that has completed executing a job is turned on.
+
+Recycling allows to minimize costs by allowing multiple runners to be brought up on
+the same server instance as Hetzner Cloud bills servers in 1 hour increments.
+Therefore, it is inefficient to delete a server if it only executed a job
+that runs for a few minutes. Instead, the after completing a job the server is powered off
+and if it can be recycled it is rebuild from scratch by reinstalling the image
+thus providing a clean environment for the next job.
+
+Powered off servers are marked as recyclable by changing their name to **github-runner-recycle-{uuid}**.
+
+Recyclable servers are deleted *10* minutes before they reach their end of life, if they were not
+recycled before that. The end of life is calculated on per hour basis.
+
+For example, if the server is running for 2 hours and 50 minutes, then it will be
+considered end of life and deleted as it has *10* minutes or less of useful life.
+However, if the server is running for 2 hours and 30 minutes, then it potentially
+has 30 minutes of life left and it will be kept around to potentially be recycled.
+
+Sometimes a job might need a server that does not match any recyclable servers,
+if the maximum number of runners has been reached **then one of the recyclable servers
+will be picked at random to be deleted** to make room for a new server.
+
+:✋ Note:
+   Randomly deleting a potentially recyclable server is not the most optimal choice,
+   as we could be deleting a server that has higher cost per hour as compared to the others.
+   However, this strategy provides a good-enough behavior in most cases without building
+   server cost comparison analysis into the program as Hetzner Cloud server costs
+   could change at any time.
+
+A recyclable server is recycled for a new job if it matches the following:
+
+* server type matches exactly what the job required or the default type
+* server location matches exactly if job requested a runner in a specific location or the default location is specified
+* server has matching SSH keys
+
+:✋ Note:
+   **Matching server type exactly means that even if a bigger more expensive server type
+   could be potentially recycled it is not used, even though a job that actually requires
+   that expensive server might not be queued before the server's end of life.**
+
+   This is intensional, as we can't predict when a job that actually requires the more expensive
+   server type could be queued. If the program would allow recycling higher server types
+   than actually requested by a job, then we could run into cases when a job
+   that requires smaller and a less expensive server runs on a bigger more expensive server instead.
+   In this case, a job that actually requires the bigger server would force a new expensive server to be created
+   and thus causing more expensive servers to be created than actually necessary.
+
+If needed, you can turn recycling off using the **--recycle {on,off}** option.
+
+.. code-block:: bash
+
+   github-runners --recycle off
+
+
 =============
 Skipping Jobs
 =============
 
 By default, a runner will be created for any **queued** job.
 
 If needed, you can skip creating runners if a job does not have some specified label
@@ -1542,14 +1586,17 @@
 
 * **-v, --version**
   show program's version number and exit
 
 * **--license**
   show program's license and exit
 
+* **-r {on,off}, --recycle {on,off}**
+  turn on or off recycling of powered off servers, either 'on' or 'off', default: *on*
+
 * **-c path, --config path**
   program configuration file
 
 * **--github-token GITHUB_TOKEN**
   GitHub token, default: *$GITHUB_TOKEN* environment variable
 
 * **--github-repository GITHUB_REPOSITORY**
@@ -1561,15 +1608,15 @@
 * **--ssh-key path**
   public SSH key file, default: *~/.ssh/id_rsa.pub*
 
 * **--default-type name**
   default runner server type name, default: *cx11*
 
 * **--default-location name**
-  default runner server location name, default: not specified
+  default runner server location name, default: *not specified*
 
 * **--default-image architecture:type:name_or_description**
   default runner server image type and name or description,
   where the architecture is either: 'x86' or 'arm',
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
```

### Comparing `testflows.github.runners-1.3.230802.1011544/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.4.230802.1135328/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

