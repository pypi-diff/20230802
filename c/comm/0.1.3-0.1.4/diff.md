# Comparing `tmp/comm-0.1.3.tar.gz` & `tmp/comm-0.1.4.tar.gz`

## Comparing `comm-0.1.3.tar` & `comm-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 comm-0.1.3/comm/__init__.py
--rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 comm-0.1.3/comm/base_comm.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 comm-0.1.3/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 comm-0.1.3/LICENSE
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 comm-0.1.3/README.md
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 comm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 comm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 comm-0.1.4/comm/__init__.py
+-rw-r--r--   0        0        0     8420 2020-02-02 00:00:00.000000 comm-0.1.4/comm/base_comm.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 comm-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 comm-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 comm-0.1.4/README.md
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 comm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4221 2020-02-02 00:00:00.000000 comm-0.1.4/PKG-INFO
```

### Comparing `comm-0.1.3/comm/__init__.py` & `comm-0.1.4/comm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 This package provides a way to register a Kernel Comm implementation, as per
 the Jupyter kernel protocol.
 It also provides a base Comm implementation and a default CommManager for the IPython case.
 """
 
 from .base_comm import BaseComm, CommManager
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
 __all__ = [
     "create_comm",
     "get_comm_manager",
     "__version__",
 ]
 
 _comm_manager = None
```

### Comparing `comm-0.1.3/comm/base_comm.py` & `comm-0.1.4/comm/base_comm.py`

 * *Files identical despite different names*

### Comparing `comm-0.1.3/LICENSE` & `comm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `comm-0.1.3/README.md` & `comm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `comm-0.1.3/pyproject.toml` & `comm-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
-    "traitlets>=5.3",
+    "traitlets>=4",
 ]
 
 [project.optional-dependencies]
 test = [
   "pytest",
 ]
 lint = [
```

### Comparing `comm-0.1.3/PKG-INFO` & `comm-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: comm
-Version: 0.1.3
+Version: 0.1.4
 Summary: Jupyter Python Comm implementation, for usage in ipykernel, xeus-python etc.
 Project-URL: Homepage, https://github.com/ipython/comm
 Author: Jupyter contributors
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Jupyter
         All rights reserved.
@@ -41,15 +41,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.6
-Requires-Dist: traitlets>=5.3
+Requires-Dist: traitlets>=4
 Provides-Extra: lint
 Requires-Dist: black>=22.6.0; extra == 'lint'
 Requires-Dist: mdformat-gfm>=0.3.5; extra == 'lint'
 Requires-Dist: mdformat>0.7; extra == 'lint'
 Requires-Dist: ruff>=0.0.156; extra == 'lint'
 Provides-Extra: test
 Requires-Dist: pytest; extra == 'test'
```

