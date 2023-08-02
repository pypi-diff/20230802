# Comparing `tmp/django_slack_bot-0.8.0.tar.gz` & `tmp/django_slack_bot-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django_slack_bot-0.8.0.tar", last modified: Tue Jul 26 01:46:53 2022, max compression
+gzip compressed data, was "dist/django_slack_bot-0.8.1.tar", last modified: Wed Aug  2 00:20:12 2023, max compression
```

## Comparing `django_slack_bot-0.8.0.tar` & `django_slack_bot-0.8.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/
--rw-r--r--   0 ST20638    (502) staff       (20)      521 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/PKG-INFO
--rw-r--r--   0 ST20638    (502) staff       (20)        7 2021-07-02 04:48:53.000000 django_slack_bot-0.8.0/README.md
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/django_slack_bot.egg-info/
--rw-r--r--   0 ST20638    (502) staff       (20)      521 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/django_slack_bot.egg-info/PKG-INFO
--rw-r--r--   0 ST20638    (502) staff       (20)      745 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/django_slack_bot.egg-info/SOURCES.txt
--rw-r--r--   0 ST20638    (502) staff       (20)        1 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/django_slack_bot.egg-info/dependency_links.txt
--rw-r--r--   0 ST20638    (502) staff       (20)      121 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/django_slack_bot.egg-info/entry_points.txt
--rw-r--r--   0 ST20638    (502) staff       (20)      115 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/django_slack_bot.egg-info/requires.txt
--rw-r--r--   0 ST20638    (502) staff       (20)       12 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/django_slack_bot.egg-info/top_level.txt
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/dsbot/
--rw-r--r--   0 ST20638    (502) staff       (20)        0 2021-07-02 04:48:05.000000 django_slack_bot-0.8.0/dsbot/__init__.py
--rw-r--r--   0 ST20638    (502) staff       (20)       85 2021-07-02 04:48:05.000000 django_slack_bot-0.8.0/dsbot/apps.py
--rw-r--r--   0 ST20638    (502) staff       (20)     3658 2022-03-25 07:37:31.000000 django_slack_bot-0.8.0/dsbot/client.py
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/dsbot/commands/
--rw-r--r--   0 ST20638    (502) staff       (20)        0 2021-07-02 04:48:05.000000 django_slack_bot-0.8.0/dsbot/commands/__init__.py
--rw-r--r--   0 ST20638    (502) staff       (20)     2026 2022-02-04 08:04:56.000000 django_slack_bot-0.8.0/dsbot/commands/default.py
--rw-r--r--   0 ST20638    (502) staff       (20)      603 2022-07-26 01:27:29.000000 django_slack_bot-0.8.0/dsbot/conf.py
--rw-r--r--   0 ST20638    (502) staff       (20)      951 2022-07-26 01:27:29.000000 django_slack_bot-0.8.0/dsbot/decorators.py
--rw-r--r--   0 ST20638    (502) staff       (20)     1307 2022-07-11 02:30:38.000000 django_slack_bot-0.8.0/dsbot/exceptions.py
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/dsbot/management/
--rw-r--r--   0 ST20638    (502) staff       (20)        0 2021-07-02 04:48:05.000000 django_slack_bot-0.8.0/dsbot/management/__init__.py
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/dsbot/management/commands/
--rw-r--r--   0 ST20638    (502) staff       (20)        0 2022-07-22 08:23:16.000000 django_slack_bot-0.8.0/dsbot/management/commands/__init__.py
--rw-r--r--   0 ST20638    (502) staff       (20)     1729 2022-07-26 01:34:53.000000 django_slack_bot-0.8.0/dsbot/management/commands/bot.py
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/dsbot/migrations/
--rw-r--r--   0 ST20638    (502) staff       (20)        0 2021-07-02 04:48:05.000000 django_slack_bot-0.8.0/dsbot/migrations/__init__.py
--rw-r--r--   0 ST20638    (502) staff       (20)      559 2022-07-26 01:27:29.000000 django_slack_bot-0.8.0/dsbot/tasks.py
--rw-r--r--   0 ST20638    (502) staff       (20)      934 2022-07-26 01:31:53.000000 django_slack_bot-0.8.0/dsbot/util.py
--rw-r--r--   0 ST20638    (502) staff       (20)     1074 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/setup.cfg
--rw-r--r--   0 ST20638    (502) staff       (20)       37 2021-07-02 02:49:55.000000 django_slack_bot-0.8.0/setup.py
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/tests/
--rw-r--r--   0 ST20638    (502) staff       (20)        0 2022-07-08 04:13:44.000000 django_slack_bot-0.8.0/tests/__init__.py
-drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2022-07-26 01:46:53.000000 django_slack_bot-0.8.0/tests/example/
--rw-r--r--   0 ST20638    (502) staff       (20)        0 2022-07-08 04:13:44.000000 django_slack_bot-0.8.0/tests/example/__init__.py
--rw-r--r--   0 ST20638    (502) staff       (20)      864 2022-07-08 04:44:40.000000 django_slack_bot-0.8.0/tests/example/__main__.py
--rw-r--r--   0 ST20638    (502) staff       (20)     1405 2022-07-08 05:07:59.000000 django_slack_bot-0.8.0/tests/example/settings.py
--rw-r--r--   0 ST20638    (502) staff       (20)      118 2022-07-08 04:13:44.000000 django_slack_bot-0.8.0/tests/example/urls.py
--rw-r--r--   0 ST20638    (502) staff       (20)     1274 2022-07-08 05:07:59.000000 django_slack_bot-0.8.0/tests/test_exceptions.py
--rw-r--r--   0 ST20638    (502) staff       (20)      959 2022-07-26 01:40:56.000000 django_slack_bot-0.8.0/tests/test_util.py
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/
+-rw-r--r--   0 ST20638    (502) staff       (20)      521 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/PKG-INFO
+-rw-r--r--   0 ST20638    (502) staff       (20)        7 2021-07-02 04:48:53.000000 django_slack_bot-0.8.1/README.md
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/django_slack_bot.egg-info/
+-rw-r--r--   0 ST20638    (502) staff       (20)      521 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/django_slack_bot.egg-info/PKG-INFO
+-rw-r--r--   0 ST20638    (502) staff       (20)      745 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/django_slack_bot.egg-info/SOURCES.txt
+-rw-r--r--   0 ST20638    (502) staff       (20)        1 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/django_slack_bot.egg-info/dependency_links.txt
+-rw-r--r--   0 ST20638    (502) staff       (20)      121 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/django_slack_bot.egg-info/entry_points.txt
+-rw-r--r--   0 ST20638    (502) staff       (20)      116 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/django_slack_bot.egg-info/requires.txt
+-rw-r--r--   0 ST20638    (502) staff       (20)       12 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/django_slack_bot.egg-info/top_level.txt
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/dsbot/
+-rw-r--r--   0 ST20638    (502) staff       (20)        0 2021-07-02 04:48:05.000000 django_slack_bot-0.8.1/dsbot/__init__.py
+-rw-r--r--   0 ST20638    (502) staff       (20)       85 2021-07-02 04:48:05.000000 django_slack_bot-0.8.1/dsbot/apps.py
+-rw-r--r--   0 ST20638    (502) staff       (20)     3658 2022-12-05 02:09:49.000000 django_slack_bot-0.8.1/dsbot/client.py
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/dsbot/commands/
+-rw-r--r--   0 ST20638    (502) staff       (20)        0 2021-07-02 04:48:05.000000 django_slack_bot-0.8.1/dsbot/commands/__init__.py
+-rw-r--r--   0 ST20638    (502) staff       (20)     2026 2022-02-04 08:04:56.000000 django_slack_bot-0.8.1/dsbot/commands/default.py
+-rw-r--r--   0 ST20638    (502) staff       (20)      603 2023-08-02 00:16:13.000000 django_slack_bot-0.8.1/dsbot/conf.py
+-rw-r--r--   0 ST20638    (502) staff       (20)      951 2023-08-02 00:16:13.000000 django_slack_bot-0.8.1/dsbot/decorators.py
+-rw-r--r--   0 ST20638    (502) staff       (20)     1307 2022-07-11 02:30:38.000000 django_slack_bot-0.8.1/dsbot/exceptions.py
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/dsbot/management/
+-rw-r--r--   0 ST20638    (502) staff       (20)        0 2021-07-02 04:48:05.000000 django_slack_bot-0.8.1/dsbot/management/__init__.py
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/dsbot/management/commands/
+-rw-r--r--   0 ST20638    (502) staff       (20)        0 2022-07-22 08:23:16.000000 django_slack_bot-0.8.1/dsbot/management/commands/__init__.py
+-rw-r--r--   0 ST20638    (502) staff       (20)     1729 2023-08-02 00:16:16.000000 django_slack_bot-0.8.1/dsbot/management/commands/bot.py
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/dsbot/migrations/
+-rw-r--r--   0 ST20638    (502) staff       (20)        0 2021-07-02 04:48:05.000000 django_slack_bot-0.8.1/dsbot/migrations/__init__.py
+-rw-r--r--   0 ST20638    (502) staff       (20)      559 2023-08-02 00:16:13.000000 django_slack_bot-0.8.1/dsbot/tasks.py
+-rw-r--r--   0 ST20638    (502) staff       (20)      934 2023-08-02 00:16:13.000000 django_slack_bot-0.8.1/dsbot/util.py
+-rw-r--r--   0 ST20638    (502) staff       (20)     1075 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/setup.cfg
+-rw-r--r--   0 ST20638    (502) staff       (20)       37 2021-07-02 02:49:55.000000 django_slack_bot-0.8.1/setup.py
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/tests/
+-rw-r--r--   0 ST20638    (502) staff       (20)        0 2022-07-08 04:13:44.000000 django_slack_bot-0.8.1/tests/__init__.py
+drwxr-xr-x   0 ST20638    (502) staff       (20)        0 2023-08-02 00:20:12.000000 django_slack_bot-0.8.1/tests/example/
+-rw-r--r--   0 ST20638    (502) staff       (20)        0 2022-07-08 04:13:44.000000 django_slack_bot-0.8.1/tests/example/__init__.py
+-rw-r--r--   0 ST20638    (502) staff       (20)      864 2022-07-08 04:44:40.000000 django_slack_bot-0.8.1/tests/example/__main__.py
+-rw-r--r--   0 ST20638    (502) staff       (20)     1405 2022-07-08 05:07:59.000000 django_slack_bot-0.8.1/tests/example/settings.py
+-rw-r--r--   0 ST20638    (502) staff       (20)      118 2022-07-08 04:13:44.000000 django_slack_bot-0.8.1/tests/example/urls.py
+-rw-r--r--   0 ST20638    (502) staff       (20)     1274 2022-07-08 05:07:59.000000 django_slack_bot-0.8.1/tests/test_exceptions.py
+-rw-r--r--   0 ST20638    (502) staff       (20)      959 2023-08-02 00:16:13.000000 django_slack_bot-0.8.1/tests/test_util.py
```

### Comparing `django_slack_bot-0.8.0/PKG-INFO` & `django_slack_bot-0.8.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_slack_bot
-Version: 0.8.0
+Version: 0.8.1
 Summary: Helpers for integrating Slack + Django
 Home-page: UNKNOWN
 Author: Paul Traylor
 License: UNKNOWN
 Description: # dsbot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django_slack_bot-0.8.0/django_slack_bot.egg-info/PKG-INFO` & `django_slack_bot-0.8.1/django_slack_bot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-slack-bot
-Version: 0.8.0
+Version: 0.8.1
 Summary: Helpers for integrating Slack + Django
 Home-page: UNKNOWN
 Author: Paul Traylor
 License: UNKNOWN
 Description: # dsbot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `django_slack_bot-0.8.0/django_slack_bot.egg-info/SOURCES.txt` & `django_slack_bot-0.8.1/django_slack_bot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/dsbot/client.py` & `django_slack_bot-0.8.1/dsbot/client.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/dsbot/commands/default.py` & `django_slack_bot-0.8.1/dsbot/commands/default.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/dsbot/conf.py` & `django_slack_bot-0.8.1/dsbot/conf.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/dsbot/decorators.py` & `django_slack_bot-0.8.1/dsbot/decorators.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/dsbot/exceptions.py` & `django_slack_bot-0.8.1/dsbot/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/dsbot/management/commands/bot.py` & `django_slack_bot-0.8.1/dsbot/management/commands/bot.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from django.core.management.base import BaseCommand
 from django.test import override_settings
 
 from dsbot.client import BotClient
 from dsbot.conf import settings
 
 try:
-    from importlib.metadata import entry_points
-except ImportError:
     from importlib_metadata import entry_points
+except ImportError:
+    from importlib.metadata import entry_points
 
 
 class Command(BaseCommand):
     def add_arguments(self, parser):
         slack = parser.add_argument_group("Slack arguments")
         slack.add_argument("--token", default=settings.SLACK_TOKEN, help="Slack token")
         slack.add_argument("--timeout", default=30, type=int)
```

### Comparing `django_slack_bot-0.8.0/dsbot/tasks.py` & `django_slack_bot-0.8.1/dsbot/tasks.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/dsbot/util.py` & `django_slack_bot-0.8.1/dsbot/util.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/setup.cfg` & `django_slack_bot-0.8.1/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django_slack_bot
-version = 0.8.0
+version = 0.8.1
 description = Helpers for integrating Slack + Django
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Paul Traylor
 classifiers = 
 	Development Status :: 3 - Alpha
 	Framework :: Django
@@ -16,15 +16,15 @@
 [options]
 packages = find:
 install_requires = 
 	Django>=3.2
 	aiohttp
 	celery
 	slack-sdk>=3.5.1
-	importlib-metadata>=1.0 ;python_version < "3.8"
+	importlib-metadata>=1.0 ;python_version < "3.10"
 
 [options.packages.find]
 exclude = 
 	dsbot.example
 	dsbot.tests
 
 [options.entry_points]
```

### Comparing `django_slack_bot-0.8.0/tests/example/__main__.py` & `django_slack_bot-0.8.1/tests/example/__main__.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/tests/example/settings.py` & `django_slack_bot-0.8.1/tests/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/tests/test_exceptions.py` & `django_slack_bot-0.8.1/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django_slack_bot-0.8.0/tests/test_util.py` & `django_slack_bot-0.8.1/tests/test_util.py`

 * *Files identical despite different names*

