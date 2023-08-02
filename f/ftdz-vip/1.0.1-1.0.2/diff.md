# Comparing `tmp/ftdz_vip-1.0.1.tar.gz` & `tmp/ftdz_vip-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ftdz_vip-1.0.1.tar", last modified: Mon Jul 24 01:58:55 2023, max compression
+gzip compressed data, was "dist\ftdz_vip-1.0.2.tar", last modified: Wed Aug  2 01:23:18 2023, max compression
```

## Comparing `ftdz_vip-1.0.1.tar` & `ftdz_vip-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/
--rw-rw-rw-   0        0        0      325 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      346 2019-08-22 10:27:16.000000 ftdz_vip-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/ftdz_vip/
--rw-rw-rw-   0        0        0       50 2023-07-24 01:56:29.000000 ftdz_vip-1.0.1/ftdz_vip/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/ftdz_vip.egg-info/
--rw-rw-rw-   0        0        0      325 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/ftdz_vip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/ftdz_vip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/ftdz_vip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/ftdz_vip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-24 01:58:55.000000 ftdz_vip-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      480 2023-07-24 01:58:29.000000 ftdz_vip-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/
+-rw-rw-rw-   0        0        0      325 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2019-08-22 10:27:16.000000 ftdz_vip-1.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/ftdz_vip/
+-rw-rw-rw-   0        0        0       72 2023-08-02 01:20:25.000000 ftdz_vip-1.0.2/ftdz_vip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/ftdz_vip.egg-info/
+-rw-rw-rw-   0        0        0      325 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/ftdz_vip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/ftdz_vip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/ftdz_vip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/ftdz_vip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 01:23:18.000000 ftdz_vip-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      480 2023-08-02 01:22:33.000000 ftdz_vip-1.0.2/setup.py
```

