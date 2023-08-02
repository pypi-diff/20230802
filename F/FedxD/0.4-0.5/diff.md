# Comparing `tmp/FedxD-0.4.tar.gz` & `tmp/FedxD-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FedxD-0.4.tar", last modified: Wed Aug  2 08:39:11 2023, max compression
+gzip compressed data, was "FedxD-0.5.tar", last modified: Wed Aug  2 15:36:12 2023, max compression
```

## Comparing `FedxD-0.4.tar` & `FedxD-0.5.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 08:39:11.916834 FedxD-0.4/
-drwxrwxrwx   0        0        0        0 2023-08-02 08:39:11.901795 FedxD-0.4/FedxD/
--rw-rw-rw-   0        0        0       53 2023-08-02 08:36:56.000000 FedxD-0.4/FedxD/__init__.py
--rw-rw-rw-   0        0        0     2226 2023-08-01 22:34:49.000000 FedxD-0.4/FedxD/color.py
--rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.4/FedxD/converters.py
-drwxrwxrwx   0        0        0        0 2023-08-02 08:39:11.913843 FedxD-0.4/FedxD.egg-info/
--rw-rw-rw-   0        0        0     1612 2023-08-02 08:39:11.000000 FedxD-0.4/FedxD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      189 2023-08-02 08:39:11.000000 FedxD-0.4/FedxD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 08:39:11.000000 FedxD-0.4/FedxD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-08-02 08:39:11.000000 FedxD-0.4/FedxD.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.4/License.txt
--rw-rw-rw-   0        0        0     1612 2023-08-02 08:39:11.915834 FedxD-0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-02 08:39:11.916834 FedxD-0.4/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-08-02 08:36:56.000000 FedxD-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:36:12.976470 FedxD-0.5/
+drwxrwxrwx   0        0        0        0 2023-08-02 15:36:12.942490 FedxD-0.5/FedxD/
+-rw-rw-rw-   0        0        0    40746 2023-08-02 15:26:35.000000 FedxD-0.5/FedxD/Lists.py
+-rw-rw-rw-   0        0        0       79 2023-08-02 14:51:40.000000 FedxD-0.5/FedxD/__init__.py
+-rw-rw-rw-   0        0        0     2250 2023-08-02 15:26:35.000000 FedxD-0.5/FedxD/color.py
+-rw-rw-rw-   0        0        0     2234 2023-08-01 22:29:02.000000 FedxD-0.5/FedxD/converters.py
+-rw-rw-rw-   0        0        0      542 2023-08-02 15:26:35.000000 FedxD-0.5/FedxD/random.py
+drwxrwxrwx   0        0        0        0 2023-08-02 15:36:12.973472 FedxD-0.5/FedxD.egg-info/
+-rw-rw-rw-   0        0        0     1993 2023-08-02 15:36:12.000000 FedxD-0.5/FedxD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-08-02 15:36:12.000000 FedxD-0.5/FedxD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 15:36:12.000000 FedxD-0.5/FedxD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-08-02 15:36:12.000000 FedxD-0.5/FedxD.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1123 2023-08-01 21:42:15.000000 FedxD-0.5/License.txt
+-rw-rw-rw-   0        0        0     1993 2023-08-02 15:36:12.975470 FedxD-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-02 15:36:12.976470 FedxD-0.5/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-08-02 15:26:35.000000 FedxD-0.5/setup.py
```

### Comparing `FedxD-0.4/FedxD/color.py` & `FedxD-0.5/FedxD/color.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,15 +30,17 @@
         'salmon': (250, 128, 114),
         'tan': (210, 180, 140),
         'aquamarine': (127, 255, 212)
     }
     if color.lower() in color_dict:
         return color_dict[color]
     else:
-        return (0,0,0)
+        raise ValueError('Invalid color')
+
+
 def hexcolor(color):
     color_to_hex = {
         'black': '#000000',
         'white': '#FFFFFF',
         'red': '#FF0000',
         'green': '#00FF00',
         'blue': '#0000FF',
@@ -67,9 +69,8 @@
         'salmon': '#FA8072',
         'tan': '#D2B48C',
         'aquamarine': '#7FFFD4'
     }
     if color.lower() in color_to_hex:
         return color_to_hex[color]
     else:
-        return (color_to_hex['black'])
-
+        raise ValueError('Invalid color')
```

### Comparing `FedxD-0.4/FedxD/converters.py` & `FedxD-0.5/FedxD/converters.py`

 * *Files identical despite different names*

### Comparing `FedxD-0.4/FedxD.egg-info/PKG-INFO` & `FedxD-0.5/FedxD.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.4
+Version: 0.5
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,29 @@
    <br>(Converts KG to Pound and Vice Versa)
    4. Lenght
    <br>(Converts Meter To Foot and vice versa,
    cm to inch and vice versa, and Meter and Foot To Yard)
     5. Temperature
    <br>(Converts Celcius to Farenhiet and vice versa ,
    and Celcius and Farenhiet To Kelvin and vice versa)
+3. random
+   1. date(year)
+      <br>(Generates a Random Date Within The Given Year)
+   2. color
+    <br>(Generates a Random Color)
+   3. name
+    <br>(Generates a Random Name)
+   4. age
+    <br>(Generates a Random Age)
+   5. fact
+   <br>(Generates a Random Fact)
+   6. true_false
+   <br>(Gives Either True Or False in Boolean)
    
 Version = 0.1 (testing) <br>
 Version = 0.2 (Fixing Bugs and testing)<br>
 Version = 0.3 (Fixing Bugs)<br>
 Version = 0.4 (Fixing Bugs And Making Ready)<br>
+Version = 0.5 (New Module(random))<br>
```

### Comparing `FedxD-0.4/License.txt` & `FedxD-0.5/License.txt`

 * *Files identical despite different names*

### Comparing `FedxD-0.4/PKG-INFO` & `FedxD-0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedxD
-Version: 0.4
+Version: 0.5
 Summary: This Package is for Quality of life stuff that you will need in your project
 Home-page: https://github.com/FedxD
 Author: FedxD
 Author-email: abbaskazim135@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -38,15 +38,29 @@
    <br>(Converts KG to Pound and Vice Versa)
    4. Lenght
    <br>(Converts Meter To Foot and vice versa,
    cm to inch and vice versa, and Meter and Foot To Yard)
     5. Temperature
    <br>(Converts Celcius to Farenhiet and vice versa ,
    and Celcius and Farenhiet To Kelvin and vice versa)
+3. random
+   1. date(year)
+      <br>(Generates a Random Date Within The Given Year)
+   2. color
+    <br>(Generates a Random Color)
+   3. name
+    <br>(Generates a Random Name)
+   4. age
+    <br>(Generates a Random Age)
+   5. fact
+   <br>(Generates a Random Fact)
+   6. true_false
+   <br>(Gives Either True Or False in Boolean)
    
 Version = 0.1 (testing) <br>
 Version = 0.2 (Fixing Bugs and testing)<br>
 Version = 0.3 (Fixing Bugs)<br>
 Version = 0.4 (Fixing Bugs And Making Ready)<br>
+Version = 0.5 (New Module(random))<br>
```

### Comparing `FedxD-0.4/setup.py` & `FedxD-0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import twine
 from setuptools import setup , find_packages
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(name='FedxD',
-    version='0.4',
+    version='0.5',
     packages=['FedxD'],
     author='FedxD',
     author_email='abbaskazim135@gmail.com',
     description='This Package is for Quality of life stuff that you will need in your project',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/FedxD',
```

