# Comparing `tmp/yvesCMD-0.0.3.tar.gz` & `tmp/yvesCMD-0.0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.3.tar", last modified: Wed Aug  2 13:17:30 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.3.1.tar", last modified: Wed Aug  2 14:35:37 2023, max compression
```

## Comparing `yvesCMD-0.0.3.tar` & `yvesCMD-0.0.3.1.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 13:17:30.019224 yvesCMD-0.0.3/
--rw-rw-rw-   0        0        0      203 2023-08-02 13:17:30.017229 yvesCMD-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-08-02 13:17:29.954398 yvesCMD-0.0.3/YvesCMD/
--rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.3/YvesCMD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 13:17:29.960383 yvesCMD-0.0.3/YvesCMD/src/
--rw-rw-rw-   0        0        0       27 2023-08-02 13:13:14.000000 yvesCMD-0.0.3/YvesCMD/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-02 13:17:30.015234 yvesCMD-0.0.3/YvesCMD/src/utils/
--rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.3/YvesCMD/src/utils/__init__.py
--rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.3/YvesCMD/src/utils/detector.py
--rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.3/YvesCMD/src/utils/hooks.py
--rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.3/YvesCMD/src/utils/register.py
--rw-rw-rw-   0        0        0     2514 2023-08-02 13:12:42.000000 yvesCMD-0.0.3/YvesCMD/src/yvescmd.py
--rw-rw-rw-   0        0        0       42 2023-08-02 13:17:30.019224 yvesCMD-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-08-02 13:15:40.000000 yvesCMD-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 13:17:30.002272 yvesCMD-0.0.3/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      203 2023-08-02 13:17:29.000000 yvesCMD-0.0.3/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      393 2023-08-02 13:17:29.000000 yvesCMD-0.0.3/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 13:17:29.000000 yvesCMD-0.0.3/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-02 13:17:29.000000 yvesCMD-0.0.3/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.362399 yvesCMD-0.0.3.1/
+-rw-rw-rw-   0        0        0      205 2023-08-02 14:35:37.360405 yvesCMD-0.0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.261670 yvesCMD-0.0.3.1/YvesCMD/
+-rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.3.1/YvesCMD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.274634 yvesCMD-0.0.3.1/YvesCMD/src/
+-rw-rw-rw-   0        0        0       53 2023-08-02 14:29:12.000000 yvesCMD-0.0.3.1/YvesCMD/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.340461 yvesCMD-0.0.3.1/YvesCMD/src/extensions/
+-rw-rw-rw-   0        0        0       37 2023-08-02 14:29:07.000000 yvesCMD-0.0.3.1/YvesCMD/src/extensions/__init__.py
+-rw-rw-rw-   0        0        0     1166 2023-08-02 14:28:56.000000 yvesCMD-0.0.3.1/YvesCMD/src/extensions/select.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.358411 yvesCMD-0.0.3.1/YvesCMD/src/utils/
+-rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.3.1/YvesCMD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.3.1/YvesCMD/src/utils/detector.py
+-rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.3.1/YvesCMD/src/utils/hooks.py
+-rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.3.1/YvesCMD/src/utils/register.py
+-rw-rw-rw-   0        0        0     2514 2023-08-02 13:12:42.000000 yvesCMD-0.0.3.1/YvesCMD/src/yvescmd.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 14:35:37.362399 yvesCMD-0.0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      335 2023-08-02 14:35:32.000000 yvesCMD-0.0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 14:35:37.307548 yvesCMD-0.0.3.1/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      205 2023-08-02 14:35:36.000000 yvesCMD-0.0.3.1/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-08-02 14:35:37.000000 yvesCMD-0.0.3.1/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 14:35:36.000000 yvesCMD-0.0.3.1/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 14:35:36.000000 yvesCMD-0.0.3.1/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.3/README.md` & `yvesCMD-0.0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.3/YvesCMD/src/utils/detector.py` & `yvesCMD-0.0.3.1/YvesCMD/src/utils/detector.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.3/YvesCMD/src/utils/hooks.py` & `yvesCMD-0.0.3.1/YvesCMD/src/utils/hooks.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.3/YvesCMD/src/utils/register.py` & `yvesCMD-0.0.3.1/YvesCMD/src/utils/register.py`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.3/YvesCMD/src/yvescmd.py` & `yvesCMD-0.0.3.1/YvesCMD/src/yvescmd.py`

 * *Files identical despite different names*

