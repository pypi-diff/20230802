# Comparing `tmp/liveramp_automation-0.1.6.tar.gz` & `tmp/liveramp_automation-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-0.1.6.tar", last modified: Wed Aug  2 07:31:20 2023, max compression
+gzip compressed data, was "liveramp_automation-0.1.7.tar", last modified: Wed Aug  2 08:05:15 2023, max compression
```

## Comparing `liveramp_automation-0.1.6.tar` & `liveramp_automation-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.062776 liveramp_automation-0.1.6/
--rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.1.6/LICENSE
--rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 07:31:20.062092 liveramp_automation-0.1.6/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/README.md
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.033259 liveramp_automation-0.1.6/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.6/liveramp_automation/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/__version__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.044022 liveramp_automation-0.1.6/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/bucket.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3786 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/file.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3957 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/login.py
--rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.6/liveramp_automation/helpers/notification.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.053341 liveramp_automation-0.1.6/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.6/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1466 2023-08-02 05:31:37.000000 liveramp_automation-0.1.6/liveramp_automation/utils/allure.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.1.6/liveramp_automation/utils/log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      968 2023-08-02 05:34:33.000000 liveramp_automation-0.1.6/liveramp_automation/utils/parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/utils/playwright.py
--rw-r--r--   0 jasqia     (502) staff       (20)     7452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/utils/request.py
--rw-r--r--   0 jasqia     (502) staff       (20)      744 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/liveramp_automation/utils/selenium.py
--rw-r--r--   0 jasqia     (502) staff       (20)      988 2023-07-20 06:35:14.000000 liveramp_automation-0.1.6/liveramp_automation/utils/time.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.038296 liveramp_automation-0.1.6/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      967 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-02 07:31:19.000000 liveramp_automation-0.1.6/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 07:31:20.063028 liveramp_automation-0.1.6/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1169 2023-08-02 07:31:06.000000 liveramp_automation-0.1.6/setup.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.054527 liveramp_automation-0.1.6/tests/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.1.6/tests/__init__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.056762 liveramp_automation-0.1.6/tests/test_helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.1.6/tests/test_helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.1.6/tests/test_helpers/test_file.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:31:20.060761 liveramp_automation-0.1.6/tests/test_utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.1.6/tests/test_utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/tests/test_utils/test_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.6/tests/test_utils/test_request.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.376174 liveramp_automation-0.1.7/
+-rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.1.7/LICENSE
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 08:05:15.375715 liveramp_automation-0.1.7/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/README.md
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.347791 liveramp_automation-0.1.7/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.7/liveramp_automation/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      479 2023-08-02 08:05:03.000000 liveramp_automation-0.1.7/liveramp_automation/__version__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.359014 liveramp_automation-0.1.7/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3786 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3957 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.7/liveramp_automation/helpers/notification.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.368823 liveramp_automation-0.1.7/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.7/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1369 2023-08-02 08:00:32.000000 liveramp_automation-0.1.7/liveramp_automation/utils/allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.1.7/liveramp_automation/utils/log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      993 2023-08-02 08:00:32.000000 liveramp_automation-0.1.7/liveramp_automation/utils/parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      746 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/liveramp_automation/utils/playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     8161 2023-08-02 08:00:32.000000 liveramp_automation-0.1.7/liveramp_automation/utils/request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      744 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/liveramp_automation/utils/selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1091 2023-08-02 08:02:29.000000 liveramp_automation-0.1.7/liveramp_automation/utils/time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.353211 liveramp_automation-0.1.7/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     2048 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      967 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-02 08:05:15.000000 liveramp_automation-0.1.7/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 08:05:15.376343 liveramp_automation-0.1.7/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1334 2023-08-02 08:05:03.000000 liveramp_automation-0.1.7/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.370020 liveramp_automation-0.1.7/tests/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.1.7/tests/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.371550 liveramp_automation-0.1.7/tests/test_helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.1.7/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.1.7/tests/test_helpers/test_file.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 08:05:15.374186 liveramp_automation-0.1.7/tests/test_utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.1.7/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      247 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      452 2023-08-02 07:24:03.000000 liveramp_automation-0.1.7/tests/test_utils/test_request.py
```

### Comparing `liveramp_automation-0.1.6/LICENSE` & `liveramp_automation-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/PKG-INFO` & `liveramp_automation-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp_automation
-Version: 0.1.6
+Version: 0.1.7
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.1.6/README.md` & `liveramp_automation-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/liveramp_automation/helpers/bucket.py` & `liveramp_automation-0.1.7/liveramp_automation/helpers/bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/liveramp_automation/helpers/file.py` & `liveramp_automation-0.1.7/liveramp_automation/helpers/file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/liveramp_automation/helpers/login.py` & `liveramp_automation-0.1.7/liveramp_automation/helpers/login.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/liveramp_automation/utils/allure.py` & `liveramp_automation-0.1.7/liveramp_automation/utils/allure.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 import allure
 
 
 def allure_page_screenshot(page, name):
     """
     Call allure_page_screenshot to show the screenshot while using Playright
-
     :param page:
     :param name:
     :return:
     """
     allure.attach(page.screenshot(), name=name, attachment_type=allure.attachment_type.PNG)
 
 
 #
 def allure_drive_screenshot(driver, name):
     """
     Call allure_drive_screenshot to show the screenshot while using Selenium
-
     :param page:
     :param name:
     :return:
     """
     allure.attach(driver.save_screenshot(), name=name, attachment_type=allure.attachment_type.PNG)
 
 
-# Call allure_attach_video to show the recording video,the video path should be provided.
 def allure_attach_video(path, video_name):
     """
     Call allure_drive_screenshot to show the screenshot while using Selenium
-
     :param page:
     :param name:
     :return:
     """
     allure.attach.file(path, name=video_name, attachment_type=allure.attachment_type.MP4)
 
 
-#
 def allure_attach_text(content, description):
     """
     Call allure_attach_text to show the content in text format.
-
     :param page:
     :param name:
     :return:
     """
     allure.attach(content, description, attachment_type=allure.attachment_type.TEXT)
 
 
 def allure_attach_json(content, description):
     """
     Call allure_attach_json to show the content in json format.
-
     :param page:
     :param name:
     :return:
     """
     allure.attach(content, description, attachment_type=allure.attachment_type.JSON)
```

### Comparing `liveramp_automation-0.1.6/liveramp_automation/utils/log.py` & `liveramp_automation-0.1.7/liveramp_automation/utils/log.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/liveramp_automation/utils/playwright.py` & `liveramp_automation-0.1.7/liveramp_automation/utils/playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/liveramp_automation/utils/request.py` & `liveramp_automation-0.1.7/liveramp_automation/utils/request.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 from liveramp_automation.utils.log import Logger
 
 
 # These are 7 types of methods to call the APIs.Each API allows to multiple parameters.
 # We also added some log/report_content while calling the APIs which would be helpful to check the errors.
 
 def request_post(url, headers, data=None, json=None, **kwargs):
-    """
-       Call request_post to show the screenshot while using Playright
+    """Sends a POST request.
 
-       :param page:
-       :param name:
-       :return:
-       """
+    :param url: URL for the new :class:`Request` object.
+    :param headers:
+    :param data:
+    :param json:
+    :param kwargs:
+    :return:
+    """
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is POST")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is POST", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
         allure_attach_text(data, "The request data infomation is as the following.")
@@ -34,14 +36,23 @@
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
 def request_get(url, headers, data=None, json=None, **kwargs):
+    """Sends a get request.
+
+    :param url:
+    :param headers:
+    :param data:
+    :param json:
+    :param kwargs:
+    :return:
+    """
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is GET")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is GET", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
@@ -55,14 +66,25 @@
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
 def request_options(url, headers, **kwargs):
+    """Sends an OPTIONS request.
+
+    :param url: URL for the new :class:`Request` object.
+    :param \*\*kwargs: Optional arguments that ``request`` takes.
+    :return: :class:`Response <Response>` object
+    :rtype: requests.Response
+    :param headers:
+    :param kwargs:
+    :return:
+    """
+
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is OPTIONS")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is OPTIONS", "Method")
     try:
         response = requests.options(url=url, headers=headers, **kwargs)
         Logger.info("The response infomation is {}".format(response.text))
@@ -72,14 +94,23 @@
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
 def request_delete(url, headers, data=None, json=None, **kwargs):
+    """
+
+    :param url:
+    :param headers:
+    :param data:
+    :param json:
+    :param kwargs:
+    :return:
+    """
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is DELETE")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is DELETE", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
@@ -93,14 +124,23 @@
         Logger.info("Request timed out {}".format(error))
     except requests.exceptions.RequestException as error:
         Logger.info("An error occurred {}".format(error))
     return response
 
 
 def request_head(url, headers, data=None, json=None, **kwargs):
+    """
+
+    :param url:
+    :param headers:
+    :param data:
+    :param json:
+    :param kwargs:
+    :return:
+    """
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is HEAD")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is HEAD", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
     if json:
```

### Comparing `liveramp_automation-0.1.6/liveramp_automation/utils/selenium.py` & `liveramp_automation-0.1.7/liveramp_automation/utils/selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/liveramp_automation/utils/time.py` & `liveramp_automation-0.1.7/liveramp_automation/utils/time.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 import time
 from datetime import date, timedelta, datetime
 
-
-# The MACROS() API prepared some expected time format.
-# You could invole the time format like: yesterday.format(**MACROS) at any code snippet.
+"""
+The MACROS() API prepared some expected time format.
+You could invole the time format like: yesterday.format(**MACROS) at any code snippet.
+"""
 MACROS = {
     "yesterday": (date.today() - timedelta(days=1)).strftime("%Y%m%d"),
     "today": date.today().strftime("%Y%m%d"),
     "dayOfYear": (date.today().timetuple()).tm_yday,
     "now": datetime.now().strftime("%Y%m%d%H%M%S"),
     "now_format": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
     "nowconnect": datetime.now().strftime("%Y%m%d-%H%M%S"),  # data ingestion must be in yyyymmdd-hhmmss format
     "three_days_ago": (date.today() - timedelta(days=0)).strftime("%Y%m%d"),
     "two_hours_from_now": (datetime.now() + timedelta(hours=2)).strftime("%Y%m%d-%H%M%S"),
     "24hours_before_now": (datetime.now() - timedelta(hours=24)).strftime("%Y%m%d%H%M%S")
 }
 
 
-# The fixed_wait() API defined the default=3 seconds wait time.
 def fixed_wait(value=3):
+    """The fixed_wait() defined the default=3 seconds wait time.
+
+    :param value: The number of seconds to wait (default is 3 seconds).
+    :return: None
+    """
     time.sleep(value)
```

### Comparing `liveramp_automation-0.1.6/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-0.1.7/liveramp_automation.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liveramp-automation
-Version: 0.1.6
+Version: 0.1.7
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/liveramp-automation
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `liveramp_automation-0.1.6/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-0.1.7/liveramp_automation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.6/setup.py` & `liveramp_automation-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,21 @@
 from setuptools import setup,find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
+import os
+version_ns = {}
+with open(os.path.join("liveramp_automation", "__version__.py")) as f:
+    exec(f.read(), version_ns)
+version = version_ns['__version__']
+
 setup(
     name='liveramp_automation',
-    version='0.1.6',
+    version=version,
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/liveramp-automation",
     packages= find_packages(),
```

