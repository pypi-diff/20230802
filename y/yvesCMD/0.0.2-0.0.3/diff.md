# Comparing `tmp/yvesCMD-0.0.2.tar.gz` & `tmp/yvesCMD-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yvesCMD-0.0.2.tar", last modified: Tue Aug  1 09:22:21 2023, max compression
+gzip compressed data, was "yvesCMD-0.0.3.tar", last modified: Wed Aug  2 13:17:30 2023, max compression
```

## Comparing `yvesCMD-0.0.2.tar` & `yvesCMD-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 09:22:21.240825 yvesCMD-0.0.2/
--rw-rw-rw-   0        0        0      203 2023-08-01 09:22:21.238828 yvesCMD-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-01 09:22:21.194944 yvesCMD-0.0.2/YvesCMD/
--rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.2/YvesCMD/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:22:21.208909 yvesCMD-0.0.2/YvesCMD/src/
--rw-rw-rw-   0        0        0       77 2023-08-01 08:32:37.000000 yvesCMD-0.0.2/YvesCMD/src/__init__.py
--rw-rw-rw-   0        0        0     1427 2023-07-31 13:41:19.000000 yvesCMD-0.0.2/YvesCMD/src/register.py
--rw-rw-rw-   0        0        0     6397 2023-08-01 09:22:01.000000 yvesCMD-0.0.2/YvesCMD/src/yvescmd.py
--rw-rw-rw-   0        0        0       42 2023-08-01 09:22:21.240825 yvesCMD-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      333 2023-08-01 09:22:15.000000 yvesCMD-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 09:22:21.234843 yvesCMD-0.0.2/yvesCMD.egg-info/
--rw-rw-rw-   0        0        0      203 2023-08-01 09:22:20.000000 yvesCMD-0.0.2/yvesCMD.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-08-01 09:22:21.000000 yvesCMD-0.0.2/yvesCMD.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 09:22:20.000000 yvesCMD-0.0.2/yvesCMD.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-08-01 09:22:20.000000 yvesCMD-0.0.2/yvesCMD.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-02 13:17:30.019224 yvesCMD-0.0.3/
+-rw-rw-rw-   0        0        0      203 2023-08-02 13:17:30.017229 yvesCMD-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      644 2023-07-31 18:07:55.000000 yvesCMD-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-02 13:17:29.954398 yvesCMD-0.0.3/YvesCMD/
+-rw-rw-rw-   0        0        0       25 2023-08-01 09:12:31.000000 yvesCMD-0.0.3/YvesCMD/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:17:29.960383 yvesCMD-0.0.3/YvesCMD/src/
+-rw-rw-rw-   0        0        0       27 2023-08-02 13:13:14.000000 yvesCMD-0.0.3/YvesCMD/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:17:30.015234 yvesCMD-0.0.3/YvesCMD/src/utils/
+-rw-rw-rw-   0        0        0      104 2023-08-02 13:11:36.000000 yvesCMD-0.0.3/YvesCMD/src/utils/__init__.py
+-rw-rw-rw-   0        0        0      527 2023-08-02 13:07:53.000000 yvesCMD-0.0.3/YvesCMD/src/utils/detector.py
+-rw-rw-rw-   0        0        0      898 2023-08-02 12:19:00.000000 yvesCMD-0.0.3/YvesCMD/src/utils/hooks.py
+-rw-rw-rw-   0        0        0     1427 2023-08-02 12:09:51.000000 yvesCMD-0.0.3/YvesCMD/src/utils/register.py
+-rw-rw-rw-   0        0        0     2514 2023-08-02 13:12:42.000000 yvesCMD-0.0.3/YvesCMD/src/yvescmd.py
+-rw-rw-rw-   0        0        0       42 2023-08-02 13:17:30.019224 yvesCMD-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      333 2023-08-02 13:15:40.000000 yvesCMD-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 13:17:30.002272 yvesCMD-0.0.3/yvesCMD.egg-info/
+-rw-rw-rw-   0        0        0      203 2023-08-02 13:17:29.000000 yvesCMD-0.0.3/yvesCMD.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      393 2023-08-02 13:17:29.000000 yvesCMD-0.0.3/yvesCMD.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 13:17:29.000000 yvesCMD-0.0.3/yvesCMD.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-08-02 13:17:29.000000 yvesCMD-0.0.3/yvesCMD.egg-info/top_level.txt
```

### Comparing `yvesCMD-0.0.2/README.md` & `yvesCMD-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `yvesCMD-0.0.2/YvesCMD/src/register.py` & `yvesCMD-0.0.3/YvesCMD/src/utils/register.py`

 * *Files identical despite different names*

