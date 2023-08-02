# Comparing `tmp/b_aws_testing_framework-1.0.0.tar.gz` & `tmp/b_aws_testing_framework-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "b_aws_testing_framework-1.0.0.tar", last modified: Tue Aug  1 09:52:03 2023, max compression
+gzip compressed data, was "b_aws_testing_framework-1.0.1.tar", last modified: Wed Aug  2 12:15:04 2023, max compression
```

## Comparing `b_aws_testing_framework-1.0.0.tar` & `b_aws_testing_framework-1.0.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     2840 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)    11357 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      164 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    10064 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4389 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)        5 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.506086 b_aws_testing_framework-1.0.0/b_aws_testing_framework/
--rw-r--r--   0 root         (0) root         (0)      538 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3945 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/base_testing_manager.py
--rw-r--r--   0 root         (0) root         (0)     2037 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/credentials.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1807 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/cdk_tool_config.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/testing_manager.py
--rw-r--r--   0 root         (0) root         (0)     3406 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/testing_stack.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/cf_tool_config.py
--rw-r--r--   0 root         (0) root         (0)     2075 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/stack_waiter.py
--rw-r--r--   0 root         (0) root         (0)     2899 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/testing_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/
--rw-r--r--   0 root         (0) root         (0)    10064 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1720 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      166 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       53 2023-08-01 09:52:03.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.502086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.510086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/__init__.py
--rw-r--r--   0 root         (0) root         (0)      164 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/app.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/conftest.py
--rw-r--r--   0 root         (0) root         (0)      514 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/infrastructure.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_outputs.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_stack_exists.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1104 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/test_stack_exists.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-08-01 09:52:03.514086 b_aws_testing_framework-1.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1353 2023-08-01 09:49:18.000000 b_aws_testing_framework-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/HISTORY.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4389 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.257754 b_aws_testing_framework-1.0.1/b_aws_testing_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3945 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/base_testing_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.257754 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.257754 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cdk_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cdk_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cdk_testing/cdk_tool_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cdk_testing/testing_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3406 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cdk_testing/testing_stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cf_testing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cf_testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cf_testing/cf_tool_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cf_testing/stack_waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cf_testing/testing_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.257754 b_aws_testing_framework-1.0.1/b_aws_testing_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7788 2023-08-02 12:15:04.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-08-02 12:15:04.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 12:15:04.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-02 12:15:04.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-02 12:15:04.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.257754 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/infrastructure.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_stack_exists.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cf/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cf/tests/test_stack_exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 12:15:04.261755 b_aws_testing_framework-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-08-02 12:11:51.000000 b_aws_testing_framework-1.0.1/setup.py
```

### Comparing `b_aws_testing_framework-1.0.0/HISTORY.md` & `b_aws_testing_framework-1.0.1/HISTORY.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Release history
 
+### 1.0.1
+* Update pipelines to fix "unclosed SSLSocket" warnings.
+
 ### 1.0.0
 * Upgrade CDK support from v1 to v2.
 * Upgrade GitHub pipelines checkout version from v2 to v3.
 * Upgrade biomapas/cicd-full image version to 5.0.0.
 
 ### 0.6.0
 * Too many bugs. Revert.
```

### Comparing `b_aws_testing_framework-1.0.0/LICENSE` & `b_aws_testing_framework-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/README.md` & `b_aws_testing_framework-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework/__init__.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework/base_testing_manager.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework/base_testing_manager.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework/credentials.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework/credentials.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/cdk_tool_config.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cdk_testing/cdk_tool_config.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/testing_manager.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cdk_testing/testing_manager.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cdk_testing/testing_stack.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cdk_testing/testing_stack.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/stack_waiter.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cf_testing/stack_waiter.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework/tools/cf_testing/testing_manager.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework/tools/cf_testing/testing_manager.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework.egg-info/SOURCES.txt` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/conftest.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/conftest.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/infrastructure.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/infrastructure.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_stack_exists.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cdk/tests/test_stack_exists.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/conftest.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cf/conftest.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/b_aws_testing_framework_test/tools/testing_with_cf/tests/test_stack_exists.py` & `b_aws_testing_framework-1.0.1/b_aws_testing_framework_test/tools/testing_with_cf/tests/test_stack_exists.py`

 * *Files identical despite different names*

### Comparing `b_aws_testing_framework-1.0.0/setup.py` & `b_aws_testing_framework-1.0.1/setup.py`

 * *Files identical despite different names*

