# Comparing `tmp/fastmega-0.0.3.tar.gz` & `tmp/fastmega-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\fastmega-0.0.3.tar", last modified: Wed Aug  2 03:54:52 2023, max compression
+gzip compressed data, was "dist\fastmega-0.0.4.tar", last modified: Wed Aug  2 04:13:00 2023, max compression
```

## Comparing `fastmega-0.0.3.tar` & `fastmega-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 03:54:52.000000 fastmega-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-08-02 03:54:52.000000 fastmega-0.0.3/fastmega/
--rw-rw-rw-   0        0        0     1276 2023-08-02 03:22:43.000000 fastmega-0.0.3/fastmega/mymega.py
--rw-rw-rw-   0        0        0       26 2023-08-02 03:08:31.000000 fastmega-0.0.3/fastmega/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 03:54:52.000000 fastmega-0.0.3/fastmega.egg-info/
--rw-rw-rw-   0        0        0        1 2023-08-02 03:54:52.000000 fastmega-0.0.3/fastmega.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      940 2023-08-02 03:54:52.000000 fastmega-0.0.3/fastmega.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       19 2023-08-02 03:54:52.000000 fastmega-0.0.3/fastmega.egg-info/requires.txt
--rw-rw-rw-   0        0        0      235 2023-08-02 03:54:52.000000 fastmega-0.0.3/fastmega.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2023-08-02 03:54:52.000000 fastmega-0.0.3/fastmega.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1090 2023-08-02 02:21:29.000000 fastmega-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      940 2023-08-02 03:54:52.000000 fastmega-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-08-02 02:21:29.000000 fastmega-0.0.3/README.md
--rw-rw-rw-   0        0        0       86 2023-08-02 03:54:52.000000 fastmega-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1354 2023-08-02 03:47:44.000000 fastmega-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:13:00.000000 fastmega-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-08-02 04:13:00.000000 fastmega-0.0.4/fastmega/
+-rw-rw-rw-   0        0        0     1276 2023-08-02 03:22:43.000000 fastmega-0.0.4/fastmega/mymega.py
+-rw-rw-rw-   0        0        0       26 2023-08-02 03:08:31.000000 fastmega-0.0.4/fastmega/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:13:00.000000 fastmega-0.0.4/fastmega.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:13:00.000000 fastmega-0.0.4/fastmega.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      940 2023-08-02 04:13:00.000000 fastmega-0.0.4/fastmega.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-08-02 04:13:00.000000 fastmega-0.0.4/fastmega.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      235 2023-08-02 04:13:00.000000 fastmega-0.0.4/fastmega.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 04:13:00.000000 fastmega-0.0.4/fastmega.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1090 2023-08-02 02:21:29.000000 fastmega-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      940 2023-08-02 04:13:00.000000 fastmega-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-08-02 02:21:29.000000 fastmega-0.0.4/README.md
+-rw-rw-rw-   0        0        0       86 2023-08-02 04:13:00.000000 fastmega-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1357 2023-08-02 04:10:12.000000 fastmega-0.0.4/setup.py
```

### Comparing `fastmega-0.0.3/fastmega/mymega.py` & `fastmega-0.0.4/fastmega/mymega.py`

 * *Files identical despite different names*

### Comparing `fastmega-0.0.3/fastmega.egg-info/PKG-INFO` & `fastmega-0.0.4/fastmega.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastmega
-Version: 0.0.3
+Version: 0.0.4
 Summary: A fast way to use the MEGA cloud API
 Home-page: https://github.com/taindp98/fastmega
 Author: Rémi NGUYEN
 Author-email: taindp98@gmail.com
 License: MIT
-Download-URL: https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.3.tar.gz
+Download-URL: https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.4.tar.gz
 Keywords: mega,storage
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastmega-0.0.3/LICENSE` & `fastmega-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastmega-0.0.3/PKG-INFO` & `fastmega-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: fastmega
-Version: 0.0.3
+Version: 0.0.4
 Summary: A fast way to use the MEGA cloud API
 Home-page: https://github.com/taindp98/fastmega
 Author: Rémi NGUYEN
 Author-email: taindp98@gmail.com
 License: MIT
-Download-URL: https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.3.tar.gz
+Download-URL: https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.4.tar.gz
 Keywords: mega,storage
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `fastmega-0.0.3/setup.py` & `fastmega-0.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools,re,sys
 
 setuptools.setup(
     name = 'fastmega',         
     packages = ['fastmega'],
-    version = '0.0.3',     
+    version = '0.0.4',     
     license='MIT', 
     description = 'A fast way to use the MEGA cloud API', 
     author = 'Rémi NGUYEN',                   
     author_email = 'taindp98@gmail.com',      
     url = 'https://github.com/taindp98/fastmega',   
-    download_url = 'https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.3.tar.gz',   
+    download_url = 'https://github.com/taindp98/fastmega/archive/refs/tags/v.0.0.4.tar.gz',   
     keywords = ['mega', 'storage'],  
     install_requires=[
         'pip', 'packaging',
-        'mega'
+        'mega.py'
     ],
     classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
```

