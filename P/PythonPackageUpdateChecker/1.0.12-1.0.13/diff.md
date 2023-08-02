# Comparing `tmp/PythonPackageUpdateChecker-1.0.12.tar.gz` & `tmp/PythonPackageUpdateChecker-1.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonPackageUpdateChecker-1.0.12.tar", last modified: Wed Aug  2 17:14:50 2023, max compression
+gzip compressed data, was "PythonPackageUpdateChecker-1.0.13.tar", last modified: Wed Aug  2 17:59:13 2023, max compression
```

## Comparing `PythonPackageUpdateChecker-1.0.12.tar` & `PythonPackageUpdateChecker-1.0.13.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:14:50.563303 PythonPackageUpdateChecker-1.0.12/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 17:14:29.000000 PythonPackageUpdateChecker-1.0.12/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 17:14:50.563303 PythonPackageUpdateChecker-1.0.12/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:14:50.563303 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:14:50.000000 PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-08-02 17:14:29.000000 PythonPackageUpdateChecker-1.0.12/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:14:50.563303 PythonPackageUpdateChecker-1.0.12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-02 17:14:29.000000 PythonPackageUpdateChecker-1.0.12/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:59:13.653543 PythonPackageUpdateChecker-1.0.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-02 17:59:04.000000 PythonPackageUpdateChecker-1.0.13/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-02 17:59:13.653543 PythonPackageUpdateChecker-1.0.13/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 17:59:13.653543 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2622 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 17:59:13.000000 PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-08-02 17:59:04.000000 PythonPackageUpdateChecker-1.0.13/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 17:59:13.653543 PythonPackageUpdateChecker-1.0.13/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-08-02 17:59:04.000000 PythonPackageUpdateChecker-1.0.13/setup.py
```

### Comparing `PythonPackageUpdateChecker-1.0.12/LICENSE.txt` & `PythonPackageUpdateChecker-1.0.13/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.12/PKG-INFO` & `PythonPackageUpdateChecker-1.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.12
+Version: 1.0.13
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
@@ -73,7 +73,9 @@
 <<<<<<< HEAD
 - https://www.linkedin.com/in/andriibohachev/
 =======
 - https://www.linkedin.com/in/andriibohachev/
 >>>>>>> 94b7e7e9cd40abf4a8244ba90cfba4359424c9cb
 "# PythonPackageUpdateChecker" 
 "# PythonPackageUpdateChecker" 
+"# PythonPackageUpdateChecker" 
+"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.12/PythonPackageUpdateChecker.egg-info/PKG-INFO` & `PythonPackageUpdateChecker-1.0.13/PythonPackageUpdateChecker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.12
+Version: 1.0.13
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
@@ -73,7 +73,9 @@
 <<<<<<< HEAD
 - https://www.linkedin.com/in/andriibohachev/
 =======
 - https://www.linkedin.com/in/andriibohachev/
 >>>>>>> 94b7e7e9cd40abf4a8244ba90cfba4359424c9cb
 "# PythonPackageUpdateChecker" 
 "# PythonPackageUpdateChecker" 
+"# PythonPackageUpdateChecker" 
+"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.12/README.md` & `PythonPackageUpdateChecker-1.0.13/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -50,7 +50,9 @@
 <<<<<<< HEAD
 - https://www.linkedin.com/in/andriibohachev/
 =======
 - https://www.linkedin.com/in/andriibohachev/
 >>>>>>> 94b7e7e9cd40abf4a8244ba90cfba4359424c9cb
 "# PythonPackageUpdateChecker" 
 "# PythonPackageUpdateChecker" 
+"# PythonPackageUpdateChecker" 
+"# PythonPackageUpdateChecker"
```

### Comparing `PythonPackageUpdateChecker-1.0.12/setup.py` & `PythonPackageUpdateChecker-1.0.13/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Зчитуємо вміст файлу README.md
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="PythonPackageUpdateChecker",
-    version="1.0.12",
+    version="1.0.13",
     description="A utility to automatically check for updates of installed Python packages and update them to the latest versions.",
     long_description=long_description,
     # Вказуємо тип контенту для README.md
     long_description_content_type="text/markdown",
     author="Andrii Bohachev",
     author_email="andriybogachev@gmail.com",
     packages=find_packages(),
```

