# Comparing `tmp/hapm-0.0.5.tar.gz` & `tmp/hapm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hapm-0.0.5.tar", last modified: Mon Jul 31 08:59:17 2023, max compression
+gzip compressed data, was "hapm-0.1.0.tar", last modified: Wed Aug  2 15:27:54 2023, max compression
```

## Comparing `hapm-0.0.5.tar` & `hapm-0.1.0.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.349519 hapm-0.0.5/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1394 2023-07-31 08:59:17.349363 hapm-0.0.5/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1034 2023-02-20 21:55:23.000000 hapm-0.0.5/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.348722 hapm-0.0.5/hapm.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1394 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      918 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)       79 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/requires.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        8 2023-07-31 08:59:17.000000 hapm-0.0.5/hapm.egg-info/top_level.txt
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.341959 hapm-0.0.5/libhapm/
--rw-r--r--   0 mishamyrt   (501) staff       (20)        0 2023-02-17 18:11:43.000000 hapm-0.0.5/libhapm/__init__.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.343880 hapm-0.0.5/libhapm/cli/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      184 2023-02-22 22:09:22.000000 hapm-0.0.5/libhapm/cli/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      390 2023-02-22 19:26:44.000000 hapm-0.0.5/libhapm/cli/ink.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1314 2023-02-25 20:31:31.000000 hapm-0.0.5/libhapm/cli/report_diff.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      871 2023-02-25 20:31:45.000000 hapm-0.0.5/libhapm/cli/report_list.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      443 2023-02-22 22:14:02.000000 hapm-0.0.5/libhapm/cli/report_no_token.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      930 2023-02-22 20:03:50.000000 hapm-0.0.5/libhapm/cli/report_summary.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      637 2023-02-25 10:20:29.000000 hapm-0.0.5/libhapm/cli/utils.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.344748 hapm-0.0.5/libhapm/github/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      147 2023-02-25 20:18:07.000000 hapm-0.0.5/libhapm/github/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      871 2023-02-25 20:12:15.000000 hapm-0.0.5/libhapm/github/file.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      325 2023-02-25 20:17:01.000000 hapm-0.0.5/libhapm/github/path.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      422 2023-02-25 20:18:42.000000 hapm-0.0.5/libhapm/github/tarball.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.345340 hapm-0.0.5/libhapm/integration/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       71 2023-02-25 10:15:54.000000 hapm-0.0.5/libhapm/integration/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2142 2023-02-26 16:02:42.000000 hapm-0.0.5/libhapm/integration/package.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.345972 hapm-0.0.5/libhapm/manager/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     5144 2023-02-26 16:07:00.000000 hapm-0.0.5/libhapm/manager/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      301 2023-02-22 12:53:26.000000 hapm-0.0.5/libhapm/manager/diff.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      985 2023-02-21 10:33:48.000000 hapm-0.0.5/libhapm/manager/lockfile.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.346825 hapm-0.0.5/libhapm/manifest/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       31 2023-02-20 20:36:51.000000 hapm-0.0.5/libhapm/manifest/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      692 2023-02-22 19:17:05.000000 hapm-0.0.5/libhapm/manifest/manifest.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1107 2023-02-25 11:28:23.000000 hapm-0.0.5/libhapm/manifest/parse.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.347436 hapm-0.0.5/libhapm/package/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      101 2023-02-25 20:13:51.000000 hapm-0.0.5/libhapm/package/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2342 2023-02-26 15:43:41.000000 hapm-0.0.5/libhapm/package/base.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      210 2023-02-25 10:18:53.000000 hapm-0.0.5/libhapm/package/description.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.347844 hapm-0.0.5/libhapm/plugin/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       34 2023-02-25 20:29:49.000000 hapm-0.0.5/libhapm/plugin/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2613 2023-02-26 16:07:40.000000 hapm-0.0.5/libhapm/plugin/package.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      961 2023-02-20 20:57:56.000000 hapm-0.0.5/libhapm/versions.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      397 2023-02-20 20:34:09.000000 hapm-0.0.5/pyproject.toml
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-07-31 08:59:17.349135 hapm-0.0.5/scripts/
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)     1954 2023-02-26 15:42:57.000000 hapm-0.0.5/scripts/hapm
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-07-31 08:59:17.349578 hapm-0.0.5/setup.cfg
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1062 2023-02-25 20:30:08.000000 hapm-0.0.5/setup.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.596918 hapm-0.1.0/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1378 2023-08-02 15:27:54.596788 hapm-0.1.0/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1018 2023-08-02 15:17:37.000000 hapm-0.1.0/README.md
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.596474 hapm-0.1.0/hapm.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1378 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      948 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      103 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/requires.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        8 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/top_level.txt
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.591749 hapm-0.1.0/libhapm/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        0 2023-02-17 18:11:43.000000 hapm-0.1.0/libhapm/__init__.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.593304 hapm-0.1.0/libhapm/cli/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      223 2023-08-02 15:03:05.000000 hapm-0.1.0/libhapm/cli/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      390 2023-02-22 19:26:44.000000 hapm-0.1.0/libhapm/cli/ink.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1314 2023-02-25 20:31:31.000000 hapm-0.1.0/libhapm/cli/report_diff.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      200 2023-08-02 13:05:34.000000 hapm-0.1.0/libhapm/cli/report_error.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      871 2023-02-25 20:31:45.000000 hapm-0.1.0/libhapm/cli/report_list.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      443 2023-02-22 22:14:02.000000 hapm-0.1.0/libhapm/cli/report_no_token.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      930 2023-02-22 20:03:50.000000 hapm-0.1.0/libhapm/cli/report_summary.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      637 2023-02-25 10:20:29.000000 hapm-0.1.0/libhapm/cli/utils.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.593957 hapm-0.1.0/libhapm/github/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      147 2023-02-25 20:18:07.000000 hapm-0.1.0/libhapm/github/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      871 2023-02-25 20:12:15.000000 hapm-0.1.0/libhapm/github/file.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      325 2023-02-25 20:17:01.000000 hapm-0.1.0/libhapm/github/path.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      422 2023-02-25 20:18:42.000000 hapm-0.1.0/libhapm/github/tarball.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.594243 hapm-0.1.0/libhapm/integration/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       71 2023-02-25 10:15:54.000000 hapm-0.1.0/libhapm/integration/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2142 2023-02-26 16:02:42.000000 hapm-0.1.0/libhapm/integration/package.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.594732 hapm-0.1.0/libhapm/manager/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     5085 2023-08-02 13:59:45.000000 hapm-0.1.0/libhapm/manager/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      301 2023-02-22 12:53:26.000000 hapm-0.1.0/libhapm/manager/diff.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      985 2023-02-21 10:33:48.000000 hapm-0.1.0/libhapm/manager/lockfile.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.595176 hapm-0.1.0/libhapm/manifest/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       31 2023-02-20 20:36:51.000000 hapm-0.1.0/libhapm/manifest/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      850 2023-08-02 13:04:20.000000 hapm-0.1.0/libhapm/manifest/manifest.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1107 2023-02-25 11:28:23.000000 hapm-0.1.0/libhapm/manifest/parse.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.595577 hapm-0.1.0/libhapm/package/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      101 2023-02-25 20:13:51.000000 hapm-0.1.0/libhapm/package/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2318 2023-08-02 14:20:33.000000 hapm-0.1.0/libhapm/package/base.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      210 2023-02-25 10:18:53.000000 hapm-0.1.0/libhapm/package/description.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.595841 hapm-0.1.0/libhapm/plugin/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       35 2023-08-02 13:59:58.000000 hapm-0.1.0/libhapm/plugin/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2942 2023-08-02 15:16:29.000000 hapm-0.1.0/libhapm/plugin/package.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      961 2023-02-20 20:57:56.000000 hapm-0.1.0/libhapm/versions.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      397 2023-02-20 20:34:09.000000 hapm-0.1.0/pyproject.toml
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.596597 hapm-0.1.0/scripts/
+-rwxr-xr-x   0 mishamyrt   (501) staff       (20)     1937 2023-08-02 14:16:54.000000 hapm-0.1.0/scripts/hapm
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-08-02 15:27:54.596966 hapm-0.1.0/setup.cfg
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1097 2023-08-02 12:19:44.000000 hapm-0.1.0/setup.py
```

### Comparing `hapm-0.0.5/PKG-INFO` & `hapm-0.1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapm
-Version: 0.0.5
+Version: 0.1.0
 Summary: The library for easily writing feature-rich Python scripts
 Home-page: UNKNOWN
 Author: Mikhael Khrustik
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,15 +43,15 @@
 ```sh
 hapm
 ```
 
 ## Export 
 
 ```sh
-hapm put -t integrations <path>
+hapm put <path>
 ```
 
 ## List 
 
 ```sh
 hapm list
 ```
```

### Comparing `hapm-0.0.5/README.md` & `hapm-0.1.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 ```sh
 hapm
 ```
 
 ## Export 
 
 ```sh
-hapm put -t integrations <path>
+hapm put <path>
 ```
 
 ## List 
 
 ```sh
 hapm list
 ```
```

### Comparing `hapm-0.0.5/hapm.egg-info/PKG-INFO` & `hapm-0.1.0/hapm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hapm
-Version: 0.0.5
+Version: 0.1.0
 Summary: The library for easily writing feature-rich Python scripts
 Home-page: UNKNOWN
 Author: Mikhael Khrustik
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -43,15 +43,15 @@
 ```sh
 hapm
 ```
 
 ## Export 
 
 ```sh
-hapm put -t integrations <path>
+hapm put <path>
 ```
 
 ## List 
 
 ```sh
 hapm list
 ```
```

### Comparing `hapm-0.0.5/hapm.egg-info/SOURCES.txt` & `hapm-0.1.0/hapm.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 setup.py
 ./libhapm/__init__.py
 ./libhapm/versions.py
 ./libhapm/cli/__init__.py
 ./libhapm/cli/ink.py
 ./libhapm/cli/report_diff.py
+./libhapm/cli/report_error.py
 ./libhapm/cli/report_list.py
 ./libhapm/cli/report_no_token.py
 ./libhapm/cli/report_summary.py
 ./libhapm/cli/utils.py
 ./libhapm/github/__init__.py
 ./libhapm/github/file.py
 ./libhapm/github/path.py
```

### Comparing `hapm-0.0.5/libhapm/cli/report_diff.py` & `hapm-0.1.0/libhapm/cli/report_diff.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/libhapm/cli/report_list.py` & `hapm-0.1.0/libhapm/cli/report_list.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/libhapm/cli/report_summary.py` & `hapm-0.1.0/libhapm/cli/report_summary.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/libhapm/cli/utils.py` & `hapm-0.1.0/libhapm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/libhapm/github/file.py` & `hapm-0.1.0/libhapm/github/file.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/libhapm/integration/package.py` & `hapm-0.1.0/libhapm/integration/package.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/libhapm/manager/__init__.py` & `hapm-0.1.0/libhapm/manager/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 from os.path import isdir, join
 from shutil import rmtree
 from typing import Dict, List
 
 from github import Github
 
 from libhapm.integration import IntegrationPackage
-from libhapm.plugin import PluginPackage
 from libhapm.package import BasePackage, PackageDescription
+from libhapm.plugin import PluginPackage
 from libhapm.versions import is_newer
 
 from .diff import PackageDiff
 from .lockfile import Lockfile
 
 PACKAGE_HANDLERS = {
     IntegrationPackage.kind: IntegrationPackage,
@@ -104,19 +104,17 @@
         """Deletes the package from the file system"""
         if isdir(path):
             rmtree(path)
         mkdir(path)
         kinds = []
         for (_, integration) in self._packages.items():
             if integration.kind not in kinds:
-                print(integration.kind, " is in ", kinds)
                 kinds.append(integration.kind)
                 PACKAGE_HANDLERS[integration.kind].pre_export(path)
             integration.export(path)
-
         for kind in kinds:
             PACKAGE_HANDLERS[kind].post_export(path)
 
     def updates(self) -> List[PackageDiff]:
         """Searches for updates for packages, returns list of available updates."""
         updates: List[PackageDiff] = []
         for (_, package) in self._packages.items():
```

### Comparing `hapm-0.0.5/libhapm/manager/lockfile.py` & `hapm-0.1.0/libhapm/manager/lockfile.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/libhapm/manifest/manifest.py` & `hapm-0.1.0/libhapm/manifest/manifest.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """HAPM manifest controller"""
 from typing import List
 
 from ruamel.yaml import safe_load
 
+from libhapm.cli import report_error
 from libhapm.package import PackageDescription
 
 from .parse import parse_category
 
 
 class Manifest:
     """HAPM manifest controller"""
@@ -18,9 +19,14 @@
         self.path = path
         self._encoding = encoding
 
     def load(self) -> List[PackageDescription]:
         """Reads the manifest file and parses its contents"""
         with open(self.path, "r", encoding="utf-8") as stream:
             raw = safe_load(stream)
-        for key in raw:
-            self.values.extend(parse_category(raw, key))
+        try:
+            for key in raw:
+                self.values.extend(parse_category(raw, key))
+        except TypeError as e:
+            report_error("parsing manifest", e)
+            exit(1)
+
```

### Comparing `hapm-0.0.5/libhapm/manifest/parse.py` & `hapm-0.1.0/libhapm/manifest/parse.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/libhapm/package/base.py` & `hapm-0.1.0/libhapm/package/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 """HAPM package"""
 from __future__ import annotations
 
 from os import remove
 from os.path import join
-from typing import List
 
 from libhapm.github import repo_name
 
 from .description import PackageDescription
 
 
 class BasePackage:
     """This is an abstract package controller class.
     The class that implements it must be able to control a certain type of package"""
 
-    # Must be overlapped by a child
+    # Must be overridden by a child
     kind: str
 
     # Package properties
     full_name: str
     version: str
     basepath: str
     extension: str
```

### Comparing `hapm-0.0.5/libhapm/plugin/package.py` & `hapm-0.1.0/libhapm/plugin/package.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """HAPM integration package module"""
 from __future__ import annotations
 
-from distutils.dir_util import copy_tree
-from os import listdir, remove, mkdir
-from os.path import isdir, join
-from shutil import rmtree, copyfile
+from os import listdir, remove
+from os.path import join
+from pathlib import Path
+from shutil import copyfile
 
 from git import Repo
 from github import Github
 
 from libhapm.github import get_release_file, get_tree_file
+from libhapm.cli.ink import ink, ANSI_YELLOW, ANSI_DIM
 from libhapm.package import BasePackage
-from libhapm.versions import find_latest_stable
 
-FOLDER_NAME = "plugins"
+FOLDER_NAME = "www/custom_lovelace"
+RESOURCES_REDIRECT_URL = "https://my.home-assistant.io/redirect/lovelace_resources/"
 
 
 class PluginPackage(BasePackage):
     """PluginPackage represent `.js` plugin packages"""
 
     repo: Repo
 
@@ -38,25 +39,30 @@
     def export(self, path: str) -> None:
         """Method should offload the package payload to the specified folder"""
         copyfile(self.path(), f"{join(path, FOLDER_NAME, self.name)}.js")
 
     @staticmethod
     def pre_export(path: str):
         """This method is called when you starting exporting packages of a certain kind"""
-        mkdir(join(path, FOLDER_NAME))
+        path_dir = Path(join(path, FOLDER_NAME))
+        path_dir.mkdir(exist_ok=True, parents=True)
 
     @staticmethod
     def post_export(path: str):
-        """This method is called after you finish exporting packages of a certain kind"""
+        """Do nothing"""
+        heading = (
+            "To connect JS plugins, they must be specified on the Lovelace resources.\n"
+            "Make sure those links are there:"
+        )
+        print(ink(heading, ANSI_YELLOW))
         plugins_dir = join(path, FOLDER_NAME)
+        prefix = ink("*", effects=ANSI_DIM)
         for plugin in listdir(plugins_dir):
-            plugin_path = join(plugins_dir, plugin)
-            print(plugin_path)
-
-        print(f"post_export plugins {path}")
+            print(f"{prefix} /local/custom_lovelace/{plugin}")
+        print(ink(f"Resources URL: {RESOURCES_REDIRECT_URL}", effects=ANSI_DIM))
 
     def _download_script(self, version: str):
         content = self._get_script(version)
         with open(self.path(version), "wb") as file:
             file.write(content)
 
     def _get_script(self, version: str) -> str | None:
```

### Comparing `hapm-0.0.5/libhapm/versions.py` & `hapm-0.1.0/libhapm/versions.py`

 * *Files identical despite different names*

### Comparing `hapm-0.0.5/scripts/hapm` & `hapm-0.1.0/scripts/hapm`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 #!/usr/bin/env python
 from argparse import BooleanOptionalAction
 from os import environ
 
-from arrrgs import arg, command, global_args, no_command, run
-from github import Github
+from arrrgs import arg, command, global_args, run
 
 from libhapm.cli import report_diff, report_list, report_no_token, report_summary
 from libhapm.manager import PackageManager
 from libhapm.manifest import Manifest
 
 TOKEN_VAR = 'GITHUB_PAT'
 if TOKEN_VAR not in environ:
@@ -23,16 +22,15 @@
     arg('--manifest', '-m', default=MANIFEST_PATH, help="Manifest path"),
     arg('--storage', '-s', default=STORAGE_DIR, help="Storage location"),
     arg('--dry', '-d',
         action=BooleanOptionalAction,
         help="Only write information. Do not make any changes to the files")
 )
 
-
-@no_command()
+@command(root=True)
 def sync(args, store: PackageManager):
     """Synchronizes local versions of components with the manifest."""
     manifest = Manifest(args.manifest)
     manifest.load()
     diff = store.diff(manifest.values)
     report_diff(diff)
     if args.dry is True:
@@ -45,22 +43,22 @@
     arg('path', default=None, help="Output path")
 )
 def put(args, store: PackageManager):
     """Synchronizes local versions of components with the manifest."""
     store.export(args.path)
 
 
-@command()
-def updates(_, store: PackageManager):
-    """Prints available packages updates."""
-    diff = store.updates()
-    if len(diff) == 0:
-        print("All packages is up to date")
-        return
-    report_diff(diff)
+# @command()
+# def updates(_, store: PackageManager):
+#     """Prints available packages updates."""
+#     diff = store.updates()
+#     if len(diff) == 0:
+#         print("All packages is up to date")
+#         return
+#     report_diff(diff)
 
 
 @command(name="list")
 def list_packages(_, store: PackageManager):
     """Print current version of components."""
     packages = store.descriptions()
     report_list(packages)
```

### Comparing `hapm-0.0.5/setup.py` & `hapm-0.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     scripts=['scripts/hapm'],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
     ],
     install_requires=[
         'ruamel.yaml==0.17.21',
-        'arrrgs==0.0.5',
+        'arrrgs==3.0.0',
+        'PyGithub==1.59.0',
         'gitpython==3.1.30',
-        'PyGithub==1.58.0',
-        'requests'
+        'requests==2.31.0',
+        'urllib3==1.26.6'
     ],
     python_requires='>=3.7',
     package_dir={'': '.'},
 )
```

