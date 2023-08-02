# Comparing `tmp/selene-2.0.0rc3.post3.tar.gz` & `tmp/selene-2.0.0rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "selene-2.0.0rc3.post3.tar", max compression
+gzip compressed data, was "selene-2.0.0rc4.tar", max compression
```

## Comparing `selene-2.0.0rc3.post3.tar` & `selene-2.0.0rc4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc3.post3/LICENSE
--rw-r--r--   0        0        0    16589 2023-07-21 19:40:03.696730 selene-2.0.0rc3.post3/README.md
--rw-r--r--   0        0        0     7963 2023-07-29 14:41:49.820807 selene-2.0.0rc3.post3/pyproject.toml
--rw-r--r--   0        0        0     6050 2023-07-29 14:41:49.824530 selene-2.0.0rc3.post3/selene/__init__.py
--rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc3.post3/selene/_managed.py
--rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc3.post3/selene/api/__init__.py
--rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc3.post3/selene/api/base/__init__.py
--rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc3.post3/selene/api/shared/__init__.py
--rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc3.post3/selene/common/__init__.py
--rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc3.post3/selene/common/data_structures/__init__.py
--rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc3.post3/selene/common/data_structures/persistent.py
--rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc3.post3/selene/common/fp.py
--rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc3.post3/selene/common/helpers.py
--rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc3.post3/selene/common/none_object.py
--rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc3.post3/selene/common/predicate.py
--rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc3.post3/selene/core/__init__.py
--rw-r--r--   0        0        0     8731 2023-07-27 13:08:17.397537 selene-2.0.0rc3.post3/selene/core/command.py
--rw-r--r--   0        0        0     6672 2023-07-01 11:00:30.192218 selene-2.0.0rc3.post3/selene/core/condition.py
--rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc3.post3/selene/core/conditions.py
--rw-r--r--   0        0        0    61351 2023-07-27 16:08:33.740156 selene-2.0.0rc3.post3/selene/core/configuration.py
--rw-r--r--   0        0        0     9441 2023-04-12 19:41:51.757408 selene-2.0.0rc3.post3/selene/core/configuration.pyi
--rw-r--r--   0        0        0    44433 2023-07-01 11:09:18.989737 selene-2.0.0rc3.post3/selene/core/entity.py
--rw-r--r--   0        0        0    12087 2023-04-12 19:44:29.895473 selene-2.0.0rc3.post3/selene/core/entity.pyi
--rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc3.post3/selene/core/exceptions.py
--rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc3.post3/selene/core/locator.py
--rw-r--r--   0        0        0    17295 2023-07-25 14:23:47.850912 selene-2.0.0rc3.post3/selene/core/match.py
--rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc3.post3/selene/core/query.py
--rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc3.post3/selene/core/wait.py
--rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc3.post3/selene/py.typed
--rw-r--r--   0        0        0      120 2023-07-21 19:00:31.406121 selene-2.0.0rc3.post3/selene/support/__init__.py
--rw-r--r--   0        0        0       32 2023-07-27 13:43:32.337434 selene-2.0.0rc3.post3/selene/support/_extensions/__init__.py
--rw-r--r--   0        0        0      271 2023-07-27 14:47:27.186714 selene-2.0.0rc3.post3/selene/support/_extensions/webdriver_manager/__init__.py
--rw-r--r--   0        0        0     9183 2023-07-29 16:36:14.462953 selene-2.0.0rc3.post3/selene/support/_extensions/webdriver_manager/patch.py
--rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc3.post3/selene/support/_logging.py
--rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc3.post3/selene/support/by.py
--rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc3.post3/selene/support/conditions/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc3.post3/selene/support/conditions/be.py
--rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc3.post3/selene/support/conditions/have.py
--rw-r--r--   0        0        0     9093 2023-07-01 10:59:38.230736 selene-2.0.0rc3.post3/selene/support/conditions/not_.py
--rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc3.post3/selene/support/shared/__init__.py
--rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc3.post3/selene/support/shared/browser.py
--rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc3.post3/selene/support/shared/config.py
--rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc3.post3/selene/support/shared/jquery_style.py
--rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc3.post3/selene/support/webdriver.py
--rw-r--r--   0        0        0    18232 1970-01-01 00:00:00.000000 selene-2.0.0rc3.post3/PKG-INFO
+-rw-r--r--   0        0        0     1077 2022-11-16 16:21:11.197245 selene-2.0.0rc4/LICENSE
+-rw-r--r--   0        0        0    16589 2023-07-21 19:40:03.696730 selene-2.0.0rc4/README.md
+-rw-r--r--   0        0        0     7958 2023-08-02 21:22:23.428514 selene-2.0.0rc4/pyproject.toml
+-rw-r--r--   0        0        0     6045 2023-08-02 21:22:23.424215 selene-2.0.0rc4/selene/__init__.py
+-rw-r--r--   0        0        0      130 2023-03-31 22:43:08.634926 selene-2.0.0rc4/selene/_managed.py
+-rw-r--r--   0        0        0     1785 2022-11-16 16:21:11.200361 selene-2.0.0rc4/selene/api/__init__.py
+-rw-r--r--   0        0        0     1359 2023-04-01 13:26:39.465175 selene-2.0.0rc4/selene/api/base/__init__.py
+-rw-r--r--   0        0        0     1212 2022-11-16 16:21:11.200558 selene-2.0.0rc4/selene/api/shared/__init__.py
+-rw-r--r--   0        0        0       50 2023-04-09 19:22:37.044489 selene-2.0.0rc4/selene/common/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-31 22:43:08.635026 selene-2.0.0rc4/selene/common/data_structures/__init__.py
+-rw-r--r--   0        0        0    11014 2023-04-10 11:06:23.425779 selene-2.0.0rc4/selene/common/data_structures/persistent.py
+-rw-r--r--   0        0        0     3403 2023-04-05 19:40:45.107843 selene-2.0.0rc4/selene/common/fp.py
+-rw-r--r--   0        0        0     3140 2023-04-01 20:10:41.773344 selene-2.0.0rc4/selene/common/helpers.py
+-rw-r--r--   0        0        0     1452 2023-04-10 11:06:23.278623 selene-2.0.0rc4/selene/common/none_object.py
+-rw-r--r--   0        0        0     3499 2023-04-10 11:06:23.345359 selene-2.0.0rc4/selene/common/predicate.py
+-rw-r--r--   0        0        0     1116 2022-11-16 16:21:11.201046 selene-2.0.0rc4/selene/core/__init__.py
+-rw-r--r--   0        0        0     8731 2023-07-27 13:08:17.397537 selene-2.0.0rc4/selene/core/command.py
+-rw-r--r--   0        0        0     6672 2023-07-01 11:00:30.192218 selene-2.0.0rc4/selene/core/condition.py
+-rw-r--r--   0        0        0     1391 2022-11-16 16:21:11.201337 selene-2.0.0rc4/selene/core/conditions.py
+-rw-r--r--   0        0        0    61351 2023-07-27 16:08:33.740156 selene-2.0.0rc4/selene/core/configuration.py
+-rw-r--r--   0        0        0     9441 2023-04-12 19:41:51.757408 selene-2.0.0rc4/selene/core/configuration.pyi
+-rw-r--r--   0        0        0    44433 2023-07-01 11:09:18.989737 selene-2.0.0rc4/selene/core/entity.py
+-rw-r--r--   0        0        0    12087 2023-04-12 19:44:29.895473 selene-2.0.0rc4/selene/core/entity.pyi
+-rw-r--r--   0        0        0     2390 2023-04-01 16:33:27.602534 selene-2.0.0rc4/selene/core/exceptions.py
+-rw-r--r--   0        0        0     1464 2022-11-16 16:21:11.202031 selene-2.0.0rc4/selene/core/locator.py
+-rw-r--r--   0        0        0    17295 2023-07-25 14:23:47.850912 selene-2.0.0rc4/selene/core/match.py
+-rw-r--r--   0        0        0     6725 2023-04-10 11:06:23.431326 selene-2.0.0rc4/selene/core/query.py
+-rw-r--r--   0        0        0     5538 2023-04-01 19:31:32.923450 selene-2.0.0rc4/selene/core/wait.py
+-rw-r--r--   0        0        0        1 2023-04-01 10:19:15.746910 selene-2.0.0rc4/selene/py.typed
+-rw-r--r--   0        0        0      120 2023-07-21 19:00:31.406121 selene-2.0.0rc4/selene/support/__init__.py
+-rw-r--r--   0        0        0       32 2023-07-27 13:43:32.337434 selene-2.0.0rc4/selene/support/_extensions/__init__.py
+-rw-r--r--   0        0        0      271 2023-07-27 14:47:27.186714 selene-2.0.0rc4/selene/support/_extensions/webdriver_manager/__init__.py
+-rw-r--r--   0        0        0     9183 2023-08-02 21:11:51.835214 selene-2.0.0rc4/selene/support/_extensions/webdriver_manager/patch.py
+-rw-r--r--   0        0        0     3466 2023-04-09 17:52:23.740196 selene-2.0.0rc4/selene/support/_logging.py
+-rw-r--r--   0        0        0     2867 2023-04-01 13:26:39.452370 selene-2.0.0rc4/selene/support/by.py
+-rw-r--r--   0        0        0        0 2022-11-16 16:21:11.202000 selene-2.0.0rc4/selene/support/conditions/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-01 13:26:39.456952 selene-2.0.0rc4/selene/support/conditions/be.py
+-rw-r--r--   0        0        0     6510 2023-04-01 13:26:39.471979 selene-2.0.0rc4/selene/support/conditions/have.py
+-rw-r--r--   0        0        0     9093 2023-07-01 10:59:38.230736 selene-2.0.0rc4/selene/support/conditions/not_.py
+-rw-r--r--   0        0        0     1234 2023-04-01 18:03:46.047687 selene-2.0.0rc4/selene/support/shared/__init__.py
+-rw-r--r--   0        0        0     1308 2023-02-15 19:39:21.396824 selene-2.0.0rc4/selene/support/shared/browser.py
+-rw-r--r--   0        0        0     1296 2023-04-10 11:06:23.393100 selene-2.0.0rc4/selene/support/shared/config.py
+-rw-r--r--   0        0        0     1459 2023-04-01 19:36:10.742856 selene-2.0.0rc4/selene/support/shared/jquery_style.py
+-rw-r--r--   0        0        0     2754 2023-04-05 13:24:18.916048 selene-2.0.0rc4/selene/support/webdriver.py
+-rw-r--r--   0        0        0    18226 1970-01-01 00:00:00.000000 selene-2.0.0rc4/PKG-INFO
```

### Comparing `selene-2.0.0rc3.post3/LICENSE` & `selene-2.0.0rc4/LICENSE`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/README.md` & `selene-2.0.0rc4/README.md`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/pyproject.toml` & `selene-2.0.0rc4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "selene"
-version = "2.0.0rc3post3"
+version = "2.0.0rc4"
 description = "User-oriented browser tests in Python (Selenide port)"
 authors = ["Iakiv Kramarenko <yashaka@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = [
 	"testing",
 	"selenium",
@@ -46,15 +46,15 @@
 Changelog = "https://github.com/yashaka/selene/releases"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 selenium = ">=4.4.3"
 future = "*"
 webdriver-manager = "==3.8.6"
-typing-extensions = "==4.3.0"
+typing-extensions = ">=4.6.1"
 
 [tool.poetry.dev-dependencies]
 black = "^23.3.0"
 pycodestyle = "*"
 pylint = "^2.7.2"
 pytest = "*"
 pytest-cov = "*"
```

### Comparing `selene-2.0.0rc3.post3/selene/__init__.py` & `selene-2.0.0rc4/selene/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,8 +223,8 @@
 """
 
 # """
 # Just types...
 # """
 from selene.core.entity import Element, Collection  # noqa
 
-__version__ = '2.0.0rc3post3'
+__version__ = '2.0.0rc4'
```

### Comparing `selene-2.0.0rc3.post3/selene/api/__init__.py` & `selene-2.0.0rc4/selene/api/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/api/base/__init__.py` & `selene-2.0.0rc4/selene/api/base/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/api/shared/__init__.py` & `selene-2.0.0rc4/selene/api/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/common/data_structures/persistent.py` & `selene-2.0.0rc4/selene/common/data_structures/persistent.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/common/fp.py` & `selene-2.0.0rc4/selene/common/fp.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/common/helpers.py` & `selene-2.0.0rc4/selene/common/helpers.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/common/none_object.py` & `selene-2.0.0rc4/selene/common/none_object.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/common/predicate.py` & `selene-2.0.0rc4/selene/common/predicate.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/__init__.py` & `selene-2.0.0rc4/selene/core/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/command.py` & `selene-2.0.0rc4/selene/core/command.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/condition.py` & `selene-2.0.0rc4/selene/core/condition.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/conditions.py` & `selene-2.0.0rc4/selene/core/conditions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/configuration.py` & `selene-2.0.0rc4/selene/core/configuration.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/configuration.pyi` & `selene-2.0.0rc4/selene/core/configuration.pyi`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/entity.py` & `selene-2.0.0rc4/selene/core/entity.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/entity.pyi` & `selene-2.0.0rc4/selene/core/entity.pyi`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/exceptions.py` & `selene-2.0.0rc4/selene/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/locator.py` & `selene-2.0.0rc4/selene/core/locator.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/match.py` & `selene-2.0.0rc4/selene/core/match.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/query.py` & `selene-2.0.0rc4/selene/core/query.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/core/wait.py` & `selene-2.0.0rc4/selene/core/wait.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/_extensions/webdriver_manager/patch.py` & `selene-2.0.0rc4/selene/support/_extensions/webdriver_manager/patch.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/_logging.py` & `selene-2.0.0rc4/selene/support/_logging.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/by.py` & `selene-2.0.0rc4/selene/support/by.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/conditions/be.py` & `selene-2.0.0rc4/selene/support/conditions/be.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/conditions/have.py` & `selene-2.0.0rc4/selene/support/conditions/have.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/conditions/not_.py` & `selene-2.0.0rc4/selene/support/conditions/not_.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/shared/__init__.py` & `selene-2.0.0rc4/selene/support/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/shared/browser.py` & `selene-2.0.0rc4/selene/support/shared/browser.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/shared/config.py` & `selene-2.0.0rc4/selene/support/shared/config.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/shared/jquery_style.py` & `selene-2.0.0rc4/selene/support/shared/jquery_style.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/selene/support/webdriver.py` & `selene-2.0.0rc4/selene/support/webdriver.py`

 * *Files identical despite different names*

### Comparing `selene-2.0.0rc3.post3/PKG-INFO` & `selene-2.0.0rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: selene
-Version: 2.0.0rc3.post3
+Version: 2.0.0rc4
 Summary: User-oriented browser tests in Python (Selenide port)
 Home-page: https://yashaka.github.io/selene/
 License: MIT
 Keywords: testing,selenium,selenide,browser,pageobject,widget,wrapper
 Author: Iakiv Kramarenko
 Author-email: yashaka@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -24,15 +24,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Internet :: WWW/HTTP :: Browsers
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: future
 Requires-Dist: selenium (>=4.4.3)
-Requires-Dist: typing-extensions (==4.3.0)
+Requires-Dist: typing-extensions (>=4.6.1)
 Requires-Dist: webdriver-manager (==3.8.6)
 Project-URL: Changelog, https://github.com/yashaka/selene/releases
 Project-URL: Documentation, https://yashaka.github.io/selene/
 Project-URL: Repository, https://github.com/yashaka/selene/
 Description-Content-Type: text/markdown
 
 <!-- --8<-- [start:githubSection] -->
```

