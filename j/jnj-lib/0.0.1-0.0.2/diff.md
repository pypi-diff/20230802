# Comparing `tmp/jnj_lib-0.0.1.tar.gz` & `tmp/jnj_lib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jnj_lib-0.0.1.tar", last modified: Wed Aug  2 05:29:33 2023, max compression
+gzip compressed data, was "jnj_lib-0.0.2.tar", last modified: Wed Aug  2 05:39:51 2023, max compression
```

## Comparing `jnj_lib-0.0.1.tar` & `jnj_lib-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-08-02 05:29:33.189976 jnj_lib-0.0.1/
--rw-rw-rw-   0        0        0      293 2023-08-02 05:29:33.188976 jnj_lib-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-02 05:29:33.180968 jnj_lib-0.0.1/jnj_lib.egg-info/
--rw-rw-rw-   0        0        0      293 2023-08-02 05:29:33.000000 jnj_lib-0.0.1/jnj_lib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      266 2023-08-02 05:29:33.000000 jnj_lib-0.0.1/jnj_lib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-02 05:29:33.000000 jnj_lib-0.0.1/jnj_lib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-02 05:29:33.000000 jnj_lib-0.0.1/jnj_lib.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       19 2023-08-02 05:29:33.000000 jnj_lib-0.0.1/jnj_lib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-08-02 05:29:33.000000 jnj_lib-0.0.1/jnj_lib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-02 05:29:33.189976 jnj_lib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      566 2023-08-02 05:27:36.000000 jnj_lib-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-02 05:29:33.186011 jnj_lib-0.0.1/util_base/
--rw-rw-rw-   0        0        0     6842 2023-08-01 22:33:27.000000 jnj_lib-0.0.1/util_base/basic.py
--rw-rw-rw-   0        0        0     2178 2023-07-31 13:54:28.000000 jnj_lib-0.0.1/util_base/builtin.py
--rw-rw-rw-   0        0        0        0 2023-07-31 11:01:03.000000 jnj_lib-0.0.1/util_base/time.py
-drwxrwxrwx   0        0        0        0 2023-08-02 05:29:33.186979 jnj_lib-0.0.1/util_doc/
--rw-rw-rw-   0        0        0      247 2023-08-02 05:12:35.000000 jnj_lib-0.0.1/util_doc/doc.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:39:51.374514 jnj_lib-0.0.2/
+-rw-rw-rw-   0        0        0      293 2023-08-02 05:39:51.374514 jnj_lib-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-02 05:39:51.364545 jnj_lib-0.0.2/jnj_lib.egg-info/
+-rw-rw-rw-   0        0        0      293 2023-08-02 05:39:51.000000 jnj_lib-0.0.2/jnj_lib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-08-02 05:39:51.000000 jnj_lib-0.0.2/jnj_lib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-02 05:39:51.000000 jnj_lib-0.0.2/jnj_lib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-02 05:39:51.000000 jnj_lib-0.0.2/jnj_lib.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       19 2023-08-02 05:39:51.000000 jnj_lib-0.0.2/jnj_lib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-08-02 05:39:51.000000 jnj_lib-0.0.2/jnj_lib.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-02 05:39:51.375512 jnj_lib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-08-02 05:39:22.000000 jnj_lib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:39:51.370512 jnj_lib-0.0.2/util_base/
+-rw-rw-rw-   0        0        0       23 2023-08-02 05:39:33.000000 jnj_lib-0.0.2/util_base/__init__.py
+-rw-rw-rw-   0        0        0     6842 2023-08-01 22:33:27.000000 jnj_lib-0.0.2/util_base/basic.py
+-rw-rw-rw-   0        0        0     2178 2023-07-31 13:54:28.000000 jnj_lib-0.0.2/util_base/builtin.py
+-rw-rw-rw-   0        0        0        0 2023-07-31 11:01:03.000000 jnj_lib-0.0.2/util_base/time.py
+drwxrwxrwx   0        0        0        0 2023-08-02 05:39:51.372514 jnj_lib-0.0.2/util_doc/
+-rw-rw-rw-   0        0        0       23 2023-08-02 05:39:28.000000 jnj_lib-0.0.2/util_doc/__init__.py
+-rw-rw-rw-   0        0        0      247 2023-08-02 05:12:35.000000 jnj_lib-0.0.2/util_doc/doc.py
```

### Comparing `jnj_lib-0.0.1/setup.py` & `jnj_lib-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="jnj_lib",
-    version="0.0.1",
+    version="0.0.2",
     description="PYPI test package",
     author="moondevpy",
     author_email="moondevpy@gmail.com",
     url="https://github.com/moondevpy/jnj_lib",
     install_requires=["util_base", "util_doc"],
     packages=["util_base", "util_doc"],
     # packages=find_packages(exclude=[]),
```

### Comparing `jnj_lib-0.0.1/util_base/basic.py` & `jnj_lib-0.0.2/util_base/basic.py`

 * *Files identical despite different names*

### Comparing `jnj_lib-0.0.1/util_base/builtin.py` & `jnj_lib-0.0.2/util_base/builtin.py`

 * *Files identical despite different names*

