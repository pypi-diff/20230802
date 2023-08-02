# Comparing `tmp/FedxD-0.1.tar.gz` & `tmp/FedxD-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FedxD-0.1.tar", last modified: Tue Aug  1 23:13:51 2023, max compression
+gzip compressed data, was "FedxD-0.2.tar", last modified: Wed Aug  2 08:25:13 2023, max compression
```

## Comparing `FedxD-0.1.tar` & `FedxD-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 23:13:51.592480 FedxD-0.1/
-drwxrwxrwx   0        0        0        0 2023-08-01 23:13:51.575490 FedxD-0.1/FedxD/
--rw-rw-rw-   0        0        0       31 2023-08-01 22:49:36.000000 FedxD-0.1/FedxD/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-08-01 22:34:49.000000 FedxD-0.1/FedxD/color.py
--rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.1/FedxD/converters.py
-drwxrwxrwx   0        0        0        0 2023-08-01 23:13:51.581487 FedxD-0.1/FedxD.egg-info/
--rw-rw-rw-   0        0        0     1469 2023-08-01 23:13:51.000000 FedxD-0.1/FedxD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-01 23:13:51.000000 FedxD-0.1/FedxD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 23:13:51.000000 FedxD-0.1/FedxD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-01 23:13:51.000000 FedxD-0.1/FedxD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.1/License.txt
--rw-rw-rw-   0        0        0     1469 2023-08-01 23:13:51.591481 FedxD-0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-01 23:13:51.593479 FedxD-0.1/setup.cfg
--rw-rw-rw-   0        0        0      720 2023-08-01 23:12:41.000000 FedxD-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:25:13.514978 FedxD-0.2/
+drwxrwxrwx   0        0        0        0 2023-08-02 08:25:13.480997 FedxD-0.2/FedxD/
+-rw-rw-rw-   0        0        0       31 2023-08-02 08:23:19.000000 FedxD-0.2/FedxD/__init__.py
+-rw-rw-rw-   0        0        0     2226 2023-08-01 22:34:49.000000 FedxD-0.2/FedxD/color.py
+-rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.2/FedxD/converters.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:25:13.508981 FedxD-0.2/FedxD.egg-info/
+-rw-rw-rw-   0        0        0     1520 2023-08-02 08:25:12.000000 FedxD-0.2/FedxD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-02 08:25:12.000000 FedxD-0.2/FedxD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:25:12.000000 FedxD-0.2/FedxD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 08:25:12.000000 FedxD-0.2/FedxD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.2/License.txt
+-rw-rw-rw-   0        0        0     1520 2023-08-02 08:25:13.511979 FedxD-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:25:13.515977 FedxD-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-08-02 07:55:16.000000 FedxD-0.2/setup.py
```

### Comparing `FedxD-0.1/FedxD/color.py` & `FedxD-0.2/FedxD/color.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.1/FedxD/converters.py` & `FedxD-0.2/FedxD/converters.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.1/FedxD.egg-info/PKG-INFO` & `FedxD-0.2/FedxD.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.1
+Version: 0.2
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,11 +39,12 @@
    4. Lenght
    <br>(Converts Meter To Foot and vice versa,
    cm to inch and vice versa, and Meter and Foot To Yard)
     5. Temperature
    <br>(Converts Celcius to Farenhiet and vice versa ,
    and Celcius and Farenhiet To Kelvin and vice versa)
    
-Version = 0.1
+Version = 0.1 (testing)
+Version = 0.2 (Fixing Bugs and testing)
```

### Comparing `FedxD-0.1/License.txt` & `FedxD-0.2/License.txt`

 * *Files identical despite different names*

### Comparing `FedxD-0.1/PKG-INFO` & `FedxD-0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.1
+Version: 0.2
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,11 +39,12 @@
    4. Lenght
    <br>(Converts Meter To Foot and vice versa,
    cm to inch and vice versa, and Meter and Foot To Yard)
     5. Temperature
    <br>(Converts Celcius to Farenhiet and vice versa ,
    and Celcius and Farenhiet To Kelvin and vice versa)
    
-Version = 0.1
+Version = 0.1 (testing)
+Version = 0.2 (Fixing Bugs and testing)
```

### Comparing `FedxD-0.1/setup.py` & `FedxD-0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import twine
 from setuptools import setup , find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(name='FedxD',
-    version='0.1',
-    packages=find_packages(),
+    version='0.2',
+    packages=['FedxD'],
     author='FedxD',
     author_email='abbaskazim135@gmail.com',
     description='This Package is for Quality of life stuff that you will need in your project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/FedxD',
     license='MIT',
```

