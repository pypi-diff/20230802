# Comparing `tmp/neo-cli-0.9.5.tar.gz` & `tmp/neo-cli-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo-cli-0.9.5.tar", last modified: Wed Aug  2 10:11:25 2023, max compression
+gzip compressed data, was "neo-cli-0.9.6.tar", last modified: Wed Aug  2 10:39:08 2023, max compression
```

## Comparing `neo-cli-0.9.5.tar` & `neo-cli-0.9.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxr-x   0 efenfauzi  (1000) efenfauzi  (1000)        0 2023-08-02 10:11:25.143699 neo-cli-0.9.5/
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     1080 2023-08-02 09:40:20.000000 neo-cli-0.9.5/LICENSE
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      179 2023-08-02 09:40:20.000000 neo-cli-0.9.5/MANIFEST.in
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     3873 2023-08-02 10:11:25.143699 neo-cli-0.9.5/PKG-INFO
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     3285 2023-08-02 10:08:26.000000 neo-cli-0.9.5/README.rst
-drwxrwxr-x   0 efenfauzi  (1000) efenfauzi  (1000)        0 2023-08-02 10:11:25.139699 neo-cli-0.9.5/neo/
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)       22 2023-08-02 10:04:08.000000 neo-cli-0.9.5/neo/__init__.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     1656 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/cli.py
-drwxrwxr-x   0 efenfauzi  (1000) efenfauzi  (1000)        0 2023-08-02 10:11:25.143699 neo-cli-0.9.5/neo/clis/
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      204 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/__init__.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     8605 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/attach.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      431 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/base.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     3397 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/create.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     1653 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/log.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     2071 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/login.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      197 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/logout.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     6029 2023-08-02 10:04:08.000000 neo-cli-0.9.5/neo/clis/ls.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     3402 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/rm.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     1455 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/update.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     4389 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/clis/vm.py
-drwxrwxr-x   0 efenfauzi  (1000) efenfauzi  (1000)        0 2023-08-02 10:11:25.143699 neo-cli-0.9.5/neo/libs/
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)        0 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/__init__.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      644 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/image.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     2775 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/interactive_ssh_utils.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      972 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/lambdafunc.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)    10979 2023-08-02 10:04:08.000000 neo-cli-0.9.5/neo/libs/login.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     6279 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/ncurses.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     4685 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/network.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     7645 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/orchestration.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     8451 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/prompt.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      843 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/storage.py
-drwxrwxr-x   0 efenfauzi  (1000) efenfauzi  (1000)        0 2023-08-02 10:11:25.143699 neo-cli-0.9.5/neo/libs/templates/
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     6657 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/templates/repo.yml
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)    14804 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/utils.py
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     5378 2023-08-02 09:40:20.000000 neo-cli-0.9.5/neo/libs/vm.py
-drwxrwxr-x   0 efenfauzi  (1000) efenfauzi  (1000)        0 2023-08-02 10:11:25.143699 neo-cli-0.9.5/neo_cli.egg-info/
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      587 2023-08-02 10:11:24.000000 neo-cli-0.9.5/neo_cli.egg-info/SOURCES.txt
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      108 2023-08-02 09:40:20.000000 neo-cli-0.9.5/requirements-dev.txt
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)      454 2023-08-02 09:40:20.000000 neo-cli-0.9.5/requirements.txt
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)       83 2023-08-02 10:11:25.147699 neo-cli-0.9.5/setup.cfg
--rw-rw-r--   0 efenfauzi  (1000) efenfauzi  (1000)     1200 2023-08-02 09:40:20.000000 neo-cli-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 10:39:08.967712 neo-cli-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (122)     1080 2023-08-02 10:38:50.000000 neo-cli-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-08-02 10:38:50.000000 neo-cli-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3873 2023-08-02 10:39:08.967712 neo-cli-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3285 2023-08-02 10:39:05.000000 neo-cli-0.9.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 10:39:08.967712 neo-cli-0.9.6/neo/
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1656 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 10:39:08.967712 neo-cli-0.9.6/neo/clis/
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8605 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/attach.py
+-rw-r--r--   0 runner    (1001) docker     (122)      431 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3397 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/create.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1653 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2071 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/logout.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6029 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/ls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3402 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/rm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1455 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/update.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4389 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/clis/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 10:39:08.967712 neo-cli-0.9.6/neo/libs/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      644 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/image.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2775 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/interactive_ssh_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      972 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/lambdafunc.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10979 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/login.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6279 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/ncurses.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4685 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/network.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7645 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/orchestration.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8451 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (122)      843 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 10:39:08.967712 neo-cli-0.9.6/neo/libs/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)     6657 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/templates/repo.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    14804 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5378 2023-08-02 10:38:50.000000 neo-cli-0.9.6/neo/libs/vm.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-02 10:39:08.967712 neo-cli-0.9.6/neo_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      587 2023-08-02 10:39:08.000000 neo-cli-0.9.6/neo_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      108 2023-08-02 10:38:50.000000 neo-cli-0.9.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-08-02 10:38:50.000000 neo-cli-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       83 2023-08-02 10:39:08.967712 neo-cli-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1200 2023-08-02 10:38:50.000000 neo-cli-0.9.6/setup.py
```

### Comparing `neo-cli-0.9.5/LICENSE` & `neo-cli-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/PKG-INFO` & `neo-cli-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo-cli
-Version: 0.9.5
+Version: 0.9.6
 Summary: A NEO command line tools
 Home-page: https://github.com/BiznetGIO/neo-cli
 Author: BiznetGio
 Author-email: support@biznetgio.com
 License: MIT license
 Keywords: cli
 Classifier: Intended Audience :: Developers
```

### Comparing `neo-cli-0.9.5/README.rst` & `neo-cli-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/cli.py` & `neo-cli-0.9.6/neo/cli.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/clis/attach.py` & `neo-cli-0.9.6/neo/clis/attach.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/clis/create.py` & `neo-cli-0.9.6/neo/clis/create.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/clis/log.py` & `neo-cli-0.9.6/neo/clis/log.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/clis/login.py` & `neo-cli-0.9.6/neo/clis/login.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/clis/ls.py` & `neo-cli-0.9.6/neo/clis/ls.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/clis/rm.py` & `neo-cli-0.9.6/neo/clis/rm.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/clis/update.py` & `neo-cli-0.9.6/neo/clis/update.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/clis/vm.py` & `neo-cli-0.9.6/neo/clis/vm.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/image.py` & `neo-cli-0.9.6/neo/libs/image.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/interactive_ssh_utils.py` & `neo-cli-0.9.6/neo/libs/interactive_ssh_utils.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/lambdafunc.py` & `neo-cli-0.9.6/neo/libs/lambdafunc.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/login.py` & `neo-cli-0.9.6/neo/libs/login.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/ncurses.py` & `neo-cli-0.9.6/neo/libs/ncurses.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/network.py` & `neo-cli-0.9.6/neo/libs/network.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/orchestration.py` & `neo-cli-0.9.6/neo/libs/orchestration.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/prompt.py` & `neo-cli-0.9.6/neo/libs/prompt.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/storage.py` & `neo-cli-0.9.6/neo/libs/storage.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/templates/repo.yml` & `neo-cli-0.9.6/neo/libs/templates/repo.yml`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/utils.py` & `neo-cli-0.9.6/neo/libs/utils.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo/libs/vm.py` & `neo-cli-0.9.6/neo/libs/vm.py`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/neo_cli.egg-info/SOURCES.txt` & `neo-cli-0.9.6/neo_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neo-cli-0.9.5/setup.py` & `neo-cli-0.9.6/setup.py`

 * *Files identical despite different names*

