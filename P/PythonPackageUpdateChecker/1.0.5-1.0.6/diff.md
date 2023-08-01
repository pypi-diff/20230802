# Comparing `tmp/PythonPackageUpdateChecker-1.0.5.tar.gz` & `tmp/PythonPackageUpdateChecker-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonPackageUpdateChecker-1.0.5.tar", last modified: Tue Aug  1 22:50:00 2023, max compression
+gzip compressed data, was "PythonPackageUpdateChecker-1.0.6.tar", last modified: Tue Aug  1 23:10:24 2023, max compression
```

## Comparing `PythonPackageUpdateChecker-1.0.5.tar` & `PythonPackageUpdateChecker-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:50:00.905726 PythonPackageUpdateChecker-1.0.5/
--rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     2450 2023-08-01 22:50:00.904728 PythonPackageUpdateChecker-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-01 22:50:00.903730 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/
--rw-rw-rw-   0        0        0     2450 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:50:00.000000 PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-08-01 22:50:00.905726 PythonPackageUpdateChecker-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1649 2023-08-01 22:49:26.000000 PythonPackageUpdateChecker-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:10:24.256074 PythonPackageUpdateChecker-1.0.6/
+-rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     2450 2023-08-01 23:10:24.255077 PythonPackageUpdateChecker-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-01 23:10:24.254080 PythonPackageUpdateChecker-1.0.6/PythonPackageUpdateChecker.egg-info/
+-rw-rw-rw-   0        0        0     2450 2023-08-01 23:10:24.000000 PythonPackageUpdateChecker-1.0.6/PythonPackageUpdateChecker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-08-01 23:10:24.000000 PythonPackageUpdateChecker-1.0.6/PythonPackageUpdateChecker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 23:10:24.000000 PythonPackageUpdateChecker-1.0.6/PythonPackageUpdateChecker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-08-01 23:10:24.000000 PythonPackageUpdateChecker-1.0.6/PythonPackageUpdateChecker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-08-01 23:10:24.000000 PythonPackageUpdateChecker-1.0.6/PythonPackageUpdateChecker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 23:10:24.000000 PythonPackageUpdateChecker-1.0.6/PythonPackageUpdateChecker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-01 23:10:24.256074 PythonPackageUpdateChecker-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1799 2023-08-01 23:03:39.000000 PythonPackageUpdateChecker-1.0.6/setup.py
```

### Comparing `PythonPackageUpdateChecker-1.0.5/LICENSE.txt` & `PythonPackageUpdateChecker-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.5/PKG-INFO` & `PythonPackageUpdateChecker-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.5
+Version: 1.0.6
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
```

### Comparing `PythonPackageUpdateChecker-1.0.5/PythonPackageUpdateChecker.egg-info/PKG-INFO` & `PythonPackageUpdateChecker-1.0.6/PythonPackageUpdateChecker.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.5
+Version: 1.0.6
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
```

### Comparing `PythonPackageUpdateChecker-1.0.5/README.md` & `PythonPackageUpdateChecker-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.5/setup.py` & `PythonPackageUpdateChecker-1.0.6/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,27 +2,32 @@
 
 # Зчитуємо вміст файлу README.md
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='PythonPackageUpdateChecker',
-    version='1.0.5',
+    version='1.0.6',
     description='A utility to automatically check for updates of installed Python packages and update them to the latest versions.',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Вказуємо тип контенту для README.md
     author='Andrii Bohachev',
     author_email='andriybogachev@gmail.com',
     packages=find_packages(),
     install_requires=[
         'setuptools>=40.0.0',
         'aiohttp',
         'tqdm',
         'asyncio'
     ],
+    entry_points={
+        'console_scripts': [
+        'pythonpackageupdatechecker = PythonPackageUpdateChecker.__main__:main'
+        ]
+    },
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
```

