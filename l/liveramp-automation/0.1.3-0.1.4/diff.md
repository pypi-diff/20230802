# Comparing `tmp/liveramp_automation-0.1.3.tar.gz` & `tmp/liveramp_automation-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-0.1.3.tar", last modified: Wed Aug  2 07:06:12 2023, max compression
+gzip compressed data, was "liveramp_automation-0.1.4.tar", last modified: Wed Aug  2 07:28:09 2023, max compression
```

## Comparing `liveramp_automation-0.1.3.tar` & `liveramp_automation-0.1.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.993700 liveramp_automation-0.1.3/
--rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.1.3/LICENSE
--rw-r--r--   0 jasqia     (502) staff       (20)     2033 2023-08-02 07:06:12.992946 liveramp_automation-0.1.3/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)     1734 2023-08-02 06:57:58.000000 liveramp_automation-0.1.3/README.md
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.962993 liveramp_automation-0.1.3/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.3/liveramp_automation/__init__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.973424 liveramp_automation-0.1.3/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/helper_bucket.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3791 2023-08-01 09:41:57.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/helper_file.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3967 2023-08-02 06:55:22.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/helper_login.py
--rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/helper_notification.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.983464 liveramp_automation-0.1.3/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.3/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1466 2023-08-02 05:31:37.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_allure.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      968 2023-08-02 05:34:33.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      751 2023-08-01 09:07:07.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_playwright.py
--rw-r--r--   0 jasqia     (502) staff       (20)     7462 2023-08-02 05:40:49.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_request.py
--rw-r--r--   0 jasqia     (502) staff       (20)      749 2023-08-01 01:28:11.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_selenium.py
--rw-r--r--   0 jasqia     (502) staff       (20)      988 2023-07-20 06:35:14.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_time.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.968310 liveramp_automation-0.1.3/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     2033 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      995 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 07:06:12.993973 liveramp_automation-0.1.3/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1206 2023-08-02 07:06:01.000000 liveramp_automation-0.1.3/setup.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.985050 liveramp_automation-0.1.3/tests/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.1.3/tests/__init__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.987346 liveramp_automation-0.1.3/tests/test_helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.1.3/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.1.3/tests/test_helpers/test_file.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.990973 liveramp_automation-0.1.3/tests/test_utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.1.3/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      252 2023-08-02 01:35:52.000000 liveramp_automation-0.1.3/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      457 2023-08-02 03:40:11.000000 liveramp_automation-0.1.3/tests/test_utils/test_request.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.407555 liveramp_automation-0.1.4/
+-rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.1.4/LICENSE
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 07:28:09.406802 liveramp_automation-0.1.4/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/README.md
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.375070 liveramp_automation-0.1.4/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.4/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.386914 liveramp_automation-0.1.4/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3786 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3957 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.4/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.397554 liveramp_automation-0.1.4/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.4/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1466 2023-08-02 05:31:37.000000 liveramp_automation-0.1.4/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.1.4/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      968 2023-08-02 05:34:33.000000 liveramp_automation-0.1.4/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     7452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      744 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      988 2023-07-20 06:35:14.000000 liveramp_automation-0.1.4/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.380301 liveramp_automation-0.1.4/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      967 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-02 07:28:09.000000 liveramp_automation-0.1.4/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 07:28:09.407797 liveramp_automation-0.1.4/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-08-02 07:28:07.000000 liveramp_automation-0.1.4/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.399189 liveramp_automation-0.1.4/tests/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.1.4/tests/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.401444 liveramp_automation-0.1.4/tests/test_helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.1.4/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.1.4/tests/test_helpers/test_file.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:28:09.405263 liveramp_automation-0.1.4/tests/test_utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.1.4/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.4/tests/test_utils/test_request.py
```

### Comparing `liveramp_automation-0.1.3/LICENSE` & `liveramp_automation-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.3/PKG-INFO` & `liveramp_automation-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is the base liveramp_automation_framework
-Home-page: https://github.com/LiveRamp/qe_api_framework
+Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # liveramp-automation
 an automation framework helps you qucikly author scripts for any automation testing 
@@ -38,13 +38,13 @@
         We would like to integrate the common helpers and libraries here and then build a lib.
         Later the only thing is to add the cases according to the features. 
         Since most of the common helpers and libraries have been integrated to the lib, 
         you only need to import that lib and methods.
 
 ### 2. Things need to follow:  
 - [x] Create a python repository
-- [x] Create a file named [requirements.txt](requirements.txt) and only input to this file [liveramp-automation](liveramp-automation), you can ignore the version
+- [x] Create a file named [requirements.txt](credentials/requirements.txt) and only input to this file [liveramp-automation](liveramp-automation), you can ignore the version
 - [x] Copy [conftest.py](conftest.py) and [pytest.ini](pytest.ini) to your repository's root directory
 - [x] Author scripts
 - [x] Done
```

### Comparing `liveramp_automation-0.1.3/README.md` & `liveramp_automation-0.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -28,13 +28,13 @@
         We would like to integrate the common helpers and libraries here and then build a lib.
         Later the only thing is to add the cases according to the features. 
         Since most of the common helpers and libraries have been integrated to the lib, 
         you only need to import that lib and methods.
 
 ### 2. Things need to follow:  
 - [x] Create a python repository
-- [x] Create a file named [requirements.txt](requirements.txt) and only input to this file [liveramp-automation](liveramp-automation), you can ignore the version
+- [x] Create a file named [requirements.txt](credentials/requirements.txt) and only input to this file [liveramp-automation](liveramp-automation), you can ignore the version
 - [x] Copy [conftest.py](conftest.py) and [pytest.ini](pytest.ini) to your repository's root directory
 - [x] Author scripts
 - [x] Done
```

### Comparing `liveramp_automation-0.1.3/liveramp_automation/helpers/helper_bucket.py` & `liveramp_automation-0.1.4/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.3/liveramp_automation/helpers/helper_file.py` & `liveramp_automation-0.1.4/liveramp_automation/helpers/file.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import configparser
 import json
 import os
 
 import yaml
-from liveramp_automation.utils.util_log import Logger
+from liveramp_automation.utils.log import Logger
 
 
 class FileHelper:
 
     @staticmethod
     def read_json_report(path) -> dict:
         with open(path, 'r') as file:
```

### Comparing `liveramp_automation-0.1.3/liveramp_automation/helpers/helper_login.py` & `liveramp_automation-0.1.4/liveramp_automation/helpers/login.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import requests
 from selenium.webdriver import Keys
 from selenium.webdriver.common.by import By
-from liveramp_automation.utils.util_log import Logger
-from liveramp_automation.utils.util_time import fixed_wait
+from liveramp_automation.utils.log import Logger
+from liveramp_automation.utils.time import fixed_wait
 
 
 class LoginHepler:
 
     @staticmethod
     def liveramp_okta_login_page(page, config, username, password):
         """
```

### Comparing `liveramp_automation-0.1.3/liveramp_automation/utils/util_allure.py` & `liveramp_automation-0.1.4/liveramp_automation/utils/allure.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.3/liveramp_automation/utils/util_log.py` & `liveramp_automation-0.1.4/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.3/liveramp_automation/utils/util_parsers.py` & `liveramp_automation-0.1.4/liveramp_automation/utils/parsers.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.3/liveramp_automation/utils/util_playwright.py` & `liveramp_automation-0.1.4/liveramp_automation/utils/playwright.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib.parse import urlparse, urlunsplit
-from liveramp_automation.utils.util_time import MACROS
+from liveramp_automation.utils.time import MACROS
 
 
 class PlaywrightUtils:
 
     def navigate_url(page, scheme=None, host_name=None, path=None, query=None):
         parsed_uri = urlparse(page.url)
         page.goto(urlunsplit((parsed_uri.scheme if scheme is None else scheme,
```

### Comparing `liveramp_automation-0.1.3/liveramp_automation/utils/util_request.py` & `liveramp_automation-0.1.4/liveramp_automation/utils/request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import requests
-from liveramp_automation.utils.util_allure import *
-from liveramp_automation.utils.util_log import Logger
+from liveramp_automation.utils.allure import *
+from liveramp_automation.utils.log import Logger
 
 
 # These are 7 types of methods to call the APIs.Each API allows to multiple parameters.
 # We also added some log/report_content while calling the APIs which would be helpful to check the errors.
 
 def request_post(url, headers, data=None, json=None, **kwargs):
     """
```

### Comparing `liveramp_automation-0.1.3/liveramp_automation/utils/util_selenium.py` & `liveramp_automation-0.1.4/liveramp_automation/utils/selenium.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from urllib.parse import urlparse, urlunsplit
-from liveramp_automation.utils.util_time import MACROS
+from liveramp_automation.utils.time import MACROS
 
 
 class SeleniumUtils:
 
     def navigate_url(driver, scheme=None, host_name=None, path=None, query=None):
         parsed_uri = urlparse(driver.url)
         driver.get(urlunsplit((parsed_uri.scheme if scheme is None else scheme,
```

### Comparing `liveramp_automation-0.1.3/liveramp_automation/utils/util_time.py` & `liveramp_automation-0.1.4/liveramp_automation/utils/time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.3/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-0.1.4/liveramp_automation.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 0.1.3
+Version: 0.1.4
 Summary: This is the base liveramp_automation_framework
-Home-page: https://github.com/LiveRamp/qe_api_framework
+Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # liveramp-automation
 an automation framework helps you qucikly author scripts for any automation testing 
@@ -38,13 +38,13 @@
         We would like to integrate the common helpers and libraries here and then build a lib.
         Later the only thing is to add the cases according to the features. 
         Since most of the common helpers and libraries have been integrated to the lib, 
         you only need to import that lib and methods.
 
 ### 2. Things need to follow:  
 - [x] Create a python repository
-- [x] Create a file named [requirements.txt](requirements.txt) and only input to this file [liveramp-automation](liveramp-automation), you can ignore the version
+- [x] Create a file named [requirements.txt](credentials/requirements.txt) and only input to this file [liveramp-automation](liveramp-automation), you can ignore the version
 - [x] Copy [conftest.py](conftest.py) and [pytest.ini](pytest.ini) to your repository's root directory
 - [x] Author scripts
 - [x] Done
```

### Comparing `liveramp_automation-0.1.3/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-0.1.4/liveramp_automation.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 LICENSE
 README.md
 setup.py
 liveramp_automation/__init__.py
+liveramp_automation/__version__.py
 liveramp_automation.egg-info/PKG-INFO
 liveramp_automation.egg-info/SOURCES.txt
 liveramp_automation.egg-info/dependency_links.txt
 liveramp_automation.egg-info/requires.txt
 liveramp_automation.egg-info/top_level.txt
 liveramp_automation/helpers/__init__.py
-liveramp_automation/helpers/helper_bucket.py
-liveramp_automation/helpers/helper_file.py
-liveramp_automation/helpers/helper_login.py
-liveramp_automation/helpers/helper_notification.py
+liveramp_automation/helpers/bucket.py
+liveramp_automation/helpers/file.py
+liveramp_automation/helpers/login.py
+liveramp_automation/helpers/notification.py
 liveramp_automation/utils/__init__.py
-liveramp_automation/utils/util_allure.py
-liveramp_automation/utils/util_log.py
-liveramp_automation/utils/util_parsers.py
-liveramp_automation/utils/util_playwright.py
-liveramp_automation/utils/util_request.py
-liveramp_automation/utils/util_selenium.py
-liveramp_automation/utils/util_time.py
+liveramp_automation/utils/allure.py
+liveramp_automation/utils/log.py
+liveramp_automation/utils/parsers.py
+liveramp_automation/utils/playwright.py
+liveramp_automation/utils/request.py
+liveramp_automation/utils/selenium.py
+liveramp_automation/utils/time.py
 tests/__init__.py
 tests/test_helpers/__init__.py
 tests/test_helpers/test_file.py
 tests/test_utils/__init__.py
 tests/test_utils/test_log.py
 tests/test_utils/test_request.py
```

### Comparing `liveramp_automation-0.1.3/setup.py` & `liveramp_automation-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from setuptools import setup,find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation',
-    version='0.1.3',
+    version='0.1.4',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/LiveRamp/qe_api_framework",
-    # packages=['liveramp_automation'],
+    url="https://github.com/LiveRamp/liveramp-automation",
     packages= find_packages(),
     install_requires=[
         'pytest',
         'pytest-bdd',
         'pytest-playwright',
         'allure-pytest-bdd',
         'allure-python-commons',
```

