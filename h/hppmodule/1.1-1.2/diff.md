# Comparing `tmp/hppmodule-1.1.tar.gz` & `tmp/hppmodule-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hppmodule-1.1.tar", last modified: Wed Aug  2 05:55:45 2023, max compression
+gzip compressed data, was "hppmodule-1.2.tar", last modified: Wed Aug  2 06:55:39 2023, max compression
```

## Comparing `hppmodule-1.1.tar` & `hppmodule-1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        0 2023-08-02 05:55:45.638039 hppmodule-1.1/
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)      155 2023-08-02 05:55:45.637743 hppmodule-1.1/PKG-INFO
-drwxr-xr-x   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        0 2023-08-02 05:55:45.635075 hppmodule-1.1/hppmodule.egg-info/
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)      155 2023-08-02 05:55:45.000000 hppmodule-1.1/hppmodule.egg-info/PKG-INFO
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)      268 2023-08-02 05:55:45.000000 hppmodule-1.1/hppmodule.egg-info/SOURCES.txt
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        1 2023-08-02 05:55:45.000000 hppmodule-1.1/hppmodule.egg-info/dependency_links.txt
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        1 2023-08-02 05:55:45.000000 hppmodule-1.1/hppmodule.egg-info/not-zip-safe
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       15 2023-08-02 05:55:45.000000 hppmodule-1.1/hppmodule.egg-info/requires.txt
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       10 2023-08-02 05:55:45.000000 hppmodule-1.1/hppmodule.egg-info/top_level.txt
-drwxr-xr-x   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        0 2023-08-02 05:55:45.637135 hppmodule-1.1/mypackage/
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       65 2023-08-02 04:44:23.000000 hppmodule-1.1/mypackage/__init__.py
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       99 2023-08-02 04:39:14.000000 hppmodule-1.1/mypackage/functions.py
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       45 2023-08-02 04:38:37.000000 hppmodule-1.1/mypackage/greet.py
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       38 2023-08-02 05:55:45.638098 hppmodule-1.1/setup.cfg
--rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)      275 2023-08-02 05:55:30.000000 hppmodule-1.1/setup.py
+drwxr-xr-x   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        0 2023-08-02 06:55:39.272517 hppmodule-1.2/
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)      155 2023-08-02 06:55:39.272269 hppmodule-1.2/PKG-INFO
+drwxr-xr-x   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        0 2023-08-02 06:55:39.269776 hppmodule-1.2/hppmodule.egg-info/
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)      155 2023-08-02 06:55:39.000000 hppmodule-1.2/hppmodule.egg-info/PKG-INFO
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)      268 2023-08-02 06:55:39.000000 hppmodule-1.2/hppmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        1 2023-08-02 06:55:39.000000 hppmodule-1.2/hppmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        1 2023-08-02 06:55:39.000000 hppmodule-1.2/hppmodule.egg-info/not-zip-safe
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       15 2023-08-02 06:55:39.000000 hppmodule-1.2/hppmodule.egg-info/requires.txt
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       10 2023-08-02 06:55:39.000000 hppmodule-1.2/hppmodule.egg-info/top_level.txt
+drwxr-xr-x   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)        0 2023-08-02 06:55:39.271652 hppmodule-1.2/mypackage/
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       65 2023-08-02 04:44:23.000000 hppmodule-1.2/mypackage/__init__.py
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       99 2023-08-02 04:39:14.000000 hppmodule-1.2/mypackage/functions.py
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       45 2023-08-02 04:38:37.000000 hppmodule-1.2/mypackage/greet.py
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)       38 2023-08-02 06:55:39.272563 hppmodule-1.2/setup.cfg
+-rw-r--r--   0 htunpapa.aung (1197275226) INTRA\Domain Users (679754705)      275 2023-08-02 06:54:20.000000 hppmodule-1.2/setup.py
```

