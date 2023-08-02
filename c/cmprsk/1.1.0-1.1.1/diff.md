# Comparing `tmp/cmprsk-1.1.0.tar.gz` & `tmp/cmprsk-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmprsk-1.1.0.tar", last modified: Fri Mar 10 01:03:07 2023, max compression
+gzip compressed data, was "cmprsk-1.1.1.tar", last modified: Wed Aug  2 10:37:07 2023, max compression
```

## Comparing `cmprsk-1.1.0.tar` & `cmprsk-1.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 omribahattreidel   (501) staff       (20)        0 2023-03-10 01:03:07.359624 cmprsk-1.1.0/
--rw-r--r--   0 omribahattreidel   (501) staff       (20)    35149 2021-11-18 08:55:05.000000 cmprsk-1.1.0/LICENSE
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     5315 2023-03-10 01:03:07.359488 cmprsk-1.1.0/PKG-INFO
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     4823 2023-03-10 00:41:58.000000 cmprsk-1.1.0/README.md
-drwxr-xr-x   0 omribahattreidel   (501) staff       (20)        0 2023-03-10 01:03:07.358422 cmprsk-1.1.0/cmprsk/
--rw-r--r--   0 omribahattreidel   (501) staff       (20)        0 2021-11-18 08:55:05.000000 cmprsk-1.1.0/cmprsk/__init__.py
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     8099 2021-12-03 06:13:38.000000 cmprsk-1.1.0/cmprsk/cmprsk.py
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     2067 2023-03-03 04:33:22.000000 cmprsk-1.1.0/cmprsk/rpy_utils.py
-drwxr-xr-x   0 omribahattreidel   (501) staff       (20)        0 2023-03-10 01:03:07.359336 cmprsk-1.1.0/cmprsk/tests/
--rw-r--r--   0 omribahattreidel   (501) staff       (20)        0 2021-11-18 08:55:05.000000 cmprsk-1.1.0/cmprsk/tests/__init__.py
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     1077 2021-11-18 08:55:05.000000 cmprsk-1.1.0/cmprsk/tests/test_cmprsk.py
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     1196 2021-12-03 06:13:38.000000 cmprsk-1.1.0/cmprsk/tests/test_rpy_utils.py
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     1462 2021-11-18 08:55:05.000000 cmprsk-1.1.0/cmprsk/tests/test_utils.py
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     1218 2021-12-03 06:13:38.000000 cmprsk-1.1.0/cmprsk/utils.py
-drwxr-xr-x   0 omribahattreidel   (501) staff       (20)        0 2023-03-10 01:03:07.358924 cmprsk-1.1.0/cmprsk.egg-info/
--rw-r--r--   0 omribahattreidel   (501) staff       (20)     5315 2023-03-10 01:03:07.000000 cmprsk-1.1.0/cmprsk.egg-info/PKG-INFO
--rw-r--r--   0 omribahattreidel   (501) staff       (20)      358 2023-03-10 01:03:07.000000 cmprsk-1.1.0/cmprsk.egg-info/SOURCES.txt
--rw-r--r--   0 omribahattreidel   (501) staff       (20)        1 2023-03-10 01:03:07.000000 cmprsk-1.1.0/cmprsk.egg-info/dependency_links.txt
--rw-r--r--   0 omribahattreidel   (501) staff       (20)       24 2023-03-10 01:03:07.000000 cmprsk-1.1.0/cmprsk.egg-info/requires.txt
--rw-r--r--   0 omribahattreidel   (501) staff       (20)        7 2023-03-10 01:03:07.000000 cmprsk-1.1.0/cmprsk.egg-info/top_level.txt
--rw-r--r--   0 omribahattreidel   (501) staff       (20)       38 2023-03-10 01:03:07.359656 cmprsk-1.1.0/setup.cfg
--rw-r--r--   0 omribahattreidel   (501) staff       (20)      916 2023-03-10 00:52:48.000000 cmprsk-1.1.0/setup.py
+drwxr-xr-x   0 omribahattreidel   (501) staff       (20)        0 2023-08-02 10:37:07.500142 cmprsk-1.1.1/
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)    35149 2021-11-18 08:55:05.000000 cmprsk-1.1.1/LICENSE
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     5315 2023-08-02 10:37:07.500004 cmprsk-1.1.1/PKG-INFO
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     4823 2023-03-10 00:41:58.000000 cmprsk-1.1.1/README.md
+drwxr-xr-x   0 omribahattreidel   (501) staff       (20)        0 2023-08-02 10:37:07.498928 cmprsk-1.1.1/cmprsk/
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)        0 2021-11-18 08:55:05.000000 cmprsk-1.1.1/cmprsk/__init__.py
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     8099 2021-12-03 06:13:38.000000 cmprsk-1.1.1/cmprsk/cmprsk.py
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     2071 2023-08-02 10:35:20.000000 cmprsk-1.1.1/cmprsk/rpy_utils.py
+drwxr-xr-x   0 omribahattreidel   (501) staff       (20)        0 2023-08-02 10:37:07.499860 cmprsk-1.1.1/cmprsk/tests/
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)        0 2021-11-18 08:55:05.000000 cmprsk-1.1.1/cmprsk/tests/__init__.py
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     1077 2021-11-18 08:55:05.000000 cmprsk-1.1.1/cmprsk/tests/test_cmprsk.py
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     1885 2023-08-02 10:35:20.000000 cmprsk-1.1.1/cmprsk/tests/test_rpy_utils.py
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     1462 2021-11-18 08:55:05.000000 cmprsk-1.1.1/cmprsk/tests/test_utils.py
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     1218 2021-12-03 06:13:38.000000 cmprsk-1.1.1/cmprsk/utils.py
+drwxr-xr-x   0 omribahattreidel   (501) staff       (20)        0 2023-08-02 10:37:07.499447 cmprsk-1.1.1/cmprsk.egg-info/
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)     5315 2023-08-02 10:37:07.000000 cmprsk-1.1.1/cmprsk.egg-info/PKG-INFO
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)      358 2023-08-02 10:37:07.000000 cmprsk-1.1.1/cmprsk.egg-info/SOURCES.txt
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)        1 2023-08-02 10:37:07.000000 cmprsk-1.1.1/cmprsk.egg-info/dependency_links.txt
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)       24 2023-08-02 10:37:07.000000 cmprsk-1.1.1/cmprsk.egg-info/requires.txt
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)        7 2023-08-02 10:37:07.000000 cmprsk-1.1.1/cmprsk.egg-info/top_level.txt
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)       38 2023-08-02 10:37:07.500177 cmprsk-1.1.1/setup.cfg
+-rw-r--r--   0 omribahattreidel   (501) staff       (20)      916 2023-08-02 10:36:08.000000 cmprsk-1.1.1/setup.py
```

### Comparing `cmprsk-1.1.0/LICENSE` & `cmprsk-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmprsk-1.1.0/PKG-INFO` & `cmprsk-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmprsk
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python wrapper around cmprsk R package
 Home-page: https://github.com/OmriTreidel/cmprsk
 Author: Omri Treidel
 Author-email: treidel2@gmail.com
 Keywords: competing risks,survival analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `cmprsk-1.1.0/README.md` & `cmprsk-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cmprsk-1.1.0/cmprsk/cmprsk.py` & `cmprsk-1.1.1/cmprsk/cmprsk.py`

 * *Files identical despite different names*

### Comparing `cmprsk-1.1.0/cmprsk/rpy_utils.py` & `cmprsk-1.1.1/cmprsk/rpy_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 class NotImplementedError(Exception):
     pass
 
 
 class InputError(Exception):
     pass
 
+
 def all_strings(np_arr) -> bool:
-    for x in arr:
+    for x in np_arr:
         if not isinstance(x, str):
             return False
     return True
 
 
 def r_vector(np_vector):
     """Convert a numpy vector to an R vector
```

### Comparing `cmprsk-1.1.0/cmprsk/tests/test_cmprsk.py` & `cmprsk-1.1.1/cmprsk/tests/test_cmprsk.py`

 * *Files identical despite different names*

### Comparing `cmprsk-1.1.0/cmprsk/tests/test_utils.py` & `cmprsk-1.1.1/cmprsk/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `cmprsk-1.1.0/cmprsk/utils.py` & `cmprsk-1.1.1/cmprsk/utils.py`

 * *Files identical despite different names*

### Comparing `cmprsk-1.1.0/cmprsk.egg-info/PKG-INFO` & `cmprsk-1.1.1/cmprsk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmprsk
-Version: 1.1.0
+Version: 1.1.1
 Summary: A python wrapper around cmprsk R package
 Home-page: https://github.com/OmriTreidel/cmprsk
 Author: Omri Treidel
 Author-email: treidel2@gmail.com
 Keywords: competing risks,survival analysis
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `cmprsk-1.1.0/setup.py` & `cmprsk-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cmprsk",
-    version="1.1.0",
+    version="1.1.1",
     author="Omri Treidel",
     author_email="treidel2@gmail.com",
     description="A python wrapper around cmprsk R package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OmriTreidel/cmprsk",
     packages=setuptools.find_packages(),
```

