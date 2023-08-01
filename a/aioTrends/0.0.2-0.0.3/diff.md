# Comparing `tmp/aioTrends-0.0.2.tar.gz` & `tmp/aioTrends-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioTrends-0.0.2.tar", last modified: Tue Aug  1 23:09:35 2023, max compression
+gzip compressed data, was "aioTrends-0.0.3.tar", last modified: Tue Aug  1 23:19:56 2023, max compression
```

## Comparing `aioTrends-0.0.2.tar` & `aioTrends-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,36 @@
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:09:35.911794 aioTrends-0.0.2/
--rw-r--r--   0 stephencheung   (501) staff       (20)     6571 2023-08-01 23:09:35.910794 aioTrends-0.0.2/PKG-INFO
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:09:35.899302 aioTrends-0.0.2/aioTrends/
--rw-r--r--   0 stephencheung   (501) staff       (20)     1363 2023-08-01 23:09:07.000000 aioTrends-0.0.2/aioTrends/SETUP.py
--rw-r--r--   0 stephencheung   (501) staff       (20)      688 2023-08-01 22:49:00.000000 aioTrends-0.0.2/aioTrends/test_example.py
-drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:09:35.909461 aioTrends-0.0.2/aioTrends.egg-info/
--rw-r--r--   0 stephencheung   (501) staff       (20)     6571 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/PKG-INFO
--rw-r--r--   0 stephencheung   (501) staff       (20)      208 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/SOURCES.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/dependency_links.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)       59 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/requires.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)       10 2023-08-01 23:09:35.000000 aioTrends-0.0.2/aioTrends.egg-info/top_level.txt
--rw-r--r--   0 stephencheung   (501) staff       (20)       38 2023-08-01 23:09:35.912011 aioTrends-0.0.2/setup.cfg
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:19:56.652880 aioTrends-0.0.3/
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:19:56.590997 aioTrends-0.0.3/.github/
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:19:56.630999 aioTrends-0.0.3/.github/ISSUE_TEMPLATE/
+-rwx------   0 stephencheung   (501) staff       (20)      872 2023-01-18 14:13:30.000000 aioTrends-0.0.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rwx------   0 stephencheung   (501) staff       (20)      136 2023-01-18 14:13:30.000000 aioTrends-0.0.3/.github/ISSUE_TEMPLATE/custom.md
+-rwx------   0 stephencheung   (501) staff       (20)      615 2023-01-18 14:13:30.000000 aioTrends-0.0.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rwx------   0 stephencheung   (501) staff       (20)     1085 2023-01-13 12:09:51.000000 aioTrends-0.0.3/LICENSE
+-rw-r--r--   0 stephencheung   (501) staff       (20)     6593 2023-08-01 23:19:56.653173 aioTrends-0.0.3/PKG-INFO
+-rwx------   0 stephencheung   (501) staff       (20)     5902 2023-08-01 23:01:51.000000 aioTrends-0.0.3/README.md
+-rwx------   0 stephencheung   (501) staff       (20)      640 2023-01-13 12:09:51.000000 aioTrends-0.0.3/SECURITY.md
+-rw-r--r--   0 stephencheung   (501) staff       (20)     1363 2023-08-01 23:19:40.000000 aioTrends-0.0.3/SETUP.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:19:56.635102 aioTrends-0.0.3/aioTrends/
+-rwx------   0 stephencheung   (501) staff       (20)      477 2023-01-18 14:13:31.000000 aioTrends-0.0.3/aioTrends/HandleExceptions.py
+-rwx------   0 stephencheung   (501) staff       (20)     6562 2023-07-24 14:41:43.000000 aioTrends-0.0.3/aioTrends/Settings.py
+-rwx------   0 stephencheung   (501) staff       (20)    37436 2023-08-01 22:10:40.000000 aioTrends-0.0.3/aioTrends/Trends.py
+-rwx------   0 stephencheung   (501) staff       (20)      377 2023-07-24 15:43:56.000000 aioTrends-0.0.3/aioTrends/__init__.py
+-rwx------   0 stephencheung   (501) staff       (20)     8836 2023-08-01 21:46:02.000000 aioTrends-0.0.3/aioTrends/processData.py
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:19:56.639851 aioTrends-0.0.3/aioTrends.egg-info/
+-rw-r--r--   0 stephencheung   (501) staff       (20)     6593 2023-08-01 23:19:56.000000 aioTrends-0.0.3/aioTrends.egg-info/PKG-INFO
+-rw-r--r--   0 stephencheung   (501) staff       (20)      625 2023-08-01 23:19:56.000000 aioTrends-0.0.3/aioTrends.egg-info/SOURCES.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)        1 2023-08-01 23:19:56.000000 aioTrends-0.0.3/aioTrends.egg-info/dependency_links.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)       59 2023-08-01 23:19:56.000000 aioTrends-0.0.3/aioTrends.egg-info/requires.txt
+-rw-r--r--   0 stephencheung   (501) staff       (20)       10 2023-08-01 23:19:56.000000 aioTrends-0.0.3/aioTrends.egg-info/top_level.txt
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:19:56.641883 aioTrends-0.0.3/data/
+-rwx------   0 stephencheung   (501) staff       (20)        0 2023-01-11 11:54:13.000000 aioTrends-0.0.3/data/IOT
+-rwx------   0 stephencheung   (501) staff       (20)      394 2023-07-26 11:15:48.000000 aioTrends-0.0.3/data/qrys.pkl
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:19:56.644372 aioTrends-0.0.3/proxies/
+-rwx------   0 stephencheung   (501) staff       (20)   109998 2023-07-26 11:13:34.000000 aioTrends-0.0.3/proxies/proxies.txt
+-rwx------   0 stephencheung   (501) staff       (20)       42 2023-07-24 13:27:06.000000 aioTrends-0.0.3/requirements.txt
+drwxr-xr-x   0 stephencheung   (501) staff       (20)        0 2023-08-01 23:19:56.649086 aioTrends-0.0.3/settings/
+-rwx------   0 stephencheung   (501) staff       (20)      531 2023-01-31 11:00:36.000000 aioTrends-0.0.3/settings/settings.json
+-rwx------   0 stephencheung   (501) staff       (20)   132936 2022-07-05 12:28:50.000000 aioTrends-0.0.3/settings/userAgents.json
+-rw-r--r--   0 stephencheung   (501) staff       (20)       79 2023-08-01 23:19:56.654084 aioTrends-0.0.3/setup.cfg
+-rw-r--r--   0 stephencheung   (501) staff       (20)      688 2023-08-01 22:49:00.000000 aioTrends-0.0.3/test_example.py
+-rw-r--r--   0 stephencheung   (501) staff       (20)   176187 2023-08-01 22:51:04.000000 aioTrends-0.0.3/test_monthly_data.png
+-rw-r--r--   0 stephencheung   (501) staff       (20)   115723 2023-08-01 22:51:12.000000 aioTrends-0.0.3/test_scaled_daily_data.png
```

### Comparing `aioTrends-0.0.2/PKG-INFO` & `aioTrends-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aioTrends
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for fetching Google Trends in an async. way
 Home-page: https://github.com/yuz0101/aioTrends
 Download-URL: https://github.com/yuz0101/aioTrends/archive/refs/tags/v_02.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: google,trends,async,asyncio,aiohttp,googletrends,pytrends
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # aioTrends
 
 ## Intro.
 
 This is a project for asynchronously obtaining data from google trends in an efficient way. Inspired by [pytrends](https://github.com/GeneralMills/pytrends), I am developing this project based on a asynchronous framework, asyncio, and a related module, [aiohttp](https://github.com/aio-libs/aiohttp).
```

### Comparing `aioTrends-0.0.2/aioTrends/SETUP.py` & `aioTrends-0.0.3/SETUP.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="aioTrends",
     packages=["aioTrends"],
-    version="0.0.2",
+    version="0.0.3",
     license="MIT",
     description="Library for fetching Google Trends in an async. way",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Stephen Zhang",
     author_email="stephen_se@outlook.com",
     url="https://github.com/yuz0101/aioTrends",
```

### Comparing `aioTrends-0.0.2/aioTrends/test_example.py` & `aioTrends-0.0.3/test_example.py`

 * *Files identical despite different names*

### Comparing `aioTrends-0.0.2/aioTrends.egg-info/PKG-INFO` & `aioTrends-0.0.3/aioTrends.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: aioTrends
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for fetching Google Trends in an async. way
 Home-page: https://github.com/yuz0101/aioTrends
 Download-URL: https://github.com/yuz0101/aioTrends/archive/refs/tags/v_02.tar.gz
 Author: Stephen Zhang
 Author-email: stephen_se@outlook.com
 License: MIT
 Keywords: google,trends,async,asyncio,aiohttp,googletrends,pytrends
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # aioTrends
 
 ## Intro.
 
 This is a project for asynchronously obtaining data from google trends in an efficient way. Inspired by [pytrends](https://github.com/GeneralMills/pytrends), I am developing this project based on a asynchronous framework, asyncio, and a related module, [aiohttp](https://github.com/aio-libs/aiohttp).
```

