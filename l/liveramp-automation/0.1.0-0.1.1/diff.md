# Comparing `tmp/liveramp_automation-0.1.0.tar.gz` & `tmp/liveramp_automation-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-0.1.0.tar", last modified: Wed Aug  2 01:06:47 2023, max compression
+gzip compressed data, was "liveramp_automation-0.1.1.tar", last modified: Wed Aug  2 01:21:46 2023, max compression
```

## Comparing `liveramp_automation-0.1.0.tar` & `liveramp_automation-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,32 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:06:47.166523 liveramp_automation-0.1.0/
--rw-r--r--   0 jasqia     (502) staff       (20)     1100 2023-08-01 09:13:05.000000 liveramp_automation-0.1.0/LICENSE
--rw-r--r--   0 jasqia     (502) staff       (20)     1697 2023-08-02 01:06:47.166054 liveramp_automation-0.1.0/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)     1398 2023-07-19 08:48:17.000000 liveramp_automation-0.1.0/README.md
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:06:47.158715 liveramp_automation-0.1.0/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.0/liveramp_automation/__init__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:06:47.163400 liveramp_automation-0.1.0/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     1697 2023-08-02 01:06:47.000000 liveramp_automation-0.1.0/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      316 2023-08-02 01:06:47.000000 liveramp_automation-0.1.0/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 01:06:47.000000 liveramp_automation-0.1.0/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 01:06:47.000000 liveramp_automation-0.1.0/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-08-02 01:06:47.000000 liveramp_automation-0.1.0/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 01:06:47.166694 liveramp_automation-0.1.0/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1159 2023-08-02 01:06:43.000000 liveramp_automation-0.1.0/setup.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:06:47.165108 liveramp_automation-0.1.0/tests/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 09:02:07.000000 liveramp_automation-0.1.0/tests/test_file.py
--rw-r--r--   0 jasqia     (502) staff       (20)      559 2023-08-01 09:11:03.000000 liveramp_automation-0.1.0/tests/test_playwright.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.218821 liveramp_automation-0.1.1/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1100 2023-08-01 09:13:05.000000 liveramp_automation-0.1.1/LICENSE
+-rw-r--r--   0 jasqia     (502) staff       (20)     1697 2023-08-02 01:21:46.218296 liveramp_automation-0.1.1/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1398 2023-07-19 08:48:17.000000 liveramp_automation-0.1.1/README.md
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.196714 liveramp_automation-0.1.1/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.1/liveramp_automation/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.206708 liveramp_automation-0.1.1/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/helper_bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3791 2023-08-01 09:41:57.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/helper_file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3596 2023-08-01 09:38:55.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/helper_login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/helper_notification.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.215418 liveramp_automation-0.1.1/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.1/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1057 2023-07-20 06:17:22.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2976 2023-08-01 01:06:55.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      902 2023-07-20 09:35:55.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      751 2023-08-01 09:07:07.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     7316 2023-08-01 01:28:11.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      749 2023-08-01 01:28:11.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      988 2023-07-20 06:35:14.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.201855 liveramp_automation-0.1.1/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     1697 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      867 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 01:21:46.219060 liveramp_automation-0.1.1/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1206 2023-08-02 01:21:44.000000 liveramp_automation-0.1.1/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.217413 liveramp_automation-0.1.1/tests/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 09:02:07.000000 liveramp_automation-0.1.1/tests/test_file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      559 2023-08-01 09:11:03.000000 liveramp_automation-0.1.1/tests/test_playwright.py
```

### Comparing `liveramp_automation-0.1.0/LICENSE` & `liveramp_automation-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.0/PKG-INFO` & `liveramp_automation-0.1.1/liveramp_automation.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: liveramp_automation
-Version: 0.1.0
+Name: liveramp-automation
+Version: 0.1.1
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.1.0/README.md` & `liveramp_automation-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.0/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: liveramp-automation
-Version: 0.1.0
+Name: liveramp_automation
+Version: 0.1.1
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.1.0/setup.py` & `liveramp_automation-0.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from setuptools import setup
+from setuptools import setup,find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation',
-    version='0.1.0',
+    version='0.1.1',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
-    packages=['liveramp_automation'],
+    # packages=['liveramp_automation'],
+    packages= find_packages(),
     install_requires=[
         'pytest',
         'pytest-bdd',
         'pytest-playwright',
         'allure-pytest-bdd',
         'allure-python-commons',
         'google',
```

### Comparing `liveramp_automation-0.1.0/tests/test_playwright.py` & `liveramp_automation-0.1.1/tests/test_playwright.py`

 * *Files identical despite different names*

