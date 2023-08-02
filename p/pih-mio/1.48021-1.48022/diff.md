# Comparing `tmp/pih-mio-1.48021.tar.gz` & `tmp/pih-mio-1.48022.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48021.tar", last modified: Wed Aug  2 07:06:17 2023, max compression
+gzip compressed data, was "pih-mio-1.48022.tar", last modified: Wed Aug  2 07:45:03 2023, max compression
```

## Comparing `pih-mio-1.48021.tar` & `pih-mio-1.48022.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 07:06:16.700121 pih-mio-1.48021/
-drwxrwxrwx   0        0        0        0 2023-08-02 07:06:17.314530 pih-mio-1.48021/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48021/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48021/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165321 2023-08-01 02:56:27.000000 pih-mio-1.48021/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48021/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48021/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48021/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-02 07:06:17.502024 pih-mio-1.48021/PKG-INFO
--rw-rw-rw-   0        0        0     1628 2023-08-02 06:40:52.000000 pih-mio-1.48021/pih-mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 07:06:17.361400 pih-mio-1.48021/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-02 07:06:15.000000 pih-mio-1.48021/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-02 07:06:16.000000 pih-mio-1.48021/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 07:06:15.000000 pih-mio-1.48021/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-02 07:06:16.000000 pih-mio-1.48021/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-02 07:06:16.000000 pih-mio-1.48021/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-02 07:06:16.000000 pih-mio-1.48021/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 07:06:17.517656 pih-mio-1.48021/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 07:45:01.137763 pih-mio-1.48022/
+drwxrwxrwx   0        0        0        0 2023-08-02 07:45:01.950268 pih-mio-1.48022/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48022/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48022/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165321 2023-08-01 02:56:27.000000 pih-mio-1.48022/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48022/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48022/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48022/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-02 07:45:03.342405 pih-mio-1.48022/PKG-INFO
+-rw-rw-rw-   0        0        0     1628 2023-08-02 06:40:52.000000 pih-mio-1.48022/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:45:03.264296 pih-mio-1.48022/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-02 07:45:00.000000 pih-mio-1.48022/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:45:03.358033 pih-mio-1.48022/setup.cfg
```

### Comparing `pih-mio-1.48021/MobileHelperCore/api.py` & `pih-mio-1.48022/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48021/MobileHelperCore/service.py` & `pih-mio-1.48022/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48021/MobileHelperCore/service_api.py` & `pih-mio-1.48022/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48021/MobileHelperCore/tools.py` & `pih-mio-1.48022/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48021/pih-mio_setup.py` & `pih-mio-1.48022/pih-mio_setup.py`

 * *Files identical despite different names*

