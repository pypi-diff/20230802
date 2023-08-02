# Comparing `tmp/PythonPackageUpdateChecker-1.0.10.tar.gz` & `tmp/PythonPackageUpdateChecker-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonPackageUpdateChecker-1.0.10.tar", last modified: Wed Aug  2 04:13:17 2023, max compression
+gzip compressed data, was "PythonPackageUpdateChecker-1.0.11.tar", last modified: Wed Aug  2 04:24:29 2023, max compression
```

## Comparing `PythonPackageUpdateChecker-1.0.10.tar` & `PythonPackageUpdateChecker-1.0.11.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 04:13:17.267514 PythonPackageUpdateChecker-1.0.10/
--rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.10/LICENSE.txt
--rw-rw-rw-   0        0        0     2451 2023-08-02 04:13:17.267514 PythonPackageUpdateChecker-1.0.10/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 04:13:17.266517 PythonPackageUpdateChecker-1.0.10/PythonPackageUpdateChecker.egg-info/
--rw-rw-rw-   0        0        0     2451 2023-08-02 04:13:17.000000 PythonPackageUpdateChecker-1.0.10/PythonPackageUpdateChecker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-08-02 04:13:17.000000 PythonPackageUpdateChecker-1.0.10/PythonPackageUpdateChecker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:13:17.000000 PythonPackageUpdateChecker-1.0.10/PythonPackageUpdateChecker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       83 2023-08-02 04:13:17.000000 PythonPackageUpdateChecker-1.0.10/PythonPackageUpdateChecker.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       32 2023-08-02 04:13:17.000000 PythonPackageUpdateChecker-1.0.10/PythonPackageUpdateChecker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 04:13:17.000000 PythonPackageUpdateChecker-1.0.10/PythonPackageUpdateChecker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.10/README.md
--rw-rw-rw-   0        0        0       42 2023-08-02 04:13:17.268513 PythonPackageUpdateChecker-1.0.10/setup.cfg
--rw-rw-rw-   0        0        0     1754 2023-08-02 04:12:48.000000 PythonPackageUpdateChecker-1.0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:29.969285 PythonPackageUpdateChecker-1.0.11/
+-rw-rw-rw-   0        0        0     1091 2023-07-31 14:52:03.000000 PythonPackageUpdateChecker-1.0.11/LICENSE.txt
+-rw-rw-rw-   0        0        0     2451 2023-08-02 04:24:29.969285 PythonPackageUpdateChecker-1.0.11/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:29.949845 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker/
+-rw-rw-rw-   0        0        0        0 2023-08-02 04:17:52.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker/__init__.py
+-rw-rw-rw-   0        0        0     5976 2023-08-02 04:19:38.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 04:24:29.968287 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/
+-rw-rw-rw-   0        0        0     2451 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       83 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       32 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2023-08-02 04:24:29.000000 PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1382 2023-07-31 14:52:04.000000 PythonPackageUpdateChecker-1.0.11/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-02 04:24:29.969285 PythonPackageUpdateChecker-1.0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1754 2023-08-02 04:24:04.000000 PythonPackageUpdateChecker-1.0.11/setup.py
```

### Comparing `PythonPackageUpdateChecker-1.0.10/LICENSE.txt` & `PythonPackageUpdateChecker-1.0.11/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.10/PKG-INFO` & `PythonPackageUpdateChecker-1.0.11/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.10
+Version: 1.0.11
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
```

### Comparing `PythonPackageUpdateChecker-1.0.10/PythonPackageUpdateChecker.egg-info/PKG-INFO` & `PythonPackageUpdateChecker-1.0.11/PythonPackageUpdateChecker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonPackageUpdateChecker
-Version: 1.0.10
+Version: 1.0.11
 Summary: A utility to automatically check for updates of installed Python packages and update them to the latest versions.
 Author: Andrii Bohachev
 Author-email: andriybogachev@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/andriybogachev/PythonPackageUpdateChecker
 Project-URL: Bug Reports, https://github.com/andriybogachev/PythonPackageUpdateChecker/issues
 Keywords: python package update checker utility async aiohttp
```

### Comparing `PythonPackageUpdateChecker-1.0.10/README.md` & `PythonPackageUpdateChecker-1.0.11/README.md`

 * *Files identical despite different names*

### Comparing `PythonPackageUpdateChecker-1.0.10/setup.py` & `PythonPackageUpdateChecker-1.0.11/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Зчитуємо вміст файлу README.md
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="PythonPackageUpdateChecker",
-    version="1.0.10",
+    version="1.0.11",
     description="A utility to automatically check for updates of installed Python packages and update them to the latest versions.",
     long_description=long_description,
     # Вказуємо тип контенту для README.md
     long_description_content_type="text/markdown",
     author="Andrii Bohachev",
     author_email="andriybogachev@gmail.com",
     packages=find_packages(),
```

