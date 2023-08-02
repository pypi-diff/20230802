# Comparing `tmp/testflows.github.runners-1.3.230801.1152824.tar.gz` & `tmp/testflows.github.runners-1.3.230801.1235756.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testflows.github.runners-1.3.230801.1152824.tar", last modified: Tue Aug  1 15:28:25 2023, max compression
+gzip compressed data, was "testflows.github.runners-1.3.230801.1235756.tar", last modified: Tue Aug  1 23:57:57 2023, max compression
```

## Comparing `testflows.github.runners-1.3.230801.1152824.tar` & `testflows.github.runners-1.3.230801.1235756.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/
--rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/LICENSE
--rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    56600 2023-07-31 22:43:07.000000 testflows.github.runners-1.3.230801.1152824/README.rst
--rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/setup.cfg
--rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-01 15:28:24.000000 testflows.github.runners-1.3.230801.1152824/setup.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/
--rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-01 15:28:24.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/actions.py
--rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/api_watch.py
--rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/args.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/bin/
--rwxrwxr-x   0 user      (1000) user      (1000)    24953 2023-08-01 15:27:48.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/bin/github-runners
--rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/cloud.py
--rw-rw-r--   0 user      (1000) user      (1000)     4164 2023-08-01 01:08:42.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/config.py
--rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/delete.py
--rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/logger.py
--rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/request.py
--rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scale_down.py
--rw-rw-r--   0 user      (1000) user      (1000)    17362 2023-08-01 03:14:02.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scale_up.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/
--rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/__init__.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/
--rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/setup.sh
--rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/setup_docker.sh
--rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/startup_arm64.sh
--rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/startup_x64.sh
--rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/server.py
--rw-rw-r--   0 user      (1000) user      (1000)     5158 2023-07-31 17:30:38.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/service.py
--rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1152824/testflows/github/runners/shell.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 15:28:25.103008 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/
--rw-rw-r--   0 user      (1000) user      (1000)    57192 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/not-zip-safe
--rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-01 15:28:25.000000 testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/top_level.txt
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.068637 testflows.github.runners-1.3.230801.1235756/
+-rw-rw-r--   0 user      (1000) user      (1000)      630 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/LICENSE
+-rw-rw-r--   0 user      (1000) user      (1000)    58949 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    58357 2023-08-01 23:57:22.000000 testflows.github.runners-1.3.230801.1235756/README.rst
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2023-08-01 23:57:57.068637 testflows.github.runners-1.3.230801.1235756/setup.cfg
+-rw-rw-r--   0 user      (1000) user      (1000)     2043 2023-08-01 23:57:56.000000 testflows.github.runners-1.3.230801.1235756/setup.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/
+-rw-rw-r--   0 user      (1000) user      (1000)     1376 2023-08-01 23:57:56.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1615 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/actions.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1951 2023-08-01 03:44:03.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/api_watch.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2599 2023-07-31 15:05:55.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/args.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/bin/
+-rwxrwxr-x   0 user      (1000) user      (1000)    25252 2023-08-01 23:26:46.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/bin/github-runners
+-rw-rw-r--   0 user      (1000) user      (1000)    13607 2023-07-29 23:57:40.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/cloud.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4210 2023-08-01 21:03:13.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/config.py
+-rw-rw-r--   0 user      (1000) user      (1000)     2473 2023-07-29 23:43:11.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/delete.py
+-rw-rw-r--   0 user      (1000) user      (1000)      726 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/logger.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1926 2023-07-29 23:39:43.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/request.py
+-rw-rw-r--   0 user      (1000) user      (1000)    11279 2023-08-01 03:43:12.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scale_down.py
+-rw-rw-r--   0 user      (1000) user      (1000)    19139 2023-08-01 23:44:19.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scale_up.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/
+-rw-rw-r--   0 user      (1000) user      (1000)     1061 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/__init__.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/
+-rw-rw-r--   0 user      (1000) user      (1000)      655 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)      519 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      260 2023-07-31 12:43:19.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/setup.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     1148 2023-07-31 12:59:30.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/setup_docker.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      775 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/startup_arm64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)      715 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/startup_x64.sh
+-rw-rw-r--   0 user      (1000) user      (1000)     2522 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/server.py
+-rw-rw-r--   0 user      (1000) user      (1000)     5322 2023-08-01 21:06:23.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/service.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1483 2023-07-29 01:22:14.000000 testflows.github.runners-1.3.230801.1235756/testflows/github/runners/shell.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2023-08-01 23:57:57.064637 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/
+-rw-rw-r--   0 user      (1000) user      (1000)    58949 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)     1192 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2023-07-29 01:22:42.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/not-zip-safe
+-rw-rw-r--   0 user      (1000) user      (1000)       61 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       10 2023-08-01 23:57:57.000000 testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/top_level.txt
```

### Comparing `testflows.github.runners-1.3.230801.1152824/LICENSE` & `testflows.github.runners-1.3.230801.1235756/LICENSE`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/PKG-INFO` & `testflows.github.runners-1.3.230801.1235756/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: testflows.github.runners
-Version: 1.3.230801.1152824
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
@@ -72,14 +55,15 @@
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
+* supports limiting the maximum number of runners used by each workflow run
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ===========
 Limitations
 ===========
 
 **Group runners are not supported**
@@ -299,17 +283,17 @@
 Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
 
 ❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
 
 ❷ Now, create an API token and save it.
 
 For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
-   
+
 ::
-   
+
    5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
 
 You should now have your Hetzner Cloud project ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
@@ -406,14 +390,45 @@
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
+=========================================================
+Specifying Maximum Number of Runners Used in Workflow Run
+=========================================================
+
+By default, the maximum number of runners that could be used by a single workflow run
+is not defined. Therefore, for example, if you have **--max-runners** set to *10*,
+and you have a few workflow runs that are **queued**, and each workflow
+contains more than *10* jobs, then only one workflow run will be running its jobs while
+the jobs in other workflow runs will be waiting as there will be no runners
+available until the run that uses all the runners for its jobs completes.
+
+If you would like for the runners to be divided more evenly between different
+**queued** workflow runs, then you can use the **--max-runners-in-workflow-run**
+option to limit the maximum number of runners used in a single workflow run.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners --max-runners 40 --max-runners-in-workflow-run 5
+
+will allow only up to *5* runners to be used at the maximum in any single workflow run, and
+therefore would allow up to *8* **queued** workflow runs to run up to *5* jobs in each **queued**
+workflow run in parallel.
+
+:✋ Note:
+   Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
+   workflow run takes to complete it jobs, if number of jobs in the workflow
+   is greater than the value of this option, as compared to the case if all available runners
+   would be allowed.
+
 ===============================
 Jobs That Require Docker Engine
 ===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
@@ -738,15 +753,16 @@
 The `Config class`_ has the following schema:
 
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
    * **ssh_key: str**
-   * **max_runners**
+   * **max_runners: count**
+   * **max_runners_in_workflow_run: count**
    * **default_image: image**
    * **default_server_type: server_type**
    * **default_location: location**
    * **workers: count**
    * **setup_script: path**
    * **startup_x64_script: path**
    * **startup_arm64_script: path**
@@ -1279,29 +1295,29 @@
 ==================
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.id}
+   github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any unused runner that for some reason
 does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact *job.id* that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 -------------------------
 Maximum Number of Runners
 -------------------------
 
@@ -1520,14 +1536,17 @@
   where the architecture is either: 'x86' or 'arm',
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
+* **--max-runners-in-workflow-run count**
+  maximum number of runners allowed in a workflow run, default: not set
+
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
```

### Comparing `testflows.github.runners-1.3.230801.1152824/README.rst` & `testflows.github.runners-1.3.230801.1235756/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: testflows.github.runners
+Version: 1.3.230801.1235756
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
@@ -55,14 +72,15 @@
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
+* supports limiting the maximum number of runners used by each workflow run
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ===========
 Limitations
 ===========
 
 **Group runners are not supported**
@@ -282,17 +300,17 @@
 Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
 
 ❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
 
 ❷ Now, create an API token and save it.
 
 For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
-   
+
 ::
-   
+
    5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
 
 You should now have your Hetzner Cloud project ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
@@ -389,14 +407,45 @@
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
+=========================================================
+Specifying Maximum Number of Runners Used in Workflow Run
+=========================================================
+
+By default, the maximum number of runners that could be used by a single workflow run
+is not defined. Therefore, for example, if you have **--max-runners** set to *10*,
+and you have a few workflow runs that are **queued**, and each workflow
+contains more than *10* jobs, then only one workflow run will be running its jobs while
+the jobs in other workflow runs will be waiting as there will be no runners
+available until the run that uses all the runners for its jobs completes.
+
+If you would like for the runners to be divided more evenly between different
+**queued** workflow runs, then you can use the **--max-runners-in-workflow-run**
+option to limit the maximum number of runners used in a single workflow run.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners --max-runners 40 --max-runners-in-workflow-run 5
+
+will allow only up to *5* runners to be used at the maximum in any single workflow run, and
+therefore would allow up to *8* **queued** workflow runs to run up to *5* jobs in each **queued**
+workflow run in parallel.
+
+:✋ Note:
+   Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
+   workflow run takes to complete it jobs, if number of jobs in the workflow
+   is greater than the value of this option, as compared to the case if all available runners
+   would be allowed.
+
 ===============================
 Jobs That Require Docker Engine
 ===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
@@ -721,15 +770,16 @@
 The `Config class`_ has the following schema:
 
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
    * **ssh_key: str**
-   * **max_runners**
+   * **max_runners: count**
+   * **max_runners_in_workflow_run: count**
    * **default_image: image**
    * **default_server_type: server_type**
    * **default_location: location**
    * **workers: count**
    * **setup_script: path**
    * **startup_x64_script: path**
    * **startup_arm64_script: path**
@@ -1262,29 +1312,29 @@
 ==================
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.id}
+   github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any unused runner that for some reason
 does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact *job.id* that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 -------------------------
 Maximum Number of Runners
 -------------------------
 
@@ -1503,14 +1553,17 @@
   where the architecture is either: 'x86' or 'arm',
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
+* **--max-runners-in-workflow-run count**
+  maximum number of runners allowed in a workflow run, default: not set
+
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
```

### Comparing `testflows.github.runners-1.3.230801.1152824/setup.py` & `testflows.github.runners-1.3.230801.1235756/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 with open("README.rst", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 
 setup(
     name="testflows.github.runners",
-    version="1.3.230801.1152824",
+    version="1.3.230801.1235756",
     description="Autoscaling GitHub Actions Runners Using Hetzner Cloud ",
     author="Vitaliy Zakaznikov",
     author_email="vzakaznikov@testflows.com",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/testflows/github-runners",
     classifiers=[
```

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/__init__.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/__init__.py`

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
-__version__ = "1.3.230801.1152824"
+__version__ = "1.3.230801.1235756"
 __license__ = f"""
 Copyright 2023 Katteli Inc.
 TestFlows.com Open-Source Software Testing Framework (http://testflows.com)
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/actions.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/actions.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/api_watch.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/api_watch.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/args.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/args.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/bin/github-runners` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/bin/github-runners`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,21 @@
         "--max-runners",
         metavar="count",
         type=args.count_type,
         help="maximum number of active runners, default: 10",
     )
 
     parser.add_argument(
+        "--max-runners-in-workflow-run",
+        metavar="count",
+        type=args.count_type,
+        help="maximum number of runners allowed for a workflow run, default: not set",
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
@@ -645,14 +652,15 @@
                     default_location=config.default_location,
                     worker_pool=worker_pool,
                     hetzner_token=config.hetzner_token,
                     github_token=config.github_token,
                     github_repository=config.github_repository,
                     interval=config.scale_up_interval,
                     max_servers=config.max_runners,
+                    max_servers_in_workflow_run=config.max_runners_in_workflow_run,
                     max_server_ready_time=config.max_server_ready_time,
                     debug=config.debug,
                     standby_runners=config.standby_runners,
                 )
 
             with Action("Creating scale down service"):
                 scale_down_service: Future = worker_pool.submit(
```

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/cloud.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/cloud.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/config.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     """Program configuration class."""
 
     github_token: str = os.getenv("GITHUB_TOKEN")
     github_repository: str = os.getenv("GITHUB_REPOSITORY")
     hetzner_token: str = os.getenv("HETZNER_TOKEN")
     ssh_key: str = os.path.expanduser("~/.ssh/id_rsa.pub")
     max_runners: count = 10
+    max_runners_in_workflow_run: count = None
     default_image: image = image("x86:system:ubuntu-22.04")
     default_server_type: server_type = server_type("cx11")
     default_location: location = None
     workers: count = 10
     setup_script: path = None
     startup_x64_script: path = None
     startup_arm64_script: path = None
```

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/delete.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/delete.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/logger.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/logger.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/request.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/request.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scale_down.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scale_down.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scale_up.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scale_up.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,27 +258,47 @@
             continue
         if labels.issubset(runner_server.labels):
             count += 1
 
     return count
 
 
+def max_servers_in_workflow_run_reached(
+    run_id, servers: list[BoundServer], max_servers_in_workflow_run: int
+):
+    """Return True if maximum number of servers in workflow run has been reached."""
+    with Action(f"Check maximum number of servers used in workflow run {run_id}"):
+        run_server_name_prefix = f"{server_name_prefix}{run_id}"
+        servers_in_run = [
+            server
+            for server in servers
+            if server.name.startswith(run_server_name_prefix)
+        ]
+        if len(servers_in_run) >= max_servers_in_workflow_run:
+            with Action(
+                f"Maximum number of servers {max_servers_in_workflow_run} for {run_id} has been reached"
+            ):
+                return True
+    return False
+
+
 def scale_up(
     terminate: threading.Event,
     scripts: Scripts,
     worker_pool: ThreadPoolExecutor,
     github_token: str,
     github_repository: str,
     hetzner_token: str,
     ssh_key: SSHKey,
     default_server_type: ServerType,
     default_location: Location,
     default_image: Image,
     interval: int,
     max_servers: int,
+    max_servers_in_workflow_run: int,
     max_server_ready_time: int,
     debug: bool = False,
     standby_runners: list[StandbyRunner] = None,
 ):
     """Scale up service."""
 
     def create_runner_server(
@@ -372,18 +392,28 @@
                             if server.name == runner.name:
                                 if runner.status == "online":
                                     server.status = "busy" if runner.busy else "ready"
 
                 with Action("Looking for queued jobs", level=logging.DEBUG):
                     try:
                         for run in workflow_runs:
+                            if max_servers_in_workflow_run is not None:
+                                if max_servers_in_workflow_run_reached(
+                                    run_id=run.id,
+                                    servers=servers,
+                                    max_servers_in_workflow_run=max_servers_in_workflow_run,
+                                ):
+                                    continue
+
                             for job in run.jobs():
                                 labels = set(job.raw_data["labels"])
 
-                                server_name = f"{server_name_prefix}{job.id}"
+                                server_name = (
+                                    f"{server_name_prefix}{job.run_id}-{job.id}"
+                                )
 
                                 if job.status != "completed":
                                     if server_name in [
                                         server.name for server in servers
                                     ]:
                                         with Action(
                                             f"Server already exists for {job.status} {job}",
@@ -406,14 +436,22 @@
                                                     label["name"]
                                                     for label in repo.get_self_hosted_runner(
                                                         job.raw_data["runner_id"]
                                                     ).labels()
                                                 ]
                                             )
 
+                                    if max_servers_in_workflow_run is not None:
+                                        if max_servers_in_workflow_run_reached(
+                                            run_id=run.id,
+                                            servers=servers,
+                                            max_servers_in_workflow_run=max_servers_in_workflow_run,
+                                        ):
+                                            break
+
                                     with Action(f"Creating new server for {job}"):
                                         create_runner_server(
                                             name=server_name,
                                             labels=labels,
                                             setup_worker_pool=setup_worker_pool,
                                             futures=futures,
                                             servers=servers,
```

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/__init__.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/__init__.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/__init__.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/deploy/setup.sh` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/deploy/setup.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/setup_docker.sh` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/setup_docker.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/startup_arm64.sh` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/startup_arm64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/scripts/startup_x64.sh` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/scripts/startup_x64.sh`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/server.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/server.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/service.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -39,14 +39,19 @@
     command += (
         f" --default-location {config.default_location.name}"
         if config.default_location
         else ""
     )
     command += f" --default-image {config.default_image.architecture}:{config.default_image.type}:{config.default_image.name or config.default_image.description}"
     command += f" --max-runners {config.max_runners}" if config.max_runners else ""
+    command += (
+        f" --max-runners-in-workflow-run {config.max_runners_in_workflow_run}"
+        if config.max_runners_in_workflow_run
+        else ""
+    )
     command += f" --setup-script {config.setup_script}" if config.setup_script else ""
     command += (
         f" --startup-x64-script {config.startup_x64_script}"
         if config.startup_x64_script
         else ""
     )
     command += (
```

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows/github/runners/shell.py` & `testflows.github.runners-1.3.230801.1235756/testflows/github/runners/shell.py`

 * *Files identical despite different names*

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/PKG-INFO` & `testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testflows.github.runners
-Version: 1.3.230801.1152824
+Version: 1.3.230801.1235756
 Summary: Autoscaling GitHub Actions Runners Using Hetzner Cloud 
 Home-page: https://github.com/testflows/github-runners
 Author: Vitaliy Zakaznikov
 Author-email: vzakaznikov@testflows.com
 License: Apache-2.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
@@ -72,14 +72,15 @@
 * supports specifying custom runner server types, images, and locations using job labels
 * self-contained program that you can use to deploy, redeploy, and manage the service on a cloud instance
 * supports x64 (x86) and ARM64 (arm) runners
 * supports using any Hetzner Cloud server types
 * supports runners with pre-installed Docker
 * supports using any standard Hetzner Cloud images and applications
 * supports auto-replenishable fixed standby runner pools for jobs to be picked up immediately
+* supports limiting the maximum number of runners used by each workflow run
 * simpler alternative to what GitHub lists in `Recommended autoscaling solutions <https://docs.github.com/en/actions/hosting-your-own-runners/managing-self-hosted-runners/autoscaling-with-self-hosted-runners#recommended-autoscaling-solutions>`_
 
 ===========
 Limitations
 ===========
 
 **Group runners are not supported**
@@ -299,17 +300,17 @@
 Next you will need to create a Hetzner Cloud project and an API token that we can use to create an manage Hetzner Cloud server instances.
 
 ❶ Create new Hetzner Cloud project **Demo GitHub Runners**.
 
 ❷ Now, create an API token and save it.
 
 For me, the Hetzner Cloud token for my *Demo GitHub Runners* project is:
-   
+
 ::
-   
+
    5Up04IHuY8mC7l0JxKwh3Aps4ghGIyL0NJ9rGlhyAmmkddzuRreR1YstTSTFCG0N
 
 You should now have your Hetzner Cloud project ready.
 
 See these steps in action:
 
 .. image:: https://raw.githubusercontent.com/testflows/TestFlows-GitHub-Runners/master/docs/images/hetzner_create_project_and_token.gif
@@ -406,14 +407,45 @@
 The default maximum number of runners is **10**. You can set a different value
 based on your Hetzner Cloud limits using the **-m count, --max-runners count** option. For example,
 
 .. code-block:: bash
 
    github-runners --max-runners 40
 
+=========================================================
+Specifying Maximum Number of Runners Used in Workflow Run
+=========================================================
+
+By default, the maximum number of runners that could be used by a single workflow run
+is not defined. Therefore, for example, if you have **--max-runners** set to *10*,
+and you have a few workflow runs that are **queued**, and each workflow
+contains more than *10* jobs, then only one workflow run will be running its jobs while
+the jobs in other workflow runs will be waiting as there will be no runners
+available until the run that uses all the runners for its jobs completes.
+
+If you would like for the runners to be divided more evenly between different
+**queued** workflow runs, then you can use the **--max-runners-in-workflow-run**
+option to limit the maximum number of runners used in a single workflow run.
+
+For example,
+
+.. code-block:: bash
+
+   github-runners --max-runners 40 --max-runners-in-workflow-run 5
+
+will allow only up to *5* runners to be used at the maximum in any single workflow run, and
+therefore would allow up to *8* **queued** workflow runs to run up to *5* jobs in each **queued**
+workflow run in parallel.
+
+:✋ Note:
+   Specifying the **--max-runners-in-workflow-run** option will increase the time a specific
+   workflow run takes to complete it jobs, if number of jobs in the workflow
+   is greater than the value of this option, as compared to the case if all available runners
+   would be allowed.
+
 ===============================
 Jobs That Require Docker Engine
 ===============================
 
 For jobs that require Docker to be installed, you can use the standard `Hetzner Docker CE application <https://docs.hetzner.com/cloud/apps/list/docker-ce/>`_
 which can be specified using the **image-** label. See `Specifying Runner Image`_ for more details about specifying custom runner images.
 
@@ -738,15 +770,16 @@
 The `Config class`_ has the following schema:
 
 :schema:
    * **github_token: str**
    * **github_repository: str**
    * **hetzner_token: str**
    * **ssh_key: str**
-   * **max_runners**
+   * **max_runners: count**
+   * **max_runners_in_workflow_run: count**
    * **default_image: image**
    * **default_server_type: server_type**
    * **default_location: location**
    * **workers: count**
    * **setup_script: path**
    * **startup_x64_script: path**
    * **startup_arm64_script: path**
@@ -1279,29 +1312,29 @@
 ==================
 
 The program scales up runners by looking for any jobs that have **queued** status.
 For each such job, a corresponding Hetzner Cloud server instance is created with the following name:
 
 ::
 
-   github-runner-{job.id}
+   github-runner-{job.run_id}-{job.id}
 
 The server is configured using default **setup** and **startup** scripts. The runner name is set
 to be the same as the server name so that servers can be deleted for any unused runner that for some reason
 does not pick up a job for which it was created within the **max-unused-runner-time** period.
 
 :Note:
    Given that the server name is fixed and specific for each *job.id*, if multiple `github-runners` are running in parallel then
    only 1 server will be created for a given `job` and any other attempts to create a server with the same name will be rejected
    by the Hetzner Cloud.
 
 Also,
 
 :Note:
-   There is no guarantee that a given runner will pick the job with the exact **job.id** that caused it to be created.
+   There is no guarantee that a given runner will pick the job with the exact *job.id* that caused it to be created.
    This is expected and because for each **queued** job a unique runner will be created the number of runners will be
    equal the number of jobs and therefore under normal conditions all jobs will be executed as expected.
 
 -------------------------
 Maximum Number of Runners
 -------------------------
 
@@ -1520,14 +1553,17 @@
   where the architecture is either: 'x86' or 'arm',
   and type is either: 'system','snapshot','backup','app',
   default: *system:ubuntu-22.04*
 
 * **-m count, --max-runners count**
   maximum number of active runners, default: *10*
 
+* **--max-runners-in-workflow-run count**
+  maximum number of runners allowed in a workflow run, default: not set
+
 * **-w count, --workers count**
   number of concurrent workers, default: *10*
 
 * **--setup-script path**
   path to custom server setup script
 
 * **--startup-x64-script path**
```

### Comparing `testflows.github.runners-1.3.230801.1152824/testflows.github.runners.egg-info/SOURCES.txt` & `testflows.github.runners-1.3.230801.1235756/testflows.github.runners.egg-info/SOURCES.txt`

 * *Files identical despite different names*

