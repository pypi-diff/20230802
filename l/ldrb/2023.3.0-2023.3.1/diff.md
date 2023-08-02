# Comparing `tmp/ldrb-2023.3.0.tar.gz` & `tmp/ldrb-2023.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldrb-2023.3.0.tar", last modified: Fri May  5 09:46:34 2023, max compression
+gzip compressed data, was "ldrb-2023.3.1.tar", last modified: Wed Aug  2 18:55:29 2023, max compression
```

## Comparing `ldrb-2023.3.0.tar` & `ldrb-2023.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:46:34.698913 ldrb-2023.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-05 09:46:20.000000 ldrb-2023.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 09:46:34.698913 ldrb-2023.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-05 09:46:20.000000 ldrb-2023.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:46:34.698913 ldrb-2023.3.0/ldrb/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/calculus.py
--rw-r--r--   0 runner    (1001) docker     (123)    24675 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/ldrb.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/save.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-05-05 09:46:20.000000 ldrb-2023.3.0/ldrb/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:46:34.698913 ldrb-2023.3.0/ldrb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 09:46:34.000000 ldrb-2023.3.0/ldrb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-05 09:46:34.702913 ldrb-2023.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 09:46:20.000000 ldrb-2023.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:46:34.698913 ldrb-2023.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-05-05 09:46:20.000000 ldrb-2023.3.0/tests/test_ldrb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-05 09:46:20.000000 ldrb-2023.3.0/tests/test_save.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:29.845966 ldrb-2023.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-02 18:55:13.000000 ldrb-2023.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-02 18:55:29.845966 ldrb-2023.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-08-02 18:55:13.000000 ldrb-2023.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:29.841966 ldrb-2023.3.1/ldrb/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-08-02 18:55:13.000000 ldrb-2023.3.1/ldrb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-08-02 18:55:13.000000 ldrb-2023.3.1/ldrb/calculus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24564 2023-08-02 18:55:13.000000 ldrb-2023.3.1/ldrb/ldrb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-02 18:55:13.000000 ldrb-2023.3.1/ldrb/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-08-02 18:55:13.000000 ldrb-2023.3.1/ldrb/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:29.841966 ldrb-2023.3.1/ldrb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-02 18:55:29.000000 ldrb-2023.3.1/ldrb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-08-02 18:55:29.000000 ldrb-2023.3.1/ldrb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:55:29.000000 ldrb-2023.3.1/ldrb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 18:55:29.000000 ldrb-2023.3.1/ldrb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-02 18:55:29.000000 ldrb-2023.3.1/ldrb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-02 18:55:29.000000 ldrb-2023.3.1/ldrb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-02 18:55:29.845966 ldrb-2023.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-08-02 18:55:13.000000 ldrb-2023.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 18:55:29.845966 ldrb-2023.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-08-02 18:55:13.000000 ldrb-2023.3.1/tests/test_ldrb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-08-02 18:55:13.000000 ldrb-2023.3.1/tests/test_save.py
```

### Comparing `ldrb-2023.3.0/LICENSE` & `ldrb-2023.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ldrb-2023.3.0/PKG-INFO` & `ldrb-2023.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ldrb
-Version: 2023.3.0
+Version: 2023.3.1
 Summary: Laplace-Dirichlet Rule-based algorithm for assigning myocardial fiber orientations.
 Home-page: https://github.com/finsberg/ldrb
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: LGPL-3.0
 Keywords: cardiac modeling,fiber orientations
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 [![CI](https://github.com/finsberg/ldrb/actions/workflows/main.yml/badge.svg)](https://github.com/finsberg/ldrb/actions/workflows/main.yml)
```

### Comparing `ldrb-2023.3.0/README.md` & `ldrb-2023.3.1/README.md`

 * *Files identical despite different names*

### Comparing `ldrb-2023.3.0/ldrb/__init__.py` & `ldrb-2023.3.1/ldrb/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .ldrb import dolfin_ldrb
 from .ldrb import project_gradients
 from .ldrb import scalar_laplacians
 from .save import fiber_to_xdmf
 from .save import fun_to_xdmf
 from .utils import space_from_string
 
-__version__ = "2023.3.0"
+__version__ = "2023.3.1"
 __author__ = "Henrik Finsberg (henriknf@simula.no)"
 
 __all__ = [
     "save",
     "fun_to_xdmf",
     "fiber_to_xdmf",
     "ldrb",
```

### Comparing `ldrb-2023.3.0/ldrb/calculus.py` & `ldrb-2023.3.1/ldrb/calculus.py`

 * *Files identical despite different names*

### Comparing `ldrb-2023.3.0/ldrb/ldrb.py` & `ldrb-2023.3.1/ldrb/ldrb.py`

 * *Files 1% similar despite different names*

```diff
@@ -530,17 +530,14 @@
             gradient_cg = df.Function(V_cg)
             projector(gradient_cg, df.grad(scalar_solution))
             gradient = df.interpolate(gradient_cg, Vv)
 
             # Add gradient data
             data[case + "_gradient"] = gradient.vector().get_local()
 
-            df.File(f"{case}.pvd") << scalar_solution_int
-            df.File(f"{case}_grad.pvd") << gradient
-
         # Add scalar data
         if case != "apex":
             data[case + "_scalar"] = scalar_solution_int.vector().get_local()
 
     # Return data
     return data
```

### Comparing `ldrb-2023.3.0/ldrb/save.py` & `ldrb-2023.3.1/ldrb/save.py`

 * *Files identical despite different names*

### Comparing `ldrb-2023.3.0/ldrb/utils.py` & `ldrb-2023.3.1/ldrb/utils.py`

 * *Files identical despite different names*

### Comparing `ldrb-2023.3.0/ldrb.egg-info/PKG-INFO` & `ldrb-2023.3.1/ldrb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: ldrb
-Version: 2023.3.0
+Version: 2023.3.1
 Summary: Laplace-Dirichlet Rule-based algorithm for assigning myocardial fiber orientations.
 Home-page: https://github.com/finsberg/ldrb
 Author: Henrik Finsberg
 Author-email: henriknf@simula.no
 License: LGPL-3.0
 Keywords: cardiac modeling,fiber orientations
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 [![CI](https://github.com/finsberg/ldrb/actions/workflows/main.yml/badge.svg)](https://github.com/finsberg/ldrb/actions/workflows/main.yml)
```

### Comparing `ldrb-2023.3.0/setup.cfg` & `ldrb-2023.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -3,28 +3,28 @@
 description = Laplace-Dirichlet Rule-based algorithm for assigning myocardial fiber orientations.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/finsberg/ldrb
 author = Henrik Finsberg
 author_email = henriknf@simula.no
 license = LGPL-3.0
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 keywords = cardiac modeling, fiber orientations
 
 [options]
 packages = find:
 install_requires = 
 	h5py
 	numba
 	numpy
-python_requires = >=3.7
+python_requires = >=3.8
 zip_safe = False
 
 [options.extras_require]
 dev = 
 	black
 	bump2version
 	flake8
```

### Comparing `ldrb-2023.3.0/tests/test_ldrb.py` & `ldrb-2023.3.1/tests/test_ldrb.py`

 * *Files identical despite different names*

### Comparing `ldrb-2023.3.0/tests/test_save.py` & `ldrb-2023.3.1/tests/test_save.py`

 * *Files identical despite different names*

