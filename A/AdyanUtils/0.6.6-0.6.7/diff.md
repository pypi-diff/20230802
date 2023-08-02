# Comparing `tmp/AdyanUtils-0.6.6.tar.gz` & `tmp/AdyanUtils-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AdyanUtils-0.6.6.tar", last modified: Wed Jun 21 05:22:31 2023, max compression
+gzip compressed data, was "AdyanUtils-0.6.7.tar", last modified: Wed Aug  2 06:59:32 2023, max compression
```

## Comparing `AdyanUtils-0.6.6.tar` & `AdyanUtils-0.6.7.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-21 05:22:31.388427 AdyanUtils-0.6.6/
-drwxrwxrwx   0        0        0        0 2023-06-21 05:22:31.372430 AdyanUtils-0.6.6/AdyanUtils.egg-info/
--rw-rw-rw-   0        0        0     1831 2023-06-21 05:22:31.000000 AdyanUtils-0.6.6/AdyanUtils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-06-21 05:22:31.000000 AdyanUtils-0.6.6/AdyanUtils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-21 05:22:31.000000 AdyanUtils-0.6.6/AdyanUtils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      197 2023-06-21 05:22:31.000000 AdyanUtils-0.6.6/AdyanUtils.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-21 05:22:31.000000 AdyanUtils-0.6.6/AdyanUtils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2022-04-12 02:49:17.000000 AdyanUtils-0.6.6/LICENSE
--rw-rw-rw-   0        0        0     1831 2023-06-21 05:22:31.387427 AdyanUtils-0.6.6/PKG-INFO
--rw-rw-rw-   0        0        0     1410 2022-04-12 02:49:17.000000 AdyanUtils-0.6.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-21 05:22:31.373432 AdyanUtils-0.6.6/Utils/
--rw-rw-rw-   0        0        0      563 2022-04-27 01:17:08.000000 AdyanUtils-0.6.6/Utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:22:31.376436 AdyanUtils-0.6.6/Utils/connect/
--rw-rw-rw-   0        0        0      131 2022-04-27 01:21:59.000000 AdyanUtils-0.6.6/Utils/connect/__init__.py
--rw-rw-rw-   0        0        0     4227 2023-06-21 05:22:20.000000 AdyanUtils-0.6.6/Utils/connect/mongo_conn.py
--rw-rw-rw-   0        0        0     3806 2022-08-10 02:25:33.000000 AdyanUtils-0.6.6/Utils/connect/rabbit_conn.py
--rw-rw-rw-   0        0        0     4497 2022-09-22 08:56:08.000000 AdyanUtils-0.6.6/Utils/connect/redis_conn.py
-drwxrwxrwx   0        0        0        0 2023-06-21 05:22:31.386427 AdyanUtils-0.6.6/Utils/crawler/
--rw-rw-rw-   0        0        0     4687 2023-06-19 08:39:04.000000 AdyanUtils-0.6.6/Utils/crawler/Forge.py
--rw-rw-rw-   0        0        0      131 2022-04-27 01:17:08.000000 AdyanUtils-0.6.6/Utils/crawler/__init__.py
--rw-rw-rw-   0        0        0     4696 2022-09-07 06:52:36.000000 AdyanUtils-0.6.6/Utils/crawler/function.py
--rw-rw-rw-   0        0        0     2749 2022-06-25 01:26:17.000000 AdyanUtils-0.6.6/Utils/crawler/init.py
--rw-rw-rw-   0        0        0     4269 2022-07-29 05:02:05.000000 AdyanUtils-0.6.6/Utils/crawler/middleware.py
--rw-rw-rw-   0        0        0     5260 2022-04-12 02:49:17.000000 AdyanUtils-0.6.6/Utils/crawler/proxy.py
--rw-rw-rw-   0        0        0     1510 2022-04-27 01:08:27.000000 AdyanUtils-0.6.6/Utils/crawler/save_xls.py
--rw-rw-rw-   0        0        0     1641 2022-04-27 01:08:33.000000 AdyanUtils-0.6.6/Utils/crawler/scheduler.py
--rw-rw-rw-   0        0        0      108 2022-04-12 02:49:17.000000 AdyanUtils-0.6.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-21 05:22:31.388427 AdyanUtils-0.6.6/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-06-21 05:22:20.000000 AdyanUtils-0.6.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:59:32.308449 AdyanUtils-0.6.7/
+drwxrwxrwx   0        0        0        0 2023-08-02 06:59:32.293443 AdyanUtils-0.6.7/AdyanUtils.egg-info/
+-rw-rw-rw-   0        0        0     1831 2023-08-02 06:59:32.000000 AdyanUtils-0.6.7/AdyanUtils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-08-02 06:59:32.000000 AdyanUtils-0.6.7/AdyanUtils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 06:59:32.000000 AdyanUtils-0.6.7/AdyanUtils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2023-08-02 06:59:32.000000 AdyanUtils-0.6.7/AdyanUtils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 06:59:32.000000 AdyanUtils-0.6.7/AdyanUtils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2022-04-12 02:49:17.000000 AdyanUtils-0.6.7/LICENSE
+-rw-rw-rw-   0        0        0     1831 2023-08-02 06:59:32.307435 AdyanUtils-0.6.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1410 2022-04-12 02:49:17.000000 AdyanUtils-0.6.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 06:59:32.294443 AdyanUtils-0.6.7/Utils/
+-rw-rw-rw-   0        0        0      563 2022-04-27 01:17:08.000000 AdyanUtils-0.6.7/Utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:59:32.298434 AdyanUtils-0.6.7/Utils/connect/
+-rw-rw-rw-   0        0        0      131 2022-04-27 01:21:59.000000 AdyanUtils-0.6.7/Utils/connect/__init__.py
+-rw-rw-rw-   0        0        0     4227 2023-06-21 05:22:20.000000 AdyanUtils-0.6.7/Utils/connect/mongo_conn.py
+-rw-rw-rw-   0        0        0     3806 2022-08-10 02:25:33.000000 AdyanUtils-0.6.7/Utils/connect/rabbit_conn.py
+-rw-rw-rw-   0        0        0     4497 2022-09-22 08:56:08.000000 AdyanUtils-0.6.7/Utils/connect/redis_conn.py
+drwxrwxrwx   0        0        0        0 2023-08-02 06:59:32.306435 AdyanUtils-0.6.7/Utils/crawler/
+-rw-rw-rw-   0        0        0     5010 2023-08-02 06:08:26.000000 AdyanUtils-0.6.7/Utils/crawler/Forge.py
+-rw-rw-rw-   0        0        0      131 2022-04-27 01:17:08.000000 AdyanUtils-0.6.7/Utils/crawler/__init__.py
+-rw-rw-rw-   0        0        0     4696 2022-09-07 06:52:36.000000 AdyanUtils-0.6.7/Utils/crawler/function.py
+-rw-rw-rw-   0        0        0     2749 2022-06-25 01:26:17.000000 AdyanUtils-0.6.7/Utils/crawler/init.py
+-rw-rw-rw-   0        0        0     4269 2022-07-29 05:02:05.000000 AdyanUtils-0.6.7/Utils/crawler/middleware.py
+-rw-rw-rw-   0        0        0     5260 2022-04-12 02:49:17.000000 AdyanUtils-0.6.7/Utils/crawler/proxy.py
+-rw-rw-rw-   0        0        0     1510 2022-04-27 01:08:27.000000 AdyanUtils-0.6.7/Utils/crawler/save_xls.py
+-rw-rw-rw-   0        0        0     1641 2022-04-27 01:08:33.000000 AdyanUtils-0.6.7/Utils/crawler/scheduler.py
+-rw-rw-rw-   0        0        0      108 2022-04-12 02:49:17.000000 AdyanUtils-0.6.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 06:59:32.308449 AdyanUtils-0.6.7/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-08-02 06:08:26.000000 AdyanUtils-0.6.7/setup.py
```

### Comparing `AdyanUtils-0.6.6/AdyanUtils.egg-info/PKG-INFO` & `AdyanUtils-0.6.7/AdyanUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdyanUtils
-Version: 0.6.6
+Version: 0.6.7
 Summary: Special package
 Home-page: https://gitee.com/liujiang99/AdyanUtils
 Author: Adyan
 Author-email: 228923910@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AdyanUtils-0.6.6/AdyanUtils.egg-info/SOURCES.txt` & `AdyanUtils-0.6.7/AdyanUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/LICENSE` & `AdyanUtils-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/PKG-INFO` & `AdyanUtils-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AdyanUtils
-Version: 0.6.6
+Version: 0.6.7
 Summary: Special package
 Home-page: https://gitee.com/liujiang99/AdyanUtils
 Author: Adyan
 Author-email: 228923910@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `AdyanUtils-0.6.6/README.md` & `AdyanUtils-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/__init__.py` & `AdyanUtils-0.6.7/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/connect/mongo_conn.py` & `AdyanUtils-0.6.7/Utils/connect/mongo_conn.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/connect/rabbit_conn.py` & `AdyanUtils-0.6.7/Utils/connect/rabbit_conn.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/connect/redis_conn.py` & `AdyanUtils-0.6.7/Utils/connect/redis_conn.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/crawler/Forge.py` & `AdyanUtils-0.6.7/Utils/crawler/Forge.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 import hashlib
 import logging
 import queue
 import random
 import re
 import threading
 import urllib.parse
+import cpca
 
 from faker import Faker
 from requests import sessions
 
 fake = Faker()
 
 
@@ -55,14 +56,23 @@
         lsl.append(l)
     for x in lsl:
         headers[str(x[0]).strip('    ')] = x[1]
 
     return headers
 
 
+def address(address: list):
+    area_list = cpca.transform(address).values.tolist()[0]
+    data = {"province": area_list[0], "city": area_list[1], "district": area_list[2]}
+    while "None" in area_list:
+        area_list.remove("None")
+    data["address"] = "".join(area_list[:-1])
+    return data
+
+
 class Headers:
 
     @classmethod
     def user_agent(cls, mobile_headers):
         while True:
             user_agent = fake.chrome(
                 version_from=63, version_to=80,
```

### Comparing `AdyanUtils-0.6.6/Utils/crawler/function.py` & `AdyanUtils-0.6.7/Utils/crawler/function.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/crawler/init.py` & `AdyanUtils-0.6.7/Utils/crawler/init.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/crawler/middleware.py` & `AdyanUtils-0.6.7/Utils/crawler/middleware.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/crawler/proxy.py` & `AdyanUtils-0.6.7/Utils/crawler/proxy.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/crawler/save_xls.py` & `AdyanUtils-0.6.7/Utils/crawler/save_xls.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/Utils/crawler/scheduler.py` & `AdyanUtils-0.6.7/Utils/crawler/scheduler.py`

 * *Files identical despite different names*

### Comparing `AdyanUtils-0.6.6/setup.py` & `AdyanUtils-0.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="AdyanUtils",
-    version="0.6.6",
+    version="0.6.7",
     author="Adyan",
     author_email="228923910@qq.com",
     description="Special package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/liujiang99/AdyanUtils",
     packages=setuptools.find_packages(),
```

