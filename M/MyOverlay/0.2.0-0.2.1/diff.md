# Comparing `tmp/MyOverlay-0.2.0.tar.gz` & `tmp/MyOverlay-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MyOverlay-0.2.0.tar", last modified: Tue Aug  1 11:57:01 2023, max compression
+gzip compressed data, was "MyOverlay-0.2.1.tar", last modified: Wed Aug  2 14:17:31 2023, max compression
```

## Comparing `MyOverlay-0.2.0.tar` & `MyOverlay-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 11:57:01.830424 MyOverlay-0.2.0/
--rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      745 2023-08-01 11:57:01.830424 MyOverlay-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.2.0/README.md
--rw-rw-rw-   0        0        0      649 2023-08-01 11:56:45.000000 MyOverlay-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-01 11:57:01.830424 MyOverlay-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-01 11:57:01.803129 MyOverlay-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-01 11:57:01.817129 MyOverlay-0.2.0/src/MyOverlay/
--rw-rw-rw-   0        0        0      324 2023-08-01 09:55:11.000000 MyOverlay-0.2.0/src/MyOverlay/Overlay.py
--rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.2.0/src/MyOverlay/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:57:01.829424 MyOverlay-0.2.0/src/MyOverlay/funcs/
--rw-rw-rw-   0        0        0     3633 2023-08-01 11:53:47.000000 MyOverlay-0.2.0/src/MyOverlay/funcs/myfunctions.py
-drwxrwxrwx   0        0        0        0 2023-08-01 11:57:01.828418 MyOverlay-0.2.0/src/MyOverlay.egg-info/
--rw-rw-rw-   0        0        0      745 2023-08-01 11:57:01.000000 MyOverlay-0.2.0/src/MyOverlay.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-08-01 11:57:01.000000 MyOverlay-0.2.0/src/MyOverlay.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 11:57:01.000000 MyOverlay-0.2.0/src/MyOverlay.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-08-01 11:57:01.000000 MyOverlay-0.2.0/src/MyOverlay.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.941042 MyOverlay-0.2.1/
+-rw-rw-rw-   0        0        0     1091 2023-08-01 09:37:41.000000 MyOverlay-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0      745 2023-08-02 14:17:31.941042 MyOverlay-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-08-01 09:37:33.000000 MyOverlay-0.2.1/README.md
+-rw-rw-rw-   0        0        0      649 2023-08-02 14:17:03.000000 MyOverlay-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-02 14:17:31.941042 MyOverlay-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.914093 MyOverlay-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.925042 MyOverlay-0.2.1/src/MyOverlay/
+-rw-rw-rw-   0        0        0      409 2023-08-02 14:16:50.000000 MyOverlay-0.2.1/src/MyOverlay/Overlay.py
+-rw-rw-rw-   0        0        0        0 2023-08-01 09:49:30.000000 MyOverlay-0.2.1/src/MyOverlay/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.940042 MyOverlay-0.2.1/src/MyOverlay/funcs/
+-rw-rw-rw-   0        0        0     4972 2023-08-02 14:15:51.000000 MyOverlay-0.2.1/src/MyOverlay/funcs/myfunctions.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:17:31.939043 MyOverlay-0.2.1/src/MyOverlay.egg-info/
+-rw-rw-rw-   0        0        0      745 2023-08-02 14:17:31.000000 MyOverlay-0.2.1/src/MyOverlay.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      266 2023-08-02 14:17:31.000000 MyOverlay-0.2.1/src/MyOverlay.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 14:17:31.000000 MyOverlay-0.2.1/src/MyOverlay.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-08-02 14:17:31.000000 MyOverlay-0.2.1/src/MyOverlay.egg-info/top_level.txt
```

### Comparing `MyOverlay-0.2.0/LICENSE` & `MyOverlay-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MyOverlay-0.2.0/PKG-INFO` & `MyOverlay-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.2.0
+Version: 0.2.1
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `MyOverlay-0.2.0/pyproject.toml` & `MyOverlay-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=61.0']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "MyOverlay"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="Erik Reimann", email="erikreimann28@gmail.com" },
 ]
 description = "Customized Text Only Screen Overlay"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `MyOverlay-0.2.0/src/MyOverlay.egg-info/PKG-INFO` & `MyOverlay-0.2.1/src/MyOverlay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MyOverlay
-Version: 0.2.0
+Version: 0.2.1
 Summary: Customized Text Only Screen Overlay
 Author-email: Erik Reimann <erikreimann28@gmail.com>
 Project-URL: Homepage, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay
 Project-URL: Bug Tracker, https://github.com/HerpesHabenderHauptmannHarry/MyOverlay/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

