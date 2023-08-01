# Comparing `tmp/PythonPackageUpdateChecker-1.0.7.tar.gz` & `tmp/PythonPackageUpdateChecker-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonPackageUpdateChecker-1.0.7.tar", last modified: Tue Aug  1 23:21:06 2023, max compression
+gzip compressed data, was "PythonPackageUpdateChecker-1.0.8.tar", last modified: Tue Aug  1 23:40:51 2023, max compression
```

## Comparing `PythonPackageUpdateChecker-1.0.7.tar` & `PythonPackageUpdateChecker-1.0.8.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 23:21:06.097837 PythonPackageUpdateChecker-1.0.7/
--rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.7/LICENSE.txt
--rw-rw-rw-   0        0        0     2450 2023-08-01 23:21:06.096839 PythonPackageUpdateChecker-1.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 23:21:06.095842 PythonPackageUpdateChecker-1.0.7/PythonPackageUpdateChecker.egg-info/
--rw-rw-rw-   0        0        0     2450 2023-08-01 23:21:06.000000 PythonPackageUpdateChecker-1.0.7/PythonPackageUpdateChecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-08-01 23:21:06.000000 PythonPackageUpdateChecker-1.0.7/PythonPackageUpdateChecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 23:21:06.000000 PythonPackageUpdateChecker-1.0.7/PythonPackageUpdateChecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       79 2023-08-01 23:21:06.000000 PythonPackageUpdateChecker-1.0.7/PythonPackageUpdateChecker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-08-01 23:21:06.000000 PythonPackageUpdateChecker-1.0.7/PythonPackageUpdateChecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 23:21:06.000000 PythonPackageUpdateChecker-1.0.7/PythonPackageUpdateChecker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.7/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 23:21:06.097837 PythonPackageUpdateChecker-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1794 2023-08-01 23:20:17.000000 PythonPackageUpdateChecker-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:40:51.569387 PythonPackageUpdateChecker-1.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     2450 2023-08-01 23:40:51.568390 PythonPackageUpdateChecker-1.0.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 23:40:51.544454 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker/
+-rw-rw-rw-   0        0        0     5976 2023-08-01 23:14:58.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker/PythonPackageUpdateChecker.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 23:27:21.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker/__init__.py
+-rw-rw-rw-   0        0        0       70 2023-08-01 22:59:09.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:40:51.567421 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker.egg-info/
+-rw-rw-rw-   0        0        0     2450 2023-08-01 23:40:51.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2023-08-01 23:40:51.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 23:40:51.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-08-01 23:40:51.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-08-01 23:40:51.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-08-01 23:40:51.000000 PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.8/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 23:40:51.569387 PythonPackageUpdateChecker-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1794 2023-08-01 23:35:12.000000 PythonPackageUpdateChecker-1.0.8/setup.py
```

### Comparing `PythonPackageUpdateChecker-1.0.7/LICENSE.txt` & `PythonPackageUpdateChecker-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.7/PKG-INFO` & `PythonPackageUpdateChecker-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.7
+Version: 1.0.8
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
```

### Comparing `PythonPackageUpdateChecker-1.0.7/PythonPackageUpdateChecker.egg-info/PKG-INFO` & `PythonPackageUpdateChecker-1.0.8/PythonPackageUpdateChecker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.7
+Version: 1.0.8
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
```

### Comparing `PythonPackageUpdateChecker-1.0.7/README.md` & `PythonPackageUpdateChecker-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.7/setup.py` & `PythonPackageUpdateChecker-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Зчитуємо вміст файлу README.md
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PythonPackageUpdateChecker',
-    version='1.0.7',
+    version='1.0.8',
     description='A utility to automatically check for updates of installed Python packages and update them to the latest versions.',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Вказуємо тип контенту для README.md
     author='Andrii Bohachev',
     author_email='andriybogachev@gmail.com',
     packages=find_packages(),
     install_requires=[
```

