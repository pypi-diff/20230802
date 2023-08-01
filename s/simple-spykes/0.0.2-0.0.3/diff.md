# Comparing `tmp/simple_spykes-0.0.2.tar.gz` & `tmp/simple_spykes-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_spykes-0.0.2.tar", last modified: Tue Aug  1 23:24:54 2023, max compression
+gzip compressed data, was "simple_spykes-0.0.3.tar", last modified: Tue Aug  1 23:27:51 2023, max compression
```

## Comparing `simple_spykes-0.0.2.tar` & `simple_spykes-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-01 23:24:54.404604 simple_spykes-0.0.2/
--rw-rw-rw-   0        0        0    35819 2023-08-01 21:31:04.000000 simple_spykes-0.0.2/LICENSE
--rw-rw-rw-   0        0        0      509 2023-08-01 23:24:54.403602 simple_spykes-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-08-01 21:30:37.000000 simple_spykes-0.0.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-08-01 23:24:54.404604 simple_spykes-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      695 2023-08-01 23:23:53.000000 simple_spykes-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-01 23:24:54.391604 simple_spykes-0.0.2/simple_spykes/
--rw-rw-rw-   0        0        0      139 2023-08-01 23:23:10.000000 simple_spykes-0.0.2/simple_spykes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-01 23:24:54.401603 simple_spykes-0.0.2/simple_spykes/util/
--rw-rw-rw-   0        0        0        0 2023-08-01 23:21:48.000000 simple_spykes-0.0.2/simple_spykes/util/__init__.py
--rw-rw-rw-   0        0        0     2694 2023-08-01 23:23:10.000000 simple_spykes-0.0.2/simple_spykes/util/ecephys.py
-drwxrwxrwx   0        0        0        0 2023-08-01 23:24:54.399603 simple_spykes-0.0.2/simple_spykes.egg-info/
--rw-rw-rw-   0        0        0      509 2023-08-01 23:24:54.000000 simple_spykes-0.0.2/simple_spykes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-08-01 23:24:54.000000 simple_spykes-0.0.2/simple_spykes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-01 23:24:54.000000 simple_spykes-0.0.2/simple_spykes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2023-08-01 23:24:54.000000 simple_spykes-0.0.2/simple_spykes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-08-01 23:24:54.000000 simple_spykes-0.0.2/simple_spykes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-01 23:27:51.838266 simple_spykes-0.0.3/
+-rw-rw-rw-   0        0        0    35819 2023-08-01 21:31:04.000000 simple_spykes-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      509 2023-08-01 23:27:51.838266 simple_spykes-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-08-01 21:30:37.000000 simple_spykes-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-08-01 23:27:51.839265 simple_spykes-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-08-01 23:27:31.000000 simple_spykes-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:27:51.827266 simple_spykes-0.0.3/simple_spykes/
+-rw-rw-rw-   0        0        0      139 2023-08-01 23:23:10.000000 simple_spykes-0.0.3/simple_spykes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:27:51.836264 simple_spykes-0.0.3/simple_spykes/util/
+-rw-rw-rw-   0        0        0        0 2023-08-01 23:21:48.000000 simple_spykes-0.0.3/simple_spykes/util/__init__.py
+-rw-rw-rw-   0        0        0     2643 2023-08-01 23:27:20.000000 simple_spykes-0.0.3/simple_spykes/util/ecephys.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:27:51.834265 simple_spykes-0.0.3/simple_spykes.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-01 23:27:51.000000 simple_spykes-0.0.3/simple_spykes.egg-info/top_level.txt
```

### Comparing `simple_spykes-0.0.2/LICENSE` & `simple_spykes-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_spykes-0.0.2/setup.py` & `simple_spykes-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = "0.0.2"
+VERSION = "0.0.3"
 
 
 def parse_requirements(requirement_file):
     with open(requirement_file) as fi:
         return fi.readlines()
```

