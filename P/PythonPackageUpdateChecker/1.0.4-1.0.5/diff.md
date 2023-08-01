# Comparing `tmp/PythonPackageUpdateChecker-1.0.4.tar.gz` & `tmp/PythonPackageUpdateChecker-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonPackageUpdateChecker-1.0.4.tar", last modified: Mon Jul 31 21:49:36 2023, max compression
+gzip compressed data, was "PythonPackageUpdateChecker-1.0.5.tar", last modified: Tue Aug  1 22:50:00 2023, max compression
```

## Comparing `PythonPackageUpdateChecker-1.0.4.tar` & `PythonPackageUpdateChecker-1.0.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-31 21:49:36.013357 PythonPackageUpdateChecker-1.0.4/
--rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     2450 2023-07-31 21:49:36.013357 PythonPackageUpdateChecker-1.0.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-31 21:49:36.012360 PythonPackageUpdateChecker-1.0.4/PythonPackageUpdateChecker.egg-info/
--rw-rw-rw-   0        0        0     2450 2023-07-31 21:49:35.000000 PythonPackageUpdateChecker-1.0.4/PythonPackageUpdateChecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-31 21:49:35.000000 PythonPackageUpdateChecker-1.0.4/PythonPackageUpdateChecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 21:49:35.000000 PythonPackageUpdateChecker-1.0.4/PythonPackageUpdateChecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-07-31 21:49:35.000000 PythonPackageUpdateChecker-1.0.4/PythonPackageUpdateChecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-07-31 21:49:35.000000 PythonPackageUpdateChecker-1.0.4/PythonPackageUpdateChecker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-07-31 21:49:36.014354 PythonPackageUpdateChecker-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-07-31 21:48:33.000000 PythonPackageUpdateChecker-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:50:00.905726 PythonPackageUpdateChecker-1.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     2450 2023-08-01 22:50:00.904728 PythonPackageUpdateChecker-1.0.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 22:50:00.903730 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/
+-rw-rw-rw-   0        0        0     2450 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 22:50:00.905726 PythonPackageUpdateChecker-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1649 2023-08-01 22:49:26.000000 PythonPackageUpdateChecker-1.0.5/setup.py
```

### Comparing `PythonPackageUpdateChecker-1.0.4/LICENSE.txt` & `PythonPackageUpdateChecker-1.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.4/PKG-INFO` & `PythonPackageUpdateChecker-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.4
+Version: 1.0.5
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
```

### Comparing `PythonPackageUpdateChecker-1.0.4/PythonPackageUpdateChecker.egg-info/PKG-INFO` & `PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.4
+Version: 1.0.5
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
```

### Comparing `PythonPackageUpdateChecker-1.0.4/README.md` & `PythonPackageUpdateChecker-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.4/setup.py` & `PythonPackageUpdateChecker-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Зчитуємо вміст файлу README.md
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PythonPackageUpdateChecker',
-    version='1.0.4',
+    version='1.0.5',
     description='A utility to automatically check for updates of installed Python packages and update them to the latest versions.',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Вказуємо тип контенту для README.md
     author='Andrii Bohachev',
     author_email='andriybogachev@gmail.com',
     packages=find_packages(),
     install_requires=[
```

