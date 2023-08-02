# Comparing `tmp/FedxD-0.5.tar.gz` & `tmp/FedxD-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FedxD-0.5.tar", last modified: Wed Aug  2 15:36:12 2023, max compression
+gzip compressed data, was "FedxD-0.6.tar", last modified: Wed Aug  2 15:48:06 2023, max compression
```

## Comparing `FedxD-0.5.tar` & `FedxD-0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 15:36:12.976470 FedxD-0.5/
-drwxrwxrwx   0        0        0        0 2023-08-02 15:36:12.942490 FedxD-0.5/FedxD/
--rw-rw-rw-   0        0        0    40746 2023-08-02 15:26:35.000000 FedxD-0.5/FedxD/Lists.py
--rw-rw-rw-   0        0        0       79 2023-08-02 14:51:40.000000 FedxD-0.5/FedxD/__init__.py
--rw-rw-rw-   0        0        0     2250 2023-08-02 15:26:35.000000 FedxD-0.5/FedxD/color.py
--rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.5/FedxD/converters.py
--rw-rw-rw-   0        0        0      542 2023-08-02 15:26:35.000000 FedxD-0.5/FedxD/random.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:36:12.973472 FedxD-0.5/FedxD.egg-info/
--rw-rw-rw-   0        0        0     1993 2023-08-02 15:36:12.000000 FedxD-0.5/FedxD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-08-02 15:36:12.000000 FedxD-0.5/FedxD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 15:36:12.000000 FedxD-0.5/FedxD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 15:36:12.000000 FedxD-0.5/FedxD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.5/License.txt
--rw-rw-rw-   0        0        0     1993 2023-08-02 15:36:12.975470 FedxD-0.5/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-02 15:36:12.976470 FedxD-0.5/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-08-02 15:26:35.000000 FedxD-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:06.052286 FedxD-0.6/
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:06.025302 FedxD-0.6/FedxD/
+-rw-rw-rw-   0        0        0    40746 2023-08-02 15:26:35.000000 FedxD-0.6/FedxD/Lists.py
+-rw-rw-rw-   0        0        0       79 2023-08-02 14:51:40.000000 FedxD-0.6/FedxD/__init__.py
+-rw-rw-rw-   0        0        0     2250 2023-08-02 15:26:35.000000 FedxD-0.6/FedxD/color.py
+-rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.6/FedxD/converters.py
+-rw-rw-rw-   0        0        0      565 2023-08-02 15:45:59.000000 FedxD-0.6/FedxD/random.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:48:06.045290 FedxD-0.6/FedxD.egg-info/
+-rw-rw-rw-   0        0        0     2025 2023-08-02 15:48:05.000000 FedxD-0.6/FedxD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-08-02 15:48:05.000000 FedxD-0.6/FedxD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 15:48:05.000000 FedxD-0.6/FedxD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 15:48:05.000000 FedxD-0.6/FedxD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.6/License.txt
+-rw-rw-rw-   0        0        0     2025 2023-08-02 15:48:06.048287 FedxD-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:48:06.052286 FedxD-0.6/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-08-02 15:47:52.000000 FedxD-0.6/setup.py
```

### Comparing `FedxD-0.5/FedxD/Lists.py` & `FedxD-0.6/FedxD/Lists.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.5/FedxD/color.py` & `FedxD-0.6/FedxD/color.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.5/FedxD/converters.py` & `FedxD-0.6/FedxD/converters.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.5/FedxD/random.py` & `FedxD-0.6/FedxD/random.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-from Lists import *
+from FedxD  import Lists
 import random
 
 
 def date(year):
     month = random.randint(1, 12)
     if month == 2:
         day = random.randint(1, 28)
     else:
         day = random.randint(1, 30)
         date = f"{day}/{month}/{year}"
         return date
 
 
 def color():
-    return random.choice(color_list())
+    return random.choice(Lists.color_list())
 
 
 def name():
-    return random.choice(name_list())
+    return random.choice(Lists.name_list())
 
 
 def age():
     return random.randint(1, 80)
 
 
 def fact():
-    return random.choice(fact_list())
+    return random.choice(Lists.fact_list())
 
 
 def true_false():
     return random.choice([True, False])
```

### Comparing `FedxD-0.5/FedxD.egg-info/PKG-INFO` & `FedxD-0.6/FedxD.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.5
+Version: 0.6
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -57,10 +57,11 @@
    <br>(Gives Either True Or False in Boolean)
    
 Version = 0.1 (testing) <br>
 Version = 0.2 (Fixing Bugs and testing)<br>
 Version = 0.3 (Fixing Bugs)<br>
 Version = 0.4 (Fixing Bugs And Making Ready)<br>
 Version = 0.5 (New Module(random))<br>
+Version = 0.6 (Bug Fixing)<br>
```

### Comparing `FedxD-0.5/License.txt` & `FedxD-0.6/License.txt`

 * *Files identical despite different names*

### Comparing `FedxD-0.5/PKG-INFO` & `FedxD-0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.5
+Version: 0.6
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -57,10 +57,11 @@
    <br>(Gives Either True Or False in Boolean)
    
 Version = 0.1 (testing) <br>
 Version = 0.2 (Fixing Bugs and testing)<br>
 Version = 0.3 (Fixing Bugs)<br>
 Version = 0.4 (Fixing Bugs And Making Ready)<br>
 Version = 0.5 (New Module(random))<br>
+Version = 0.6 (Bug Fixing)<br>
```

### Comparing `FedxD-0.5/setup.py` & `FedxD-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import twine
 from setuptools import setup , find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(name='FedxD',
-    version='0.5',
+    version='0.6',
     packages=['FedxD'],
     author='FedxD',
     author_email='abbaskazim135@gmail.com',
     description='This Package is for Quality of life stuff that you will need in your project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/FedxD',
```

