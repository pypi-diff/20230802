# Comparing `tmp/microjoy-0.0.2.tar.gz` & `tmp/microjoy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microjoy-0.0.2.tar", last modified: Tue Aug  1 22:47:51 2023, max compression
+gzip compressed data, was "microjoy-0.0.3.tar", last modified: Tue Aug  1 22:49:14 2023, max compression
```

## Comparing `microjoy-0.0.2.tar` & `microjoy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 22:47:51.124426 microjoy-0.0.2/
--rw-rw-rw-   0        0        0     1078 2023-08-01 22:27:35.000000 microjoy-0.0.2/LICENCE
--rw-rw-rw-   0        0        0      693 2023-08-01 22:47:51.123920 microjoy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-08-01 22:44:31.000000 microjoy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 22:47:51.094574 microjoy-0.0.2/j/
--rw-rw-rw-   0        0        0        0 2023-08-01 22:47:26.000000 microjoy-0.0.2/j/__init__.py
--rw-rw-rw-   0        0        0      728 2023-08-01 22:41:23.000000 microjoy-0.0.2/j/joy.py
-drwxrwxrwx   0        0        0        0 2023-08-01 22:47:51.122857 microjoy-0.0.2/microjoy.egg-info/
--rw-rw-rw-   0        0        0      693 2023-08-01 22:47:51.000000 microjoy-0.0.2/microjoy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-08-01 22:47:51.000000 microjoy-0.0.2/microjoy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 22:47:51.000000 microjoy-0.0.2/microjoy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-01 22:47:51.000000 microjoy-0.0.2/microjoy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 22:47:51.124426 microjoy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      477 2023-08-01 22:47:46.000000 microjoy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:49:14.460434 microjoy-0.0.3/
+-rw-rw-rw-   0        0        0     1078 2023-08-01 22:27:35.000000 microjoy-0.0.3/LICENCE
+-rw-rw-rw-   0        0        0      693 2023-08-01 22:49:14.428589 microjoy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      330 2023-08-01 22:44:31.000000 microjoy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-01 22:49:14.390201 microjoy-0.0.3/j/
+-rw-rw-rw-   0        0        0        0 2023-08-01 22:47:26.000000 microjoy-0.0.3/j/__init__.py
+-rw-rw-rw-   0        0        0      679 2023-08-01 22:48:59.000000 microjoy-0.0.3/j/joy.py
+drwxrwxrwx   0        0        0        0 2023-08-01 22:49:14.424085 microjoy-0.0.3/microjoy.egg-info/
+-rw-rw-rw-   0        0        0      693 2023-08-01 22:49:14.000000 microjoy-0.0.3/microjoy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-08-01 22:49:14.000000 microjoy-0.0.3/microjoy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 22:49:14.000000 microjoy-0.0.3/microjoy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-01 22:49:14.000000 microjoy-0.0.3/microjoy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 22:49:14.460434 microjoy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      477 2023-08-01 22:48:59.000000 microjoy-0.0.3/setup.py
```

### Comparing `microjoy-0.0.2/LICENCE` & `microjoy-0.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `microjoy-0.0.2/PKG-INFO` & `microjoy-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microjoy
-Version: 0.0.2
+Version: 0.0.3
 Summary: biblioteca para leitura de joystick com micropython
 Home-page: UNKNOWN
 Author: Issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: joystick micropython
 Platform: UNKNOWN
```

### Comparing `microjoy-0.0.2/microjoy.egg-info/PKG-INFO` & `microjoy-0.0.3/microjoy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microjoy
-Version: 0.0.2
+Version: 0.0.3
 Summary: biblioteca para leitura de joystick com micropython
 Home-page: UNKNOWN
 Author: Issei momonge
 Author-email: mggyggf@gmail.com
 License: MIT License
 Keywords: joystick micropython
 Platform: UNKNOWN
```

