# Comparing `tmp/FedxD-0.3.tar.gz` & `tmp/FedxD-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FedxD-0.3.tar", last modified: Wed Aug  2 08:30:57 2023, max compression
+gzip compressed data, was "FedxD-0.4.tar", last modified: Wed Aug  2 08:39:11 2023, max compression
```

## Comparing `FedxD-0.3.tar` & `FedxD-0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:30:57.722841 FedxD-0.3/
-drwxrwxrwx   0        0        0        0 2023-08-02 08:30:57.690861 FedxD-0.3/FedxD/
--rw-rw-rw-   0        0        0        0 2023-08-02 08:30:38.000000 FedxD-0.3/FedxD/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-08-01 22:34:49.000000 FedxD-0.3/FedxD/color.py
--rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.3/FedxD/converters.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:30:57.714846 FedxD-0.3/FedxD.egg-info/
--rw-rw-rw-   0        0        0     1549 2023-08-02 08:30:57.000000 FedxD-0.3/FedxD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-02 08:30:57.000000 FedxD-0.3/FedxD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:30:57.000000 FedxD-0.3/FedxD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 08:30:57.000000 FedxD-0.3/FedxD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.3/License.txt
--rw-rw-rw-   0        0        0     1549 2023-08-02 08:30:57.720842 FedxD-0.3/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-02 08:30:57.722841 FedxD-0.3/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-08-02 08:30:38.000000 FedxD-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:39:11.916834 FedxD-0.4/
+drwxrwxrwx   0        0        0        0 2023-08-02 08:39:11.901795 FedxD-0.4/FedxD/
+-rw-rw-rw-   0        0        0       53 2023-08-02 08:36:56.000000 FedxD-0.4/FedxD/__init__.py
+-rw-rw-rw-   0        0        0     2226 2023-08-01 22:34:49.000000 FedxD-0.4/FedxD/color.py
+-rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.4/FedxD/converters.py
+drwxrwxrwx   0        0        0        0 2023-08-02 08:39:11.913843 FedxD-0.4/FedxD.egg-info/
+-rw-rw-rw-   0        0        0     1612 2023-08-02 08:39:11.000000 FedxD-0.4/FedxD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-02 08:39:11.000000 FedxD-0.4/FedxD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 08:39:11.000000 FedxD-0.4/FedxD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 08:39:11.000000 FedxD-0.4/FedxD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.4/License.txt
+-rw-rw-rw-   0        0        0     1612 2023-08-02 08:39:11.915834 FedxD-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-02 08:39:11.916834 FedxD-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-08-02 08:36:56.000000 FedxD-0.4/setup.py
```

### Comparing `FedxD-0.3/FedxD/color.py` & `FedxD-0.4/FedxD/color.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.3/FedxD/converters.py` & `FedxD-0.4/FedxD/converters.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.3/FedxD.egg-info/PKG-INFO` & `FedxD-0.4/FedxD.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.3
+Version: 0.4
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,13 +39,14 @@
    4. Lenght
    <br>(Converts Meter To Foot and vice versa,
    cm to inch and vice versa, and Meter and Foot To Yard)
     5. Temperature
    <br>(Converts Celcius to Farenhiet and vice versa ,
    and Celcius and Farenhiet To Kelvin and vice versa)
    
-Version = 0.1 (testing)
-Version = 0.2 (Fixing Bugs and testing)
-Version = 0.3 (Fixing Bugs)
+Version = 0.1 (testing) <br>
+Version = 0.2 (Fixing Bugs and testing)<br>
+Version = 0.3 (Fixing Bugs)<br>
+Version = 0.4 (Fixing Bugs And Making Ready)<br>
```

### Comparing `FedxD-0.3/License.txt` & `FedxD-0.4/License.txt`

 * *Files identical despite different names*

### Comparing `FedxD-0.3/PKG-INFO` & `FedxD-0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.3
+Version: 0.4
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -39,13 +39,14 @@
    4. Lenght
    <br>(Converts Meter To Foot and vice versa,
    cm to inch and vice versa, and Meter and Foot To Yard)
     5. Temperature
    <br>(Converts Celcius to Farenhiet and vice versa ,
    and Celcius and Farenhiet To Kelvin and vice versa)
    
-Version = 0.1 (testing)
-Version = 0.2 (Fixing Bugs and testing)
-Version = 0.3 (Fixing Bugs)
+Version = 0.1 (testing) <br>
+Version = 0.2 (Fixing Bugs and testing)<br>
+Version = 0.3 (Fixing Bugs)<br>
+Version = 0.4 (Fixing Bugs And Making Ready)<br>
```

### Comparing `FedxD-0.3/setup.py` & `FedxD-0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import twine
 from setuptools import setup , find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(name='FedxD',
-    version='0.3',
+    version='0.4',
     packages=['FedxD'],
     author='FedxD',
     author_email='abbaskazim135@gmail.com',
     description='This Package is for Quality of life stuff that you will need in your project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/FedxD',
```

