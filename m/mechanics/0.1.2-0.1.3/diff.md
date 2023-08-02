# Comparing `tmp/mechanics-0.1.2.tar.gz` & `tmp/mechanics-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mechanics-0.1.2.tar", last modified: Tue Aug  1 17:56:01 2023, max compression
+gzip compressed data, was "mechanics-0.1.3.tar", last modified: Wed Aug  2 08:43:27 2023, max compression
```

## Comparing `mechanics-0.1.2.tar` & `mechanics-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-01 17:56:01.425500 mechanics-0.1.2/
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1762 2023-08-01 17:56:01.417334 mechanics-0.1.2/PKG-INFO
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1502 2023-08-01 17:21:26.000000 mechanics-0.1.2/README.md
-drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-01 17:56:01.348306 mechanics-0.1.2/mechanics.egg-info/
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1762 2023-08-01 17:56:00.000000 mechanics-0.1.2/mechanics.egg-info/PKG-INFO
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)      163 2023-08-01 17:56:00.000000 mechanics-0.1.2/mechanics.egg-info/SOURCES.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)        1 2023-08-01 17:56:00.000000 mechanics-0.1.2/mechanics.egg-info/dependency_links.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)       10 2023-08-01 17:56:00.000000 mechanics-0.1.2/mechanics.egg-info/top_level.txt
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1079 2023-08-01 17:15:31.000000 mechanics-0.1.2/mechanics.py
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)       38 2023-08-01 17:56:01.428195 mechanics-0.1.2/setup.cfg
--rwxrwxrwx   0 alextras  (1000) alextras  (1000)      446 2023-08-01 17:55:53.000000 mechanics-0.1.2/setup.py
+drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-02 08:43:27.360815 mechanics-0.1.3/
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1762 2023-08-02 08:43:27.336483 mechanics-0.1.3/PKG-INFO
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1502 2023-08-01 17:21:26.000000 mechanics-0.1.3/README.md
+drwxrwxrwx   0 alextras  (1000) alextras  (1000)        0 2023-08-02 08:43:27.256654 mechanics-0.1.3/mechanics.egg-info/
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1762 2023-08-02 08:43:26.000000 mechanics-0.1.3/mechanics.egg-info/PKG-INFO
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)      163 2023-08-02 08:43:26.000000 mechanics-0.1.3/mechanics.egg-info/SOURCES.txt
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)        1 2023-08-02 08:43:26.000000 mechanics-0.1.3/mechanics.egg-info/dependency_links.txt
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)       10 2023-08-02 08:43:26.000000 mechanics-0.1.3/mechanics.egg-info/top_level.txt
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)     1991 2023-08-02 08:41:51.000000 mechanics-0.1.3/mechanics.py
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)       38 2023-08-02 08:43:27.365572 mechanics-0.1.3/setup.cfg
+-rwxrwxrwx   0 alextras  (1000) alextras  (1000)      453 2023-08-02 08:43:13.000000 mechanics-0.1.3/setup.py
```

### Comparing `mechanics-0.1.2/PKG-INFO` & `mechanics-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanics
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for solving simple mechanics problems
 Home-page: UNKNOWN
 Author: alextras
 Author-email: alextrasias@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `mechanics-0.1.2/README.md` & `mechanics-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mechanics-0.1.2/mechanics.egg-info/PKG-INFO` & `mechanics-0.1.3/mechanics.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mechanics
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library for solving simple mechanics problems
 Home-page: UNKNOWN
 Author: alextras
 Author-email: alextrasias@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

