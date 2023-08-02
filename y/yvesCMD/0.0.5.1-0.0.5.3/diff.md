# Comparing `tmp/yvesCMD-0.0.5.1.tar.gz` & `tmp/yvesCMD-0.0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.5.1.tar", last modified: Wed Aug  2 15:30:38 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.5.3.tar", last modified: Wed Aug  2 16:23:50 2023, max compression
```

## Comparing `yvesCMD-0.0.5.1.tar` & `yvesCMD-0.0.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 15:30:38.643851 yvesCMD-0.0.5.1/
--rw-rw-rw-   0        0        0      205 2023-08-02 15:30:38.642853 yvesCMD-0.0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 15:30:38.580021 yvesCMD-0.0.5.1/YvesCMD/
--rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.5.1/YvesCMD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:30:38.588000 yvesCMD-0.0.5.1/YvesCMD/src/
--rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.5.1/YvesCMD/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:30:38.624901 yvesCMD-0.0.5.1/YvesCMD/src/extensions/
--rw-rw-rw-   0        0        0       37 2023-08-02 14:29:07.000000 yvesCMD-0.0.5.1/YvesCMD/src/extensions/__init__.py
--rw-rw-rw-   0        0        0     1351 2023-08-02 15:30:13.000000 yvesCMD-0.0.5.1/YvesCMD/src/extensions/select.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:30:38.638865 yvesCMD-0.0.5.1/YvesCMD/src/utils/
--rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.5.1/YvesCMD/src/utils/__init__.py
--rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.5.1/YvesCMD/src/utils/detector.py
--rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.5.1/YvesCMD/src/utils/hooks.py
--rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.5.1/YvesCMD/src/utils/register.py
--rw-rw-rw-   0        0        0     2518 2023-08-02 15:11:19.000000 yvesCMD-0.0.5.1/YvesCMD/src/yvescmd.py
--rw-rw-rw-   0        0        0       42 2023-08-02 15:30:38.643851 yvesCMD-0.0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      335 2023-08-02 15:30:30.000000 yvesCMD-0.0.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 15:30:38.613930 yvesCMD-0.0.5.1/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      205 2023-08-02 15:30:38.000000 yvesCMD-0.0.5.1/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-08-02 15:30:38.000000 yvesCMD-0.0.5.1/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 15:30:38.000000 yvesCMD-0.0.5.1/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 15:30:38.000000 yvesCMD-0.0.5.1/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.250730 yvesCMD-0.0.5.3/
+-rw-rw-rw-   0        0        0     1730 2023-08-02 16:23:50.246739 yvesCMD-0.0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1412 2023-08-02 16:18:12.000000 yvesCMD-0.0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.156981 yvesCMD-0.0.5.3/YvesCMD/
+-rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.5.3/YvesCMD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.166956 yvesCMD-0.0.5.3/YvesCMD/src/
+-rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.5.3/YvesCMD/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.222804 yvesCMD-0.0.5.3/YvesCMD/src/extensions/
+-rw-rw-rw-   0        0        0       37 2023-08-02 14:29:07.000000 yvesCMD-0.0.5.3/YvesCMD/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1351 2023-08-02 15:30:13.000000 yvesCMD-0.0.5.3/YvesCMD/src/extensions/select.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.242755 yvesCMD-0.0.5.3/YvesCMD/src/utils/
+-rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.5.3/YvesCMD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.5.3/YvesCMD/src/utils/detector.py
+-rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.5.3/YvesCMD/src/utils/hooks.py
+-rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.5.3/YvesCMD/src/utils/register.py
+-rw-rw-rw-   0        0        0     2518 2023-08-02 15:11:19.000000 yvesCMD-0.0.5.3/YvesCMD/src/yvescmd.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 16:23:50.250730 yvesCMD-0.0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      613 2023-08-02 16:23:00.000000 yvesCMD-0.0.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 16:23:50.205850 yvesCMD-0.0.5.3/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0     1730 2023-08-02 16:23:49.000000 yvesCMD-0.0.5.3/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-08-02 16:23:49.000000 yvesCMD-0.0.5.3/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 16:23:49.000000 yvesCMD-0.0.5.3/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 16:23:49.000000 yvesCMD-0.0.5.3/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.5.1/YvesCMD/src/extensions/select.py` & `yvesCMD-0.0.5.3/YvesCMD/src/extensions/select.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.1/YvesCMD/src/utils/detector.py` & `yvesCMD-0.0.5.3/YvesCMD/src/utils/detector.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.1/YvesCMD/src/utils/hooks.py` & `yvesCMD-0.0.5.3/YvesCMD/src/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.1/YvesCMD/src/utils/register.py` & `yvesCMD-0.0.5.3/YvesCMD/src/utils/register.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.5.1/YvesCMD/src/yvescmd.py` & `yvesCMD-0.0.5.3/YvesCMD/src/yvescmd.py`

 * *Files identical despite different names*

