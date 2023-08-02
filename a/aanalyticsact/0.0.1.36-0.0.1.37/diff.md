# Comparing `tmp/aanalyticsact-0.0.1.36.tar.gz` & `tmp/aanalyticsact-0.0.1.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aanalyticsact-0.0.1.36.tar", last modified: Thu Jul 20 00:19:31 2023, max compression
+gzip compressed data, was "aanalyticsact-0.0.1.37.tar", last modified: Wed Aug  2 02:06:47 2023, max compression
```

## Comparing `aanalyticsact-0.0.1.36.tar` & `aanalyticsact-0.0.1.37.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 00:19:31.569693 aanalyticsact-0.0.1.36/
--rw-rw-rw-   0        0        0     1216 2023-07-20 00:19:31.571118 aanalyticsact-0.0.1.36/PKG-INFO
--rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.36/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 00:19:31.510869 aanalyticsact-0.0.1.36/aanalyticsact/
--rw-rw-rw-   0        0        0      118 2023-07-12 05:33:21.000000 aanalyticsact-0.0.1.36/aanalyticsact/__init__.py
--rw-rw-rw-   0        0        0       24 2023-07-20 00:14:02.000000 aanalyticsact-0.0.1.36/aanalyticsact/__version__.py
--rw-rw-rw-   0        0        0     6727 2023-07-20 00:15:03.000000 aanalyticsact-0.0.1.36/aanalyticsact/actExecute.py
--rw-rw-rw-   0        0        0    15589 2023-07-20 00:18:30.000000 aanalyticsact-0.0.1.36/aanalyticsact/actModuler.py
--rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.36/aanalyticsact/actRunner.py
-drwxrwxrwx   0        0        0        0 2023-07-20 00:19:31.563714 aanalyticsact-0.0.1.36/aanalyticsact.egg-info/
--rw-rw-rw-   0        0        0     1216 2023-07-20 00:19:30.000000 aanalyticsact-0.0.1.36/aanalyticsact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      314 2023-07-20 00:19:31.000000 aanalyticsact-0.0.1.36/aanalyticsact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 00:19:30.000000 aanalyticsact-0.0.1.36/aanalyticsact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-20 00:19:30.000000 aanalyticsact-0.0.1.36/aanalyticsact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-07-20 00:19:31.580248 aanalyticsact-0.0.1.36/setup.cfg
--rw-rw-rw-   0        0        0      696 2023-07-20 00:01:34.000000 aanalyticsact-0.0.1.36/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:06:47.532731 aanalyticsact-0.0.1.37/
+-rw-rw-rw-   0        0        0     1216 2023-08-02 02:06:47.534312 aanalyticsact-0.0.1.37/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.37/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 02:06:47.482580 aanalyticsact-0.0.1.37/aanalyticsact/
+-rw-rw-rw-   0        0        0      118 2023-07-12 05:33:21.000000 aanalyticsact-0.0.1.37/aanalyticsact/__init__.py
+-rw-rw-rw-   0        0        0       24 2023-08-02 02:05:35.000000 aanalyticsact-0.0.1.37/aanalyticsact/__version__.py
+-rw-rw-rw-   0        0        0     6727 2023-07-20 00:15:03.000000 aanalyticsact-0.0.1.37/aanalyticsact/actExecute.py
+-rw-rw-rw-   0        0        0    15611 2023-08-02 02:05:58.000000 aanalyticsact-0.0.1.37/aanalyticsact/actModuler.py
+-rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.37/aanalyticsact/actRunner.py
+drwxrwxrwx   0        0        0        0 2023-08-02 02:06:47.524510 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/
+-rw-rw-rw-   0        0        0     1216 2023-08-02 02:06:46.000000 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      314 2023-08-02 02:06:47.000000 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 02:06:46.000000 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-08-02 02:06:46.000000 aanalyticsact-0.0.1.37/aanalyticsact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-02 02:06:47.541452 aanalyticsact-0.0.1.37/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-08-02 02:05:36.000000 aanalyticsact-0.0.1.37/setup.py
```

### Comparing `aanalyticsact-0.0.1.36/PKG-INFO` & `aanalyticsact-0.0.1.37/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.1.36
+Version: 0.0.1.37
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.1.36/README.md` & `aanalyticsact-0.0.1.37/README.md`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.36/aanalyticsact/actExecute.py` & `aanalyticsact-0.0.1.37/aanalyticsact/actExecute.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.36/aanalyticsact/actModuler.py` & `aanalyticsact-0.0.1.37/aanalyticsact/actModuler.py`

 * *Files 1% similar despite different names*

```diff
@@ -286,15 +286,15 @@
             dataFrame2.insert(5, "is_us_epp", epp, True)
 
             dataFrame2.columns = tbColumn
             stackTodb(dataFrame2, dbTableName)
 
     else:
         dataInitiator()
-        dateChange = jsonDateChange(startDate, endDate, jsonFile)
+        dateChange = jsonDateChange(startDate, endDate, jsonFile, start_hour, end_hour)
         dataFrame = dataretriever_data(dateChange)
 
         dataFrame.columns = list(map(int, range(dataFrame.shape[1])))
         
         if limit == 0:
             dataFrame2 = dataFrame
         else:
```

### Comparing `aanalyticsact-0.0.1.36/aanalyticsact/actRunner.py` & `aanalyticsact-0.0.1.37/aanalyticsact/actRunner.py`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.1.36/aanalyticsact.egg-info/PKG-INFO` & `aanalyticsact-0.0.1.37/aanalyticsact.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.1.36
+Version: 0.0.1.37
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
 Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aanalyticsact-0.0.1.36/setup.py` & `aanalyticsact-0.0.1.37/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aanalyticsact",
-    version="0.0.1.36",
+    version="0.0.1.37",
     author="Sunkyeong Lee",
     author_email="sunkyeong.lee@concentrix.com",
     description="adobe analytics library for Team ACT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SunkyeongLee/aanalyticsact",
     packages=setuptools.find_packages(),
```

