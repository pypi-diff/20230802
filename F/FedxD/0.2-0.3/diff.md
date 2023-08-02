# Comparing `tmp/FedxD-0.2.tar.gz` & `tmp/FedxD-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FedxD-0.2.tar", last modified: Wed Aug  2 08:25:13 2023, max compression
+gzip compressed data, was "FedxD-0.3.tar", last modified: Wed Aug  2 08:30:57 2023, max compression
```

## Comparing `FedxD-0.2.tar` & `FedxD-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:25:13.514978 FedxD-0.2/
-drwxrwxrwx   0        0        0        0 2023-08-02 08:25:13.480997 FedxD-0.2/FedxD/
--rw-rw-rw-   0        0        0       31 2023-08-02 08:23:19.000000 FedxD-0.2/FedxD/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-08-01 22:34:49.000000 FedxD-0.2/FedxD/color.py
--rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.2/FedxD/converters.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:25:13.508981 FedxD-0.2/FedxD.egg-info/
--rw-rw-rw-   0        0        0     1520 2023-08-02 08:25:12.000000 FedxD-0.2/FedxD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-02 08:25:12.000000 FedxD-0.2/FedxD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:25:12.000000 FedxD-0.2/FedxD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 08:25:12.000000 FedxD-0.2/FedxD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.2/License.txt
--rw-rw-rw-   0        0        0     1520 2023-08-02 08:25:13.511979 FedxD-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-02 08:25:13.515977 FedxD-0.2/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-08-02 07:55:16.000000 FedxD-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:30:57.722841 FedxD-0.3/
+drwxrwxrwx   0        0        0        0 2023-08-02 08:30:57.690861 FedxD-0.3/FedxD/
+-rw-rw-rw-   0        0        0        0 2023-08-02 08:30:38.000000 FedxD-0.3/FedxD/__init__.py
+-rw-rw-rw-   0        0        0     2226 2023-08-01 22:34:49.000000 FedxD-0.3/FedxD/color.py
+-rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.3/FedxD/converters.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:30:57.714846 FedxD-0.3/FedxD.egg-info/
+-rw-rw-rw-   0        0        0     1549 2023-08-02 08:30:57.000000 FedxD-0.3/FedxD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-02 08:30:57.000000 FedxD-0.3/FedxD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:30:57.000000 FedxD-0.3/FedxD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 08:30:57.000000 FedxD-0.3/FedxD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.3/License.txt
+-rw-rw-rw-   0        0        0     1549 2023-08-02 08:30:57.720842 FedxD-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:30:57.722841 FedxD-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-08-02 08:30:38.000000 FedxD-0.3/setup.py
```

### Comparing `FedxD-0.2/FedxD/color.py` & `FedxD-0.3/FedxD/color.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.2/FedxD/converters.py` & `FedxD-0.3/FedxD/converters.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.2/FedxD.egg-info/PKG-INFO` & `FedxD-0.3/FedxD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.2
+Version: 0.3
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,10 +41,11 @@
    cm to inch and vice versa, and Meter and Foot To Yard)
     5. Temperature
    <br>(Converts Celcius to Farenhiet and vice versa ,
    and Celcius and Farenhiet To Kelvin and vice versa)
    
 Version = 0.1 (testing)
 Version = 0.2 (Fixing Bugs and testing)
+Version = 0.3 (Fixing Bugs)
```

### Comparing `FedxD-0.2/License.txt` & `FedxD-0.3/License.txt`

 * *Files identical despite different names*

### Comparing `FedxD-0.2/PKG-INFO` & `FedxD-0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.2
+Version: 0.3
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -41,10 +41,11 @@
    cm to inch and vice versa, and Meter and Foot To Yard)
     5. Temperature
    <br>(Converts Celcius to Farenhiet and vice versa ,
    and Celcius and Farenhiet To Kelvin and vice versa)
    
 Version = 0.1 (testing)
 Version = 0.2 (Fixing Bugs and testing)
+Version = 0.3 (Fixing Bugs)
```

### Comparing `FedxD-0.2/setup.py` & `FedxD-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import twine
 from setuptools import setup , find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(name='FedxD',
-    version='0.2',
+    version='0.3',
     packages=['FedxD'],
     author='FedxD',
     author_email='abbaskazim135@gmail.com',
     description='This Package is for Quality of life stuff that you will need in your project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/FedxD',
```

