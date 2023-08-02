# Comparing `tmp/scipion-em-aretomo-3.7.tar.gz` & `tmp/scipion-em-aretomo-3.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-aretomo-3.7.tar", last modified: Sat Jun 10 11:31:36 2023, max compression
+gzip compressed data, was "scipion-em-aretomo-3.7.1.tar", last modified: Wed Aug  2 11:06:13 2023, max compression
```

## Comparing `scipion-em-aretomo-3.7.tar` & `scipion-em-aretomo-3.7.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.457180 scipion-em-aretomo-3.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/aretomo/
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/convert.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/aretomo/protocols/
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/protocols/protocol_aretomo.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/aretomo/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/aretomo/tests/test_protocols_aretomo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:31:36.453180 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-10 11:31:36.000000 scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 11:31:36.457180 scipion-em-aretomo-3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-06-10 11:29:42.000000 scipion-em-aretomo-3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:06:13.370379 scipion-em-aretomo-3.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-02 11:06:13.366379 scipion-em-aretomo-3.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:06:13.366379 scipion-em-aretomo-3.7.1/aretomo/
+-rw-r--r--   0 runner    (1001) docker     (123)     3299 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3378 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/convert.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:06:13.366379 scipion-em-aretomo-3.7.1/aretomo/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31625 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/protocols/protocol_aretomo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:06:13.366379 scipion-em-aretomo-3.7.1/aretomo/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3853 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/aretomo/tests/test_protocols_aretomo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:06:13.366379 scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-08-02 11:06:13.000000 scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-08-02 11:06:13.000000 scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:06:13.000000 scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-08-02 11:06:13.000000 scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-08-02 11:06:13.000000 scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 11:06:13.000000 scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 11:06:13.370379 scipion-em-aretomo-3.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-08-02 11:04:02.000000 scipion-em-aretomo-3.7.1/setup.py
```

### Comparing `scipion-em-aretomo-3.7/CHANGES.txt` & `scipion-em-aretomo-3.7.1/CHANGES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+3.7.1: fix pw requirements
 3.7: initial streaming support (@albertmena)
 3.6.5: allow unsorted tilt series
 3.6.4: adding type hints
 3.6.3: reduce number of Set[item] calls
 3.6.2:
  - fix applyTransform in the convert step
  - add interpolated flag
```

### Comparing `scipion-em-aretomo-3.7/LICENSE` & `scipion-em-aretomo-3.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/PKG-INFO` & `scipion-em-aretomo-3.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.7
+Version: 3.7.1
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
```

### Comparing `scipion-em-aretomo-3.7/README.rst` & `scipion-em-aretomo-3.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/aretomo/__init__.py` & `scipion-em-aretomo-3.7.1/aretomo/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import pwem
 import pyworkflow.utils as pwutils
 
 from .constants import *
 
 
-__version__ = '3.7'
+__version__ = '3.7.1'
 _logo = "aretomo_logo.png"
 _references = ['Zheng2022']
 
 
 class Plugin(pwem.Plugin):
     _homeVar = ARETOMO_HOME
     _pathVars = [ARETOMO_HOME, ARETOMO_CUDA_LIB]
```

### Comparing `scipion-em-aretomo-3.7/aretomo/bibtex.py` & `scipion-em-aretomo-3.7.1/aretomo/bibtex.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/aretomo/constants.py` & `scipion-em-aretomo-3.7.1/aretomo/constants.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/aretomo/convert.py` & `scipion-em-aretomo-3.7.1/aretomo/convert.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/aretomo/protocols/__init__.py` & `scipion-em-aretomo-3.7.1/aretomo/protocols/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/aretomo/protocols/protocol_aretomo.py` & `scipion-em-aretomo-3.7.1/aretomo/protocols/protocol_aretomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/aretomo/protocols.conf` & `scipion-em-aretomo-3.7.1/aretomo/protocols.conf`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/aretomo/tests/__init__.py` & `scipion-em-aretomo-3.7.1/aretomo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/aretomo/tests/test_protocols_aretomo.py` & `scipion-em-aretomo-3.7.1/aretomo/tests/test_protocols_aretomo.py`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/PKG-INFO` & `scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: scipion-em-aretomo
-Version: 3.7
+Version: 3.7.1
 Summary: Plugin to use AreTomo program within the Scipion framework
 Home-page: https://github.com/scipion-em/scipion-em-aretomo
 Author: Grigory Sharov
 Author-email: sharov.grigory@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/scipion-em/scipion-em-aretomo/issues
 Project-URL: Source, https://github.com/scipion-em/scipion-em-aretomo/
```

### Comparing `scipion-em-aretomo-3.7/scipion_em_aretomo.egg-info/SOURCES.txt` & `scipion-em-aretomo-3.7.1/scipion_em_aretomo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-aretomo-3.7/setup.py` & `scipion-em-aretomo-3.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,16 @@
     packages=find_packages(),
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    install_requires=['scipion-em', 'scipion-em-tomo'],  # Optional
+    install_requires=['scipion-em', 'scipion-em-tomo',
+                      'scipion-pyworkflow>=3.0.30'],  # Optional
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
```

