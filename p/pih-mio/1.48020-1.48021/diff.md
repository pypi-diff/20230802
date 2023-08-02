# Comparing `tmp/pih-mio-1.48020.tar.gz` & `tmp/pih-mio-1.48021.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48020.tar", last modified: Tue Aug  1 02:58:53 2023, max compression
+gzip compressed data, was "pih-mio-1.48021.tar", last modified: Wed Aug  2 07:06:17 2023, max compression
```

## Comparing `pih-mio-1.48020.tar` & `pih-mio-1.48021.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 02:58:52.647787 pih-mio-1.48020/
-drwxrwxrwx   0        0        0        0 2023-08-01 02:58:48.551481 pih-mio-1.48020/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48020/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48020/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165321 2023-08-01 02:56:27.000000 pih-mio-1.48020/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48020/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48020/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48020/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-01 02:58:52.616531 pih-mio-1.48020/PKG-INFO
--rw-rw-rw-   0        0        0     1624 2023-08-01 02:47:46.000000 pih-mio-1.48020/mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 02:58:52.330303 pih-mio-1.48020/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-01 02:58:37.000000 pih-mio-1.48020/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2023-08-01 02:58:39.000000 pih-mio-1.48020/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 02:58:37.000000 pih-mio-1.48020/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-01 02:58:38.000000 pih-mio-1.48020/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-01 02:58:38.000000 pih-mio-1.48020/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-01 02:58:38.000000 pih-mio-1.48020/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-01 02:58:52.694652 pih-mio-1.48020/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-02 07:06:16.700121 pih-mio-1.48021/
+drwxrwxrwx   0        0        0        0 2023-08-02 07:06:17.314530 pih-mio-1.48021/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48021/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48021/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165321 2023-08-01 02:56:27.000000 pih-mio-1.48021/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48021/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9434 2023-08-01 00:38:40.000000 pih-mio-1.48021/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48021/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-02 07:06:17.502024 pih-mio-1.48021/PKG-INFO
+-rw-rw-rw-   0        0        0     1628 2023-08-02 06:40:52.000000 pih-mio-1.48021/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 07:06:17.361400 pih-mio-1.48021/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-02 07:06:15.000000 pih-mio-1.48021/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-02 07:06:16.000000 pih-mio-1.48021/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 07:06:15.000000 pih-mio-1.48021/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-02 07:06:16.000000 pih-mio-1.48021/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-02 07:06:16.000000 pih-mio-1.48021/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-02 07:06:16.000000 pih-mio-1.48021/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 07:06:17.517656 pih-mio-1.48021/setup.cfg
```

### Comparing `pih-mio-1.48020/MobileHelperCore/api.py` & `pih-mio-1.48021/MobileHelperCore/api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48020/MobileHelperCore/service.py` & `pih-mio-1.48021/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48020/MobileHelperCore/service_api.py` & `pih-mio-1.48021/MobileHelperCore/service_api.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48020/MobileHelperCore/tools.py` & `pih-mio-1.48021/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48020/mio_setup.py` & `pih-mio-1.48021/pih-mio_setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 #########################################################################################################
 """
 1. python mio_setup.py sdist --dist-dir mio_dist bdist_wheel --dist-dir mio_dist build --build-base pih_mio_build
 2. twine upload --repository pypi mio_dist/*
 3. pip install pih_mio -U
 """
-folder = "//pih/facade/mio_dist"
+folder = "//pih/facade/pih-mio_dist"
 for filename in os.listdir(folder):
     file_path = os.path.join(folder, filename)
     try:
         if os.path.isfile(file_path) or os.path.islink(file_path):
             os.unlink(file_path)
         elif os.path.isdir(file_path):
             shutil.rmtree(file_path)
```

