# Comparing `tmp/liveramp_automation-0.1.1.tar.gz` & `tmp/liveramp_automation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liveramp_automation-0.1.1.tar", last modified: Wed Aug  2 01:21:46 2023, max compression
+gzip compressed data, was "liveramp_automation-0.1.3.tar", last modified: Wed Aug  2 07:06:12 2023, max compression
```

## Comparing `liveramp_automation-0.1.1.tar` & `liveramp_automation-0.1.3.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.218821 liveramp_automation-0.1.1/
--rw-r--r--   0 jasqia     (502) staff       (20)     1100 2023-08-01 09:13:05.000000 liveramp_automation-0.1.1/LICENSE
--rw-r--r--   0 jasqia     (502) staff       (20)     1697 2023-08-02 01:21:46.218296 liveramp_automation-0.1.1/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)     1398 2023-07-19 08:48:17.000000 liveramp_automation-0.1.1/README.md
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.196714 liveramp_automation-0.1.1/liveramp_automation/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.1/liveramp_automation/__init__.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.206708 liveramp_automation-0.1.1/liveramp_automation/helpers/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/helper_bucket.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3791 2023-08-01 09:41:57.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/helper_file.py
--rw-r--r--   0 jasqia     (502) staff       (20)     3596 2023-08-01 09:38:55.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/helper_login.py
--rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.1/liveramp_automation/helpers/helper_notification.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.215418 liveramp_automation-0.1.1/liveramp_automation/utils/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.1/liveramp_automation/utils/__init__.py
--rw-r--r--   0 jasqia     (502) staff       (20)     1057 2023-07-20 06:17:22.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_allure.py
--rw-r--r--   0 jasqia     (502) staff       (20)     2976 2023-08-01 01:06:55.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_log.py
--rw-r--r--   0 jasqia     (502) staff       (20)      902 2023-07-20 09:35:55.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_parsers.py
--rw-r--r--   0 jasqia     (502) staff       (20)      751 2023-08-01 09:07:07.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_playwright.py
--rw-r--r--   0 jasqia     (502) staff       (20)     7316 2023-08-01 01:28:11.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_request.py
--rw-r--r--   0 jasqia     (502) staff       (20)      749 2023-08-01 01:28:11.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_selenium.py
--rw-r--r--   0 jasqia     (502) staff       (20)      988 2023-07-20 06:35:14.000000 liveramp_automation-0.1.1/liveramp_automation/utils/util_time.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.201855 liveramp_automation-0.1.1/liveramp_automation.egg-info/
--rw-r--r--   0 jasqia     (502) staff       (20)     1697 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/PKG-INFO
--rw-r--r--   0 jasqia     (502) staff       (20)      867 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/SOURCES.txt
--rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/dependency_links.txt
--rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/requires.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       20 2023-08-02 01:21:46.000000 liveramp_automation-0.1.1/liveramp_automation.egg-info/top_level.txt
--rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 01:21:46.219060 liveramp_automation-0.1.1/setup.cfg
--rw-r--r--   0 jasqia     (502) staff       (20)     1206 2023-08-02 01:21:44.000000 liveramp_automation-0.1.1/setup.py
-drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 01:21:46.217413 liveramp_automation-0.1.1/tests/
--rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 09:02:07.000000 liveramp_automation-0.1.1/tests/test_file.py
--rw-r--r--   0 jasqia     (502) staff       (20)      559 2023-08-01 09:11:03.000000 liveramp_automation-0.1.1/tests/test_playwright.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.993700 liveramp_automation-0.1.3/
+-rw-r--r--   0 jasqia     (502) staff       (20)    11356 2023-08-02 06:57:58.000000 liveramp_automation-0.1.3/LICENSE
+-rw-r--r--   0 jasqia     (502) staff       (20)     2033 2023-08-02 07:06:12.992946 liveramp_automation-0.1.3/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)     1734 2023-08-02 06:57:58.000000 liveramp_automation-0.1.3/README.md
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.962993 liveramp_automation-0.1.3/liveramp_automation/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.3/liveramp_automation/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.973424 liveramp_automation-0.1.3/liveramp_automation/helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1711 2023-07-19 08:04:46.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/helper_bucket.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3791 2023-08-01 09:41:57.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/helper_file.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     3967 2023-08-02 06:55:22.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/helper_login.py
+-rw-r--r--   0 jasqia     (502) staff       (20)       70 2023-07-19 08:17:12.000000 liveramp_automation-0.1.3/liveramp_automation/helpers/helper_notification.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.983464 liveramp_automation-0.1.3/liveramp_automation/utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-01 08:30:54.000000 liveramp_automation-0.1.3/liveramp_automation/utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     1466 2023-08-02 05:31:37.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_allure.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     2583 2023-08-02 05:34:33.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      968 2023-08-02 05:34:33.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_parsers.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      751 2023-08-01 09:07:07.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_playwright.py
+-rw-r--r--   0 jasqia     (502) staff       (20)     7462 2023-08-02 05:40:49.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_request.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      749 2023-08-01 01:28:11.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_selenium.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      988 2023-07-20 06:35:14.000000 liveramp_automation-0.1.3/liveramp_automation/utils/util_time.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.968310 liveramp_automation-0.1.3/liveramp_automation.egg-info/
+-rw-r--r--   0 jasqia     (502) staff       (20)     2033 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/PKG-INFO
+-rw-r--r--   0 jasqia     (502) staff       (20)      995 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/SOURCES.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)        1 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/dependency_links.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)      381 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/requires.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       26 2023-08-02 07:06:12.000000 liveramp_automation-0.1.3/liveramp_automation.egg-info/top_level.txt
+-rw-r--r--   0 jasqia     (502) staff       (20)       38 2023-08-02 07:06:12.993973 liveramp_automation-0.1.3/setup.cfg
+-rw-r--r--   0 jasqia     (502) staff       (20)     1206 2023-08-02 07:06:01.000000 liveramp_automation-0.1.3/setup.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.985050 liveramp_automation-0.1.3/tests/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:41.000000 liveramp_automation-0.1.3/tests/__init__.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.987346 liveramp_automation-0.1.3/tests/test_helpers/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:03.000000 liveramp_automation-0.1.3/tests/test_helpers/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 03:27:48.000000 liveramp_automation-0.1.3/tests/test_helpers/test_file.py
+drwxr-xr-x   0 jasqia     (502) staff       (20)        0 2023-08-02 07:06:12.990973 liveramp_automation-0.1.3/tests/test_utils/
+-rw-r--r--   0 jasqia     (502) staff       (20)        0 2023-08-02 01:29:13.000000 liveramp_automation-0.1.3/tests/test_utils/__init__.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      252 2023-08-02 01:35:52.000000 liveramp_automation-0.1.3/tests/test_utils/test_log.py
+-rw-r--r--   0 jasqia     (502) staff       (20)      457 2023-08-02 03:40:11.000000 liveramp_automation-0.1.3/tests/test_utils/test_request.py
```

### Comparing `liveramp_automation-0.1.1/PKG-INFO` & `liveramp_automation-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-Metadata-Version: 2.1
-Name: liveramp_automation
-Version: 0.1.1
-Summary: This is the base liveramp_automation_framework
-Home-page: https://github.com/LiveRamp/qe_api_framework
-Author: Jasmine Qian
-Author-email: jasmine.qian@liveramp.com
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # liveramp-automation
 an automation framework helps you qucikly author scripts for any automation testing 
 
 
 
-### Background 
+### Background
 
-    Do you want to create your own test project, 
-    but struggle with configuring the environment, 
-    feel lost in choosing a testing framework, 
-    confused about integration and execution, 
-    and helpless in displaying test reports or recording test results in the long run?
-
-    Don't worry.
-
-    We provide an open-source and easy-to-use testing framework 
-    that helps QE/DEV and anyone interested in quickly getting started 
-    with various types of automation testing.
+    Are you eager to embark on your journey of creating a remarkable test project? 
+    But, you find yourself grappling with the complexities of environment configuration, 
+    puzzled by the plethora of testing frameworks to choose from, 
+    and unsure about integration and execution strategies. 
+
+    Moreover, you feel helpless when it comes to presenting test reports 
+    or recording test results effectively in the long term.
+
+    Fret not!
+
+    We have a perfect solution for you. 
+    Our team offers an exceptional open-source and user-friendly testing framework designed 
+    to empower QE/DEV professionals and anyone enthusiastic about automation testing. 
+    
+    With our solution, you can effortlessly kickstart your automation endeavors, 
+    exploring various types of tests with ease and confidence.
 
 
 ### 1. Descprition of the repository
         This repository is to build a base autoamtion framework. 
         We would like to integrate the common helpers and libraries here and then build a lib.
         Later the only thing is to add the cases according to the features. 
         Since most of the common helpers and libraries have been integrated to the lib,
```

### Comparing `liveramp_automation-0.1.1/liveramp_automation/helpers/helper_bucket.py` & `liveramp_automation-0.1.3/liveramp_automation/helpers/helper_bucket.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.1/liveramp_automation/helpers/helper_file.py` & `liveramp_automation-0.1.3/liveramp_automation/helpers/helper_file.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.1/liveramp_automation/helpers/helper_login.py` & `liveramp_automation-0.1.3/liveramp_automation/helpers/helper_login.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,20 +3,26 @@
 from selenium.webdriver.common.by import By
 from liveramp_automation.utils.util_log import Logger
 from liveramp_automation.utils.util_time import fixed_wait
 
 
 class LoginHepler:
 
-    # This method liveramp_okta_login_page is to login okta with Playwright.
-    # The username and passowrd are requried.
-    # Please try to call this API with the username and password provided in os.environ[]
     @staticmethod
     def liveramp_okta_login_page(page, config, username, password):
-        # navigate to the Okta login page
+        """
+        This function, "liveramp_okta_login_page," facilitates Okta login using Playwright.
+        Both the username and password are mandatory.
+        Please invoke this API with the username and password provided in os.environ[].
+        :param page:
+        :param config:
+        :param username:
+        :param password:
+        :return:
+        """
         Logger.info("We are going to login to OKTA")
         url = config['login_url']
         Logger.info("The login url is {}".format(url))
         page.goto(url)
         fixed_wait()
         url_new = page.url
         Logger.info("The current url is {}".format(url_new))
@@ -27,20 +33,27 @@
             page.get_by_role("button", name="Next").click()
             page.get_by_role("textbox", name="Password").fill(password)
             page.get_by_role("button", name="Sign In").click()
             Logger.info("We could login to OKTA successfully")
             # wait for the login process to complete
             fixed_wait(20)
 
-    # This method liveramp_okta_login_driver is to login okta with Selenium.
-    # The username and passowrd are requried.
-    # Please try to call this API with the username and password provided in os.environ[]
+    #
     @staticmethod
     def liveramp_okta_login_driver(driver, config, username, password):
-        # navigate to the Okta login page
+        """
+         "liveramp_okta_login_driver," is to facilitate Okta login using Selenium.
+         Both the username and password are mandatory.
+         Please utilize this API by providing the username and password from os.environ[].
+        :param driver:
+        :param config:
+        :param username:
+        :param password:
+        :return:
+        """
         Logger.info("We are going to login to OKTA")
         url = config['login_url']
         Logger.info("The login url is {}".format(url))
         driver.get(url)
         fixed_wait()
         if driver.current_url.__contains__(url):
             Logger.info("We've already logan to OKTA succefully")
@@ -53,19 +66,25 @@
             password_box.send_keys(password)
             submit_button = driver.find_element(by=By.ID, value='okta-signin-submit')
             submit_button.click()
             Logger.info("We could login to OKTA successfully")
             # wait for the login process to complete
             fixed_wait(20)
 
-    # This method call_oauth2_get_token is to all oauth2 to login, the API username and password(sereect) are required.
-    # The username and passowrd are requried.
-    # Please try to call this API with the username and password provided in os.environ[]
+    #
     @staticmethod
-    def call_oauth2_get_token(username, password):
+    def call_oauth2_get_token(username, password) -> str:
+        """
+        The purpose of the method `call_oauth2_get_token` is to initiate an OAuth2 login.
+        Both the API username and password (sensitive) are mandatory for this process.
+        Please ensure that you provide the required username and password from os.environ[] when calling this API.
+        :param username:
+        :param password:
+        :return:
+        """
         params = {
             "grant_type": "password",
             "scope": "openid",
             "client_id": "liveramp-api"
         }
         Logger.info("The default params are the {}".format(params))
         headers = {"content-type": "application/x-www-form-urlencoded"}
```

### Comparing `liveramp_automation-0.1.1/liveramp_automation/utils/util_log.py` & `liveramp_automation-0.1.3/liveramp_automation/utils/util_log.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,59 +1,55 @@
 # -*- coding: utf-8 -*-
+import configparser
 import os
 import logging
 from datetime import datetime
 from logging import handlers
 from threading import Lock
 
-from liveramp_automation.helpers.helper_file import FileHelper
-
 
 class LoggerUtils:
-    # This object is a single pattern instance to log.
-    # If we haven't set the default log_path in the pytest.ini file, it would use the path = "reports/"
-    # If we haven't set the default log_name in the pytest.ini file, it would use the log_name = "%Y%m%d%H%M%S.log"
+    """
+    This object is a single pattern instance to log.
+    If we haven't set the default log_path in the pytest.ini file, it would use the path = "reports/"
+    If we haven't set the default log_name in the pytest.ini file, it would use the log_name = "%Y%m%d%H%M%S.log"
+    :param
+    :type
+    :return:
+    :rtype:
+    :raises
+    """
     _instance = None
     _lock = Lock()
 
     @classmethod
     def get_logger(cls):
         if not cls._instance:
             with cls._lock:
                 if not cls._instance:
                     cls._instance = cls._configure_logging()
         return cls._instance
 
     @staticmethod
     def _configure_logging():
-        data_dict = FileHelper.read_init_file(file_path='', file_name='pytest.ini', file_mode="log")
-        # if data_dict:
-        if data_dict['log_path']:
-            log_path = data_dict['log_path']
-        else:
+        config = configparser.ConfigParser()
+        try:
+            with open("pytest.ini", 'r') as file:
+                config.read_file(file)
+                try:
+                    log_path = config.get('log', 'log_path')
+                except (configparser.NoSectionError, configparser.NoOptionError):
+                    log_path = "reports/"
+                try:
+                    log_name = config.get('log', 'log_name')
+                except (configparser.NoSectionError, configparser.NoOptionError):
+                    log_name = "%Y%m%d%H%M%S.log"
+        except FileNotFoundError:
             log_path = "reports/"
-        if data_dict['log_path']:
-            log_name = data_dict['log_name']
-        else:
             log_name = "%Y%m%d%H%M%S.log"
-        # config = configparser.ConfigParser()
-        # try:
-        #     with open("pytest.ini", 'r') as file:
-        #         config.read_file(file)
-        #         try:
-        #             log_path = config.get('log', 'log_path')
-        #         except (configparser.NoSectionError, configparser.NoOptionError):
-        #             log_path = "reports/"
-        #         try:
-        #             log_name = config.get('log', 'log_name')
-        #         except (configparser.NoSectionError, configparser.NoOptionError):
-        #             log_name = "%Y%m%d%H%M%S.log"
-        # except FileNotFoundError:
-        #     log_path = "reports/"
-        #     log_name = "%Y%m%d%H%M%S.log"
         log_format = logging.Formatter('%(asctime)s - %(levelname)s - [ %(filename)s: %(lineno)d ] - %(message)s')
         log_directory = os.path.join(os.getcwd(), log_path)
         if not os.path.exists(log_directory):
             os.makedirs(log_directory)
         log_name = datetime.now().strftime(log_name)
         file_name = os.path.join(log_path, log_name)
```

### Comparing `liveramp_automation-0.1.1/liveramp_automation/utils/util_parsers.py` & `liveramp_automation-0.1.3/liveramp_automation/utils/util_parsers.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,17 +4,24 @@
 from pytest_bdd.parsers import StepParser
 import parse as base_parse
 
 EXTRA_TYPES = {}
 
 
 class ParseUtils(StepParser):
-    """parse step parser."""
+    """
+    parse step parser.
+    This is a Factory method pattern to parse the steps in the BDD scenarios
+    :param
+    :type
+    :return:
+    :rtype:
+    :raises
+    """
 
-    # This is a Factory method pattern to parse the steps in the BDD scenarios
     def __init__(self, name, *args):
         """Compile parse expression."""
         super(ParseUtils, self).__init__(name)
         self.parser = base_parse.compile(self.name, *args, extra_types=EXTRA_TYPES)
 
     def parse_arguments(self, name: str) -> dict[str, Any]:
         """Get step arguments.
```

### Comparing `liveramp_automation-0.1.1/liveramp_automation/utils/util_playwright.py` & `liveramp_automation-0.1.3/liveramp_automation/utils/util_playwright.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.1/liveramp_automation/utils/util_request.py` & `liveramp_automation-0.1.3/liveramp_automation/utils/util_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 from liveramp_automation.utils.util_log import Logger
 
 
 # These are 7 types of methods to call the APIs.Each API allows to multiple parameters.
 # We also added some log/report_content while calling the APIs which would be helpful to check the errors.
 
 def request_post(url, headers, data=None, json=None, **kwargs):
+    """
+       Call request_post to show the screenshot while using Playright
+
+       :param page:
+       :param name:
+       :return:
+       """
     Logger.info("The url infomation is {}".format(url))
     Logger.info("The request method is POST")
     allure_attach_text("The url infomation is {}".format(url), "URL")
     allure_attach_text("The request method is POST", "Method")
     if data:
         Logger.info("The request data infomation is {}".format(data))
         allure_attach_text(data, "The request data infomation is as the following.")
```

### Comparing `liveramp_automation-0.1.1/liveramp_automation/utils/util_selenium.py` & `liveramp_automation-0.1.3/liveramp_automation/utils/util_selenium.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.1/liveramp_automation/utils/util_time.py` & `liveramp_automation-0.1.3/liveramp_automation/utils/util_time.py`

 * *Files identical despite different names*

### Comparing `liveramp_automation-0.1.1/liveramp_automation.egg-info/PKG-INFO` & `liveramp_automation-0.1.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 Metadata-Version: 2.1
-Name: liveramp-automation
-Version: 0.1.1
+Name: liveramp_automation
+Version: 0.1.3
 Summary: This is the base liveramp_automation_framework
 Home-page: https://github.com/LiveRamp/qe_api_framework
 Author: Jasmine Qian
 Author-email: jasmine.qian@liveramp.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # liveramp-automation
 an automation framework helps you qucikly author scripts for any automation testing 
 
 
 
-### Background 
+### Background
 
-    Do you want to create your own test project, 
-    but struggle with configuring the environment, 
-    feel lost in choosing a testing framework, 
-    confused about integration and execution, 
-    and helpless in displaying test reports or recording test results in the long run?
-
-    Don't worry.
-
-    We provide an open-source and easy-to-use testing framework 
-    that helps QE/DEV and anyone interested in quickly getting started 
-    with various types of automation testing.
+    Are you eager to embark on your journey of creating a remarkable test project? 
+    But, you find yourself grappling with the complexities of environment configuration, 
+    puzzled by the plethora of testing frameworks to choose from, 
+    and unsure about integration and execution strategies. 
+
+    Moreover, you feel helpless when it comes to presenting test reports 
+    or recording test results effectively in the long term.
+
+    Fret not!
+
+    We have a perfect solution for you. 
+    Our team offers an exceptional open-source and user-friendly testing framework designed 
+    to empower QE/DEV professionals and anyone enthusiastic about automation testing. 
+    
+    With our solution, you can effortlessly kickstart your automation endeavors, 
+    exploring various types of tests with ease and confidence.
 
 
 ### 1. Descprition of the repository
         This repository is to build a base autoamtion framework. 
         We would like to integrate the common helpers and libraries here and then build a lib.
         Later the only thing is to add the cases according to the features. 
         Since most of the common helpers and libraries have been integrated to the lib,
```

### Comparing `liveramp_automation-0.1.1/liveramp_automation.egg-info/SOURCES.txt` & `liveramp_automation-0.1.3/liveramp_automation.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -16,9 +16,13 @@
 liveramp_automation/utils/util_allure.py
 liveramp_automation/utils/util_log.py
 liveramp_automation/utils/util_parsers.py
 liveramp_automation/utils/util_playwright.py
 liveramp_automation/utils/util_request.py
 liveramp_automation/utils/util_selenium.py
 liveramp_automation/utils/util_time.py
-tests/test_file.py
-tests/test_playwright.py
+tests/__init__.py
+tests/test_helpers/__init__.py
+tests/test_helpers/test_file.py
+tests/test_utils/__init__.py
+tests/test_utils/test_log.py
+tests/test_utils/test_request.py
```

### Comparing `liveramp_automation-0.1.1/setup.py` & `liveramp_automation-0.1.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup,find_packages
 
 with open("readme.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='liveramp_automation',
-    version='0.1.1',
+    version='0.1.3',
     author='Jasmine Qian',
     author_email='jasmine.qian@liveramp.com',
     description="This is the base liveramp_automation_framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/LiveRamp/qe_api_framework",
     # packages=['liveramp_automation'],
```

