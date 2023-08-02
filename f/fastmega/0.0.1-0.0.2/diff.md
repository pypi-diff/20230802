# Comparing `tmp/fastmega-0.0.1.tar.gz` & `tmp/fastmega-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastmega-0.0.1.tar", last modified: Wed Aug  2 03:11:14 2023, max compression
+gzip compressed data, was "fastmega-0.0.2.tar", last modified: Wed Aug  2 03:25:08 2023, max compression
```

## Comparing `fastmega-0.0.1.tar` & `fastmega-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 03:11:14.886420 fastmega-0.0.1/
--rw-rw-rw-   0        0        0     1090 2023-08-02 02:21:29.000000 fastmega-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      908 2023-08-02 03:11:14.886420 fastmega-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-08-02 02:21:29.000000 fastmega-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 03:11:14.811619 fastmega-0.0.1/fastmega/
--rw-rw-rw-   0        0        0       26 2023-08-02 03:08:31.000000 fastmega-0.0.1/fastmega/__init__.py
--rw-rw-rw-   0        0        0     1275 2023-08-02 03:05:57.000000 fastmega-0.0.1/fastmega/mymega.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:11:14.884425 fastmega-0.0.1/fastmega.egg-info/
--rw-rw-rw-   0        0        0      908 2023-08-02 03:11:14.000000 fastmega-0.0.1/fastmega.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-08-02 03:11:14.000000 fastmega-0.0.1/fastmega.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 03:11:14.000000 fastmega-0.0.1/fastmega.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-08-02 03:11:14.000000 fastmega-0.0.1/fastmega.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 03:11:14.000000 fastmega-0.0.1/fastmega.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-02 03:11:14.889410 fastmega-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1354 2023-08-02 02:29:11.000000 fastmega-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:25:08.871218 fastmega-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2023-08-02 02:21:29.000000 fastmega-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      908 2023-08-02 03:25:08.872214 fastmega-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-08-02 02:21:29.000000 fastmega-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 03:25:08.821353 fastmega-0.0.2/fastmega/
+-rw-rw-rw-   0        0        0       26 2023-08-02 03:08:31.000000 fastmega-0.0.2/fastmega/__init__.py
+-rw-rw-rw-   0        0        0     1276 2023-08-02 03:22:43.000000 fastmega-0.0.2/fastmega/mymega.py
+drwxrwxrwx   0        0        0        0 2023-08-02 03:25:08.869223 fastmega-0.0.2/fastmega.egg-info/
+-rw-rw-rw-   0        0        0      908 2023-08-02 03:25:08.000000 fastmega-0.0.2/fastmega.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-08-02 03:25:08.000000 fastmega-0.0.2/fastmega.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 03:25:08.000000 fastmega-0.0.2/fastmega.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 03:25:08.000000 fastmega-0.0.2/fastmega.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 03:25:08.000000 fastmega-0.0.2/fastmega.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-02 03:25:08.882192 fastmega-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1354 2023-08-02 03:25:03.000000 fastmega-0.0.2/setup.py
```

### Comparing `fastmega-0.0.1/LICENSE` & `fastmega-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmega-0.0.1/PKG-INFO` & `fastmega-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fastmega
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fast way to use the MEGA cloud API
 Home-page: https://github.com/taindp98/fastmega
-Download-URL: https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.1.tar.gz
+Download-URL: https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.2.tar.gz
 Author: Rémi NGUYEN
 Author-email: taindp98@gmail.com
 License: MIT
 Keywords: mega,storage
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fastmega-0.0.1/fastmega/mymega.py` & `fastmega-0.0.2/fastmega/mymega.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 """
 https://www.geeksforgeeks.org/how-to-use-mega-nz-api-with-python/
 https://github.com/odwyersoftware/mega.py/blob/master/src/mega/mega.py
 """
 
 class MyMega:
-    def __int__(self, username: str, password: str) -> None:
+    def __init__(self, username: str, password: str) -> None:
         self.username=username
         self.password=password
         self.mega = Mega()
         self.mega = self.mega.login(
             self.username,
             self.password
         )
```

### Comparing `fastmega-0.0.1/fastmega.egg-info/PKG-INFO` & `fastmega-0.0.2/fastmega.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: fastmega
-Version: 0.0.1
+Version: 0.0.2
 Summary: A fast way to use the MEGA cloud API
 Home-page: https://github.com/taindp98/fastmega
-Download-URL: https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.1.tar.gz
+Download-URL: https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.2.tar.gz
 Author: Rémi NGUYEN
 Author-email: taindp98@gmail.com
 License: MIT
 Keywords: mega,storage
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `fastmega-0.0.1/setup.py` & `fastmega-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import setuptools,re,sys
 
 setuptools.setup(
     name = 'fastmega',         
     packages = ['fastmega'],
-    version = '0.0.1',     
+    version = '0.0.2',     
     license='MIT', 
     description = 'A fast way to use the MEGA cloud API', 
     author = 'Rémi NGUYEN',                   
     author_email = 'taindp98@gmail.com',      
     url = 'https://github.com/taindp98/fastmega',   
-    download_url = 'https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.1.tar.gz',   
+    download_url = 'https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.2.tar.gz',   
     keywords = ['mega', 'storage'],  
     install_requires=[
         'pip', 'packaging',
         'mega'
     ],
     classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
```

