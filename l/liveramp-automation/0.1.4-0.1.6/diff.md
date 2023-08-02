# Comparing `tmp/liveramp_automation-0.1.4.tar.gz` & `tmp/liveramp_automation-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-0.1.4.tar", last modified: Wed Aug  2 07:28:09 2023, max compression
+gzip compressed data, was "liveramp_automation-0.1.6.tar", last modified: Wed Aug  2 07:31:20 2023, max compression
```

## Comparing `liveramp_automation-0.1.4.tar` & `liveramp_automation-0.1.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.407555 liveramp_automation-0.1.4/
--rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.1.4/LICENSE
--rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 07:28:09.406802 liveramp_automation-0.1.4/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/README.md
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.375070 liveramp_automation-0.1.4/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.4/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.386914 liveramp_automation-0.1.4/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3786 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3957 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.397554 liveramp_automation-0.1.4/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.4/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1466 2023-08-02 05:31:37.000000 liveramp_automation-0.1.4/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.1.4/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      968 2023-08-02 05:34:33.000000 liveramp_automation-0.1.4/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (502) staff       (20)     7452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (502) staff       (20)      744 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (502) staff       (20)      988 2023-07-20 06:35:14.000000 liveramp_automation-0.1.4/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.380301 liveramp_automation-0.1.4/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      967 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 07:28:09.407797 liveramp_automation-0.1.4/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-08-02 07:28:07.000000 liveramp_automation-0.1.4/setup.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.399189 liveramp_automation-0.1.4/tests/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.1.4/tests/__init__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.401444 liveramp_automation-0.1.4/tests/test_helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.1.4/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.1.4/tests/test_helpers/test_file.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.405263 liveramp_automation-0.1.4/tests/test_utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.1.4/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/tests/test_utils/test_request.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.062776 liveramp_automation-0.1.6/
+-rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.1.6/LICENSE
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 07:31:20.062092 liveramp_automation-0.1.6/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/README.md
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.033259 liveramp_automation-0.1.6/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.6/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.044022 liveramp_automation-0.1.6/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3786 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3957 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.053341 liveramp_automation-0.1.6/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.6/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1466 2023-08-02 05:31:37.000000 liveramp_automation-0.1.6/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.1.6/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      968 2023-08-02 05:34:33.000000 liveramp_automation-0.1.6/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     7452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      744 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      988 2023-07-20 06:35:14.000000 liveramp_automation-0.1.6/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.038296 liveramp_automation-0.1.6/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      967 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 07:31:20.063028 liveramp_automation-0.1.6/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-08-02 07:31:06.000000 liveramp_automation-0.1.6/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.054527 liveramp_automation-0.1.6/tests/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.1.6/tests/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.056762 liveramp_automation-0.1.6/tests/test_helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.1.6/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.1.6/tests/test_helpers/test_file.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.060761 liveramp_automation-0.1.6/tests/test_utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.1.6/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/tests/test_utils/test_request.py
```

### Comparing `liveramp_automation-0.1.4/LICENSE` & `liveramp_automation-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/PKG-INFO` & `liveramp_automation-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 0.1.4
+Version: 0.1.6
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.1.4/README.md` & `liveramp_automation-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/helpers/bucket.py` & `liveramp_automation-0.1.6/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/helpers/file.py` & `liveramp_automation-0.1.6/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/helpers/login.py` & `liveramp_automation-0.1.6/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/utils/allure.py` & `liveramp_automation-0.1.6/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/utils/log.py` & `liveramp_automation-0.1.6/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/utils/parsers.py` & `liveramp_automation-0.1.6/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/utils/playwright.py` & `liveramp_automation-0.1.6/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/utils/request.py` & `liveramp_automation-0.1.6/liveramp_automation/utils/request.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/utils/selenium.py` & `liveramp_automation-0.1.6/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation/utils/time.py` & `liveramp_automation-0.1.6/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-0.1.6/liveramp_automation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 0.1.4
+Version: 0.1.6
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.1.4/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-0.1.6/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.4/setup.py` & `liveramp_automation-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation',
-    version='0.1.4',
+    version='0.1.6',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/liveramp-automation",
     packages= find_packages(),
```

