# Comparing `tmp/CyRK-0.6.0.tar.gz` & `tmp/CyRK-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CyRK-0.6.0.tar", last modified: Thu Jul 27 23:38:40 2023, max compression
+gzip compressed data, was "CyRK-0.6.1.tar", last modified: Wed Aug  2 01:17:01 2023, max compression
```

## Comparing `CyRK-0.6.0.tar` & `CyRK-0.6.1.tar`

### file list

```diff
@@ -1,44 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:40.707764 CyRK-0.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:40.691763 CyRK-0.6.0/CyRK/
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:40.695763 CyRK-0.6.0/CyRK/array/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1205683 2023-07-27 23:38:35.000000 CyRK-0.6.0/CyRK/array/interp.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/array/interp.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    14844 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/array/interp.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:40.707764 CyRK-0.6.0/CyRK/cy/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/cy/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/cy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/cy/__init__.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1899465 2023-07-27 23:38:36.000000 CyRK-0.6.0/CyRK/cy/cyrk.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    36012 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/cy/cyrk.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1735523 2023-07-27 23:38:38.000000 CyRK-0.6.0/CyRK/cy/cysolver.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/cy/cysolver.pxd
--rw-r--r--   0 runner    (1001) docker     (123)    40668 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/cy/cysolver.pyx
--rw-r--r--   0 runner    (1001) docker     (123)  1996591 2023-07-27 23:38:39.000000 CyRK-0.6.0/CyRK/cy/cysolvertest.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/cy/cysolvertest.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:40.707764 CyRK-0.6.0/CyRK/nb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/nb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/nb/dop_coefficients.py
--rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/nb/nbrk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:40.707764 CyRK-0.6.0/CyRK/rk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/rk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   232685 2023-07-27 23:38:39.000000 CyRK-0.6.0/CyRK/rk/rk.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/rk/rk.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-07-27 23:38:19.000000 CyRK-0.6.0/CyRK/rk/rk.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-27 23:38:40.691763 CyRK-0.6.0/CyRK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-07-27 23:38:40.000000 CyRK-0.6.0/CyRK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-27 23:38:40.000000 CyRK-0.6.0/CyRK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-27 23:38:40.000000 CyRK-0.6.0/CyRK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-27 23:38:40.000000 CyRK-0.6.0/CyRK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-27 23:38:40.000000 CyRK-0.6.0/CyRK.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-07-27 23:38:19.000000 CyRK-0.6.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-27 23:38:19.000000 CyRK-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    34969 2023-07-27 23:38:40.707764 CyRK-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-07-27 23:38:19.000000 CyRK-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-07-27 23:38:19.000000 CyRK-0.6.0/_build_cyrk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-07-27 23:38:19.000000 CyRK-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-27 23:38:40.707764 CyRK-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-07-27 23:38:19.000000 CyRK-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:17:01.169325 CyRK-0.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:17:01.161325 CyRK-0.6.1/CyRK/
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:17:01.161325 CyRK-0.6.1/CyRK/array/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/array/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/array/__init__.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1277801 2023-08-02 01:16:56.000000 CyRK-0.6.1/CyRK/array/interp.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/array/interp.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    23579 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/array/interp.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:17:01.169325 CyRK-0.6.1/CyRK/cy/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/cy/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/cy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/cy/__init__.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1901798 2023-08-02 01:16:58.000000 CyRK-0.6.1/CyRK/cy/cyrk.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    36012 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/cy/cyrk.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  1743673 2023-08-02 01:16:59.000000 CyRK-0.6.1/CyRK/cy/cysolver.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/cy/cysolver.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    40668 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/cy/cysolver.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)  2000388 2023-08-02 01:17:00.000000 CyRK-0.6.1/CyRK/cy/cysolvertest.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/cy/cysolvertest.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:17:01.169325 CyRK-0.6.1/CyRK/nb/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/nb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7329 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/nb/dop_coefficients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24589 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/nb/nbrk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:17:01.169325 CyRK-0.6.1/CyRK/rk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/rk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   232685 2023-08-02 01:17:00.000000 CyRK-0.6.1/CyRK/rk/rk.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1357 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/rk/rk.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-08-02 01:16:43.000000 CyRK-0.6.1/CyRK/rk/rk.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 01:17:01.161325 CyRK-0.6.1/CyRK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 2023-08-02 01:17:00.000000 CyRK-0.6.1/CyRK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-02 01:17:01.000000 CyRK-0.6.1/CyRK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 01:17:00.000000 CyRK-0.6.1/CyRK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 01:17:00.000000 CyRK-0.6.1/CyRK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-02 01:17:00.000000 CyRK-0.6.1/CyRK.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18625 2023-08-02 01:16:43.000000 CyRK-0.6.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-02 01:16:43.000000 CyRK-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 2023-08-02 01:17:01.169325 CyRK-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13930 2023-08-02 01:16:43.000000 CyRK-0.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-08-02 01:16:43.000000 CyRK-0.6.1/_build_cyrk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-08-02 01:16:43.000000 CyRK-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 01:17:01.169325 CyRK-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2003 2023-08-02 01:16:43.000000 CyRK-0.6.1/setup.py
```

### Comparing `CyRK-0.6.0/CyRK/_test.py` & `CyRK-0.6.1/CyRK/_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 
 def test_cysolver():
 
     from CyRK.cy.cysolvertest import CySolverTester
 
     # TODO: Currently CySolver only works with floats not complex
-    CySolverTesterInst = CySolverTester(time_span, np.asarray(initial_conds, dtype=np.float64))
+    CySolverTesterInst = CySolverTester(time_span, np.asarray(np.real(initial_conds), dtype=np.float64))
     CySolverTesterInst.solve()
 
     assert CySolverTesterInst.success
     assert type(CySolverTesterInst.solution_t) == np.ndarray
     assert type(CySolverTesterInst.solution_y) == np.ndarray
     assert CySolverTesterInst.solution_y.shape[0] == 2
```

### Comparing `CyRK-0.6.0/CyRK/array/interp.cpp` & `CyRK-0.6.1/CyRK/array/interp.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 /* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
             "CyRK/array",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "CyRK.array.interp",
         "sources": [
             "CyRK/array/interp.pyx"
         ]
     },
@@ -1560,177 +1560,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1763,49 +1763,113 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
+struct __pyx_ctuple_double__and_int;
+typedef struct __pyx_ctuple_double__and_int __pyx_ctuple_double__and_int;
+struct __pyx_opt_args_4CyRK_5array_6interp_interpj;
+struct __pyx_ctuple___dunderpyx_t_double_complex__and_int;
+typedef struct __pyx_ctuple___dunderpyx_t_double_complex__and_int __pyx_ctuple___dunderpyx_t_double_complex__and_int;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex;
+
+/* "CyRK/array/interp.pxd":5
+ * cdef unsigned int binary_search_with_guess(double key, double[:] array, unsigned int length, unsigned int guess) nogil
+ * 
+ * cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                             int provided_j = *) nogil
+ * 
+ */
+struct __pyx_ctuple_double__and_int {
+  double f0;
+  int f1;
+};
+struct __pyx_opt_args_4CyRK_5array_6interp_interpj {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":8
+ *                             int provided_j = *) nogil
+ * 
+ * cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
+ *                                             double complex[:] dependent_values, int provided_j = *) nogil
+ * 
+ */
+struct __pyx_ctuple___dunderpyx_t_double_complex__and_int {
+  __pyx_t_double_complex f0;
+  int f1;
+};
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":11
+ *                                             double complex[:] dependent_values, int provided_j = *) nogil
+ * 
+ * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                     int provided_j = *) nogil
+ * 
+ */
+struct __pyx_opt_args_4CyRK_5array_6interp_interp {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":14
+ *                     int provided_j = *) nogil
+ * 
+ * cpdef double complex interp_complex(double desired_x, double[:] x_domain, double complex[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                                     int provided_j = *) nogil
+ * 
+ */
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex {
+  int __pyx_n;
+  int provided_j;
+};
 
 /* "View.MemoryView":114
  * @cython.collection_type("sequence")
  * @cname("__pyx_array")
  * cdef class array:             # <<<<<<<<<<<<<<
  * 
  *     cdef:
@@ -2819,19 +2883,25 @@
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(PyObject *, int writable_flag);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_double(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_double(const char *itemp, PyObject *obj);
 
+/* ToPyCTupleUtility.proto */
+static PyObject* __pyx_convert__to_py___pyx_ctuple_double__and_int(__pyx_ctuple_double__and_int);
+
 /* ToPy.proto */
 #define __pyx_PyComplex_FromComplex(z)\
         PyComplex_FromDoubles((double)__Pyx_CREAL(z),\
                               (double)__Pyx_CIMAG(z))
 
+/* ToPyCTupleUtility.proto */
+static PyObject* __pyx_convert__to_py___pyx_ctuple___dunderpyx_t_double_complex__and_int(__pyx_ctuple___dunderpyx_t_double_complex__and_int);
+
 /* Arithmetic.proto */
 #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
     #define __Pyx_c_eq_float(a, b)   ((a)==(b))
     #define __Pyx_c_sum_float(a, b)  ((a)+(b))
     #define __Pyx_c_diff_float(a, b) ((a)-(b))
     #define __Pyx_c_prod_float(a, b) ((a)*(b))
     #define __Pyx_c_quot_float(a, b) ((a)/(b))
@@ -2894,26 +2964,26 @@
     __pyx_atomic_int_type *acquisition_count, PyThread_type_lock lock);
 #define __pyx_get_slice_count_pointer(memview) (&memview->acquisition_count)
 #define __PYX_INC_MEMVIEW(slice, have_gil) __Pyx_INC_MEMVIEW(slice, have_gil, __LINE__)
 #define __PYX_XCLEAR_MEMVIEW(slice, have_gil) __Pyx_XCLEAR_MEMVIEW(slice, have_gil, __LINE__)
 static CYTHON_INLINE void __Pyx_INC_MEMVIEW(__Pyx_memviewslice *, int, int);
 static CYTHON_INLINE void __Pyx_XCLEAR_MEMVIEW(__Pyx_memviewslice *, int, int);
 
-/* None.proto */
-#include <new>
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
-/* CIntFromPy.proto */
-static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value);
 
+/* None.proto */
+#include <new>
+
+/* CIntFromPy.proto */
+static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
+
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE char __Pyx_PyInt_As_char(PyObject *);
 
 /* FormatTypeName.proto */
@@ -2996,16 +3066,18 @@
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
 static unsigned int __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(double, __Pyx_memviewslice, unsigned int, unsigned int); /*proto*/
-static double __pyx_f_4CyRK_5array_6interp_interp(double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
-static __pyx_t_double_complex __pyx_f_4CyRK_5array_6interp_interp_complex(double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
+static __pyx_ctuple_double__and_int __pyx_f_4CyRK_5array_6interp_interpj(double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interpj *__pyx_optional_args); /*proto*/
+static __pyx_ctuple___dunderpyx_t_double_complex__and_int __pyx_f_4CyRK_5array_6interp_interp_complexj(double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj *__pyx_optional_args); /*proto*/
+static double __pyx_f_4CyRK_5array_6interp_interp(double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp *__pyx_optional_args); /*proto*/
+static __pyx_t_double_complex __pyx_f_4CyRK_5array_6interp_interp_complex(double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex *__pyx_optional_args); /*proto*/
 static void __pyx_f_4CyRK_5array_6interp_interp_array(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
 static void __pyx_f_4CyRK_5array_6interp_interp_complex_array(__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch); /*proto*/
 static int __pyx_array_allocate_buffer(struct __pyx_array_obj *); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
@@ -3066,15 +3138,15 @@
 static const char __pyx_k__2[] = ".";
 static const char __pyx_k__3[] = "*";
 static const char __pyx_k__6[] = "'";
 static const char __pyx_k__7[] = ")";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
-static const char __pyx_k__28[] = "?";
+static const char __pyx_k__30[] = "?";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_eps[] = "eps";
 static const char __pyx_k_got[] = " (got ";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_sys[] = "sys";
@@ -3112,14 +3184,15 @@
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_float64[] = "float64";
 static const char __pyx_k_fortran[] = "fortran";
+static const char __pyx_k_interpj[] = "interpj";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_Sequence[] = "Sequence";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_register[] = "register";
@@ -3129,14 +3202,15 @@
 static const char __pyx_k_desired_x[] = "desired_x";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
+static const char __pyx_k_provided_j[] = "provided_j";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_collections[] = "collections";
 static const char __pyx_k_initializing[] = "_initializing";
@@ -3150,14 +3224,15 @@
 static const char __pyx_k_AssertionError[] = "AssertionError";
 static const char __pyx_k_interp_complex[] = "interp_complex";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_collections_abc[] = "collections.abc";
 static const char __pyx_k_desired_x_array[] = "desired_x_array";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
+static const char __pyx_k_interp_complexj[] = "interp_complexj";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
 static const char __pyx_k_dependent_values[] = "dependent_values";
 static const char __pyx_k_CyRK_array_interp[] = "CyRK.array.interp";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
@@ -3233,18 +3308,20 @@
 static PyObject *__pyx_memoryview___pyx_pf_15View_dot_MemoryView_10memoryview_22copy_fortran(struct __pyx_memoryview_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryview___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryview_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryview_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static void __pyx_memoryviewslice___pyx_pf_15View_dot_MemoryView_16_memoryviewslice___dealloc__(struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice___reduce_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf___pyx_memoryviewslice_2__setstate_cython__(CYTHON_UNUSED struct __pyx_memoryviewslice_obj *__pyx_v_self, CYTHON_UNUSED PyObject *__pyx_v___pyx_state); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView___pyx_unpickle_Enum(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_4CyRK_5array_6interp_interp(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values); /* proto */
-static PyObject *__pyx_pf_4CyRK_5array_6interp_2interp_complex(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values); /* proto */
-static PyObject *__pyx_pf_4CyRK_5array_6interp_4interp_array(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array); /* proto */
-static PyObject *__pyx_pf_4CyRK_5array_6interp_6interp_complex_array(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array); /* proto */
+static PyObject *__pyx_pf_4CyRK_5array_6interp_interpj(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, int __pyx_v_provided_j); /* proto */
+static PyObject *__pyx_pf_4CyRK_5array_6interp_2interp_complexj(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, int __pyx_v_provided_j); /* proto */
+static PyObject *__pyx_pf_4CyRK_5array_6interp_4interp(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, int __pyx_v_provided_j); /* proto */
+static PyObject *__pyx_pf_4CyRK_5array_6interp_6interp_complex(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, int __pyx_v_provided_j); /* proto */
+static PyObject *__pyx_pf_4CyRK_5array_6interp_8interp_array(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array); /* proto */
+static PyObject *__pyx_pf_4CyRK_5array_6interp_10interp_complex_array(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array); /* proto */
 static PyObject *__pyx_tp_new_array(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 /* #### Code section: late_includes ### */
 /* #### Code section: module_state ### */
 typedef struct {
@@ -3357,16 +3434,16 @@
   PyObject *__pyx_n_s_Sequence;
   PyObject *__pyx_kp_s_Step_may_not_be_zero_axis_d;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_View_MemoryView;
   PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_n_s__28;
   PyObject *__pyx_n_s__3;
+  PyObject *__pyx_n_s__30;
   PyObject *__pyx_kp_u__6;
   PyObject *__pyx_kp_u__7;
   PyObject *__pyx_n_s_abc;
   PyObject *__pyx_n_s_allocate_buffer;
   PyObject *__pyx_kp_u_and;
   PyObject *__pyx_n_s_asyncio_coroutines;
   PyObject *__pyx_n_s_base;
@@ -3407,14 +3484,16 @@
   PyObject *__pyx_n_s_import;
   PyObject *__pyx_n_s_index;
   PyObject *__pyx_n_s_initializing;
   PyObject *__pyx_n_s_interp;
   PyObject *__pyx_n_s_interp_array;
   PyObject *__pyx_n_s_interp_complex;
   PyObject *__pyx_n_s_interp_complex_array;
+  PyObject *__pyx_n_s_interp_complexj;
+  PyObject *__pyx_n_s_interpj;
   PyObject *__pyx_n_s_is_coroutine;
   PyObject *__pyx_kp_u_isenabled;
   PyObject *__pyx_n_s_itemsize;
   PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
   PyObject *__pyx_n_s_main;
   PyObject *__pyx_n_s_memview;
   PyObject *__pyx_n_s_mode;
@@ -3426,14 +3505,15 @@
   PyObject *__pyx_n_s_np;
   PyObject *__pyx_n_s_numpy;
   PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
   PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
   PyObject *__pyx_n_s_obj;
   PyObject *__pyx_n_s_pack;
   PyObject *__pyx_n_s_pickle;
+  PyObject *__pyx_n_s_provided_j;
   PyObject *__pyx_n_s_pyx_PickleError;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_Enum;
   PyObject *__pyx_n_s_pyx_vtable;
@@ -3482,20 +3562,22 @@
   PyObject *__pyx_tuple__15;
   PyObject *__pyx_tuple__16;
   PyObject *__pyx_tuple__17;
   PyObject *__pyx_tuple__18;
   PyObject *__pyx_tuple__19;
   PyObject *__pyx_tuple__20;
   PyObject *__pyx_tuple__22;
-  PyObject *__pyx_tuple__25;
+  PyObject *__pyx_tuple__27;
   PyObject *__pyx_codeobj__21;
   PyObject *__pyx_codeobj__23;
   PyObject *__pyx_codeobj__24;
+  PyObject *__pyx_codeobj__25;
   PyObject *__pyx_codeobj__26;
-  PyObject *__pyx_codeobj__27;
+  PyObject *__pyx_codeobj__28;
+  PyObject *__pyx_codeobj__29;
 } __pyx_mstate;
 
 #if CYTHON_USE_MODULE_STATE
 #ifdef __cplusplus
 namespace {
   extern struct PyModuleDef __pyx_moduledef;
 } /* anonymous namespace */
@@ -3589,16 +3671,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_Sequence);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_View_MemoryView);
   Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_n_s__28);
   Py_CLEAR(clear_module_state->__pyx_n_s__3);
+  Py_CLEAR(clear_module_state->__pyx_n_s__30);
   Py_CLEAR(clear_module_state->__pyx_kp_u__6);
   Py_CLEAR(clear_module_state->__pyx_kp_u__7);
   Py_CLEAR(clear_module_state->__pyx_n_s_abc);
   Py_CLEAR(clear_module_state->__pyx_n_s_allocate_buffer);
   Py_CLEAR(clear_module_state->__pyx_kp_u_and);
   Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
   Py_CLEAR(clear_module_state->__pyx_n_s_base);
@@ -3639,14 +3721,16 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_import);
   Py_CLEAR(clear_module_state->__pyx_n_s_index);
   Py_CLEAR(clear_module_state->__pyx_n_s_initializing);
   Py_CLEAR(clear_module_state->__pyx_n_s_interp);
   Py_CLEAR(clear_module_state->__pyx_n_s_interp_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_interp_complex);
   Py_CLEAR(clear_module_state->__pyx_n_s_interp_complex_array);
+  Py_CLEAR(clear_module_state->__pyx_n_s_interp_complexj);
+  Py_CLEAR(clear_module_state->__pyx_n_s_interpj);
   Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
   Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
   Py_CLEAR(clear_module_state->__pyx_n_s_itemsize);
   Py_CLEAR(clear_module_state->__pyx_kp_s_itemsize_0_for_cython_array);
   Py_CLEAR(clear_module_state->__pyx_n_s_main);
   Py_CLEAR(clear_module_state->__pyx_n_s_memview);
   Py_CLEAR(clear_module_state->__pyx_n_s_mode);
@@ -3658,14 +3742,15 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_np);
   Py_CLEAR(clear_module_state->__pyx_n_s_numpy);
   Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
   Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj);
   Py_CLEAR(clear_module_state->__pyx_n_s_pack);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
+  Py_CLEAR(clear_module_state->__pyx_n_s_provided_j);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_Enum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
@@ -3714,20 +3799,22 @@
   Py_CLEAR(clear_module_state->__pyx_tuple__15);
   Py_CLEAR(clear_module_state->__pyx_tuple__16);
   Py_CLEAR(clear_module_state->__pyx_tuple__17);
   Py_CLEAR(clear_module_state->__pyx_tuple__18);
   Py_CLEAR(clear_module_state->__pyx_tuple__19);
   Py_CLEAR(clear_module_state->__pyx_tuple__20);
   Py_CLEAR(clear_module_state->__pyx_tuple__22);
-  Py_CLEAR(clear_module_state->__pyx_tuple__25);
+  Py_CLEAR(clear_module_state->__pyx_tuple__27);
   Py_CLEAR(clear_module_state->__pyx_codeobj__21);
   Py_CLEAR(clear_module_state->__pyx_codeobj__23);
   Py_CLEAR(clear_module_state->__pyx_codeobj__24);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__25);
   Py_CLEAR(clear_module_state->__pyx_codeobj__26);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__27);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__28);
+  Py_CLEAR(clear_module_state->__pyx_codeobj__29);
   return 0;
 }
 #endif
 /* #### Code section: module_state_traverse ### */
 #if CYTHON_USE_MODULE_STATE
 static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
   __pyx_mstate *traverse_module_state = __pyx_mstate(m);
@@ -3799,16 +3886,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_Sequence);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_View_MemoryView);
   Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_n_s__28);
   Py_VISIT(traverse_module_state->__pyx_n_s__3);
+  Py_VISIT(traverse_module_state->__pyx_n_s__30);
   Py_VISIT(traverse_module_state->__pyx_kp_u__6);
   Py_VISIT(traverse_module_state->__pyx_kp_u__7);
   Py_VISIT(traverse_module_state->__pyx_n_s_abc);
   Py_VISIT(traverse_module_state->__pyx_n_s_allocate_buffer);
   Py_VISIT(traverse_module_state->__pyx_kp_u_and);
   Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
   Py_VISIT(traverse_module_state->__pyx_n_s_base);
@@ -3849,14 +3936,16 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_import);
   Py_VISIT(traverse_module_state->__pyx_n_s_index);
   Py_VISIT(traverse_module_state->__pyx_n_s_initializing);
   Py_VISIT(traverse_module_state->__pyx_n_s_interp);
   Py_VISIT(traverse_module_state->__pyx_n_s_interp_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_interp_complex);
   Py_VISIT(traverse_module_state->__pyx_n_s_interp_complex_array);
+  Py_VISIT(traverse_module_state->__pyx_n_s_interp_complexj);
+  Py_VISIT(traverse_module_state->__pyx_n_s_interpj);
   Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
   Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
   Py_VISIT(traverse_module_state->__pyx_n_s_itemsize);
   Py_VISIT(traverse_module_state->__pyx_kp_s_itemsize_0_for_cython_array);
   Py_VISIT(traverse_module_state->__pyx_n_s_main);
   Py_VISIT(traverse_module_state->__pyx_n_s_memview);
   Py_VISIT(traverse_module_state->__pyx_n_s_mode);
@@ -3868,14 +3957,15 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_np);
   Py_VISIT(traverse_module_state->__pyx_n_s_numpy);
   Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_multiarray_failed_to);
   Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj);
   Py_VISIT(traverse_module_state->__pyx_n_s_pack);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
+  Py_VISIT(traverse_module_state->__pyx_n_s_provided_j);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_Enum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
@@ -3924,20 +4014,22 @@
   Py_VISIT(traverse_module_state->__pyx_tuple__15);
   Py_VISIT(traverse_module_state->__pyx_tuple__16);
   Py_VISIT(traverse_module_state->__pyx_tuple__17);
   Py_VISIT(traverse_module_state->__pyx_tuple__18);
   Py_VISIT(traverse_module_state->__pyx_tuple__19);
   Py_VISIT(traverse_module_state->__pyx_tuple__20);
   Py_VISIT(traverse_module_state->__pyx_tuple__22);
-  Py_VISIT(traverse_module_state->__pyx_tuple__25);
+  Py_VISIT(traverse_module_state->__pyx_tuple__27);
   Py_VISIT(traverse_module_state->__pyx_codeobj__21);
   Py_VISIT(traverse_module_state->__pyx_codeobj__23);
   Py_VISIT(traverse_module_state->__pyx_codeobj__24);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__25);
   Py_VISIT(traverse_module_state->__pyx_codeobj__26);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__27);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__28);
+  Py_VISIT(traverse_module_state->__pyx_codeobj__29);
   return 0;
 }
 #endif
 /* #### Code section: module_state_defines ### */
 #define __pyx_d __pyx_mstate_global->__pyx_d
 #define __pyx_b __pyx_mstate_global->__pyx_b
 #define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
@@ -4047,16 +4139,16 @@
 #define __pyx_n_s_Sequence __pyx_mstate_global->__pyx_n_s_Sequence
 #define __pyx_kp_s_Step_may_not_be_zero_axis_d __pyx_mstate_global->__pyx_kp_s_Step_may_not_be_zero_axis_d
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_kp_s_Unable_to_convert_item_to_object __pyx_mstate_global->__pyx_kp_s_Unable_to_convert_item_to_object
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_View_MemoryView __pyx_mstate_global->__pyx_n_s_View_MemoryView
 #define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_n_s__28 __pyx_mstate_global->__pyx_n_s__28
 #define __pyx_n_s__3 __pyx_mstate_global->__pyx_n_s__3
+#define __pyx_n_s__30 __pyx_mstate_global->__pyx_n_s__30
 #define __pyx_kp_u__6 __pyx_mstate_global->__pyx_kp_u__6
 #define __pyx_kp_u__7 __pyx_mstate_global->__pyx_kp_u__7
 #define __pyx_n_s_abc __pyx_mstate_global->__pyx_n_s_abc
 #define __pyx_n_s_allocate_buffer __pyx_mstate_global->__pyx_n_s_allocate_buffer
 #define __pyx_kp_u_and __pyx_mstate_global->__pyx_kp_u_and
 #define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
 #define __pyx_n_s_base __pyx_mstate_global->__pyx_n_s_base
@@ -4097,14 +4189,16 @@
 #define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
 #define __pyx_n_s_index __pyx_mstate_global->__pyx_n_s_index
 #define __pyx_n_s_initializing __pyx_mstate_global->__pyx_n_s_initializing
 #define __pyx_n_s_interp __pyx_mstate_global->__pyx_n_s_interp
 #define __pyx_n_s_interp_array __pyx_mstate_global->__pyx_n_s_interp_array
 #define __pyx_n_s_interp_complex __pyx_mstate_global->__pyx_n_s_interp_complex
 #define __pyx_n_s_interp_complex_array __pyx_mstate_global->__pyx_n_s_interp_complex_array
+#define __pyx_n_s_interp_complexj __pyx_mstate_global->__pyx_n_s_interp_complexj
+#define __pyx_n_s_interpj __pyx_mstate_global->__pyx_n_s_interpj
 #define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
 #define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
 #define __pyx_n_s_itemsize __pyx_mstate_global->__pyx_n_s_itemsize
 #define __pyx_kp_s_itemsize_0_for_cython_array __pyx_mstate_global->__pyx_kp_s_itemsize_0_for_cython_array
 #define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
 #define __pyx_n_s_memview __pyx_mstate_global->__pyx_n_s_memview
 #define __pyx_n_s_mode __pyx_mstate_global->__pyx_n_s_mode
@@ -4116,14 +4210,15 @@
 #define __pyx_n_s_np __pyx_mstate_global->__pyx_n_s_np
 #define __pyx_n_s_numpy __pyx_mstate_global->__pyx_n_s_numpy
 #define __pyx_kp_u_numpy_core_multiarray_failed_to __pyx_mstate_global->__pyx_kp_u_numpy_core_multiarray_failed_to
 #define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
 #define __pyx_n_s_obj __pyx_mstate_global->__pyx_n_s_obj
 #define __pyx_n_s_pack __pyx_mstate_global->__pyx_n_s_pack
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
+#define __pyx_n_s_provided_j __pyx_mstate_global->__pyx_n_s_provided_j
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_Enum __pyx_mstate_global->__pyx_n_s_pyx_unpickle_Enum
 #define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
@@ -4172,20 +4267,22 @@
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__16 __pyx_mstate_global->__pyx_tuple__16
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_tuple__18 __pyx_mstate_global->__pyx_tuple__18
 #define __pyx_tuple__19 __pyx_mstate_global->__pyx_tuple__19
 #define __pyx_tuple__20 __pyx_mstate_global->__pyx_tuple__20
 #define __pyx_tuple__22 __pyx_mstate_global->__pyx_tuple__22
-#define __pyx_tuple__25 __pyx_mstate_global->__pyx_tuple__25
+#define __pyx_tuple__27 __pyx_mstate_global->__pyx_tuple__27
 #define __pyx_codeobj__21 __pyx_mstate_global->__pyx_codeobj__21
 #define __pyx_codeobj__23 __pyx_mstate_global->__pyx_codeobj__23
 #define __pyx_codeobj__24 __pyx_mstate_global->__pyx_codeobj__24
+#define __pyx_codeobj__25 __pyx_mstate_global->__pyx_codeobj__25
 #define __pyx_codeobj__26 __pyx_mstate_global->__pyx_codeobj__26
-#define __pyx_codeobj__27 __pyx_mstate_global->__pyx_codeobj__27
+#define __pyx_codeobj__28 __pyx_mstate_global->__pyx_codeobj__28
+#define __pyx_codeobj__29 __pyx_mstate_global->__pyx_codeobj__29
 /* #### Code section: module_code ### */
 
 /* "View.MemoryView":131
  *         cdef bint dtype_is_object
  * 
  *     def __cinit__(array self, tuple shape, Py_ssize_t itemsize, format not None,             # <<<<<<<<<<<<<<
  *                   mode="c", bint allocate_buffer=True):
@@ -17486,261 +17583,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -17749,29 +17846,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -17782,15 +17879,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -17799,29 +17896,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -17832,15 +17929,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -17849,29 +17946,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -17882,15 +17979,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -17899,29 +17996,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -17932,15 +18029,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -17949,29 +18046,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -17982,89 +18079,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18072,33 +18169,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18106,96 +18203,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18211,15 +18308,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18227,68 +18324,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18296,15 +18393,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18319,15 +18416,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18343,15 +18440,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18359,68 +18456,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18428,15 +18525,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18451,15 +18548,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18475,15 +18572,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18491,68 +18588,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18560,15 +18657,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18583,176 +18680,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19212,358 +19309,1807 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "CyRK/array/interp.pyx":96
  * 
  * 
- * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values) nogil:             # <<<<<<<<<<<<<<
+ * cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                             int provided_j = -1) nogil:
+ *     """ Interpolation function for floats. This function will return the index that it found during interpolation.
+ */
+
+static PyObject *__pyx_pw_4CyRK_5array_6interp_1interpj(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static __pyx_ctuple_double__and_int __pyx_f_4CyRK_5array_6interp_interpj(double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interpj *__pyx_optional_args) {
+  int __pyx_v_provided_j = ((int)-1);
+  unsigned int __pyx_v_lenx;
+  double __pyx_v_left_value;
+  double __pyx_v_right_value;
+  unsigned int __pyx_v_j;
+  double __pyx_v_slope;
+  double __pyx_v_result;
+  double __pyx_v_fp_at_j;
+  double __pyx_v_xp_at_j;
+  double __pyx_v_fp_at_jp1;
+  double __pyx_v_xp_at_jp1;
+  int __pyx_v_j_out;
+  __pyx_ctuple_double__and_int __pyx_r;
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  int __pyx_t_3;
+  unsigned int __pyx_t_4;
+  size_t __pyx_t_5;
+  int __pyx_t_6;
+  __pyx_ctuple_double__and_int __pyx_t_7;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
+  if (__pyx_optional_args) {
+    if (__pyx_optional_args->__pyx_n > 0) {
+      __pyx_v_provided_j = __pyx_optional_args->provided_j;
+    }
+  }
+
+  /* "CyRK/array/interp.pyx":128
+ * 
+ *     cdef unsigned int lenx
+ *     lenx = len(x_domain)             # <<<<<<<<<<<<<<
+ *     # TODO: Needs to be at least 3 item long array. Add exception here?
+ * 
+ */
+  __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_x_domain); 
+  __pyx_v_lenx = __pyx_t_1;
+
+  /* "CyRK/array/interp.pyx":132
+ * 
+ *     cdef double left_value
+ *     left_value = dependent_values[0]             # <<<<<<<<<<<<<<
+ *     cdef double right_value
+ *     right_value = dependent_values[lenx - 1]
+ */
+  __pyx_t_2 = 0;
+  __pyx_v_left_value = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
+
+  /* "CyRK/array/interp.pyx":134
+ *     left_value = dependent_values[0]
+ *     cdef double right_value
+ *     right_value = dependent_values[lenx - 1]             # <<<<<<<<<<<<<<
+ * 
+ *     # Binary Search with Guess
+ */
+  __pyx_t_2 = (__pyx_v_lenx - 1);
+  __pyx_v_right_value = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
+
+  /* "CyRK/array/interp.pyx":138
+ *     # Binary Search with Guess
+ *     cdef unsigned int j
+ *     j = 0             # <<<<<<<<<<<<<<
+ *     cdef double slope
+ * 
+ */
+  __pyx_v_j = 0;
+
+  /* "CyRK/array/interp.pyx":148
+ * 
+ *     # Perform binary search with guess
+ *     if provided_j == -1:             # <<<<<<<<<<<<<<
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ */
+  __pyx_t_3 = (__pyx_v_provided_j == -1L);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":150
+ *     if provided_j == -1:
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     elif provided_j < -1:
+ *         # Error
+ */
+    __pyx_t_4 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_4 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 150, __pyx_L1_error)
+    __pyx_v_j = __pyx_t_4;
+
+    /* "CyRK/array/interp.pyx":148
+ * 
+ *     # Perform binary search with guess
+ *     if provided_j == -1:             # <<<<<<<<<<<<<<
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ */
+    goto __pyx_L3;
+  }
+
+  /* "CyRK/array/interp.pyx":151
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ *     elif provided_j < -1:             # <<<<<<<<<<<<<<
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ */
+  __pyx_t_3 = (__pyx_v_provided_j < -1L);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":154
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     else:
+ *         # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+ */
+    __pyx_t_4 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_4 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 154, __pyx_L1_error)
+    __pyx_v_j = __pyx_t_4;
+
+    /* "CyRK/array/interp.pyx":151
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ *     elif provided_j < -1:             # <<<<<<<<<<<<<<
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ */
+    goto __pyx_L3;
+  }
+
+  /* "CyRK/array/interp.pyx":157
+ *     else:
+ *         # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+ *         j = <unsigned int>provided_j             # <<<<<<<<<<<<<<
+ * 
+ *     cdef int j_out
+ */
+  /*else*/ {
+    __pyx_v_j = ((unsigned int)__pyx_v_provided_j);
+  }
+  __pyx_L3:;
+
+  /* "CyRK/array/interp.pyx":160
+ * 
+ *     cdef int j_out
+ *     j_out = <int>j             # <<<<<<<<<<<<<<
+ * 
+ *     if j == 0:
+ */
+  __pyx_v_j_out = ((int)__pyx_v_j);
+
+  /* "CyRK/array/interp.pyx":162
+ *     j_out = <int>j
+ * 
+ *     if j == 0:             # <<<<<<<<<<<<<<
+ *         result = left_value
+ *     elif j == lenx:
+ */
+  __pyx_t_3 = (__pyx_v_j == 0);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":163
+ * 
+ *     if j == 0:
+ *         result = left_value             # <<<<<<<<<<<<<<
+ *     elif j == lenx:
+ *         result = right_value
+ */
+    __pyx_v_result = __pyx_v_left_value;
+
+    /* "CyRK/array/interp.pyx":162
+ *     j_out = <int>j
+ * 
+ *     if j == 0:             # <<<<<<<<<<<<<<
+ *         result = left_value
+ *     elif j == lenx:
+ */
+    goto __pyx_L4;
+  }
+
+  /* "CyRK/array/interp.pyx":164
+ *     if j == 0:
+ *         result = left_value
+ *     elif j == lenx:             # <<<<<<<<<<<<<<
+ *         result = right_value
+ *     else:
+ */
+  __pyx_t_3 = (__pyx_v_j == __pyx_v_lenx);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":165
+ *         result = left_value
+ *     elif j == lenx:
+ *         result = right_value             # <<<<<<<<<<<<<<
+ *     else:
+ *         fp_at_j = dependent_values[j]
+ */
+    __pyx_v_result = __pyx_v_right_value;
+
+    /* "CyRK/array/interp.pyx":164
+ *     if j == 0:
+ *         result = left_value
+ *     elif j == lenx:             # <<<<<<<<<<<<<<
+ *         result = right_value
+ *     else:
+ */
+    goto __pyx_L4;
+  }
+
+  /* "CyRK/array/interp.pyx":167
+ *         result = right_value
+ *     else:
+ *         fp_at_j = dependent_values[j]             # <<<<<<<<<<<<<<
+ *         xp_at_j = x_domain[j]
+ *         if j == lenx - 1:
+ */
+  /*else*/ {
+    __pyx_t_5 = __pyx_v_j;
+    __pyx_v_fp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_5 * __pyx_v_dependent_values.strides[0]) )));
+
+    /* "CyRK/array/interp.pyx":168
+ *     else:
+ *         fp_at_j = dependent_values[j]
+ *         xp_at_j = x_domain[j]             # <<<<<<<<<<<<<<
+ *         if j == lenx - 1:
+ *             result = fp_at_j
+ */
+    __pyx_t_5 = __pyx_v_j;
+    __pyx_v_xp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_5 * __pyx_v_x_domain.strides[0]) )));
+
+    /* "CyRK/array/interp.pyx":169
+ *         fp_at_j = dependent_values[j]
+ *         xp_at_j = x_domain[j]
+ *         if j == lenx - 1:             # <<<<<<<<<<<<<<
+ *             result = fp_at_j
+ *         elif xp_at_j == desired_x:
+ */
+    __pyx_t_3 = (__pyx_v_j == (__pyx_v_lenx - 1));
+    if (__pyx_t_3) {
+
+      /* "CyRK/array/interp.pyx":170
+ *         xp_at_j = x_domain[j]
+ *         if j == lenx - 1:
+ *             result = fp_at_j             # <<<<<<<<<<<<<<
+ *         elif xp_at_j == desired_x:
+ *             result = fp_at_j
+ */
+      __pyx_v_result = __pyx_v_fp_at_j;
+
+      /* "CyRK/array/interp.pyx":169
+ *         fp_at_j = dependent_values[j]
+ *         xp_at_j = x_domain[j]
+ *         if j == lenx - 1:             # <<<<<<<<<<<<<<
+ *             result = fp_at_j
+ *         elif xp_at_j == desired_x:
+ */
+      goto __pyx_L5;
+    }
+
+    /* "CyRK/array/interp.pyx":171
+ *         if j == lenx - 1:
+ *             result = fp_at_j
+ *         elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
+ *             result = fp_at_j
+ *         else:
+ */
+    __pyx_t_3 = (__pyx_v_xp_at_j == __pyx_v_desired_x);
+    if (__pyx_t_3) {
+
+      /* "CyRK/array/interp.pyx":172
+ *             result = fp_at_j
+ *         elif xp_at_j == desired_x:
+ *             result = fp_at_j             # <<<<<<<<<<<<<<
+ *         else:
+ *             fp_at_jp1 = dependent_values[j + 1]
+ */
+      __pyx_v_result = __pyx_v_fp_at_j;
+
+      /* "CyRK/array/interp.pyx":171
+ *         if j == lenx - 1:
+ *             result = fp_at_j
+ *         elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
+ *             result = fp_at_j
+ *         else:
+ */
+      goto __pyx_L5;
+    }
+
+    /* "CyRK/array/interp.pyx":174
+ *             result = fp_at_j
+ *         else:
+ *             fp_at_jp1 = dependent_values[j + 1]             # <<<<<<<<<<<<<<
+ *             xp_at_jp1 = x_domain[j + 1]
+ *             slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)
+ */
+    /*else*/ {
+      __pyx_t_2 = (__pyx_v_j + 1);
+      __pyx_v_fp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
+
+      /* "CyRK/array/interp.pyx":175
+ *         else:
+ *             fp_at_jp1 = dependent_values[j + 1]
+ *             xp_at_jp1 = x_domain[j + 1]             # <<<<<<<<<<<<<<
+ *             slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)
+ * 
+ */
+      __pyx_t_2 = (__pyx_v_j + 1);
+      __pyx_v_xp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_2 * __pyx_v_x_domain.strides[0]) )));
+
+      /* "CyRK/array/interp.pyx":176
+ *             fp_at_jp1 = dependent_values[j + 1]
+ *             xp_at_jp1 = x_domain[j + 1]
+ *             slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)             # <<<<<<<<<<<<<<
+ * 
+ *             # If we get nan in one direction, try the other
+ */
+      __pyx_v_slope = ((__pyx_v_fp_at_jp1 - __pyx_v_fp_at_j) / (__pyx_v_xp_at_jp1 - __pyx_v_xp_at_j));
+
+      /* "CyRK/array/interp.pyx":179
+ * 
+ *             # If we get nan in one direction, try the other
+ *             result = slope * (desired_x - xp_at_j) + fp_at_j             # <<<<<<<<<<<<<<
+ *             if isnan(result):
+ *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
+ */
+      __pyx_v_result = ((__pyx_v_slope * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j);
+
+      /* "CyRK/array/interp.pyx":180
+ *             # If we get nan in one direction, try the other
+ *             result = slope * (desired_x - xp_at_j) + fp_at_j
+ *             if isnan(result):             # <<<<<<<<<<<<<<
+ *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
+ *                 if isnan(result) and (fp_at_jp1 == fp_at_j):
+ */
+      __pyx_t_3 = isnan(__pyx_v_result);
+      if (__pyx_t_3) {
+
+        /* "CyRK/array/interp.pyx":181
+ *             result = slope * (desired_x - xp_at_j) + fp_at_j
+ *             if isnan(result):
+ *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1             # <<<<<<<<<<<<<<
+ *                 if isnan(result) and (fp_at_jp1 == fp_at_j):
+ *                     result = fp_at_j
+ */
+        __pyx_v_result = ((__pyx_v_slope * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1);
+
+        /* "CyRK/array/interp.pyx":182
+ *             if isnan(result):
+ *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
+ *                 if isnan(result) and (fp_at_jp1 == fp_at_j):             # <<<<<<<<<<<<<<
+ *                     result = fp_at_j
+ * 
+ */
+        __pyx_t_6 = isnan(__pyx_v_result);
+        if (__pyx_t_6) {
+        } else {
+          __pyx_t_3 = __pyx_t_6;
+          goto __pyx_L8_bool_binop_done;
+        }
+        __pyx_t_6 = (__pyx_v_fp_at_jp1 == __pyx_v_fp_at_j);
+        __pyx_t_3 = __pyx_t_6;
+        __pyx_L8_bool_binop_done:;
+        if (__pyx_t_3) {
+
+          /* "CyRK/array/interp.pyx":183
+ *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
+ *                 if isnan(result) and (fp_at_jp1 == fp_at_j):
+ *                     result = fp_at_j             # <<<<<<<<<<<<<<
+ * 
+ *     return result, j_out
+ */
+          __pyx_v_result = __pyx_v_fp_at_j;
+
+          /* "CyRK/array/interp.pyx":182
+ *             if isnan(result):
+ *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
+ *                 if isnan(result) and (fp_at_jp1 == fp_at_j):             # <<<<<<<<<<<<<<
+ *                     result = fp_at_j
+ * 
+ */
+        }
+
+        /* "CyRK/array/interp.pyx":180
+ *             # If we get nan in one direction, try the other
+ *             result = slope * (desired_x - xp_at_j) + fp_at_j
+ *             if isnan(result):             # <<<<<<<<<<<<<<
+ *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
+ *                 if isnan(result) and (fp_at_jp1 == fp_at_j):
+ */
+      }
+    }
+    __pyx_L5:;
+  }
+  __pyx_L4:;
+
+  /* "CyRK/array/interp.pyx":185
+ *                     result = fp_at_j
+ * 
+ *     return result, j_out             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_7.f0 = __pyx_v_result;
+  __pyx_t_7.f1 = __pyx_v_j_out;
+  __pyx_r = __pyx_t_7;
+  goto __pyx_L0;
+
+  /* "CyRK/array/interp.pyx":96
+ * 
+ * 
+ * cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                             int provided_j = -1) nogil:
+ *     """ Interpolation function for floats. This function will return the index that it found during interpolation.
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
+  __Pyx_AddTraceback("CyRK.array.interp.interpj", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4CyRK_5array_6interp_1interpj(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_4CyRK_5array_6interp_interpj, " Interpolation function for floats. This function will return the index that it found during interpolation.\n\n    Provided a domain, `x_domain` and a dependent array `dependent_values` search domain for value closest to \n    `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local \n    slopes of `x_domain` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.\n\n    Based on `numpy`'s `interp` function.\n\n    Parameters\n    ----------\n    desired_x : float\n        Location where `dependent_variables` is desired.\n    x_domain : np.ndarray[float]\n        Domain to search for the correct location.\n    dependent_values : np.ndarray[float]\n        Dependent values that are to be returned after search and interpolation.\n    provided_j : int\n        Give a j index from a previous interpolation to improve performance.\n\n    Returns\n    -------\n    result : float\n        Desired value of `dependent_values`.\n    j_out : int\n        The index that was found during binary_search_with_guess which can be used by other interpolation functions \n        to improve performance.\n\n    ");
+static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_1interpj = {"interpj", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_1interpj, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_4CyRK_5array_6interp_interpj};
+static PyObject *__pyx_pw_4CyRK_5array_6interp_1interpj(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  double __pyx_v_desired_x;
+  __Pyx_memviewslice __pyx_v_x_domain = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_dependent_values = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_v_provided_j;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("interpj (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_desired_x,&__pyx_n_s_x_domain,&__pyx_n_s_dependent_values,&__pyx_n_s_provided_j,0};
+    PyObject* values[4] = {0,0,0,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_desired_x)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x_domain)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("interpj", 0, 3, 4, 1); __PYX_ERR(1, 96, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dependent_values)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("interpj", 0, 3, 4, 2); __PYX_ERR(1, 96, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_provided_j);
+          if (value) { values[3] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interpj") < 0)) __PYX_ERR(1, 96, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_desired_x = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_desired_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
+    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 96, __pyx_L3_error)
+    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 96, __pyx_L3_error)
+    if (values[3]) {
+      __pyx_v_provided_j = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_provided_j == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 97, __pyx_L3_error)
+    } else {
+      __pyx_v_provided_j = ((int)-1);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("interpj", 0, 3, 4, __pyx_nargs); __PYX_ERR(1, 96, __pyx_L3_error)
+  __pyx_L3_error:;
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
+  __Pyx_AddTraceback("CyRK.array.interp.interpj", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_4CyRK_5array_6interp_interpj(__pyx_self, __pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_provided_j);
+
+  /* function exit code */
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4CyRK_5array_6interp_interpj(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, int __pyx_v_provided_j) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __pyx_ctuple_double__and_int __pyx_t_1;
+  struct __pyx_opt_args_4CyRK_5array_6interp_interpj __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("interpj", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2.__pyx_n = 1;
+  __pyx_t_2.provided_j = __pyx_v_provided_j;
+  __pyx_t_1 = __pyx_f_4CyRK_5array_6interp_interpj(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, 0, &__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert__to_py___pyx_ctuple_double__and_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("CyRK.array.interp.interpj", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "CyRK/array/interp.pyx":188
+ * 
+ * 
+ * cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
+ *                                             double complex[:] dependent_values, int provided_j = -1) nogil:
+ *     """ Interpolation function for complex numbers.
+ */
+
+static PyObject *__pyx_pw_4CyRK_5array_6interp_3interp_complexj(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+static __pyx_ctuple___dunderpyx_t_double_complex__and_int __pyx_f_4CyRK_5array_6interp_interp_complexj(double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj *__pyx_optional_args) {
+  int __pyx_v_provided_j = ((int)-1);
+  unsigned int __pyx_v_lenx;
+  __pyx_t_double_complex __pyx_v_left_value;
+  __pyx_t_double_complex __pyx_v_right_value;
+  unsigned int __pyx_v_j;
+  double __pyx_v_slope_real;
+  double __pyx_v_slope_imag;
+  double __pyx_v_x_slope_inverse;
+  double __pyx_v_result_real;
+  double __pyx_v_result_imag;
+  __pyx_t_double_complex __pyx_v_fp_at_j;
+  double __pyx_v_fp_at_j_real;
+  double __pyx_v_fp_at_j_imag;
+  double __pyx_v_xp_at_j;
+  __pyx_t_double_complex __pyx_v_fp_at_jp1;
+  double __pyx_v_fp_at_jp1_real;
+  double __pyx_v_fp_at_jp1_imag;
+  double __pyx_v_xp_at_jp1;
+  int __pyx_v_j_out;
+  __pyx_t_double_complex __pyx_v_result;
+  __pyx_ctuple___dunderpyx_t_double_complex__and_int __pyx_r;
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  int __pyx_t_3;
+  unsigned int __pyx_t_4;
+  double __pyx_t_5;
+  size_t __pyx_t_6;
+  int __pyx_t_7;
+  __pyx_ctuple___dunderpyx_t_double_complex__and_int __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  #ifdef WITH_THREAD
+  PyGILState_STATE __pyx_gilstate_save;
+  #endif
+  if (__pyx_optional_args) {
+    if (__pyx_optional_args->__pyx_n > 0) {
+      __pyx_v_provided_j = __pyx_optional_args->provided_j;
+    }
+  }
+
+  /* "CyRK/array/interp.pyx":220
+ * 
+ *     cdef unsigned int lenx
+ *     lenx = len(x_domain)             # <<<<<<<<<<<<<<
+ *     # Note: Needs to be at least 3 item long array. Add exception here?
+ * 
+ */
+  __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_x_domain); 
+  __pyx_v_lenx = __pyx_t_1;
+
+  /* "CyRK/array/interp.pyx":224
+ * 
+ *     cdef double complex left_value
+ *     left_value = dependent_values[0]             # <<<<<<<<<<<<<<
+ *     cdef double complex right_value
+ *     right_value = dependent_values[lenx - 1]
+ */
+  __pyx_t_2 = 0;
+  __pyx_v_left_value = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
+
+  /* "CyRK/array/interp.pyx":226
+ *     left_value = dependent_values[0]
+ *     cdef double complex right_value
+ *     right_value = dependent_values[lenx - 1]             # <<<<<<<<<<<<<<
+ * 
+ *     # Binary Search with Guess
+ */
+  __pyx_t_2 = (__pyx_v_lenx - 1);
+  __pyx_v_right_value = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
+
+  /* "CyRK/array/interp.pyx":230
+ *     # Binary Search with Guess
+ *     cdef unsigned int j
+ *     j = 0             # <<<<<<<<<<<<<<
+ *     cdef double slope_real
+ *     cdef double slope_imag
+ */
+  __pyx_v_j = 0;
+
+  /* "CyRK/array/interp.pyx":247
+ * 
+ *     # Perform binary search with guess
+ *     if provided_j == -1:             # <<<<<<<<<<<<<<
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ */
+  __pyx_t_3 = (__pyx_v_provided_j == -1L);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":249
+ *     if provided_j == -1:
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     elif provided_j < -1:
+ *         # Error
+ */
+    __pyx_t_4 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_4 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 249, __pyx_L1_error)
+    __pyx_v_j = __pyx_t_4;
+
+    /* "CyRK/array/interp.pyx":247
+ * 
+ *     # Perform binary search with guess
+ *     if provided_j == -1:             # <<<<<<<<<<<<<<
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ */
+    goto __pyx_L3;
+  }
+
+  /* "CyRK/array/interp.pyx":250
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ *     elif provided_j < -1:             # <<<<<<<<<<<<<<
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ */
+  __pyx_t_3 = (__pyx_v_provided_j < -1L);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":253
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     else:
+ *         # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+ */
+    __pyx_t_4 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_4 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 253, __pyx_L1_error)
+    __pyx_v_j = __pyx_t_4;
+
+    /* "CyRK/array/interp.pyx":250
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ *     elif provided_j < -1:             # <<<<<<<<<<<<<<
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ */
+    goto __pyx_L3;
+  }
+
+  /* "CyRK/array/interp.pyx":256
+ *     else:
+ *         # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+ *         j = <unsigned int> provided_j             # <<<<<<<<<<<<<<
+ * 
+ *     cdef int j_out
+ */
+  /*else*/ {
+    __pyx_v_j = ((unsigned int)__pyx_v_provided_j);
+  }
+  __pyx_L3:;
+
+  /* "CyRK/array/interp.pyx":259
+ * 
+ *     cdef int j_out
+ *     j_out = <int> j             # <<<<<<<<<<<<<<
+ * 
+ *     if j == 0:
+ */
+  __pyx_v_j_out = ((int)__pyx_v_j);
+
+  /* "CyRK/array/interp.pyx":261
+ *     j_out = <int> j
+ * 
+ *     if j == 0:             # <<<<<<<<<<<<<<
+ *         result_real = left_value.real
+ *         result_imag = left_value.imag
+ */
+  __pyx_t_3 = (__pyx_v_j == 0);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":262
+ * 
+ *     if j == 0:
+ *         result_real = left_value.real             # <<<<<<<<<<<<<<
+ *         result_imag = left_value.imag
+ *     elif j == lenx:
+ */
+    __pyx_t_5 = __Pyx_CREAL(__pyx_v_left_value);
+    __pyx_v_result_real = __pyx_t_5;
+
+    /* "CyRK/array/interp.pyx":263
+ *     if j == 0:
+ *         result_real = left_value.real
+ *         result_imag = left_value.imag             # <<<<<<<<<<<<<<
+ *     elif j == lenx:
+ *         result_real = right_value.real
+ */
+    __pyx_t_5 = __Pyx_CIMAG(__pyx_v_left_value);
+    __pyx_v_result_imag = __pyx_t_5;
+
+    /* "CyRK/array/interp.pyx":261
+ *     j_out = <int> j
+ * 
+ *     if j == 0:             # <<<<<<<<<<<<<<
+ *         result_real = left_value.real
+ *         result_imag = left_value.imag
+ */
+    goto __pyx_L4;
+  }
+
+  /* "CyRK/array/interp.pyx":264
+ *         result_real = left_value.real
+ *         result_imag = left_value.imag
+ *     elif j == lenx:             # <<<<<<<<<<<<<<
+ *         result_real = right_value.real
+ *         result_imag = right_value.imag
+ */
+  __pyx_t_3 = (__pyx_v_j == __pyx_v_lenx);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":265
+ *         result_imag = left_value.imag
+ *     elif j == lenx:
+ *         result_real = right_value.real             # <<<<<<<<<<<<<<
+ *         result_imag = right_value.imag
+ *     else:
+ */
+    __pyx_t_5 = __Pyx_CREAL(__pyx_v_right_value);
+    __pyx_v_result_real = __pyx_t_5;
+
+    /* "CyRK/array/interp.pyx":266
+ *     elif j == lenx:
+ *         result_real = right_value.real
+ *         result_imag = right_value.imag             # <<<<<<<<<<<<<<
+ *     else:
+ *         fp_at_j = dependent_values[j]
+ */
+    __pyx_t_5 = __Pyx_CIMAG(__pyx_v_right_value);
+    __pyx_v_result_imag = __pyx_t_5;
+
+    /* "CyRK/array/interp.pyx":264
+ *         result_real = left_value.real
+ *         result_imag = left_value.imag
+ *     elif j == lenx:             # <<<<<<<<<<<<<<
+ *         result_real = right_value.real
+ *         result_imag = right_value.imag
+ */
+    goto __pyx_L4;
+  }
+
+  /* "CyRK/array/interp.pyx":268
+ *         result_imag = right_value.imag
+ *     else:
+ *         fp_at_j = dependent_values[j]             # <<<<<<<<<<<<<<
+ *         fp_at_j_real = fp_at_j.real
+ *         fp_at_j_imag = fp_at_j.imag
+ */
+  /*else*/ {
+    __pyx_t_6 = __pyx_v_j;
+    __pyx_v_fp_at_j = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_6 * __pyx_v_dependent_values.strides[0]) )));
+
+    /* "CyRK/array/interp.pyx":269
+ *     else:
+ *         fp_at_j = dependent_values[j]
+ *         fp_at_j_real = fp_at_j.real             # <<<<<<<<<<<<<<
+ *         fp_at_j_imag = fp_at_j.imag
+ *         xp_at_j = x_domain[j]
+ */
+    __pyx_t_5 = __Pyx_CREAL(__pyx_v_fp_at_j);
+    __pyx_v_fp_at_j_real = __pyx_t_5;
+
+    /* "CyRK/array/interp.pyx":270
+ *         fp_at_j = dependent_values[j]
+ *         fp_at_j_real = fp_at_j.real
+ *         fp_at_j_imag = fp_at_j.imag             # <<<<<<<<<<<<<<
+ *         xp_at_j = x_domain[j]
+ *         if j == lenx - 1:
+ */
+    __pyx_t_5 = __Pyx_CIMAG(__pyx_v_fp_at_j);
+    __pyx_v_fp_at_j_imag = __pyx_t_5;
+
+    /* "CyRK/array/interp.pyx":271
+ *         fp_at_j_real = fp_at_j.real
+ *         fp_at_j_imag = fp_at_j.imag
+ *         xp_at_j = x_domain[j]             # <<<<<<<<<<<<<<
+ *         if j == lenx - 1:
+ *             result_real = fp_at_j_real
+ */
+    __pyx_t_6 = __pyx_v_j;
+    __pyx_v_xp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_6 * __pyx_v_x_domain.strides[0]) )));
+
+    /* "CyRK/array/interp.pyx":272
+ *         fp_at_j_imag = fp_at_j.imag
+ *         xp_at_j = x_domain[j]
+ *         if j == lenx - 1:             # <<<<<<<<<<<<<<
+ *             result_real = fp_at_j_real
+ *             result_imag = fp_at_j_imag
+ */
+    __pyx_t_3 = (__pyx_v_j == (__pyx_v_lenx - 1));
+    if (__pyx_t_3) {
+
+      /* "CyRK/array/interp.pyx":273
+ *         xp_at_j = x_domain[j]
+ *         if j == lenx - 1:
+ *             result_real = fp_at_j_real             # <<<<<<<<<<<<<<
+ *             result_imag = fp_at_j_imag
+ *         elif xp_at_j == desired_x:
+ */
+      __pyx_v_result_real = __pyx_v_fp_at_j_real;
+
+      /* "CyRK/array/interp.pyx":274
+ *         if j == lenx - 1:
+ *             result_real = fp_at_j_real
+ *             result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
+ *         elif xp_at_j == desired_x:
+ *             result_real = fp_at_j_real
+ */
+      __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
+
+      /* "CyRK/array/interp.pyx":272
+ *         fp_at_j_imag = fp_at_j.imag
+ *         xp_at_j = x_domain[j]
+ *         if j == lenx - 1:             # <<<<<<<<<<<<<<
+ *             result_real = fp_at_j_real
+ *             result_imag = fp_at_j_imag
+ */
+      goto __pyx_L5;
+    }
+
+    /* "CyRK/array/interp.pyx":275
+ *             result_real = fp_at_j_real
+ *             result_imag = fp_at_j_imag
+ *         elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
+ *             result_real = fp_at_j_real
+ *             result_imag = fp_at_j_imag
+ */
+    __pyx_t_3 = (__pyx_v_xp_at_j == __pyx_v_desired_x);
+    if (__pyx_t_3) {
+
+      /* "CyRK/array/interp.pyx":276
+ *             result_imag = fp_at_j_imag
+ *         elif xp_at_j == desired_x:
+ *             result_real = fp_at_j_real             # <<<<<<<<<<<<<<
+ *             result_imag = fp_at_j_imag
+ *         else:
+ */
+      __pyx_v_result_real = __pyx_v_fp_at_j_real;
+
+      /* "CyRK/array/interp.pyx":277
+ *         elif xp_at_j == desired_x:
+ *             result_real = fp_at_j_real
+ *             result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
+ *         else:
+ *             fp_at_jp1 = dependent_values[j + 1]
+ */
+      __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
+
+      /* "CyRK/array/interp.pyx":275
+ *             result_real = fp_at_j_real
+ *             result_imag = fp_at_j_imag
+ *         elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
+ *             result_real = fp_at_j_real
+ *             result_imag = fp_at_j_imag
+ */
+      goto __pyx_L5;
+    }
+
+    /* "CyRK/array/interp.pyx":279
+ *             result_imag = fp_at_j_imag
+ *         else:
+ *             fp_at_jp1 = dependent_values[j + 1]             # <<<<<<<<<<<<<<
+ *             fp_at_jp1_real = fp_at_jp1.real
+ *             fp_at_jp1_imag = fp_at_jp1.imag
+ */
+    /*else*/ {
+      __pyx_t_2 = (__pyx_v_j + 1);
+      __pyx_v_fp_at_jp1 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
+
+      /* "CyRK/array/interp.pyx":280
+ *         else:
+ *             fp_at_jp1 = dependent_values[j + 1]
+ *             fp_at_jp1_real = fp_at_jp1.real             # <<<<<<<<<<<<<<
+ *             fp_at_jp1_imag = fp_at_jp1.imag
+ *             xp_at_jp1 = x_domain[j + 1]
+ */
+      __pyx_t_5 = __Pyx_CREAL(__pyx_v_fp_at_jp1);
+      __pyx_v_fp_at_jp1_real = __pyx_t_5;
+
+      /* "CyRK/array/interp.pyx":281
+ *             fp_at_jp1 = dependent_values[j + 1]
+ *             fp_at_jp1_real = fp_at_jp1.real
+ *             fp_at_jp1_imag = fp_at_jp1.imag             # <<<<<<<<<<<<<<
+ *             xp_at_jp1 = x_domain[j + 1]
+ *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
+ */
+      __pyx_t_5 = __Pyx_CIMAG(__pyx_v_fp_at_jp1);
+      __pyx_v_fp_at_jp1_imag = __pyx_t_5;
+
+      /* "CyRK/array/interp.pyx":282
+ *             fp_at_jp1_real = fp_at_jp1.real
+ *             fp_at_jp1_imag = fp_at_jp1.imag
+ *             xp_at_jp1 = x_domain[j + 1]             # <<<<<<<<<<<<<<
+ *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
+ *             slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
+ */
+      __pyx_t_2 = (__pyx_v_j + 1);
+      __pyx_v_xp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_2 * __pyx_v_x_domain.strides[0]) )));
+
+      /* "CyRK/array/interp.pyx":283
+ *             fp_at_jp1_imag = fp_at_jp1.imag
+ *             xp_at_jp1 = x_domain[j + 1]
+ *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)             # <<<<<<<<<<<<<<
+ *             slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
+ *             slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse
+ */
+      __pyx_v_x_slope_inverse = (1.0 / (__pyx_v_xp_at_jp1 - __pyx_v_xp_at_j));
+
+      /* "CyRK/array/interp.pyx":284
+ *             xp_at_jp1 = x_domain[j + 1]
+ *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
+ *             slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse             # <<<<<<<<<<<<<<
+ *             slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse
+ * 
+ */
+      __pyx_v_slope_real = ((__pyx_v_fp_at_jp1_real - __pyx_v_fp_at_j_real) * __pyx_v_x_slope_inverse);
+
+      /* "CyRK/array/interp.pyx":285
+ *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
+ *             slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
+ *             slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse             # <<<<<<<<<<<<<<
+ * 
+ *             # If we get nan in one direction try the other
+ */
+      __pyx_v_slope_imag = ((__pyx_v_fp_at_jp1_imag - __pyx_v_fp_at_j_imag) * __pyx_v_x_slope_inverse);
+
+      /* "CyRK/array/interp.pyx":289
+ *             # If we get nan in one direction try the other
+ *             # Real Part
+ *             result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real             # <<<<<<<<<<<<<<
+ *             if isnan(result_real):
+ *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
+ */
+      __pyx_v_result_real = ((__pyx_v_slope_real * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j_real);
+
+      /* "CyRK/array/interp.pyx":290
+ *             # Real Part
+ *             result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
+ *             if isnan(result_real):             # <<<<<<<<<<<<<<
+ *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
+ *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
+ */
+      __pyx_t_3 = isnan(__pyx_v_result_real);
+      if (__pyx_t_3) {
+
+        /* "CyRK/array/interp.pyx":291
+ *             result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
+ *             if isnan(result_real):
+ *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real             # <<<<<<<<<<<<<<
+ *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
+ *                     result_real = fp_at_j_real
+ */
+        __pyx_v_result_real = ((__pyx_v_slope_real * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1_real);
+
+        /* "CyRK/array/interp.pyx":292
+ *             if isnan(result_real):
+ *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
+ *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):             # <<<<<<<<<<<<<<
+ *                     result_real = fp_at_j_real
+ * 
+ */
+        __pyx_t_7 = isnan(__pyx_v_result_real);
+        if (__pyx_t_7) {
+        } else {
+          __pyx_t_3 = __pyx_t_7;
+          goto __pyx_L8_bool_binop_done;
+        }
+        __pyx_t_7 = (__pyx_v_fp_at_jp1_real == __pyx_v_fp_at_j_real);
+        __pyx_t_3 = __pyx_t_7;
+        __pyx_L8_bool_binop_done:;
+        if (__pyx_t_3) {
+
+          /* "CyRK/array/interp.pyx":293
+ *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
+ *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
+ *                     result_real = fp_at_j_real             # <<<<<<<<<<<<<<
+ * 
+ *             # Imaginary Part
+ */
+          __pyx_v_result_real = __pyx_v_fp_at_j_real;
+
+          /* "CyRK/array/interp.pyx":292
+ *             if isnan(result_real):
+ *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
+ *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):             # <<<<<<<<<<<<<<
+ *                     result_real = fp_at_j_real
+ * 
+ */
+        }
+
+        /* "CyRK/array/interp.pyx":290
+ *             # Real Part
+ *             result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
+ *             if isnan(result_real):             # <<<<<<<<<<<<<<
+ *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
+ *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
+ */
+      }
+
+      /* "CyRK/array/interp.pyx":296
+ * 
+ *             # Imaginary Part
+ *             result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag             # <<<<<<<<<<<<<<
+ *             if isnan(result_imag):
+ *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
+ */
+      __pyx_v_result_imag = ((__pyx_v_slope_imag * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j_imag);
+
+      /* "CyRK/array/interp.pyx":297
+ *             # Imaginary Part
+ *             result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
+ *             if isnan(result_imag):             # <<<<<<<<<<<<<<
+ *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
+ *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
+ */
+      __pyx_t_3 = isnan(__pyx_v_result_imag);
+      if (__pyx_t_3) {
+
+        /* "CyRK/array/interp.pyx":298
+ *             result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
+ *             if isnan(result_imag):
+ *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag             # <<<<<<<<<<<<<<
+ *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
+ *                     result_imag = fp_at_j_imag
+ */
+        __pyx_v_result_imag = ((__pyx_v_slope_imag * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1_imag);
+
+        /* "CyRK/array/interp.pyx":299
+ *             if isnan(result_imag):
+ *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
+ *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):             # <<<<<<<<<<<<<<
+ *                     result_imag = fp_at_j_imag
+ * 
+ */
+        __pyx_t_7 = isnan(__pyx_v_result_imag);
+        if (__pyx_t_7) {
+        } else {
+          __pyx_t_3 = __pyx_t_7;
+          goto __pyx_L12_bool_binop_done;
+        }
+        __pyx_t_7 = (__pyx_v_fp_at_jp1_imag == __pyx_v_fp_at_j_imag);
+        __pyx_t_3 = __pyx_t_7;
+        __pyx_L12_bool_binop_done:;
+        if (__pyx_t_3) {
+
+          /* "CyRK/array/interp.pyx":300
+ *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
+ *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
+ *                     result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
+ * 
+ *     cdef double complex result
+ */
+          __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
+
+          /* "CyRK/array/interp.pyx":299
+ *             if isnan(result_imag):
+ *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
+ *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):             # <<<<<<<<<<<<<<
+ *                     result_imag = fp_at_j_imag
+ * 
+ */
+        }
+
+        /* "CyRK/array/interp.pyx":297
+ *             # Imaginary Part
+ *             result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
+ *             if isnan(result_imag):             # <<<<<<<<<<<<<<
+ *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
+ *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
+ */
+      }
+    }
+    __pyx_L5:;
+  }
+  __pyx_L4:;
+
+  /* "CyRK/array/interp.pyx":303
+ * 
+ *     cdef double complex result
+ *     result = result_real + 1.0j * result_imag             # <<<<<<<<<<<<<<
+ * 
+ *     return result, j_out
+ */
+  __pyx_v_result = __Pyx_c_sum_double(__pyx_t_double_complex_from_parts(__pyx_v_result_real, 0), __Pyx_c_prod_double(__pyx_t_double_complex_from_parts(0, 1.0), __pyx_t_double_complex_from_parts(__pyx_v_result_imag, 0)));
+
+  /* "CyRK/array/interp.pyx":305
+ *     result = result_real + 1.0j * result_imag
+ * 
+ *     return result, j_out             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __pyx_t_8.f0 = __pyx_v_result;
+  __pyx_t_8.f1 = __pyx_v_j_out;
+  __pyx_r = __pyx_t_8;
+  goto __pyx_L0;
+
+  /* "CyRK/array/interp.pyx":188
+ * 
+ * 
+ * cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
+ *                                             double complex[:] dependent_values, int provided_j = -1) nogil:
+ *     """ Interpolation function for complex numbers.
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  #ifdef WITH_THREAD
+  __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+  #endif
+  __Pyx_AddTraceback("CyRK.array.interp.interp_complexj", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_pretend_to_initialize(&__pyx_r);
+  #ifdef WITH_THREAD
+  __Pyx_PyGILState_Release(__pyx_gilstate_save);
+  #endif
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* Python wrapper */
+static PyObject *__pyx_pw_4CyRK_5array_6interp_3interp_complexj(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+); /*proto*/
+PyDoc_STRVAR(__pyx_doc_4CyRK_5array_6interp_2interp_complexj, " Interpolation function for complex numbers.\n\n    Provided a domain, `desired_x` and a dependent array `dependent_values` search domain for value closest to \n    `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local \n    slopes of `desired_x` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.\n\n    Based on `numpy`'s `interp` function.\n\n    Parameters\n    ----------\n    desired_x : float\n        Location where `dependent_variables` is desired.\n    x_domain : np.ndarray[float]\n        Domain to search for the correct location.\n    dependent_values : np.ndarray[complex]\n        Dependent values that are to be returned after search and interpolation.\n    provided_j : int\n        Give a j index from a previous interpolation to improve performance.\n\n    Returns\n    -------\n    result : complex\n        Desired value of `dependent_values`.\n    j_out : int\n        The index that was found during binary_search_with_guess which can be used by other interpolation functions \n        to improve performance.\n\n    ");
+static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_3interp_complexj = {"interp_complexj", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_3interp_complexj, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_4CyRK_5array_6interp_2interp_complexj};
+static PyObject *__pyx_pw_4CyRK_5array_6interp_3interp_complexj(PyObject *__pyx_self, 
+#if CYTHON_METH_FASTCALL
+PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
+#else
+PyObject *__pyx_args, PyObject *__pyx_kwds
+#endif
+) {
+  double __pyx_v_desired_x;
+  __Pyx_memviewslice __pyx_v_x_domain = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_dependent_values = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_v_provided_j;
+  #if !CYTHON_METH_FASTCALL
+  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
+  #endif
+  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("interp_complexj (wrapper)", 0);
+  {
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_desired_x,&__pyx_n_s_x_domain,&__pyx_n_s_dependent_values,&__pyx_n_s_provided_j,0};
+    PyObject* values[4] = {0,0,0,0};
+    if (__pyx_kwds) {
+      Py_ssize_t kw_args;
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
+      switch (__pyx_nargs) {
+        case  0:
+        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_desired_x)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L3_error)
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x_domain)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("interp_complexj", 0, 3, 4, 1); __PYX_ERR(1, 188, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dependent_values)) != 0)) kw_args--;
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L3_error)
+        else {
+          __Pyx_RaiseArgtupleInvalid("interp_complexj", 0, 3, 4, 2); __PYX_ERR(1, 188, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_provided_j);
+          if (value) { values[3] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        const Py_ssize_t kwd_pos_args = __pyx_nargs;
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp_complexj") < 0)) __PYX_ERR(1, 188, __pyx_L3_error)
+      }
+    } else {
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_desired_x = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_desired_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L3_error)
+    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 188, __pyx_L3_error)
+    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 189, __pyx_L3_error)
+    if (values[3]) {
+      __pyx_v_provided_j = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_provided_j == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 189, __pyx_L3_error)
+    } else {
+      __pyx_v_provided_j = ((int)-1);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("interp_complexj", 0, 3, 4, __pyx_nargs); __PYX_ERR(1, 188, __pyx_L3_error)
+  __pyx_L3_error:;
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
+  __Pyx_AddTraceback("CyRK.array.interp.interp_complexj", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_4CyRK_5array_6interp_2interp_complexj(__pyx_self, __pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_provided_j);
+
+  /* function exit code */
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
+  __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_4CyRK_5array_6interp_2interp_complexj(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, int __pyx_v_provided_j) {
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  __pyx_ctuple___dunderpyx_t_double_complex__and_int __pyx_t_1;
+  struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("interp_complexj", 0);
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2.__pyx_n = 1;
+  __pyx_t_2.provided_j = __pyx_v_provided_j;
+  __pyx_t_1 = __pyx_f_4CyRK_5array_6interp_interp_complexj(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, 0, &__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 188, __pyx_L1_error)
+  __pyx_t_3 = __pyx_convert__to_py___pyx_ctuple___dunderpyx_t_double_complex__and_int(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 188, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
+  goto __pyx_L0;
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_AddTraceback("CyRK.array.interp.interp_complexj", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "CyRK/array/interp.pyx":308
+ * 
+ * 
+ * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values, int provided_j = -1) nogil:             # <<<<<<<<<<<<<<
  *     """ Interpolation function for floats.
  * 
  */
 
-static PyObject *__pyx_pw_4CyRK_5array_6interp_1interp(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4CyRK_5array_6interp_5interp(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static double __pyx_f_4CyRK_5array_6interp_interp(double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static double __pyx_f_4CyRK_5array_6interp_interp(double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp *__pyx_optional_args) {
+  int __pyx_v_provided_j = ((int)-1);
   unsigned int __pyx_v_lenx;
   double __pyx_v_left_value;
   double __pyx_v_right_value;
   unsigned int __pyx_v_j;
   double __pyx_v_slope;
   double __pyx_v_result;
   double __pyx_v_fp_at_j;
   double __pyx_v_xp_at_j;
   double __pyx_v_fp_at_jp1;
   double __pyx_v_xp_at_jp1;
   double __pyx_r;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
-  unsigned int __pyx_t_3;
-  int __pyx_t_4;
+  int __pyx_t_3;
+  unsigned int __pyx_t_4;
   size_t __pyx_t_5;
   int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
+  if (__pyx_optional_args) {
+    if (__pyx_optional_args->__pyx_n > 0) {
+      __pyx_v_provided_j = __pyx_optional_args->provided_j;
+    }
+  }
 
-  /* "CyRK/array/interp.pyx":122
+  /* "CyRK/array/interp.pyx":336
  * 
  *     cdef unsigned int lenx
  *     lenx = len(x_domain)             # <<<<<<<<<<<<<<
  *     # TODO: Needs to be at least 3 item long array. Add exception here?
  * 
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_x_domain); 
   __pyx_v_lenx = __pyx_t_1;
 
-  /* "CyRK/array/interp.pyx":126
+  /* "CyRK/array/interp.pyx":340
  * 
  *     cdef double left_value
  *     left_value = dependent_values[0]             # <<<<<<<<<<<<<<
  *     cdef double right_value
  *     right_value = dependent_values[lenx - 1]
  */
   __pyx_t_2 = 0;
   __pyx_v_left_value = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-  /* "CyRK/array/interp.pyx":128
+  /* "CyRK/array/interp.pyx":342
  *     left_value = dependent_values[0]
  *     cdef double right_value
  *     right_value = dependent_values[lenx - 1]             # <<<<<<<<<<<<<<
  * 
  *     # Binary Search with Guess
  */
   __pyx_t_2 = (__pyx_v_lenx - 1);
   __pyx_v_right_value = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-  /* "CyRK/array/interp.pyx":132
+  /* "CyRK/array/interp.pyx":346
  *     # Binary Search with Guess
  *     cdef unsigned int j
  *     j = 0             # <<<<<<<<<<<<<<
  *     cdef double slope
  * 
  */
   __pyx_v_j = 0;
 
-  /* "CyRK/array/interp.pyx":142
+  /* "CyRK/array/interp.pyx":356
+ * 
+ *     # Perform binary search with guess
+ *     if provided_j == -1:             # <<<<<<<<<<<<<<
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ */
+  __pyx_t_3 = (__pyx_v_provided_j == -1L);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":358
+ *     if provided_j == -1:
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     elif provided_j < -1:
+ *         # Error
+ */
+    __pyx_t_4 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_4 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 358, __pyx_L1_error)
+    __pyx_v_j = __pyx_t_4;
+
+    /* "CyRK/array/interp.pyx":356
  * 
  *     # Perform binary search with guess
- *     j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     if provided_j == -1:             # <<<<<<<<<<<<<<
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ */
+    goto __pyx_L3;
+  }
+
+  /* "CyRK/array/interp.pyx":359
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ *     elif provided_j < -1:             # <<<<<<<<<<<<<<
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ */
+  __pyx_t_3 = (__pyx_v_provided_j < -1L);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":362
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     else:
+ *         # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+ */
+    __pyx_t_4 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_4 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 362, __pyx_L1_error)
+    __pyx_v_j = __pyx_t_4;
+
+    /* "CyRK/array/interp.pyx":359
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ *     elif provided_j < -1:             # <<<<<<<<<<<<<<
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ */
+    goto __pyx_L3;
+  }
+
+  /* "CyRK/array/interp.pyx":365
+ *     else:
+ *         # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+ *         j = <unsigned int>provided_j             # <<<<<<<<<<<<<<
  * 
  *     if j == 0:
  */
-  __pyx_t_3 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_3 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 142, __pyx_L1_error)
-  __pyx_v_j = __pyx_t_3;
+  /*else*/ {
+    __pyx_v_j = ((unsigned int)__pyx_v_provided_j);
+  }
+  __pyx_L3:;
 
-  /* "CyRK/array/interp.pyx":144
- *     j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+  /* "CyRK/array/interp.pyx":367
+ *         j = <unsigned int>provided_j
  * 
  *     if j == 0:             # <<<<<<<<<<<<<<
  *         result = left_value
  *     elif j == lenx:
  */
-  __pyx_t_4 = (__pyx_v_j == 0);
-  if (__pyx_t_4) {
+  __pyx_t_3 = (__pyx_v_j == 0);
+  if (__pyx_t_3) {
 
-    /* "CyRK/array/interp.pyx":145
+    /* "CyRK/array/interp.pyx":368
  * 
  *     if j == 0:
  *         result = left_value             # <<<<<<<<<<<<<<
  *     elif j == lenx:
  *         result = right_value
  */
     __pyx_v_result = __pyx_v_left_value;
 
-    /* "CyRK/array/interp.pyx":144
- *     j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    /* "CyRK/array/interp.pyx":367
+ *         j = <unsigned int>provided_j
  * 
  *     if j == 0:             # <<<<<<<<<<<<<<
  *         result = left_value
  *     elif j == lenx:
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "CyRK/array/interp.pyx":146
+  /* "CyRK/array/interp.pyx":369
  *     if j == 0:
  *         result = left_value
  *     elif j == lenx:             # <<<<<<<<<<<<<<
  *         result = right_value
  *     else:
  */
-  __pyx_t_4 = (__pyx_v_j == __pyx_v_lenx);
-  if (__pyx_t_4) {
+  __pyx_t_3 = (__pyx_v_j == __pyx_v_lenx);
+  if (__pyx_t_3) {
 
-    /* "CyRK/array/interp.pyx":147
+    /* "CyRK/array/interp.pyx":370
  *         result = left_value
  *     elif j == lenx:
  *         result = right_value             # <<<<<<<<<<<<<<
  *     else:
  *         fp_at_j = dependent_values[j]
  */
     __pyx_v_result = __pyx_v_right_value;
 
-    /* "CyRK/array/interp.pyx":146
+    /* "CyRK/array/interp.pyx":369
  *     if j == 0:
  *         result = left_value
  *     elif j == lenx:             # <<<<<<<<<<<<<<
  *         result = right_value
  *     else:
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "CyRK/array/interp.pyx":149
+  /* "CyRK/array/interp.pyx":372
  *         result = right_value
  *     else:
  *         fp_at_j = dependent_values[j]             # <<<<<<<<<<<<<<
  *         xp_at_j = x_domain[j]
  *         if j == lenx - 1:
  */
   /*else*/ {
     __pyx_t_5 = __pyx_v_j;
     __pyx_v_fp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_5 * __pyx_v_dependent_values.strides[0]) )));
 
-    /* "CyRK/array/interp.pyx":150
+    /* "CyRK/array/interp.pyx":373
  *     else:
  *         fp_at_j = dependent_values[j]
  *         xp_at_j = x_domain[j]             # <<<<<<<<<<<<<<
  *         if j == lenx - 1:
  *             result = fp_at_j
  */
     __pyx_t_5 = __pyx_v_j;
     __pyx_v_xp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_5 * __pyx_v_x_domain.strides[0]) )));
 
-    /* "CyRK/array/interp.pyx":151
+    /* "CyRK/array/interp.pyx":374
  *         fp_at_j = dependent_values[j]
  *         xp_at_j = x_domain[j]
  *         if j == lenx - 1:             # <<<<<<<<<<<<<<
  *             result = fp_at_j
  *         elif xp_at_j == desired_x:
  */
-    __pyx_t_4 = (__pyx_v_j == (__pyx_v_lenx - 1));
-    if (__pyx_t_4) {
+    __pyx_t_3 = (__pyx_v_j == (__pyx_v_lenx - 1));
+    if (__pyx_t_3) {
 
-      /* "CyRK/array/interp.pyx":152
+      /* "CyRK/array/interp.pyx":375
  *         xp_at_j = x_domain[j]
  *         if j == lenx - 1:
  *             result = fp_at_j             # <<<<<<<<<<<<<<
  *         elif xp_at_j == desired_x:
  *             result = fp_at_j
  */
       __pyx_v_result = __pyx_v_fp_at_j;
 
-      /* "CyRK/array/interp.pyx":151
+      /* "CyRK/array/interp.pyx":374
  *         fp_at_j = dependent_values[j]
  *         xp_at_j = x_domain[j]
  *         if j == lenx - 1:             # <<<<<<<<<<<<<<
  *             result = fp_at_j
  *         elif xp_at_j == desired_x:
  */
-      goto __pyx_L4;
+      goto __pyx_L5;
     }
 
-    /* "CyRK/array/interp.pyx":153
+    /* "CyRK/array/interp.pyx":376
  *         if j == lenx - 1:
  *             result = fp_at_j
  *         elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
  *             result = fp_at_j
  *         else:
  */
-    __pyx_t_4 = (__pyx_v_xp_at_j == __pyx_v_desired_x);
-    if (__pyx_t_4) {
+    __pyx_t_3 = (__pyx_v_xp_at_j == __pyx_v_desired_x);
+    if (__pyx_t_3) {
 
-      /* "CyRK/array/interp.pyx":154
+      /* "CyRK/array/interp.pyx":377
  *             result = fp_at_j
  *         elif xp_at_j == desired_x:
  *             result = fp_at_j             # <<<<<<<<<<<<<<
  *         else:
  *             fp_at_jp1 = dependent_values[j + 1]
  */
       __pyx_v_result = __pyx_v_fp_at_j;
 
-      /* "CyRK/array/interp.pyx":153
+      /* "CyRK/array/interp.pyx":376
  *         if j == lenx - 1:
  *             result = fp_at_j
  *         elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
  *             result = fp_at_j
  *         else:
  */
-      goto __pyx_L4;
+      goto __pyx_L5;
     }
 
-    /* "CyRK/array/interp.pyx":156
+    /* "CyRK/array/interp.pyx":379
  *             result = fp_at_j
  *         else:
  *             fp_at_jp1 = dependent_values[j + 1]             # <<<<<<<<<<<<<<
  *             xp_at_jp1 = x_domain[j + 1]
  *             slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_j + 1);
       __pyx_v_fp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-      /* "CyRK/array/interp.pyx":157
+      /* "CyRK/array/interp.pyx":380
  *         else:
  *             fp_at_jp1 = dependent_values[j + 1]
  *             xp_at_jp1 = x_domain[j + 1]             # <<<<<<<<<<<<<<
  *             slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)
  * 
  */
       __pyx_t_2 = (__pyx_v_j + 1);
       __pyx_v_xp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_2 * __pyx_v_x_domain.strides[0]) )));
 
-      /* "CyRK/array/interp.pyx":158
+      /* "CyRK/array/interp.pyx":381
  *             fp_at_jp1 = dependent_values[j + 1]
  *             xp_at_jp1 = x_domain[j + 1]
  *             slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)             # <<<<<<<<<<<<<<
  * 
  *             # If we get nan in one direction, try the other
  */
       __pyx_v_slope = ((__pyx_v_fp_at_jp1 - __pyx_v_fp_at_j) / (__pyx_v_xp_at_jp1 - __pyx_v_xp_at_j));
 
-      /* "CyRK/array/interp.pyx":161
+      /* "CyRK/array/interp.pyx":384
  * 
  *             # If we get nan in one direction, try the other
  *             result = slope * (desired_x - xp_at_j) + fp_at_j             # <<<<<<<<<<<<<<
  *             if isnan(result):
  *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  */
       __pyx_v_result = ((__pyx_v_slope * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j);
 
-      /* "CyRK/array/interp.pyx":162
+      /* "CyRK/array/interp.pyx":385
  *             # If we get nan in one direction, try the other
  *             result = slope * (desired_x - xp_at_j) + fp_at_j
  *             if isnan(result):             # <<<<<<<<<<<<<<
  *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                 if isnan(result) and (fp_at_jp1 == fp_at_j):
  */
-      __pyx_t_4 = isnan(__pyx_v_result);
-      if (__pyx_t_4) {
+      __pyx_t_3 = isnan(__pyx_v_result);
+      if (__pyx_t_3) {
 
-        /* "CyRK/array/interp.pyx":163
+        /* "CyRK/array/interp.pyx":386
  *             result = slope * (desired_x - xp_at_j) + fp_at_j
  *             if isnan(result):
  *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1             # <<<<<<<<<<<<<<
  *                 if isnan(result) and (fp_at_jp1 == fp_at_j):
  *                     result = fp_at_j
  */
         __pyx_v_result = ((__pyx_v_slope * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1);
 
-        /* "CyRK/array/interp.pyx":164
+        /* "CyRK/array/interp.pyx":387
  *             if isnan(result):
  *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                 if isnan(result) and (fp_at_jp1 == fp_at_j):             # <<<<<<<<<<<<<<
  *                     result = fp_at_j
  * 
  */
         __pyx_t_6 = isnan(__pyx_v_result);
         if (__pyx_t_6) {
         } else {
-          __pyx_t_4 = __pyx_t_6;
-          goto __pyx_L7_bool_binop_done;
+          __pyx_t_3 = __pyx_t_6;
+          goto __pyx_L8_bool_binop_done;
         }
         __pyx_t_6 = (__pyx_v_fp_at_jp1 == __pyx_v_fp_at_j);
-        __pyx_t_4 = __pyx_t_6;
-        __pyx_L7_bool_binop_done:;
-        if (__pyx_t_4) {
+        __pyx_t_3 = __pyx_t_6;
+        __pyx_L8_bool_binop_done:;
+        if (__pyx_t_3) {
 
-          /* "CyRK/array/interp.pyx":165
+          /* "CyRK/array/interp.pyx":388
  *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                 if isnan(result) and (fp_at_jp1 == fp_at_j):
  *                     result = fp_at_j             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
           __pyx_v_result = __pyx_v_fp_at_j;
 
-          /* "CyRK/array/interp.pyx":164
+          /* "CyRK/array/interp.pyx":387
  *             if isnan(result):
  *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                 if isnan(result) and (fp_at_jp1 == fp_at_j):             # <<<<<<<<<<<<<<
  *                     result = fp_at_j
  * 
  */
         }
 
-        /* "CyRK/array/interp.pyx":162
+        /* "CyRK/array/interp.pyx":385
  *             # If we get nan in one direction, try the other
  *             result = slope * (desired_x - xp_at_j) + fp_at_j
  *             if isnan(result):             # <<<<<<<<<<<<<<
  *                 result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                 if isnan(result) and (fp_at_jp1 == fp_at_j):
  */
       }
     }
-    __pyx_L4:;
+    __pyx_L5:;
   }
-  __pyx_L3:;
+  __pyx_L4:;
 
-  /* "CyRK/array/interp.pyx":167
+  /* "CyRK/array/interp.pyx":390
  *                     result = fp_at_j
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "CyRK/array/interp.pyx":96
+  /* "CyRK/array/interp.pyx":308
  * 
  * 
- * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values) nogil:             # <<<<<<<<<<<<<<
+ * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values, int provided_j = -1) nogil:             # <<<<<<<<<<<<<<
  *     """ Interpolation function for floats.
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   #ifdef WITH_THREAD
@@ -19575,159 +21121,180 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4CyRK_5array_6interp_1interp(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4CyRK_5array_6interp_5interp(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_4CyRK_5array_6interp_interp, " Interpolation function for floats.\n\n    Provided a domain, `x_domain` and a dependent array `dependent_values` search domain for value closest to \n    `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local \n    slopes of `x_domain` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.\n\n    Based on `numpy`'s `interp` function.\n\n    Parameters\n    ----------\n    desired_x : float\n        Location where `dependent_variables` is desired.\n    x_domain : np.ndarray[float]\n        Domain to search for the correct location.\n    dependent_values : np.ndarray[float]\n        Dependent values that are to be returned after search and interpolation.\n\n    Returns\n    -------\n    result : float\n        Desired value of `dependent_values`.\n\n    ");
-static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_1interp = {"interp", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_1interp, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_4CyRK_5array_6interp_interp};
-static PyObject *__pyx_pw_4CyRK_5array_6interp_1interp(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_4CyRK_5array_6interp_4interp, " Interpolation function for floats.\n\n    Provided a domain, `x_domain` and a dependent array `dependent_values` search domain for value closest to \n    `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local \n    slopes of `x_domain` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.\n\n    Based on `numpy`'s `interp` function.\n\n    Parameters\n    ----------\n    desired_x : float\n        Location where `dependent_variables` is desired.\n    x_domain : np.ndarray[float]\n        Domain to search for the correct location.\n    dependent_values : np.ndarray[float]\n        Dependent values that are to be returned after search and interpolation.\n    provided_j : int\n        Give a j index from a previous interpolation to improve performance.\n\n    Returns\n    -------\n    result : float\n        Desired value of `dependent_values`.\n\n    ");
+static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_5interp = {"interp", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_5interp, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_4CyRK_5array_6interp_4interp};
+static PyObject *__pyx_pw_4CyRK_5array_6interp_5interp(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   double __pyx_v_desired_x;
   __Pyx_memviewslice __pyx_v_x_domain = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dependent_values = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_v_provided_j;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("interp (wrapper)", 0);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_desired_x,&__pyx_n_s_x_domain,&__pyx_n_s_dependent_values,0};
-    PyObject* values[3] = {0,0,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_desired_x,&__pyx_n_s_x_domain,&__pyx_n_s_dependent_values,&__pyx_n_s_provided_j,0};
+    PyObject* values[4] = {0,0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_desired_x)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x_domain)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp", 1, 3, 3, 1); __PYX_ERR(1, 96, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp", 0, 3, 4, 1); __PYX_ERR(1, 308, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dependent_values)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp", 1, 3, 3, 2); __PYX_ERR(1, 96, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp", 0, 3, 4, 2); __PYX_ERR(1, 308, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_provided_j);
+          if (value) { values[3] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp") < 0)) __PYX_ERR(1, 96, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp") < 0)) __PYX_ERR(1, 308, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 3)) {
-      goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_desired_x = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_desired_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L3_error)
+    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 308, __pyx_L3_error)
+    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 308, __pyx_L3_error)
+    if (values[3]) {
+      __pyx_v_provided_j = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_provided_j == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L3_error)
+    } else {
+      __pyx_v_provided_j = ((int)-1);
     }
-    __pyx_v_desired_x = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_desired_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L3_error)
-    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 96, __pyx_L3_error)
-    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 96, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("interp", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 96, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("interp", 0, 3, 4, __pyx_nargs); __PYX_ERR(1, 308, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
   __Pyx_AddTraceback("CyRK.array.interp.interp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4CyRK_5array_6interp_interp(__pyx_self, __pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values);
+  __pyx_r = __pyx_pf_4CyRK_5array_6interp_4interp(__pyx_self, __pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_provided_j);
 
   /* function exit code */
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4CyRK_5array_6interp_interp(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values) {
+static PyObject *__pyx_pf_4CyRK_5array_6interp_4interp(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, int __pyx_v_provided_j) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   double __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
+  struct __pyx_opt_args_4CyRK_5array_6interp_interp __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("interp", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_x_domain.memview)) { __Pyx_RaiseUnboundLocalError("x_domain"); __PYX_ERR(1, 96, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_dependent_values.memview)) { __Pyx_RaiseUnboundLocalError("dependent_values"); __PYX_ERR(1, 96, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_f_4CyRK_5array_6interp_interp(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, 0); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(1, 96, __pyx_L1_error)
-  __pyx_t_2 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 96, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_2.__pyx_n = 1;
+  __pyx_t_2.provided_j = __pyx_v_provided_j;
+  __pyx_t_1 = __pyx_f_4CyRK_5array_6interp_interp(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, 0, &__pyx_t_2); if (unlikely(__pyx_t_1 == ((double)-1) && PyErr_Occurred())) __PYX_ERR(1, 308, __pyx_L1_error)
+  __pyx_t_3 = PyFloat_FromDouble(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 308, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("CyRK.array.interp.interp", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "CyRK/array/interp.pyx":170
+/* "CyRK/array/interp.pyx":393
  * 
  * 
  * cpdef double complex interp_complex(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
- *                                     double complex[:] dependent_values) nogil:
+ *                                     double complex[:] dependent_values, int provided_j = -1) nogil:
  *     """ Interpolation function for complex numbers.
  */
 
-static PyObject *__pyx_pw_4CyRK_5array_6interp_3interp_complex(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4CyRK_5array_6interp_7interp_complex(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static __pyx_t_double_complex __pyx_f_4CyRK_5array_6interp_interp_complex(double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, CYTHON_UNUSED int __pyx_skip_dispatch) {
+static __pyx_t_double_complex __pyx_f_4CyRK_5array_6interp_interp_complex(double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, CYTHON_UNUSED int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex *__pyx_optional_args) {
+  int __pyx_v_provided_j = ((int)-1);
   unsigned int __pyx_v_lenx;
   __pyx_t_double_complex __pyx_v_left_value;
   __pyx_t_double_complex __pyx_v_right_value;
   unsigned int __pyx_v_j;
   double __pyx_v_slope_real;
   double __pyx_v_slope_imag;
   double __pyx_v_x_slope_inverse;
@@ -19741,514 +21308,581 @@
   double __pyx_v_fp_at_jp1_real;
   double __pyx_v_fp_at_jp1_imag;
   double __pyx_v_xp_at_jp1;
   __pyx_t_double_complex __pyx_v_result;
   __pyx_t_double_complex __pyx_r;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
-  unsigned int __pyx_t_3;
-  int __pyx_t_4;
+  int __pyx_t_3;
+  unsigned int __pyx_t_4;
   double __pyx_t_5;
   size_t __pyx_t_6;
   int __pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
+  if (__pyx_optional_args) {
+    if (__pyx_optional_args->__pyx_n > 0) {
+      __pyx_v_provided_j = __pyx_optional_args->provided_j;
+    }
+  }
 
-  /* "CyRK/array/interp.pyx":197
+  /* "CyRK/array/interp.pyx":422
  * 
  *     cdef unsigned int lenx
  *     lenx = len(x_domain)             # <<<<<<<<<<<<<<
  *     # Note: Needs to be at least 3 item long array. Add exception here?
  * 
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_x_domain); 
   __pyx_v_lenx = __pyx_t_1;
 
-  /* "CyRK/array/interp.pyx":201
+  /* "CyRK/array/interp.pyx":426
  * 
  *     cdef double complex left_value
  *     left_value = dependent_values[0]             # <<<<<<<<<<<<<<
  *     cdef double complex right_value
  *     right_value = dependent_values[lenx - 1]
  */
   __pyx_t_2 = 0;
   __pyx_v_left_value = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-  /* "CyRK/array/interp.pyx":203
+  /* "CyRK/array/interp.pyx":428
  *     left_value = dependent_values[0]
  *     cdef double complex right_value
  *     right_value = dependent_values[lenx - 1]             # <<<<<<<<<<<<<<
  * 
  *     # Binary Search with Guess
  */
   __pyx_t_2 = (__pyx_v_lenx - 1);
   __pyx_v_right_value = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-  /* "CyRK/array/interp.pyx":207
+  /* "CyRK/array/interp.pyx":432
  *     # Binary Search with Guess
  *     cdef unsigned int j
  *     j = 0             # <<<<<<<<<<<<<<
  *     cdef double slope_real
  *     cdef double slope_imag
  */
   __pyx_v_j = 0;
 
-  /* "CyRK/array/interp.pyx":224
+  /* "CyRK/array/interp.pyx":449
+ * 
+ *     # Perform binary search with guess
+ *     if provided_j == -1:             # <<<<<<<<<<<<<<
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ */
+  __pyx_t_3 = (__pyx_v_provided_j == -1L);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":451
+ *     if provided_j == -1:
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     elif provided_j < -1:
+ *         # Error
+ */
+    __pyx_t_4 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_4 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 451, __pyx_L1_error)
+    __pyx_v_j = __pyx_t_4;
+
+    /* "CyRK/array/interp.pyx":449
  * 
  *     # Perform binary search with guess
- *     j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     if provided_j == -1:             # <<<<<<<<<<<<<<
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ */
+    goto __pyx_L3;
+  }
+
+  /* "CyRK/array/interp.pyx":452
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ *     elif provided_j < -1:             # <<<<<<<<<<<<<<
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ */
+  __pyx_t_3 = (__pyx_v_provided_j < -1L);
+  if (__pyx_t_3) {
+
+    /* "CyRK/array/interp.pyx":455
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)             # <<<<<<<<<<<<<<
+ *     else:
+ *         # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+ */
+    __pyx_t_4 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_4 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 455, __pyx_L1_error)
+    __pyx_v_j = __pyx_t_4;
+
+    /* "CyRK/array/interp.pyx":452
+ *         # No j provided; search for it instead.
+ *         j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+ *     elif provided_j < -1:             # <<<<<<<<<<<<<<
+ *         # Error
+ *         # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+ */
+    goto __pyx_L3;
+  }
+
+  /* "CyRK/array/interp.pyx":458
+ *     else:
+ *         # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+ *         j = <unsigned int> provided_j             # <<<<<<<<<<<<<<
  * 
  *     if j == 0:
  */
-  __pyx_t_3 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_j); if (unlikely(__pyx_t_3 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 224, __pyx_L1_error)
-  __pyx_v_j = __pyx_t_3;
+  /*else*/ {
+    __pyx_v_j = ((unsigned int)__pyx_v_provided_j);
+  }
+  __pyx_L3:;
 
-  /* "CyRK/array/interp.pyx":226
- *     j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+  /* "CyRK/array/interp.pyx":460
+ *         j = <unsigned int> provided_j
  * 
  *     if j == 0:             # <<<<<<<<<<<<<<
  *         result_real = left_value.real
  *         result_imag = left_value.imag
  */
-  __pyx_t_4 = (__pyx_v_j == 0);
-  if (__pyx_t_4) {
+  __pyx_t_3 = (__pyx_v_j == 0);
+  if (__pyx_t_3) {
 
-    /* "CyRK/array/interp.pyx":227
+    /* "CyRK/array/interp.pyx":461
  * 
  *     if j == 0:
  *         result_real = left_value.real             # <<<<<<<<<<<<<<
  *         result_imag = left_value.imag
  *     elif j == lenx:
  */
     __pyx_t_5 = __Pyx_CREAL(__pyx_v_left_value);
     __pyx_v_result_real = __pyx_t_5;
 
-    /* "CyRK/array/interp.pyx":228
+    /* "CyRK/array/interp.pyx":462
  *     if j == 0:
  *         result_real = left_value.real
  *         result_imag = left_value.imag             # <<<<<<<<<<<<<<
  *     elif j == lenx:
  *         result_real = right_value.real
  */
     __pyx_t_5 = __Pyx_CIMAG(__pyx_v_left_value);
     __pyx_v_result_imag = __pyx_t_5;
 
-    /* "CyRK/array/interp.pyx":226
- *     j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    /* "CyRK/array/interp.pyx":460
+ *         j = <unsigned int> provided_j
  * 
  *     if j == 0:             # <<<<<<<<<<<<<<
  *         result_real = left_value.real
  *         result_imag = left_value.imag
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "CyRK/array/interp.pyx":229
+  /* "CyRK/array/interp.pyx":463
  *         result_real = left_value.real
  *         result_imag = left_value.imag
  *     elif j == lenx:             # <<<<<<<<<<<<<<
  *         result_real = right_value.real
  *         result_imag = right_value.imag
  */
-  __pyx_t_4 = (__pyx_v_j == __pyx_v_lenx);
-  if (__pyx_t_4) {
+  __pyx_t_3 = (__pyx_v_j == __pyx_v_lenx);
+  if (__pyx_t_3) {
 
-    /* "CyRK/array/interp.pyx":230
+    /* "CyRK/array/interp.pyx":464
  *         result_imag = left_value.imag
  *     elif j == lenx:
  *         result_real = right_value.real             # <<<<<<<<<<<<<<
  *         result_imag = right_value.imag
  *     else:
  */
     __pyx_t_5 = __Pyx_CREAL(__pyx_v_right_value);
     __pyx_v_result_real = __pyx_t_5;
 
-    /* "CyRK/array/interp.pyx":231
+    /* "CyRK/array/interp.pyx":465
  *     elif j == lenx:
  *         result_real = right_value.real
  *         result_imag = right_value.imag             # <<<<<<<<<<<<<<
  *     else:
  *         fp_at_j = dependent_values[j]
  */
     __pyx_t_5 = __Pyx_CIMAG(__pyx_v_right_value);
     __pyx_v_result_imag = __pyx_t_5;
 
-    /* "CyRK/array/interp.pyx":229
+    /* "CyRK/array/interp.pyx":463
  *         result_real = left_value.real
  *         result_imag = left_value.imag
  *     elif j == lenx:             # <<<<<<<<<<<<<<
  *         result_real = right_value.real
  *         result_imag = right_value.imag
  */
-    goto __pyx_L3;
+    goto __pyx_L4;
   }
 
-  /* "CyRK/array/interp.pyx":233
+  /* "CyRK/array/interp.pyx":467
  *         result_imag = right_value.imag
  *     else:
  *         fp_at_j = dependent_values[j]             # <<<<<<<<<<<<<<
  *         fp_at_j_real = fp_at_j.real
  *         fp_at_j_imag = fp_at_j.imag
  */
   /*else*/ {
     __pyx_t_6 = __pyx_v_j;
     __pyx_v_fp_at_j = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_6 * __pyx_v_dependent_values.strides[0]) )));
 
-    /* "CyRK/array/interp.pyx":234
+    /* "CyRK/array/interp.pyx":468
  *     else:
  *         fp_at_j = dependent_values[j]
  *         fp_at_j_real = fp_at_j.real             # <<<<<<<<<<<<<<
  *         fp_at_j_imag = fp_at_j.imag
  *         xp_at_j = x_domain[j]
  */
     __pyx_t_5 = __Pyx_CREAL(__pyx_v_fp_at_j);
     __pyx_v_fp_at_j_real = __pyx_t_5;
 
-    /* "CyRK/array/interp.pyx":235
+    /* "CyRK/array/interp.pyx":469
  *         fp_at_j = dependent_values[j]
  *         fp_at_j_real = fp_at_j.real
  *         fp_at_j_imag = fp_at_j.imag             # <<<<<<<<<<<<<<
  *         xp_at_j = x_domain[j]
  *         if j == lenx - 1:
  */
     __pyx_t_5 = __Pyx_CIMAG(__pyx_v_fp_at_j);
     __pyx_v_fp_at_j_imag = __pyx_t_5;
 
-    /* "CyRK/array/interp.pyx":236
+    /* "CyRK/array/interp.pyx":470
  *         fp_at_j_real = fp_at_j.real
  *         fp_at_j_imag = fp_at_j.imag
  *         xp_at_j = x_domain[j]             # <<<<<<<<<<<<<<
  *         if j == lenx - 1:
  *             result_real = fp_at_j_real
  */
     __pyx_t_6 = __pyx_v_j;
     __pyx_v_xp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_6 * __pyx_v_x_domain.strides[0]) )));
 
-    /* "CyRK/array/interp.pyx":237
+    /* "CyRK/array/interp.pyx":471
  *         fp_at_j_imag = fp_at_j.imag
  *         xp_at_j = x_domain[j]
  *         if j == lenx - 1:             # <<<<<<<<<<<<<<
  *             result_real = fp_at_j_real
  *             result_imag = fp_at_j_imag
  */
-    __pyx_t_4 = (__pyx_v_j == (__pyx_v_lenx - 1));
-    if (__pyx_t_4) {
+    __pyx_t_3 = (__pyx_v_j == (__pyx_v_lenx - 1));
+    if (__pyx_t_3) {
 
-      /* "CyRK/array/interp.pyx":238
+      /* "CyRK/array/interp.pyx":472
  *         xp_at_j = x_domain[j]
  *         if j == lenx - 1:
  *             result_real = fp_at_j_real             # <<<<<<<<<<<<<<
  *             result_imag = fp_at_j_imag
  *         elif xp_at_j == desired_x:
  */
       __pyx_v_result_real = __pyx_v_fp_at_j_real;
 
-      /* "CyRK/array/interp.pyx":239
+      /* "CyRK/array/interp.pyx":473
  *         if j == lenx - 1:
  *             result_real = fp_at_j_real
  *             result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
  *         elif xp_at_j == desired_x:
  *             result_real = fp_at_j_real
  */
       __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
 
-      /* "CyRK/array/interp.pyx":237
+      /* "CyRK/array/interp.pyx":471
  *         fp_at_j_imag = fp_at_j.imag
  *         xp_at_j = x_domain[j]
  *         if j == lenx - 1:             # <<<<<<<<<<<<<<
  *             result_real = fp_at_j_real
  *             result_imag = fp_at_j_imag
  */
-      goto __pyx_L4;
+      goto __pyx_L5;
     }
 
-    /* "CyRK/array/interp.pyx":240
+    /* "CyRK/array/interp.pyx":474
  *             result_real = fp_at_j_real
  *             result_imag = fp_at_j_imag
  *         elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
  *             result_real = fp_at_j_real
  *             result_imag = fp_at_j_imag
  */
-    __pyx_t_4 = (__pyx_v_xp_at_j == __pyx_v_desired_x);
-    if (__pyx_t_4) {
+    __pyx_t_3 = (__pyx_v_xp_at_j == __pyx_v_desired_x);
+    if (__pyx_t_3) {
 
-      /* "CyRK/array/interp.pyx":241
+      /* "CyRK/array/interp.pyx":475
  *             result_imag = fp_at_j_imag
  *         elif xp_at_j == desired_x:
  *             result_real = fp_at_j_real             # <<<<<<<<<<<<<<
  *             result_imag = fp_at_j_imag
  *         else:
  */
       __pyx_v_result_real = __pyx_v_fp_at_j_real;
 
-      /* "CyRK/array/interp.pyx":242
+      /* "CyRK/array/interp.pyx":476
  *         elif xp_at_j == desired_x:
  *             result_real = fp_at_j_real
  *             result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
  *         else:
  *             fp_at_jp1 = dependent_values[j + 1]
  */
       __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
 
-      /* "CyRK/array/interp.pyx":240
+      /* "CyRK/array/interp.pyx":474
  *             result_real = fp_at_j_real
  *             result_imag = fp_at_j_imag
  *         elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
  *             result_real = fp_at_j_real
  *             result_imag = fp_at_j_imag
  */
-      goto __pyx_L4;
+      goto __pyx_L5;
     }
 
-    /* "CyRK/array/interp.pyx":244
+    /* "CyRK/array/interp.pyx":478
  *             result_imag = fp_at_j_imag
  *         else:
  *             fp_at_jp1 = dependent_values[j + 1]             # <<<<<<<<<<<<<<
  *             fp_at_jp1_real = fp_at_jp1.real
  *             fp_at_jp1_imag = fp_at_jp1.imag
  */
     /*else*/ {
       __pyx_t_2 = (__pyx_v_j + 1);
       __pyx_v_fp_at_jp1 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-      /* "CyRK/array/interp.pyx":245
+      /* "CyRK/array/interp.pyx":479
  *         else:
  *             fp_at_jp1 = dependent_values[j + 1]
  *             fp_at_jp1_real = fp_at_jp1.real             # <<<<<<<<<<<<<<
  *             fp_at_jp1_imag = fp_at_jp1.imag
  *             xp_at_jp1 = x_domain[j + 1]
  */
       __pyx_t_5 = __Pyx_CREAL(__pyx_v_fp_at_jp1);
       __pyx_v_fp_at_jp1_real = __pyx_t_5;
 
-      /* "CyRK/array/interp.pyx":246
+      /* "CyRK/array/interp.pyx":480
  *             fp_at_jp1 = dependent_values[j + 1]
  *             fp_at_jp1_real = fp_at_jp1.real
  *             fp_at_jp1_imag = fp_at_jp1.imag             # <<<<<<<<<<<<<<
  *             xp_at_jp1 = x_domain[j + 1]
  *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
  */
       __pyx_t_5 = __Pyx_CIMAG(__pyx_v_fp_at_jp1);
       __pyx_v_fp_at_jp1_imag = __pyx_t_5;
 
-      /* "CyRK/array/interp.pyx":247
+      /* "CyRK/array/interp.pyx":481
  *             fp_at_jp1_real = fp_at_jp1.real
  *             fp_at_jp1_imag = fp_at_jp1.imag
  *             xp_at_jp1 = x_domain[j + 1]             # <<<<<<<<<<<<<<
  *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
  *             slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
  */
       __pyx_t_2 = (__pyx_v_j + 1);
       __pyx_v_xp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_2 * __pyx_v_x_domain.strides[0]) )));
 
-      /* "CyRK/array/interp.pyx":248
+      /* "CyRK/array/interp.pyx":482
  *             fp_at_jp1_imag = fp_at_jp1.imag
  *             xp_at_jp1 = x_domain[j + 1]
  *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)             # <<<<<<<<<<<<<<
  *             slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
  *             slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse
  */
       __pyx_v_x_slope_inverse = (1.0 / (__pyx_v_xp_at_jp1 - __pyx_v_xp_at_j));
 
-      /* "CyRK/array/interp.pyx":249
+      /* "CyRK/array/interp.pyx":483
  *             xp_at_jp1 = x_domain[j + 1]
  *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
  *             slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse             # <<<<<<<<<<<<<<
  *             slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse
  * 
  */
       __pyx_v_slope_real = ((__pyx_v_fp_at_jp1_real - __pyx_v_fp_at_j_real) * __pyx_v_x_slope_inverse);
 
-      /* "CyRK/array/interp.pyx":250
+      /* "CyRK/array/interp.pyx":484
  *             x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
  *             slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
  *             slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse             # <<<<<<<<<<<<<<
  * 
  *             # If we get nan in one direction try the other
  */
       __pyx_v_slope_imag = ((__pyx_v_fp_at_jp1_imag - __pyx_v_fp_at_j_imag) * __pyx_v_x_slope_inverse);
 
-      /* "CyRK/array/interp.pyx":254
+      /* "CyRK/array/interp.pyx":488
  *             # If we get nan in one direction try the other
  *             # Real Part
  *             result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real             # <<<<<<<<<<<<<<
  *             if isnan(result_real):
  *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  */
       __pyx_v_result_real = ((__pyx_v_slope_real * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j_real);
 
-      /* "CyRK/array/interp.pyx":255
+      /* "CyRK/array/interp.pyx":489
  *             # Real Part
  *             result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
  *             if isnan(result_real):             # <<<<<<<<<<<<<<
  *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
  */
-      __pyx_t_4 = isnan(__pyx_v_result_real);
-      if (__pyx_t_4) {
+      __pyx_t_3 = isnan(__pyx_v_result_real);
+      if (__pyx_t_3) {
 
-        /* "CyRK/array/interp.pyx":256
+        /* "CyRK/array/interp.pyx":490
  *             result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
  *             if isnan(result_real):
  *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real             # <<<<<<<<<<<<<<
  *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
  *                     result_real = fp_at_j_real
  */
         __pyx_v_result_real = ((__pyx_v_slope_real * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1_real);
 
-        /* "CyRK/array/interp.pyx":257
+        /* "CyRK/array/interp.pyx":491
  *             if isnan(result_real):
  *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):             # <<<<<<<<<<<<<<
  *                     result_real = fp_at_j_real
  * 
  */
         __pyx_t_7 = isnan(__pyx_v_result_real);
         if (__pyx_t_7) {
         } else {
-          __pyx_t_4 = __pyx_t_7;
-          goto __pyx_L7_bool_binop_done;
+          __pyx_t_3 = __pyx_t_7;
+          goto __pyx_L8_bool_binop_done;
         }
         __pyx_t_7 = (__pyx_v_fp_at_jp1_real == __pyx_v_fp_at_j_real);
-        __pyx_t_4 = __pyx_t_7;
-        __pyx_L7_bool_binop_done:;
-        if (__pyx_t_4) {
+        __pyx_t_3 = __pyx_t_7;
+        __pyx_L8_bool_binop_done:;
+        if (__pyx_t_3) {
 
-          /* "CyRK/array/interp.pyx":258
+          /* "CyRK/array/interp.pyx":492
  *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
  *                     result_real = fp_at_j_real             # <<<<<<<<<<<<<<
  * 
  *             # Imaginary Part
  */
           __pyx_v_result_real = __pyx_v_fp_at_j_real;
 
-          /* "CyRK/array/interp.pyx":257
+          /* "CyRK/array/interp.pyx":491
  *             if isnan(result_real):
  *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):             # <<<<<<<<<<<<<<
  *                     result_real = fp_at_j_real
  * 
  */
         }
 
-        /* "CyRK/array/interp.pyx":255
+        /* "CyRK/array/interp.pyx":489
  *             # Real Part
  *             result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
  *             if isnan(result_real):             # <<<<<<<<<<<<<<
  *                 result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                 if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
  */
       }
 
-      /* "CyRK/array/interp.pyx":261
+      /* "CyRK/array/interp.pyx":495
  * 
  *             # Imaginary Part
  *             result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag             # <<<<<<<<<<<<<<
  *             if isnan(result_imag):
  *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  */
       __pyx_v_result_imag = ((__pyx_v_slope_imag * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j_imag);
 
-      /* "CyRK/array/interp.pyx":262
+      /* "CyRK/array/interp.pyx":496
  *             # Imaginary Part
  *             result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
  *             if isnan(result_imag):             # <<<<<<<<<<<<<<
  *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
  */
-      __pyx_t_4 = isnan(__pyx_v_result_imag);
-      if (__pyx_t_4) {
+      __pyx_t_3 = isnan(__pyx_v_result_imag);
+      if (__pyx_t_3) {
 
-        /* "CyRK/array/interp.pyx":263
+        /* "CyRK/array/interp.pyx":497
  *             result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
  *             if isnan(result_imag):
  *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag             # <<<<<<<<<<<<<<
  *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
  *                     result_imag = fp_at_j_imag
  */
         __pyx_v_result_imag = ((__pyx_v_slope_imag * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1_imag);
 
-        /* "CyRK/array/interp.pyx":264
+        /* "CyRK/array/interp.pyx":498
  *             if isnan(result_imag):
  *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):             # <<<<<<<<<<<<<<
  *                     result_imag = fp_at_j_imag
  * 
  */
         __pyx_t_7 = isnan(__pyx_v_result_imag);
         if (__pyx_t_7) {
         } else {
-          __pyx_t_4 = __pyx_t_7;
-          goto __pyx_L11_bool_binop_done;
+          __pyx_t_3 = __pyx_t_7;
+          goto __pyx_L12_bool_binop_done;
         }
         __pyx_t_7 = (__pyx_v_fp_at_jp1_imag == __pyx_v_fp_at_j_imag);
-        __pyx_t_4 = __pyx_t_7;
-        __pyx_L11_bool_binop_done:;
-        if (__pyx_t_4) {
+        __pyx_t_3 = __pyx_t_7;
+        __pyx_L12_bool_binop_done:;
+        if (__pyx_t_3) {
 
-          /* "CyRK/array/interp.pyx":265
+          /* "CyRK/array/interp.pyx":499
  *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
  *                     result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
  * 
  *     cdef double complex result
  */
           __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
 
-          /* "CyRK/array/interp.pyx":264
+          /* "CyRK/array/interp.pyx":498
  *             if isnan(result_imag):
  *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):             # <<<<<<<<<<<<<<
  *                     result_imag = fp_at_j_imag
  * 
  */
         }
 
-        /* "CyRK/array/interp.pyx":262
+        /* "CyRK/array/interp.pyx":496
  *             # Imaginary Part
  *             result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
  *             if isnan(result_imag):             # <<<<<<<<<<<<<<
  *                 result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                 if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
  */
       }
     }
-    __pyx_L4:;
+    __pyx_L5:;
   }
-  __pyx_L3:;
+  __pyx_L4:;
 
-  /* "CyRK/array/interp.pyx":268
+  /* "CyRK/array/interp.pyx":502
  * 
  *     cdef double complex result
  *     result = result_real + 1.0j * result_imag             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   __pyx_v_result = __Pyx_c_sum_double(__pyx_t_double_complex_from_parts(__pyx_v_result_real, 0), __Pyx_c_prod_double(__pyx_t_double_complex_from_parts(0, 1.0), __pyx_t_double_complex_from_parts(__pyx_v_result_imag, 0)));
 
-  /* "CyRK/array/interp.pyx":270
+  /* "CyRK/array/interp.pyx":504
  *     result = result_real + 1.0j * result_imag
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "CyRK/array/interp.pyx":170
+  /* "CyRK/array/interp.pyx":393
  * 
  * 
  * cpdef double complex interp_complex(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
- *                                     double complex[:] dependent_values) nogil:
+ *                                     double complex[:] dependent_values, int provided_j = -1) nogil:
  *     """ Interpolation function for complex numbers.
  */
 
   /* function exit code */
   __pyx_L1_error:;
   #ifdef WITH_THREAD
   __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
@@ -20259,152 +21893,172 @@
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4CyRK_5array_6interp_3interp_complex(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4CyRK_5array_6interp_7interp_complex(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-PyDoc_STRVAR(__pyx_doc_4CyRK_5array_6interp_2interp_complex, " Interpolation function for complex numbers.\n\n    Provided a domain, `desired_x` and a dependent array `dependent_values` search domain for value closest to \n    `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local \n    slopes of `desired_x` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.\n\n    Based on `numpy`'s `interp` function.\n\n    Parameters\n    ----------\n    desired_x : float\n        Location where `dependent_variables` is desired.\n    x_domain : np.ndarray[float]\n        Domain to search for the correct location.\n    dependent_values : np.ndarray[complex]\n        Dependent values that are to be returned after search and interpolation.\n\n    Returns\n    -------\n    result : complex\n        Desired value of `dependent_values`.\n\n    ");
-static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_3interp_complex = {"interp_complex", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_3interp_complex, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_4CyRK_5array_6interp_2interp_complex};
-static PyObject *__pyx_pw_4CyRK_5array_6interp_3interp_complex(PyObject *__pyx_self, 
+PyDoc_STRVAR(__pyx_doc_4CyRK_5array_6interp_6interp_complex, " Interpolation function for complex numbers.\n\n    Provided a domain, `desired_x` and a dependent array `dependent_values` search domain for value closest to \n    `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local \n    slopes of `desired_x` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.\n\n    Based on `numpy`'s `interp` function.\n\n    Parameters\n    ----------\n    desired_x : float\n        Location where `dependent_variables` is desired.\n    x_domain : np.ndarray[float]\n        Domain to search for the correct location.\n    dependent_values : np.ndarray[complex]\n        Dependent values that are to be returned after search and interpolation.\n    provided_j : int\n        Give a j index from a previous interpolation to improve performance.\n\n    Returns\n    -------\n    result : complex\n        Desired value of `dependent_values`.\n\n    ");
+static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_7interp_complex = {"interp_complex", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_7interp_complex, __Pyx_METH_FASTCALL|METH_KEYWORDS, __pyx_doc_4CyRK_5array_6interp_6interp_complex};
+static PyObject *__pyx_pw_4CyRK_5array_6interp_7interp_complex(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   double __pyx_v_desired_x;
   __Pyx_memviewslice __pyx_v_x_domain = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_dependent_values = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_v_provided_j;
   #if !CYTHON_METH_FASTCALL
   CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
   #endif
   CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("interp_complex (wrapper)", 0);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_desired_x,&__pyx_n_s_x_domain,&__pyx_n_s_dependent_values,0};
-    PyObject* values[3] = {0,0,0};
+    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_desired_x,&__pyx_n_s_x_domain,&__pyx_n_s_dependent_values,&__pyx_n_s_provided_j,0};
+    PyObject* values[4] = {0,0,0,0};
     if (__pyx_kwds) {
       Py_ssize_t kw_args;
       switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
         case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
         case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_desired_x)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 170, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x_domain)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 170, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp_complex", 1, 3, 3, 1); __PYX_ERR(1, 170, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp_complex", 0, 3, 4, 1); __PYX_ERR(1, 393, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dependent_values)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 170, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp_complex", 1, 3, 3, 2); __PYX_ERR(1, 170, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp_complex", 0, 3, 4, 2); __PYX_ERR(1, 393, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_provided_j);
+          if (value) { values[3] = value; kw_args--; }
+          else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp_complex") < 0)) __PYX_ERR(1, 170, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp_complex") < 0)) __PYX_ERR(1, 393, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 3)) {
-      goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      switch (__pyx_nargs) {
+        case  4: values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+        values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_desired_x = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_desired_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L3_error)
+    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 393, __pyx_L3_error)
+    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 394, __pyx_L3_error)
+    if (values[3]) {
+      __pyx_v_provided_j = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_provided_j == (int)-1) && PyErr_Occurred())) __PYX_ERR(1, 394, __pyx_L3_error)
+    } else {
+      __pyx_v_provided_j = ((int)-1);
     }
-    __pyx_v_desired_x = __pyx_PyFloat_AsDouble(values[0]); if (unlikely((__pyx_v_desired_x == (double)-1) && PyErr_Occurred())) __PYX_ERR(1, 170, __pyx_L3_error)
-    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 170, __pyx_L3_error)
-    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 171, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("interp_complex", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 170, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("interp_complex", 0, 3, 4, __pyx_nargs); __PYX_ERR(1, 393, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
   __Pyx_AddTraceback("CyRK.array.interp.interp_complex", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4CyRK_5array_6interp_2interp_complex(__pyx_self, __pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values);
+  __pyx_r = __pyx_pf_4CyRK_5array_6interp_6interp_complex(__pyx_self, __pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_provided_j);
 
   /* function exit code */
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4CyRK_5array_6interp_2interp_complex(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values) {
+static PyObject *__pyx_pf_4CyRK_5array_6interp_6interp_complex(CYTHON_UNUSED PyObject *__pyx_self, double __pyx_v_desired_x, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, int __pyx_v_provided_j) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __pyx_t_double_complex __pyx_t_1;
-  PyObject *__pyx_t_2 = NULL;
+  struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex __pyx_t_2;
+  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("interp_complex", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_x_domain.memview)) { __Pyx_RaiseUnboundLocalError("x_domain"); __PYX_ERR(1, 170, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_dependent_values.memview)) { __Pyx_RaiseUnboundLocalError("dependent_values"); __PYX_ERR(1, 170, __pyx_L1_error) }
-  __pyx_t_1 = __pyx_f_4CyRK_5array_6interp_interp_complex(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 170, __pyx_L1_error)
-  __pyx_t_2 = __pyx_PyComplex_FromComplex(__pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 170, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
-  __pyx_r = __pyx_t_2;
-  __pyx_t_2 = 0;
+  __pyx_t_2.__pyx_n = 1;
+  __pyx_t_2.provided_j = __pyx_v_provided_j;
+  __pyx_t_1 = __pyx_f_4CyRK_5array_6interp_interp_complex(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_dependent_values, 0, &__pyx_t_2); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 393, __pyx_L1_error)
+  __pyx_t_3 = __pyx_PyComplex_FromComplex(__pyx_t_1); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 393, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_r = __pyx_t_3;
+  __pyx_t_3 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
   __Pyx_AddTraceback("CyRK.array.interp.interp_complex", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "CyRK/array/interp.pyx":273
+/* "CyRK/array/interp.pyx":507
  * 
  * 
  * cpdef void interp_array(double[:] desired_x_array, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
  *                         double[:] desired_dependent_array) nogil:
  * 
  */
 
-static PyObject *__pyx_pw_4CyRK_5array_6interp_5interp_array(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4CyRK_5array_6interp_9interp_array(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 static void __pyx_f_4CyRK_5array_6interp_interp_array(__Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array, CYTHON_UNUSED int __pyx_skip_dispatch) {
@@ -20434,92 +22088,92 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
 
-  /* "CyRK/array/interp.pyx":279
+  /* "CyRK/array/interp.pyx":513
  *     cdef Py_ssize_t index
  *     cdef unsigned int desired_len
  *     desired_len = len(desired_x_array)             # <<<<<<<<<<<<<<
  * 
  *     # Interpolation variables
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_desired_x_array); 
   __pyx_v_desired_len = __pyx_t_1;
 
-  /* "CyRK/array/interp.pyx":283
+  /* "CyRK/array/interp.pyx":517
  *     # Interpolation variables
  *     cdef unsigned int lenx
  *     lenx = len(x_domain)             # <<<<<<<<<<<<<<
  *     cdef double left_value
  *     left_value = dependent_values[0]
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_x_domain); 
   __pyx_v_lenx = __pyx_t_1;
 
-  /* "CyRK/array/interp.pyx":285
+  /* "CyRK/array/interp.pyx":519
  *     lenx = len(x_domain)
  *     cdef double left_value
  *     left_value = dependent_values[0]             # <<<<<<<<<<<<<<
  *     cdef double right_value
  *     right_value = dependent_values[lenx - 1]
  */
   __pyx_t_2 = 0;
   __pyx_v_left_value = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-  /* "CyRK/array/interp.pyx":287
+  /* "CyRK/array/interp.pyx":521
  *     left_value = dependent_values[0]
  *     cdef double right_value
  *     right_value = dependent_values[lenx - 1]             # <<<<<<<<<<<<<<
  * 
  *     # Binary Search with Guess
  */
   __pyx_t_2 = (__pyx_v_lenx - 1);
   __pyx_v_right_value = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-  /* "CyRK/array/interp.pyx":305
+  /* "CyRK/array/interp.pyx":539
  *     cdef double x_slope
  *     cdef unsigned int guess
  *     x_slope = lenx / desired_len             # <<<<<<<<<<<<<<
  *     if x_slope < 1.:
  *         x_slope = 1.
  */
   __pyx_v_x_slope = (__pyx_v_lenx / __pyx_v_desired_len);
 
-  /* "CyRK/array/interp.pyx":306
+  /* "CyRK/array/interp.pyx":540
  *     cdef unsigned int guess
  *     x_slope = lenx / desired_len
  *     if x_slope < 1.:             # <<<<<<<<<<<<<<
  *         x_slope = 1.
  * 
  */
   __pyx_t_3 = (__pyx_v_x_slope < 1.);
   if (__pyx_t_3) {
 
-    /* "CyRK/array/interp.pyx":307
+    /* "CyRK/array/interp.pyx":541
  *     x_slope = lenx / desired_len
  *     if x_slope < 1.:
  *         x_slope = 1.             # <<<<<<<<<<<<<<
  * 
  *     cdef double desired_x
  */
     __pyx_v_x_slope = 1.;
 
-    /* "CyRK/array/interp.pyx":306
+    /* "CyRK/array/interp.pyx":540
  *     cdef unsigned int guess
  *     x_slope = lenx / desired_len
  *     if x_slope < 1.:             # <<<<<<<<<<<<<<
  *         x_slope = 1.
  * 
  */
   }
 
-  /* "CyRK/array/interp.pyx":310
+  /* "CyRK/array/interp.pyx":544
  * 
  *     cdef double desired_x
  *     for index in prange(desired_len, nogil=True):             # <<<<<<<<<<<<<<
  *         desired_x = desired_x_array[index]
  * 
  */
   {
@@ -20581,239 +22235,239 @@
                             __pyx_v_guess = ((unsigned int)0xbad0bad0);
                             __pyx_v_j = ((unsigned int)0xbad0bad0);
                             __pyx_v_result = ((double)__PYX_NAN());
                             __pyx_v_slope = ((double)__PYX_NAN());
                             __pyx_v_xp_at_j = ((double)__PYX_NAN());
                             __pyx_v_xp_at_jp1 = ((double)__PYX_NAN());
 
-                            /* "CyRK/array/interp.pyx":311
+                            /* "CyRK/array/interp.pyx":545
  *     cdef double desired_x
  *     for index in prange(desired_len, nogil=True):
  *         desired_x = desired_x_array[index]             # <<<<<<<<<<<<<<
  * 
  *         # Perform binary search with guess
  */
                             __pyx_t_2 = __pyx_v_index;
                             __pyx_v_desired_x = (*((double *) ( /* dim=0 */ (__pyx_v_desired_x_array.data + __pyx_t_2 * __pyx_v_desired_x_array.strides[0]) )));
 
-                            /* "CyRK/array/interp.pyx":314
+                            /* "CyRK/array/interp.pyx":548
  * 
  *         # Perform binary search with guess
  *         guess = <unsigned int>x_slope * index             # <<<<<<<<<<<<<<
  *         j = binary_search_with_guess(desired_x, x_domain, lenx, guess)
  * 
  */
                             __pyx_v_guess = (((unsigned int)__pyx_v_x_slope) * __pyx_v_index);
 
-                            /* "CyRK/array/interp.pyx":315
+                            /* "CyRK/array/interp.pyx":549
  *         # Perform binary search with guess
  *         guess = <unsigned int>x_slope * index
  *         j = binary_search_with_guess(desired_x, x_domain, lenx, guess)             # <<<<<<<<<<<<<<
  * 
  *         if j == 0:
  */
-                            __pyx_t_6 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_guess); if (unlikely(__pyx_t_6 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 315, __pyx_L9_error)
+                            __pyx_t_6 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_guess); if (unlikely(__pyx_t_6 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 549, __pyx_L9_error)
                             __pyx_v_j = __pyx_t_6;
 
-                            /* "CyRK/array/interp.pyx":317
+                            /* "CyRK/array/interp.pyx":551
  *         j = binary_search_with_guess(desired_x, x_domain, lenx, guess)
  * 
  *         if j == 0:             # <<<<<<<<<<<<<<
  *             result = left_value
  *         elif j == lenx:
  */
                             __pyx_t_3 = (__pyx_v_j == 0);
                             if (__pyx_t_3) {
 
-                              /* "CyRK/array/interp.pyx":318
+                              /* "CyRK/array/interp.pyx":552
  * 
  *         if j == 0:
  *             result = left_value             # <<<<<<<<<<<<<<
  *         elif j == lenx:
  *             result = right_value
  */
                               __pyx_v_result = __pyx_v_left_value;
 
-                              /* "CyRK/array/interp.pyx":317
+                              /* "CyRK/array/interp.pyx":551
  *         j = binary_search_with_guess(desired_x, x_domain, lenx, guess)
  * 
  *         if j == 0:             # <<<<<<<<<<<<<<
  *             result = left_value
  *         elif j == lenx:
  */
                               goto __pyx_L11;
                             }
 
-                            /* "CyRK/array/interp.pyx":319
+                            /* "CyRK/array/interp.pyx":553
  *         if j == 0:
  *             result = left_value
  *         elif j == lenx:             # <<<<<<<<<<<<<<
  *             result = right_value
  *         else:
  */
                             __pyx_t_3 = (__pyx_v_j == __pyx_v_lenx);
                             if (__pyx_t_3) {
 
-                              /* "CyRK/array/interp.pyx":320
+                              /* "CyRK/array/interp.pyx":554
  *             result = left_value
  *         elif j == lenx:
  *             result = right_value             # <<<<<<<<<<<<<<
  *         else:
  *             fp_at_j = dependent_values[j]
  */
                               __pyx_v_result = __pyx_v_right_value;
 
-                              /* "CyRK/array/interp.pyx":319
+                              /* "CyRK/array/interp.pyx":553
  *         if j == 0:
  *             result = left_value
  *         elif j == lenx:             # <<<<<<<<<<<<<<
  *             result = right_value
  *         else:
  */
                               goto __pyx_L11;
                             }
 
-                            /* "CyRK/array/interp.pyx":322
+                            /* "CyRK/array/interp.pyx":556
  *             result = right_value
  *         else:
  *             fp_at_j = dependent_values[j]             # <<<<<<<<<<<<<<
  *             xp_at_j = x_domain[j]
  *             if j == lenx - 1:
  */
                             /*else*/ {
                               __pyx_t_7 = __pyx_v_j;
                               __pyx_v_fp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_7 * __pyx_v_dependent_values.strides[0]) )));
 
-                              /* "CyRK/array/interp.pyx":323
+                              /* "CyRK/array/interp.pyx":557
  *         else:
  *             fp_at_j = dependent_values[j]
  *             xp_at_j = x_domain[j]             # <<<<<<<<<<<<<<
  *             if j == lenx - 1:
  *                 result = fp_at_j
  */
                               __pyx_t_7 = __pyx_v_j;
                               __pyx_v_xp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_7 * __pyx_v_x_domain.strides[0]) )));
 
-                              /* "CyRK/array/interp.pyx":324
+                              /* "CyRK/array/interp.pyx":558
  *             fp_at_j = dependent_values[j]
  *             xp_at_j = x_domain[j]
  *             if j == lenx - 1:             # <<<<<<<<<<<<<<
  *                 result = fp_at_j
  *             elif xp_at_j == desired_x:
  */
                               __pyx_t_3 = (__pyx_v_j == (__pyx_v_lenx - 1));
                               if (__pyx_t_3) {
 
-                                /* "CyRK/array/interp.pyx":325
+                                /* "CyRK/array/interp.pyx":559
  *             xp_at_j = x_domain[j]
  *             if j == lenx - 1:
  *                 result = fp_at_j             # <<<<<<<<<<<<<<
  *             elif xp_at_j == desired_x:
  *                 result = fp_at_j
  */
                                 __pyx_v_result = __pyx_v_fp_at_j;
 
-                                /* "CyRK/array/interp.pyx":324
+                                /* "CyRK/array/interp.pyx":558
  *             fp_at_j = dependent_values[j]
  *             xp_at_j = x_domain[j]
  *             if j == lenx - 1:             # <<<<<<<<<<<<<<
  *                 result = fp_at_j
  *             elif xp_at_j == desired_x:
  */
                                 goto __pyx_L12;
                               }
 
-                              /* "CyRK/array/interp.pyx":326
+                              /* "CyRK/array/interp.pyx":560
  *             if j == lenx - 1:
  *                 result = fp_at_j
  *             elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
  *                 result = fp_at_j
  *             else:
  */
                               __pyx_t_3 = (__pyx_v_xp_at_j == __pyx_v_desired_x);
                               if (__pyx_t_3) {
 
-                                /* "CyRK/array/interp.pyx":327
+                                /* "CyRK/array/interp.pyx":561
  *                 result = fp_at_j
  *             elif xp_at_j == desired_x:
  *                 result = fp_at_j             # <<<<<<<<<<<<<<
  *             else:
  *                 fp_at_jp1 = dependent_values[j + 1]
  */
                                 __pyx_v_result = __pyx_v_fp_at_j;
 
-                                /* "CyRK/array/interp.pyx":326
+                                /* "CyRK/array/interp.pyx":560
  *             if j == lenx - 1:
  *                 result = fp_at_j
  *             elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
  *                 result = fp_at_j
  *             else:
  */
                                 goto __pyx_L12;
                               }
 
-                              /* "CyRK/array/interp.pyx":329
+                              /* "CyRK/array/interp.pyx":563
  *                 result = fp_at_j
  *             else:
  *                 fp_at_jp1 = dependent_values[j + 1]             # <<<<<<<<<<<<<<
  *                 xp_at_jp1 = x_domain[j + 1]
  *                 slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)
  */
                               /*else*/ {
                                 __pyx_t_2 = (__pyx_v_j + 1);
                                 __pyx_v_fp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-                                /* "CyRK/array/interp.pyx":330
+                                /* "CyRK/array/interp.pyx":564
  *             else:
  *                 fp_at_jp1 = dependent_values[j + 1]
  *                 xp_at_jp1 = x_domain[j + 1]             # <<<<<<<<<<<<<<
  *                 slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)
  * 
  */
                                 __pyx_t_2 = (__pyx_v_j + 1);
                                 __pyx_v_xp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_2 * __pyx_v_x_domain.strides[0]) )));
 
-                                /* "CyRK/array/interp.pyx":331
+                                /* "CyRK/array/interp.pyx":565
  *                 fp_at_jp1 = dependent_values[j + 1]
  *                 xp_at_jp1 = x_domain[j + 1]
  *                 slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)             # <<<<<<<<<<<<<<
  * 
  *                 # If we get nan in one direction, try the other
  */
                                 __pyx_v_slope = ((__pyx_v_fp_at_jp1 - __pyx_v_fp_at_j) / (__pyx_v_xp_at_jp1 - __pyx_v_xp_at_j));
 
-                                /* "CyRK/array/interp.pyx":334
+                                /* "CyRK/array/interp.pyx":568
  * 
  *                 # If we get nan in one direction, try the other
  *                 result = slope * (desired_x - xp_at_j) + fp_at_j             # <<<<<<<<<<<<<<
  *                 if isnan(result):
  *                     result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  */
                                 __pyx_v_result = ((__pyx_v_slope * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j);
 
-                                /* "CyRK/array/interp.pyx":335
+                                /* "CyRK/array/interp.pyx":569
  *                 # If we get nan in one direction, try the other
  *                 result = slope * (desired_x - xp_at_j) + fp_at_j
  *                 if isnan(result):             # <<<<<<<<<<<<<<
  *                     result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                     if isnan(result) and (fp_at_jp1 == fp_at_j):
  */
                                 __pyx_t_3 = isnan(__pyx_v_result);
                                 if (__pyx_t_3) {
 
-                                  /* "CyRK/array/interp.pyx":336
+                                  /* "CyRK/array/interp.pyx":570
  *                 result = slope * (desired_x - xp_at_j) + fp_at_j
  *                 if isnan(result):
  *                     result = slope * (desired_x - xp_at_jp1) + fp_at_jp1             # <<<<<<<<<<<<<<
  *                     if isnan(result) and (fp_at_jp1 == fp_at_j):
  *                         result = fp_at_j
  */
                                   __pyx_v_result = ((__pyx_v_slope * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1);
 
-                                  /* "CyRK/array/interp.pyx":337
+                                  /* "CyRK/array/interp.pyx":571
  *                 if isnan(result):
  *                     result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                     if isnan(result) and (fp_at_jp1 == fp_at_j):             # <<<<<<<<<<<<<<
  *                         result = fp_at_j
  * 
  */
                                   __pyx_t_8 = isnan(__pyx_v_result);
@@ -20823,46 +22477,46 @@
                                     goto __pyx_L15_bool_binop_done;
                                   }
                                   __pyx_t_8 = (__pyx_v_fp_at_jp1 == __pyx_v_fp_at_j);
                                   __pyx_t_3 = __pyx_t_8;
                                   __pyx_L15_bool_binop_done:;
                                   if (__pyx_t_3) {
 
-                                    /* "CyRK/array/interp.pyx":338
+                                    /* "CyRK/array/interp.pyx":572
  *                     result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                     if isnan(result) and (fp_at_jp1 == fp_at_j):
  *                         result = fp_at_j             # <<<<<<<<<<<<<<
  * 
  *         desired_dependent_array[index] = result
  */
                                     __pyx_v_result = __pyx_v_fp_at_j;
 
-                                    /* "CyRK/array/interp.pyx":337
+                                    /* "CyRK/array/interp.pyx":571
  *                 if isnan(result):
  *                     result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                     if isnan(result) and (fp_at_jp1 == fp_at_j):             # <<<<<<<<<<<<<<
  *                         result = fp_at_j
  * 
  */
                                   }
 
-                                  /* "CyRK/array/interp.pyx":335
+                                  /* "CyRK/array/interp.pyx":569
  *                 # If we get nan in one direction, try the other
  *                 result = slope * (desired_x - xp_at_j) + fp_at_j
  *                 if isnan(result):             # <<<<<<<<<<<<<<
  *                     result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
  *                     if isnan(result) and (fp_at_jp1 == fp_at_j):
  */
                                 }
                               }
                               __pyx_L12:;
                             }
                             __pyx_L11:;
 
-                            /* "CyRK/array/interp.pyx":340
+                            /* "CyRK/array/interp.pyx":574
  *                         result = fp_at_j
  * 
  *         desired_dependent_array[index] = result             # <<<<<<<<<<<<<<
  * 
  * 
  */
                             __pyx_t_2 = __pyx_v_index;
@@ -20962,15 +22616,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "CyRK/array/interp.pyx":310
+      /* "CyRK/array/interp.pyx":544
  * 
  *     cdef double desired_x
  *     for index in prange(desired_len, nogil=True):             # <<<<<<<<<<<<<<
  *         desired_x = desired_x_array[index]
  * 
  */
       /*finally:*/ {
@@ -20992,15 +22646,15 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L6:;
       }
   }
 
-  /* "CyRK/array/interp.pyx":273
+  /* "CyRK/array/interp.pyx":507
  * 
  * 
  * cpdef void interp_array(double[:] desired_x_array, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
  *                         double[:] desired_dependent_array) nogil:
  * 
  */
 
@@ -21014,23 +22668,23 @@
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4CyRK_5array_6interp_5interp_array(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4CyRK_5array_6interp_9interp_array(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_5interp_array = {"interp_array", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_5interp_array, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_4CyRK_5array_6interp_5interp_array(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_9interp_array = {"interp_array", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_9interp_array, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4CyRK_5array_6interp_9interp_array(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __Pyx_memviewslice __pyx_v_desired_x_array = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -21064,93 +22718,89 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_desired_x_array)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 507, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x_domain)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 507, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp_array", 1, 4, 4, 1); __PYX_ERR(1, 273, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp_array", 1, 4, 4, 1); __PYX_ERR(1, 507, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dependent_values)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 507, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp_array", 1, 4, 4, 2); __PYX_ERR(1, 273, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp_array", 1, 4, 4, 2); __PYX_ERR(1, 507, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_desired_dependent_array)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 507, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp_array", 1, 4, 4, 3); __PYX_ERR(1, 273, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp_array", 1, 4, 4, 3); __PYX_ERR(1, 507, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp_array") < 0)) __PYX_ERR(1, 273, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp_array") < 0)) __PYX_ERR(1, 507, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_desired_x_array = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_desired_x_array.memview)) __PYX_ERR(1, 273, __pyx_L3_error)
-    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 273, __pyx_L3_error)
-    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 273, __pyx_L3_error)
-    __pyx_v_desired_dependent_array = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_desired_dependent_array.memview)) __PYX_ERR(1, 274, __pyx_L3_error)
+    __pyx_v_desired_x_array = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_desired_x_array.memview)) __PYX_ERR(1, 507, __pyx_L3_error)
+    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 507, __pyx_L3_error)
+    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 507, __pyx_L3_error)
+    __pyx_v_desired_dependent_array = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_desired_dependent_array.memview)) __PYX_ERR(1, 508, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("interp_array", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 273, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("interp_array", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 507, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_desired_x_array, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_desired_dependent_array, 1);
   __Pyx_AddTraceback("CyRK.array.interp.interp_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4CyRK_5array_6interp_4interp_array(__pyx_self, __pyx_v_desired_x_array, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_desired_dependent_array);
+  __pyx_r = __pyx_pf_4CyRK_5array_6interp_8interp_array(__pyx_self, __pyx_v_desired_x_array, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_desired_dependent_array);
 
   /* function exit code */
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_desired_x_array, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_desired_dependent_array, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4CyRK_5array_6interp_4interp_array(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array) {
+static PyObject *__pyx_pf_4CyRK_5array_6interp_8interp_array(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("interp_array", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_desired_x_array.memview)) { __Pyx_RaiseUnboundLocalError("desired_x_array"); __PYX_ERR(1, 273, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_x_domain.memview)) { __Pyx_RaiseUnboundLocalError("x_domain"); __PYX_ERR(1, 273, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_dependent_values.memview)) { __Pyx_RaiseUnboundLocalError("dependent_values"); __PYX_ERR(1, 273, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_desired_dependent_array.memview)) { __Pyx_RaiseUnboundLocalError("desired_dependent_array"); __PYX_ERR(1, 273, __pyx_L1_error) }
-  __pyx_f_4CyRK_5array_6interp_interp_array(__pyx_v_desired_x_array, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_desired_dependent_array, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 273, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 273, __pyx_L1_error)
+  __pyx_f_4CyRK_5array_6interp_interp_array(__pyx_v_desired_x_array, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_desired_dependent_array, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 507, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 507, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -21159,23 +22809,23 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "CyRK/array/interp.pyx":343
+/* "CyRK/array/interp.pyx":577
  * 
  * 
  * cpdef void interp_complex_array(double[:] desired_x_array, double[:] x_domain, double complex[:] dependent_values,             # <<<<<<<<<<<<<<
  *                                 double complex[:] desired_dependent_array) nogil:
  * 
  */
 
-static PyObject *__pyx_pw_4CyRK_5array_6interp_7interp_complex_array(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4CyRK_5array_6interp_11interp_complex_array(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
 static void __pyx_f_4CyRK_5array_6interp_interp_complex_array(__Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array, CYTHON_UNUSED int __pyx_skip_dispatch) {
@@ -21214,92 +22864,92 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   #ifdef WITH_THREAD
   PyGILState_STATE __pyx_gilstate_save;
   #endif
 
-  /* "CyRK/array/interp.pyx":349
+  /* "CyRK/array/interp.pyx":583
  *     cdef Py_ssize_t index
  *     cdef unsigned int desired_len
  *     desired_len = len(desired_x_array)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_desired_x_array); 
   __pyx_v_desired_len = __pyx_t_1;
 
-  /* "CyRK/array/interp.pyx":353
+  /* "CyRK/array/interp.pyx":587
  * 
  *     cdef unsigned int lenx
  *     lenx = len(x_domain)             # <<<<<<<<<<<<<<
  *     # Note: Needs to be at least 3 item long array. Add exception here?
  * 
  */
   __pyx_t_1 = __Pyx_MemoryView_Len(__pyx_v_x_domain); 
   __pyx_v_lenx = __pyx_t_1;
 
-  /* "CyRK/array/interp.pyx":358
+  /* "CyRK/array/interp.pyx":592
  *     # Interpolation variables
  *     cdef double complex left_value
  *     left_value = dependent_values[0]             # <<<<<<<<<<<<<<
  *     cdef double complex right_value
  *     right_value = dependent_values[lenx - 1]
  */
   __pyx_t_2 = 0;
   __pyx_v_left_value = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-  /* "CyRK/array/interp.pyx":360
+  /* "CyRK/array/interp.pyx":594
  *     left_value = dependent_values[0]
  *     cdef double complex right_value
  *     right_value = dependent_values[lenx - 1]             # <<<<<<<<<<<<<<
  * 
  *     # Binary Search with Guess
  */
   __pyx_t_2 = (__pyx_v_lenx - 1);
   __pyx_v_right_value = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-  /* "CyRK/array/interp.pyx":385
+  /* "CyRK/array/interp.pyx":619
  *     cdef double x_slope
  *     cdef unsigned int guess
  *     x_slope = lenx / desired_len             # <<<<<<<<<<<<<<
  *     if x_slope < 1.:
  *         x_slope = 1.
  */
   __pyx_v_x_slope = (__pyx_v_lenx / __pyx_v_desired_len);
 
-  /* "CyRK/array/interp.pyx":386
+  /* "CyRK/array/interp.pyx":620
  *     cdef unsigned int guess
  *     x_slope = lenx / desired_len
  *     if x_slope < 1.:             # <<<<<<<<<<<<<<
  *         x_slope = 1.
  * 
  */
   __pyx_t_3 = (__pyx_v_x_slope < 1.);
   if (__pyx_t_3) {
 
-    /* "CyRK/array/interp.pyx":387
+    /* "CyRK/array/interp.pyx":621
  *     x_slope = lenx / desired_len
  *     if x_slope < 1.:
  *         x_slope = 1.             # <<<<<<<<<<<<<<
  * 
  *     cdef double desired_x
  */
     __pyx_v_x_slope = 1.;
 
-    /* "CyRK/array/interp.pyx":386
+    /* "CyRK/array/interp.pyx":620
  *     cdef unsigned int guess
  *     x_slope = lenx / desired_len
  *     if x_slope < 1.:             # <<<<<<<<<<<<<<
  *         x_slope = 1.
  * 
  */
   }
 
-  /* "CyRK/array/interp.pyx":391
+  /* "CyRK/array/interp.pyx":625
  *     cdef double desired_x
  *     cdef double complex result
  *     for index in prange(desired_len, nogil=True):             # <<<<<<<<<<<<<<
  *         desired_x = desired_x_array[index]
  * 
  */
   {
@@ -21374,337 +23024,337 @@
                             __pyx_v_result_real = ((double)__PYX_NAN());
                             __pyx_v_slope_imag = ((double)__PYX_NAN());
                             __pyx_v_slope_real = ((double)__PYX_NAN());
                             __pyx_v_x_slope_inverse = ((double)__PYX_NAN());
                             __pyx_v_xp_at_j = ((double)__PYX_NAN());
                             __pyx_v_xp_at_jp1 = ((double)__PYX_NAN());
 
-                            /* "CyRK/array/interp.pyx":392
+                            /* "CyRK/array/interp.pyx":626
  *     cdef double complex result
  *     for index in prange(desired_len, nogil=True):
  *         desired_x = desired_x_array[index]             # <<<<<<<<<<<<<<
  * 
  *         # Perform binary search with guess
  */
                             __pyx_t_2 = __pyx_v_index;
                             __pyx_v_desired_x = (*((double *) ( /* dim=0 */ (__pyx_v_desired_x_array.data + __pyx_t_2 * __pyx_v_desired_x_array.strides[0]) )));
 
-                            /* "CyRK/array/interp.pyx":395
+                            /* "CyRK/array/interp.pyx":629
  * 
  *         # Perform binary search with guess
  *         guess = <unsigned int>x_slope * index             # <<<<<<<<<<<<<<
  *         # Perform binary search with guess
  *         j = binary_search_with_guess(desired_x, x_domain, lenx, guess)
  */
                             __pyx_v_guess = (((unsigned int)__pyx_v_x_slope) * __pyx_v_index);
 
-                            /* "CyRK/array/interp.pyx":397
+                            /* "CyRK/array/interp.pyx":631
  *         guess = <unsigned int>x_slope * index
  *         # Perform binary search with guess
  *         j = binary_search_with_guess(desired_x, x_domain, lenx, guess)             # <<<<<<<<<<<<<<
  * 
  *         if j == 0:
  */
-                            __pyx_t_6 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_guess); if (unlikely(__pyx_t_6 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 397, __pyx_L9_error)
+                            __pyx_t_6 = __pyx_f_4CyRK_5array_6interp_binary_search_with_guess(__pyx_v_desired_x, __pyx_v_x_domain, __pyx_v_lenx, __pyx_v_guess); if (unlikely(__pyx_t_6 == ((unsigned int)-1) && __Pyx_ErrOccurredWithGIL())) __PYX_ERR(1, 631, __pyx_L9_error)
                             __pyx_v_j = __pyx_t_6;
 
-                            /* "CyRK/array/interp.pyx":399
+                            /* "CyRK/array/interp.pyx":633
  *         j = binary_search_with_guess(desired_x, x_domain, lenx, guess)
  * 
  *         if j == 0:             # <<<<<<<<<<<<<<
  *             result_real = left_value.real
  *             result_imag = left_value.imag
  */
                             __pyx_t_3 = (__pyx_v_j == 0);
                             if (__pyx_t_3) {
 
-                              /* "CyRK/array/interp.pyx":400
+                              /* "CyRK/array/interp.pyx":634
  * 
  *         if j == 0:
  *             result_real = left_value.real             # <<<<<<<<<<<<<<
  *             result_imag = left_value.imag
  *         elif j == lenx:
  */
                               __pyx_t_7 = __Pyx_CREAL(__pyx_v_left_value);
                               __pyx_v_result_real = __pyx_t_7;
 
-                              /* "CyRK/array/interp.pyx":401
+                              /* "CyRK/array/interp.pyx":635
  *         if j == 0:
  *             result_real = left_value.real
  *             result_imag = left_value.imag             # <<<<<<<<<<<<<<
  *         elif j == lenx:
  *             result_real = right_value.real
  */
                               __pyx_t_7 = __Pyx_CIMAG(__pyx_v_left_value);
                               __pyx_v_result_imag = __pyx_t_7;
 
-                              /* "CyRK/array/interp.pyx":399
+                              /* "CyRK/array/interp.pyx":633
  *         j = binary_search_with_guess(desired_x, x_domain, lenx, guess)
  * 
  *         if j == 0:             # <<<<<<<<<<<<<<
  *             result_real = left_value.real
  *             result_imag = left_value.imag
  */
                               goto __pyx_L11;
                             }
 
-                            /* "CyRK/array/interp.pyx":402
+                            /* "CyRK/array/interp.pyx":636
  *             result_real = left_value.real
  *             result_imag = left_value.imag
  *         elif j == lenx:             # <<<<<<<<<<<<<<
  *             result_real = right_value.real
  *             result_imag = right_value.imag
  */
                             __pyx_t_3 = (__pyx_v_j == __pyx_v_lenx);
                             if (__pyx_t_3) {
 
-                              /* "CyRK/array/interp.pyx":403
+                              /* "CyRK/array/interp.pyx":637
  *             result_imag = left_value.imag
  *         elif j == lenx:
  *             result_real = right_value.real             # <<<<<<<<<<<<<<
  *             result_imag = right_value.imag
  *         else:
  */
                               __pyx_t_7 = __Pyx_CREAL(__pyx_v_right_value);
                               __pyx_v_result_real = __pyx_t_7;
 
-                              /* "CyRK/array/interp.pyx":404
+                              /* "CyRK/array/interp.pyx":638
  *         elif j == lenx:
  *             result_real = right_value.real
  *             result_imag = right_value.imag             # <<<<<<<<<<<<<<
  *         else:
  *             fp_at_j = dependent_values[j]
  */
                               __pyx_t_7 = __Pyx_CIMAG(__pyx_v_right_value);
                               __pyx_v_result_imag = __pyx_t_7;
 
-                              /* "CyRK/array/interp.pyx":402
+                              /* "CyRK/array/interp.pyx":636
  *             result_real = left_value.real
  *             result_imag = left_value.imag
  *         elif j == lenx:             # <<<<<<<<<<<<<<
  *             result_real = right_value.real
  *             result_imag = right_value.imag
  */
                               goto __pyx_L11;
                             }
 
-                            /* "CyRK/array/interp.pyx":406
+                            /* "CyRK/array/interp.pyx":640
  *             result_imag = right_value.imag
  *         else:
  *             fp_at_j = dependent_values[j]             # <<<<<<<<<<<<<<
  *             fp_at_j_real = fp_at_j.real
  *             fp_at_j_imag = fp_at_j.imag
  */
                             /*else*/ {
                               __pyx_t_8 = __pyx_v_j;
                               __pyx_v_fp_at_j = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_8 * __pyx_v_dependent_values.strides[0]) )));
 
-                              /* "CyRK/array/interp.pyx":407
+                              /* "CyRK/array/interp.pyx":641
  *         else:
  *             fp_at_j = dependent_values[j]
  *             fp_at_j_real = fp_at_j.real             # <<<<<<<<<<<<<<
  *             fp_at_j_imag = fp_at_j.imag
  *             xp_at_j = x_domain[j]
  */
                               __pyx_t_7 = __Pyx_CREAL(__pyx_v_fp_at_j);
                               __pyx_v_fp_at_j_real = __pyx_t_7;
 
-                              /* "CyRK/array/interp.pyx":408
+                              /* "CyRK/array/interp.pyx":642
  *             fp_at_j = dependent_values[j]
  *             fp_at_j_real = fp_at_j.real
  *             fp_at_j_imag = fp_at_j.imag             # <<<<<<<<<<<<<<
  *             xp_at_j = x_domain[j]
  *             if j == lenx - 1:
  */
                               __pyx_t_7 = __Pyx_CIMAG(__pyx_v_fp_at_j);
                               __pyx_v_fp_at_j_imag = __pyx_t_7;
 
-                              /* "CyRK/array/interp.pyx":409
+                              /* "CyRK/array/interp.pyx":643
  *             fp_at_j_real = fp_at_j.real
  *             fp_at_j_imag = fp_at_j.imag
  *             xp_at_j = x_domain[j]             # <<<<<<<<<<<<<<
  *             if j == lenx - 1:
  *                 result_real = fp_at_j_real
  */
                               __pyx_t_8 = __pyx_v_j;
                               __pyx_v_xp_at_j = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_8 * __pyx_v_x_domain.strides[0]) )));
 
-                              /* "CyRK/array/interp.pyx":410
+                              /* "CyRK/array/interp.pyx":644
  *             fp_at_j_imag = fp_at_j.imag
  *             xp_at_j = x_domain[j]
  *             if j == lenx - 1:             # <<<<<<<<<<<<<<
  *                 result_real = fp_at_j_real
  *                 result_imag = fp_at_j_imag
  */
                               __pyx_t_3 = (__pyx_v_j == (__pyx_v_lenx - 1));
                               if (__pyx_t_3) {
 
-                                /* "CyRK/array/interp.pyx":411
+                                /* "CyRK/array/interp.pyx":645
  *             xp_at_j = x_domain[j]
  *             if j == lenx - 1:
  *                 result_real = fp_at_j_real             # <<<<<<<<<<<<<<
  *                 result_imag = fp_at_j_imag
  *             elif xp_at_j == desired_x:
  */
                                 __pyx_v_result_real = __pyx_v_fp_at_j_real;
 
-                                /* "CyRK/array/interp.pyx":412
+                                /* "CyRK/array/interp.pyx":646
  *             if j == lenx - 1:
  *                 result_real = fp_at_j_real
  *                 result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
  *             elif xp_at_j == desired_x:
  *                 result_real = fp_at_j_real
  */
                                 __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
 
-                                /* "CyRK/array/interp.pyx":410
+                                /* "CyRK/array/interp.pyx":644
  *             fp_at_j_imag = fp_at_j.imag
  *             xp_at_j = x_domain[j]
  *             if j == lenx - 1:             # <<<<<<<<<<<<<<
  *                 result_real = fp_at_j_real
  *                 result_imag = fp_at_j_imag
  */
                                 goto __pyx_L12;
                               }
 
-                              /* "CyRK/array/interp.pyx":413
+                              /* "CyRK/array/interp.pyx":647
  *                 result_real = fp_at_j_real
  *                 result_imag = fp_at_j_imag
  *             elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
  *                 result_real = fp_at_j_real
  *                 result_imag = fp_at_j_imag
  */
                               __pyx_t_3 = (__pyx_v_xp_at_j == __pyx_v_desired_x);
                               if (__pyx_t_3) {
 
-                                /* "CyRK/array/interp.pyx":414
+                                /* "CyRK/array/interp.pyx":648
  *                 result_imag = fp_at_j_imag
  *             elif xp_at_j == desired_x:
  *                 result_real = fp_at_j_real             # <<<<<<<<<<<<<<
  *                 result_imag = fp_at_j_imag
  *             else:
  */
                                 __pyx_v_result_real = __pyx_v_fp_at_j_real;
 
-                                /* "CyRK/array/interp.pyx":415
+                                /* "CyRK/array/interp.pyx":649
  *             elif xp_at_j == desired_x:
  *                 result_real = fp_at_j_real
  *                 result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
  *             else:
  *                 fp_at_jp1 = dependent_values[j + 1]
  */
                                 __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
 
-                                /* "CyRK/array/interp.pyx":413
+                                /* "CyRK/array/interp.pyx":647
  *                 result_real = fp_at_j_real
  *                 result_imag = fp_at_j_imag
  *             elif xp_at_j == desired_x:             # <<<<<<<<<<<<<<
  *                 result_real = fp_at_j_real
  *                 result_imag = fp_at_j_imag
  */
                                 goto __pyx_L12;
                               }
 
-                              /* "CyRK/array/interp.pyx":417
+                              /* "CyRK/array/interp.pyx":651
  *                 result_imag = fp_at_j_imag
  *             else:
  *                 fp_at_jp1 = dependent_values[j + 1]             # <<<<<<<<<<<<<<
  *                 fp_at_jp1_real = fp_at_jp1.real
  *                 fp_at_jp1_imag = fp_at_jp1.imag
  */
                               /*else*/ {
                                 __pyx_t_2 = (__pyx_v_j + 1);
                                 __pyx_v_fp_at_jp1 = (*((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_dependent_values.data + __pyx_t_2 * __pyx_v_dependent_values.strides[0]) )));
 
-                                /* "CyRK/array/interp.pyx":418
+                                /* "CyRK/array/interp.pyx":652
  *             else:
  *                 fp_at_jp1 = dependent_values[j + 1]
  *                 fp_at_jp1_real = fp_at_jp1.real             # <<<<<<<<<<<<<<
  *                 fp_at_jp1_imag = fp_at_jp1.imag
  *                 xp_at_jp1 = x_domain[j + 1]
  */
                                 __pyx_t_7 = __Pyx_CREAL(__pyx_v_fp_at_jp1);
                                 __pyx_v_fp_at_jp1_real = __pyx_t_7;
 
-                                /* "CyRK/array/interp.pyx":419
+                                /* "CyRK/array/interp.pyx":653
  *                 fp_at_jp1 = dependent_values[j + 1]
  *                 fp_at_jp1_real = fp_at_jp1.real
  *                 fp_at_jp1_imag = fp_at_jp1.imag             # <<<<<<<<<<<<<<
  *                 xp_at_jp1 = x_domain[j + 1]
  *                 x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
  */
                                 __pyx_t_7 = __Pyx_CIMAG(__pyx_v_fp_at_jp1);
                                 __pyx_v_fp_at_jp1_imag = __pyx_t_7;
 
-                                /* "CyRK/array/interp.pyx":420
+                                /* "CyRK/array/interp.pyx":654
  *                 fp_at_jp1_real = fp_at_jp1.real
  *                 fp_at_jp1_imag = fp_at_jp1.imag
  *                 xp_at_jp1 = x_domain[j + 1]             # <<<<<<<<<<<<<<
  *                 x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
  *                 slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
  */
                                 __pyx_t_2 = (__pyx_v_j + 1);
                                 __pyx_v_xp_at_jp1 = (*((double *) ( /* dim=0 */ (__pyx_v_x_domain.data + __pyx_t_2 * __pyx_v_x_domain.strides[0]) )));
 
-                                /* "CyRK/array/interp.pyx":421
+                                /* "CyRK/array/interp.pyx":655
  *                 fp_at_jp1_imag = fp_at_jp1.imag
  *                 xp_at_jp1 = x_domain[j + 1]
  *                 x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)             # <<<<<<<<<<<<<<
  *                 slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
  *                 slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse
  */
                                 __pyx_v_x_slope_inverse = (1.0 / (__pyx_v_xp_at_jp1 - __pyx_v_xp_at_j));
 
-                                /* "CyRK/array/interp.pyx":422
+                                /* "CyRK/array/interp.pyx":656
  *                 xp_at_jp1 = x_domain[j + 1]
  *                 x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
  *                 slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse             # <<<<<<<<<<<<<<
  *                 slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse
  * 
  */
                                 __pyx_v_slope_real = ((__pyx_v_fp_at_jp1_real - __pyx_v_fp_at_j_real) * __pyx_v_x_slope_inverse);
 
-                                /* "CyRK/array/interp.pyx":423
+                                /* "CyRK/array/interp.pyx":657
  *                 x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
  *                 slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
  *                 slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse             # <<<<<<<<<<<<<<
  * 
  *                 # If we get nan in one direction try the other
  */
                                 __pyx_v_slope_imag = ((__pyx_v_fp_at_jp1_imag - __pyx_v_fp_at_j_imag) * __pyx_v_x_slope_inverse);
 
-                                /* "CyRK/array/interp.pyx":427
+                                /* "CyRK/array/interp.pyx":661
  *                 # If we get nan in one direction try the other
  *                 # Real Part
  *                 result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real             # <<<<<<<<<<<<<<
  *                 if isnan(result_real):
  *                     result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  */
                                 __pyx_v_result_real = ((__pyx_v_slope_real * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j_real);
 
-                                /* "CyRK/array/interp.pyx":428
+                                /* "CyRK/array/interp.pyx":662
  *                 # Real Part
  *                 result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
  *                 if isnan(result_real):             # <<<<<<<<<<<<<<
  *                     result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                     if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
  */
                                 __pyx_t_3 = isnan(__pyx_v_result_real);
                                 if (__pyx_t_3) {
 
-                                  /* "CyRK/array/interp.pyx":429
+                                  /* "CyRK/array/interp.pyx":663
  *                 result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
  *                 if isnan(result_real):
  *                     result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real             # <<<<<<<<<<<<<<
  *                     if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
  *                         result_real = fp_at_j_real
  */
                                   __pyx_v_result_real = ((__pyx_v_slope_real * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1_real);
 
-                                  /* "CyRK/array/interp.pyx":430
+                                  /* "CyRK/array/interp.pyx":664
  *                 if isnan(result_real):
  *                     result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                     if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):             # <<<<<<<<<<<<<<
  *                         result_real = fp_at_j_real
  * 
  */
                                   __pyx_t_9 = isnan(__pyx_v_result_real);
@@ -21714,70 +23364,70 @@
                                     goto __pyx_L15_bool_binop_done;
                                   }
                                   __pyx_t_9 = (__pyx_v_fp_at_jp1_real == __pyx_v_fp_at_j_real);
                                   __pyx_t_3 = __pyx_t_9;
                                   __pyx_L15_bool_binop_done:;
                                   if (__pyx_t_3) {
 
-                                    /* "CyRK/array/interp.pyx":431
+                                    /* "CyRK/array/interp.pyx":665
  *                     result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                     if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
  *                         result_real = fp_at_j_real             # <<<<<<<<<<<<<<
  * 
  *                 # Imaginary Part
  */
                                     __pyx_v_result_real = __pyx_v_fp_at_j_real;
 
-                                    /* "CyRK/array/interp.pyx":430
+                                    /* "CyRK/array/interp.pyx":664
  *                 if isnan(result_real):
  *                     result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                     if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):             # <<<<<<<<<<<<<<
  *                         result_real = fp_at_j_real
  * 
  */
                                   }
 
-                                  /* "CyRK/array/interp.pyx":428
+                                  /* "CyRK/array/interp.pyx":662
  *                 # Real Part
  *                 result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
  *                 if isnan(result_real):             # <<<<<<<<<<<<<<
  *                     result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
  *                     if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
  */
                                 }
 
-                                /* "CyRK/array/interp.pyx":434
+                                /* "CyRK/array/interp.pyx":668
  * 
  *                 # Imaginary Part
  *                 result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag             # <<<<<<<<<<<<<<
  *                 if isnan(result_imag):
  *                     result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  */
                                 __pyx_v_result_imag = ((__pyx_v_slope_imag * (__pyx_v_desired_x - __pyx_v_xp_at_j)) + __pyx_v_fp_at_j_imag);
 
-                                /* "CyRK/array/interp.pyx":435
+                                /* "CyRK/array/interp.pyx":669
  *                 # Imaginary Part
  *                 result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
  *                 if isnan(result_imag):             # <<<<<<<<<<<<<<
  *                     result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                     if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
  */
                                 __pyx_t_3 = isnan(__pyx_v_result_imag);
                                 if (__pyx_t_3) {
 
-                                  /* "CyRK/array/interp.pyx":436
+                                  /* "CyRK/array/interp.pyx":670
  *                 result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
  *                 if isnan(result_imag):
  *                     result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag             # <<<<<<<<<<<<<<
  *                     if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
  *                         result_imag = fp_at_j_imag
  */
                                   __pyx_v_result_imag = ((__pyx_v_slope_imag * (__pyx_v_desired_x - __pyx_v_xp_at_jp1)) + __pyx_v_fp_at_jp1_imag);
 
-                                  /* "CyRK/array/interp.pyx":437
+                                  /* "CyRK/array/interp.pyx":671
  *                 if isnan(result_imag):
  *                     result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                     if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):             # <<<<<<<<<<<<<<
  *                         result_imag = fp_at_j_imag
  * 
  */
                                   __pyx_t_9 = isnan(__pyx_v_result_imag);
@@ -21787,55 +23437,55 @@
                                     goto __pyx_L19_bool_binop_done;
                                   }
                                   __pyx_t_9 = (__pyx_v_fp_at_jp1_imag == __pyx_v_fp_at_j_imag);
                                   __pyx_t_3 = __pyx_t_9;
                                   __pyx_L19_bool_binop_done:;
                                   if (__pyx_t_3) {
 
-                                    /* "CyRK/array/interp.pyx":438
+                                    /* "CyRK/array/interp.pyx":672
  *                     result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                     if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
  *                         result_imag = fp_at_j_imag             # <<<<<<<<<<<<<<
  * 
  *         result = result_real + 1.0j * result_imag
  */
                                     __pyx_v_result_imag = __pyx_v_fp_at_j_imag;
 
-                                    /* "CyRK/array/interp.pyx":437
+                                    /* "CyRK/array/interp.pyx":671
  *                 if isnan(result_imag):
  *                     result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                     if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):             # <<<<<<<<<<<<<<
  *                         result_imag = fp_at_j_imag
  * 
  */
                                   }
 
-                                  /* "CyRK/array/interp.pyx":435
+                                  /* "CyRK/array/interp.pyx":669
  *                 # Imaginary Part
  *                 result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
  *                 if isnan(result_imag):             # <<<<<<<<<<<<<<
  *                     result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
  *                     if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
  */
                                 }
                               }
                               __pyx_L12:;
                             }
                             __pyx_L11:;
 
-                            /* "CyRK/array/interp.pyx":440
+                            /* "CyRK/array/interp.pyx":674
  *                         result_imag = fp_at_j_imag
  * 
  *         result = result_real + 1.0j * result_imag             # <<<<<<<<<<<<<<
  * 
  *         desired_dependent_array[index] = result
  */
                             __pyx_v_result = __Pyx_c_sum_double(__pyx_t_double_complex_from_parts(__pyx_v_result_real, 0), __Pyx_c_prod_double(__pyx_t_double_complex_from_parts(0, 1.0), __pyx_t_double_complex_from_parts(__pyx_v_result_imag, 0)));
 
-                            /* "CyRK/array/interp.pyx":442
+                            /* "CyRK/array/interp.pyx":676
  *         result = result_real + 1.0j * result_imag
  * 
  *         desired_dependent_array[index] = result             # <<<<<<<<<<<<<<
  */
                             __pyx_t_2 = __pyx_v_index;
                             *((__pyx_t_double_complex *) ( /* dim=0 */ (__pyx_v_desired_dependent_array.data + __pyx_t_2 * __pyx_v_desired_dependent_array.strides[0]) )) = __pyx_v_result;
                             goto __pyx_L22;
@@ -21949,15 +23599,15 @@
             #undef likely
             #undef unlikely
             #define likely(x)   __builtin_expect(!!(x), 1)
             #define unlikely(x) __builtin_expect(!!(x), 0)
         #endif
       }
 
-      /* "CyRK/array/interp.pyx":391
+      /* "CyRK/array/interp.pyx":625
  *     cdef double desired_x
  *     cdef double complex result
  *     for index in prange(desired_len, nogil=True):             # <<<<<<<<<<<<<<
  *         desired_x = desired_x_array[index]
  * 
  */
       /*finally:*/ {
@@ -21979,15 +23629,15 @@
           #endif
           goto __pyx_L1_error;
         }
         __pyx_L6:;
       }
   }
 
-  /* "CyRK/array/interp.pyx":343
+  /* "CyRK/array/interp.pyx":577
  * 
  * 
  * cpdef void interp_complex_array(double[:] desired_x_array, double[:] x_domain, double complex[:] dependent_values,             # <<<<<<<<<<<<<<
  *                                 double complex[:] desired_dependent_array) nogil:
  * 
  */
 
@@ -22001,23 +23651,23 @@
   #ifdef WITH_THREAD
   __Pyx_PyGILState_Release(__pyx_gilstate_save);
   #endif
   __pyx_L0:;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_pw_4CyRK_5array_6interp_7interp_complex_array(PyObject *__pyx_self, 
+static PyObject *__pyx_pw_4CyRK_5array_6interp_11interp_complex_array(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ); /*proto*/
-static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_7interp_complex_array = {"interp_complex_array", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_7interp_complex_array, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_4CyRK_5array_6interp_7interp_complex_array(PyObject *__pyx_self, 
+static PyMethodDef __pyx_mdef_4CyRK_5array_6interp_11interp_complex_array = {"interp_complex_array", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_4CyRK_5array_6interp_11interp_complex_array, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_4CyRK_5array_6interp_11interp_complex_array(PyObject *__pyx_self, 
 #if CYTHON_METH_FASTCALL
 PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
 #else
 PyObject *__pyx_args, PyObject *__pyx_kwds
 #endif
 ) {
   __Pyx_memviewslice __pyx_v_desired_x_array = { 0, 0, { 0 }, { 0 }, { 0 } };
@@ -22051,93 +23701,89 @@
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
       kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
       switch (__pyx_nargs) {
         case  0:
         if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_desired_x_array)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 343, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 577, __pyx_L3_error)
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_x_domain)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 343, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 577, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp_complex_array", 1, 4, 4, 1); __PYX_ERR(1, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp_complex_array", 1, 4, 4, 1); __PYX_ERR(1, 577, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_dependent_values)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 343, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 577, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp_complex_array", 1, 4, 4, 2); __PYX_ERR(1, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp_complex_array", 1, 4, 4, 2); __PYX_ERR(1, 577, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_desired_dependent_array)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 343, __pyx_L3_error)
+        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 577, __pyx_L3_error)
         else {
-          __Pyx_RaiseArgtupleInvalid("interp_complex_array", 1, 4, 4, 3); __PYX_ERR(1, 343, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("interp_complex_array", 1, 4, 4, 3); __PYX_ERR(1, 577, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
         const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp_complex_array") < 0)) __PYX_ERR(1, 343, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "interp_complex_array") < 0)) __PYX_ERR(1, 577, __pyx_L3_error)
       }
     } else if (unlikely(__pyx_nargs != 4)) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
       values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
       values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
       values[3] = __Pyx_Arg_FASTCALL(__pyx_args, 3);
     }
-    __pyx_v_desired_x_array = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_desired_x_array.memview)) __PYX_ERR(1, 343, __pyx_L3_error)
-    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 343, __pyx_L3_error)
-    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 343, __pyx_L3_error)
-    __pyx_v_desired_dependent_array = __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_desired_dependent_array.memview)) __PYX_ERR(1, 344, __pyx_L3_error)
+    __pyx_v_desired_x_array = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[0], PyBUF_WRITABLE); if (unlikely(!__pyx_v_desired_x_array.memview)) __PYX_ERR(1, 577, __pyx_L3_error)
+    __pyx_v_x_domain = __Pyx_PyObject_to_MemoryviewSlice_ds_double(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_x_domain.memview)) __PYX_ERR(1, 577, __pyx_L3_error)
+    __pyx_v_dependent_values = __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(values[2], PyBUF_WRITABLE); if (unlikely(!__pyx_v_dependent_values.memview)) __PYX_ERR(1, 577, __pyx_L3_error)
+    __pyx_v_desired_dependent_array = __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(values[3], PyBUF_WRITABLE); if (unlikely(!__pyx_v_desired_dependent_array.memview)) __PYX_ERR(1, 578, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("interp_complex_array", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 343, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("interp_complex_array", 1, 4, 4, __pyx_nargs); __PYX_ERR(1, 577, __pyx_L3_error)
   __pyx_L3_error:;
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_desired_x_array, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_desired_dependent_array, 1);
   __Pyx_AddTraceback("CyRK.array.interp.interp_complex_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_4CyRK_5array_6interp_6interp_complex_array(__pyx_self, __pyx_v_desired_x_array, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_desired_dependent_array);
+  __pyx_r = __pyx_pf_4CyRK_5array_6interp_10interp_complex_array(__pyx_self, __pyx_v_desired_x_array, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_desired_dependent_array);
 
   /* function exit code */
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_desired_x_array, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_x_domain, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_dependent_values, 1);
   __PYX_XCLEAR_MEMVIEW(&__pyx_v_desired_dependent_array, 1);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_4CyRK_5array_6interp_6interp_complex_array(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array) {
+static PyObject *__pyx_pf_4CyRK_5array_6interp_10interp_complex_array(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_desired_x_array, __Pyx_memviewslice __pyx_v_x_domain, __Pyx_memviewslice __pyx_v_dependent_values, __Pyx_memviewslice __pyx_v_desired_dependent_array) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("interp_complex_array", 0);
   __Pyx_XDECREF(__pyx_r);
-  if (unlikely(!__pyx_v_desired_x_array.memview)) { __Pyx_RaiseUnboundLocalError("desired_x_array"); __PYX_ERR(1, 343, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_x_domain.memview)) { __Pyx_RaiseUnboundLocalError("x_domain"); __PYX_ERR(1, 343, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_dependent_values.memview)) { __Pyx_RaiseUnboundLocalError("dependent_values"); __PYX_ERR(1, 343, __pyx_L1_error) }
-  if (unlikely(!__pyx_v_desired_dependent_array.memview)) { __Pyx_RaiseUnboundLocalError("desired_dependent_array"); __PYX_ERR(1, 343, __pyx_L1_error) }
-  __pyx_f_4CyRK_5array_6interp_interp_complex_array(__pyx_v_desired_x_array, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_desired_dependent_array, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 343, __pyx_L1_error)
-  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_f_4CyRK_5array_6interp_interp_complex_array(__pyx_v_desired_x_array, __pyx_v_x_domain, __pyx_v_dependent_values, __pyx_v_desired_dependent_array, 0); if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 577, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_void_to_None(NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -23124,16 +24770,16 @@
     {&__pyx_n_s_Sequence, __pyx_k_Sequence, sizeof(__pyx_k_Sequence), 0, 0, 1, 1},
     {&__pyx_kp_s_Step_may_not_be_zero_axis_d, __pyx_k_Step_may_not_be_zero_axis_d, sizeof(__pyx_k_Step_may_not_be_zero_axis_d), 0, 0, 1, 0},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
     {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-    {&__pyx_n_s__28, __pyx_k__28, sizeof(__pyx_k__28), 0, 0, 1, 1},
     {&__pyx_n_s__3, __pyx_k__3, sizeof(__pyx_k__3), 0, 0, 1, 1},
+    {&__pyx_n_s__30, __pyx_k__30, sizeof(__pyx_k__30), 0, 0, 1, 1},
     {&__pyx_kp_u__6, __pyx_k__6, sizeof(__pyx_k__6), 0, 1, 0, 0},
     {&__pyx_kp_u__7, __pyx_k__7, sizeof(__pyx_k__7), 0, 1, 0, 0},
     {&__pyx_n_s_abc, __pyx_k_abc, sizeof(__pyx_k_abc), 0, 0, 1, 1},
     {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
     {&__pyx_kp_u_and, __pyx_k_and, sizeof(__pyx_k_and), 0, 1, 0, 0},
     {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
     {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
@@ -23174,14 +24820,16 @@
     {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
     {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
     {&__pyx_n_s_initializing, __pyx_k_initializing, sizeof(__pyx_k_initializing), 0, 0, 1, 1},
     {&__pyx_n_s_interp, __pyx_k_interp, sizeof(__pyx_k_interp), 0, 0, 1, 1},
     {&__pyx_n_s_interp_array, __pyx_k_interp_array, sizeof(__pyx_k_interp_array), 0, 0, 1, 1},
     {&__pyx_n_s_interp_complex, __pyx_k_interp_complex, sizeof(__pyx_k_interp_complex), 0, 0, 1, 1},
     {&__pyx_n_s_interp_complex_array, __pyx_k_interp_complex_array, sizeof(__pyx_k_interp_complex_array), 0, 0, 1, 1},
+    {&__pyx_n_s_interp_complexj, __pyx_k_interp_complexj, sizeof(__pyx_k_interp_complexj), 0, 0, 1, 1},
+    {&__pyx_n_s_interpj, __pyx_k_interpj, sizeof(__pyx_k_interpj), 0, 0, 1, 1},
     {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
     {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
     {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
     {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
     {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
     {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
     {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
@@ -23193,14 +24841,15 @@
     {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
     {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
     {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
     {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
     {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
     {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
+    {&__pyx_n_s_provided_j, __pyx_k_provided_j, sizeof(__pyx_k_provided_j), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
@@ -23289,26 +24938,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 989, __pyx_L1_error)
@@ -23415,52 +25064,70 @@
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
   __pyx_codeobj__21 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__20, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__21)) __PYX_ERR(0, 1, __pyx_L1_error)
 
   /* "CyRK/array/interp.pyx":96
  * 
  * 
- * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values) nogil:             # <<<<<<<<<<<<<<
- *     """ Interpolation function for floats.
- * 
+ * cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                             int provided_j = -1) nogil:
+ *     """ Interpolation function for floats. This function will return the index that it found during interpolation.
  */
-  __pyx_tuple__22 = PyTuple_Pack(3, __pyx_n_s_desired_x, __pyx_n_s_x_domain, __pyx_n_s_dependent_values); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 96, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(4, __pyx_n_s_desired_x, __pyx_n_s_x_domain, __pyx_n_s_dependent_values, __pyx_n_s_provided_j); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 96, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp, 96, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 96, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interpj, 96, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(1, 96, __pyx_L1_error)
+
+  /* "CyRK/array/interp.pyx":188
+ * 
+ * 
+ * cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
+ *                                             double complex[:] dependent_values, int provided_j = -1) nogil:
+ *     """ Interpolation function for complex numbers.
+ */
+  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp_complexj, 188, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 188, __pyx_L1_error)
+
+  /* "CyRK/array/interp.pyx":308
+ * 
+ * 
+ * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values, int provided_j = -1) nogil:             # <<<<<<<<<<<<<<
+ *     """ Interpolation function for floats.
+ * 
+ */
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp, 308, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(1, 308, __pyx_L1_error)
 
-  /* "CyRK/array/interp.pyx":170
+  /* "CyRK/array/interp.pyx":393
  * 
  * 
  * cpdef double complex interp_complex(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
- *                                     double complex[:] dependent_values) nogil:
+ *                                     double complex[:] dependent_values, int provided_j = -1) nogil:
  *     """ Interpolation function for complex numbers.
  */
-  __pyx_codeobj__24 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 3, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp_complex, 170, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__24)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp_complex, 393, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(1, 393, __pyx_L1_error)
 
-  /* "CyRK/array/interp.pyx":273
+  /* "CyRK/array/interp.pyx":507
  * 
  * 
  * cpdef void interp_array(double[:] desired_x_array, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
  *                         double[:] desired_dependent_array) nogil:
  * 
  */
-  __pyx_tuple__25 = PyTuple_Pack(4, __pyx_n_s_desired_x_array, __pyx_n_s_x_domain, __pyx_n_s_dependent_values, __pyx_n_s_desired_dependent_array); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 273, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__25);
-  __Pyx_GIVEREF(__pyx_tuple__25);
-  __pyx_codeobj__26 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp_array, 273, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__26)) __PYX_ERR(1, 273, __pyx_L1_error)
+  __pyx_tuple__27 = PyTuple_Pack(4, __pyx_n_s_desired_x_array, __pyx_n_s_x_domain, __pyx_n_s_dependent_values, __pyx_n_s_desired_dependent_array); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 507, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_codeobj__28 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp_array, 507, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__28)) __PYX_ERR(1, 507, __pyx_L1_error)
 
-  /* "CyRK/array/interp.pyx":343
+  /* "CyRK/array/interp.pyx":577
  * 
  * 
  * cpdef void interp_complex_array(double[:] desired_x_array, double[:] x_domain, double complex[:] dependent_values,             # <<<<<<<<<<<<<<
  *                                 double complex[:] desired_dependent_array) nogil:
  * 
  */
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__25, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp_complex_array, 343, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(4, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__27, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_CyRK_array_interp_pyx, __pyx_n_s_interp_complex_array, 577, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(1, 577, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 /* #### Code section: init_constants ### */
@@ -23533,16 +25200,18 @@
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
   if (__Pyx_ExportFunction("binary_search_with_guess", (void (*)(void))__pyx_f_4CyRK_5array_6interp_binary_search_with_guess, "unsigned int (double, __Pyx_memviewslice, unsigned int, unsigned int)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("interp", (void (*)(void))__pyx_f_4CyRK_5array_6interp_interp, "double (double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  if (__Pyx_ExportFunction("interp_complex", (void (*)(void))__pyx_f_4CyRK_5array_6interp_interp_complex, "__pyx_t_double_complex (double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("interpj", (void (*)(void))__pyx_f_4CyRK_5array_6interp_interpj, "__pyx_ctuple_double__and_int (double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interpj *__pyx_optional_args)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("interp_complexj", (void (*)(void))__pyx_f_4CyRK_5array_6interp_interp_complexj, "__pyx_ctuple___dunderpyx_t_double_complex__and_int (double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj *__pyx_optional_args)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("interp", (void (*)(void))__pyx_f_4CyRK_5array_6interp_interp, "double (double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp *__pyx_optional_args)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ExportFunction("interp_complex", (void (*)(void))__pyx_f_4CyRK_5array_6interp_interp_complex, "__pyx_t_double_complex (double, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch, struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex *__pyx_optional_args)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("interp_array", (void (*)(void))__pyx_f_4CyRK_5array_6interp_interp_array, "void (__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   if (__Pyx_ExportFunction("interp_complex_array", (void (*)(void))__pyx_f_4CyRK_5array_6interp_interp_complex_array, "void (__Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, __Pyx_memviewslice, int __pyx_skip_dispatch)") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -24629,62 +26298,90 @@
  * 
  */
   __pyx_v_4CyRK_5array_6interp_LIKELY_IN_CACHE_SIZE = 8;
 
   /* "CyRK/array/interp.pyx":96
  * 
  * 
- * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values) nogil:             # <<<<<<<<<<<<<<
+ * cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                             int provided_j = -1) nogil:
+ *     """ Interpolation function for floats. This function will return the index that it found during interpolation.
+ */
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_1interpj, 0, __pyx_n_s_interpj, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 96, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interpj, __pyx_t_7) < 0) __PYX_ERR(1, 96, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "CyRK/array/interp.pyx":188
+ * 
+ * 
+ * cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
+ *                                             double complex[:] dependent_values, int provided_j = -1) nogil:
+ *     """ Interpolation function for complex numbers.
+ */
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_3interp_complexj, 0, __pyx_n_s_interp_complexj, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 188, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp_complexj, __pyx_t_7) < 0) __PYX_ERR(1, 188, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+
+  /* "CyRK/array/interp.pyx":308
+ * 
+ * 
+ * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values, int provided_j = -1) nogil:             # <<<<<<<<<<<<<<
  *     """ Interpolation function for floats.
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_1interp, 0, __pyx_n_s_interp, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__23)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 96, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_5interp, 0, __pyx_n_s_interp, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__25)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 308, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp, __pyx_t_7) < 0) __PYX_ERR(1, 96, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp, __pyx_t_7) < 0) __PYX_ERR(1, 308, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "CyRK/array/interp.pyx":170
+  /* "CyRK/array/interp.pyx":393
  * 
  * 
  * cpdef double complex interp_complex(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
- *                                     double complex[:] dependent_values) nogil:
+ *                                     double complex[:] dependent_values, int provided_j = -1) nogil:
  *     """ Interpolation function for complex numbers.
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_3interp_complex, 0, __pyx_n_s_interp_complex, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__24)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 170, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_7interp_complex, 0, __pyx_n_s_interp_complex, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 393, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp_complex, __pyx_t_7) < 0) __PYX_ERR(1, 170, __pyx_L1_error)
+  __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_7, __pyx_tuple__4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp_complex, __pyx_t_7) < 0) __PYX_ERR(1, 393, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "CyRK/array/interp.pyx":273
+  /* "CyRK/array/interp.pyx":507
  * 
  * 
  * cpdef void interp_array(double[:] desired_x_array, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
  *                         double[:] desired_dependent_array) nogil:
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_5interp_array, 0, __pyx_n_s_interp_array, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__26)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 273, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_9interp_array, 0, __pyx_n_s_interp_array, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__28)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 507, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp_array, __pyx_t_7) < 0) __PYX_ERR(1, 273, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp_array, __pyx_t_7) < 0) __PYX_ERR(1, 507, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
-  /* "CyRK/array/interp.pyx":343
+  /* "CyRK/array/interp.pyx":577
  * 
  * 
  * cpdef void interp_complex_array(double[:] desired_x_array, double[:] x_domain, double complex[:] dependent_values,             # <<<<<<<<<<<<<<
  *                                 double complex[:] desired_dependent_array) nogil:
  * 
  */
-  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_7interp_complex_array, 0, __pyx_n_s_interp_complex_array, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__27)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 343, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_CyFunction_New(&__pyx_mdef_4CyRK_5array_6interp_11interp_complex_array, 0, __pyx_n_s_interp_complex_array, NULL, __pyx_n_s_CyRK_array_interp, __pyx_d, ((PyObject *)__pyx_codeobj__29)); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 577, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp_complex_array, __pyx_t_7) < 0) __PYX_ERR(1, 343, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_interp_complex_array, __pyx_t_7) < 0) __PYX_ERR(1, 577, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
   /* "CyRK/array/interp.pyx":1
  * # distutils: language = c++             # <<<<<<<<<<<<<<
- * # cython: boundscheck=False, wraparound=False, nonecheck=False, cdivision=True
+ * # cython: boundscheck=False, wraparound=False, nonecheck=False, cdivision=True, initializedcheck=False
  * import cython
  */
   __pyx_t_7 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_7) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
@@ -30041,14 +31738,36 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* CIntFromPyVerify */
+  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
+#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
+    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
+#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
+    {\
+        func_type value = func_value;\
+        if (sizeof(target_type) < sizeof(func_type)) {\
+            if (unlikely(value != (func_type) (target_type) value)) {\
+                func_type zero = 0;\
+                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
+                    return (target_type) -1;\
+                if (is_unsigned && unlikely(value < zero))\
+                    goto raise_neg_overflow;\
+                else\
+                    goto raise_overflow;\
+            }\
+        }\
+        return (target_type) value;\
+    }
+
 /* ObjectToMemviewSlice */
   static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_ds___pyx_t_double_complex(PyObject *obj, int writable_flag) {
     __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
     __Pyx_BufFmt_StackElem stack[1];
     int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_STRIDED) };
     int retcode;
     if (obj == Py_None) {
@@ -30076,14 +31795,50 @@
     double value = __pyx_PyFloat_AsDouble(obj);
     if (unlikely((value == (double)-1) && PyErr_Occurred()))
         return 0;
     *(double *) itemp = value;
     return 1;
 }
 
+/* ToPyCTupleUtility */
+  static PyObject* __pyx_convert__to_py___pyx_ctuple_double__and_int(__pyx_ctuple_double__and_int value) {
+    PyObject* item = NULL;
+    PyObject* result = PyTuple_New(2);
+    if (!result) goto bad;
+        item = PyFloat_FromDouble(value.f0);
+        if (!item) goto bad;
+        PyTuple_SET_ITEM(result, 0, item);
+        item = __Pyx_PyInt_From_int(value.f1);
+        if (!item) goto bad;
+        PyTuple_SET_ITEM(result, 1, item);
+    return result;
+bad:
+    Py_XDECREF(item);
+    Py_XDECREF(result);
+    return NULL;
+}
+
+/* ToPyCTupleUtility */
+  static PyObject* __pyx_convert__to_py___pyx_ctuple___dunderpyx_t_double_complex__and_int(__pyx_ctuple___dunderpyx_t_double_complex__and_int value) {
+    PyObject* item = NULL;
+    PyObject* result = PyTuple_New(2);
+    if (!result) goto bad;
+        item = __pyx_PyComplex_FromComplex(value.f0);
+        if (!item) goto bad;
+        PyTuple_SET_ITEM(result, 0, item);
+        item = __Pyx_PyInt_From_int(value.f1);
+        if (!item) goto bad;
+        PyTuple_SET_ITEM(result, 1, item);
+    return result;
+bad:
+    Py_XDECREF(item);
+    Py_XDECREF(result);
+    return NULL;
+}
+
 /* Declarations */
   #if CYTHON_CCOMPLEX && (1) && (!0 || __cplusplus)
   #ifdef __cplusplus
     static CYTHON_INLINE __pyx_t_float_complex __pyx_t_float_complex_from_parts(float x, float y) {
       return ::std::complex< float >(x, y);
     }
   #else
@@ -30432,36 +32187,14 @@
         }
     } else {
         __pyx_fatalerror("Acquisition count is %d (line %d)",
                          old_acquisition_count-1, lineno);
     }
 }
 
-/* CIntFromPyVerify */
-  #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
-#define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
-    __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
-#define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
-    {\
-        func_type value = func_value;\
-        if (sizeof(target_type) < sizeof(func_type)) {\
-            if (unlikely(value != (func_type) (target_type) value)) {\
-                func_type zero = 0;\
-                if (exc && unlikely(value == (func_type)-1 && PyErr_Occurred()))\
-                    return (target_type) -1;\
-                if (is_unsigned && unlikely(value < zero))\
-                    goto raise_neg_overflow;\
-                else\
-                    goto raise_overflow;\
-            }\
-        }\
-        return (target_type) value;\
-    }
-
 /* CIntFromPy */
   static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const int neg_one = (int) -1, const_zero = (int) 0;
@@ -30727,14 +32460,52 @@
     return (int) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to int");
     return (int) -1;
 }
 
+/* CIntToPy */
+  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic push
+#pragma GCC diagnostic ignored "-Wconversion"
+#endif
+    const int neg_one = (int) -1, const_zero = (int) 0;
+#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
+#pragma GCC diagnostic pop
+#endif
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(int) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(int) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
+#endif
+        }
+    } else {
+        if (sizeof(int) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(int),
+                                     little, !is_unsigned);
+    }
+}
+
 /* CIntFromPy */
   static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
@@ -31001,52 +32772,14 @@
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
 /* CIntToPy */
-  static CYTHON_INLINE PyObject* __Pyx_PyInt_From_int(int value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(int) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(int) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(int) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(int),
-                                     little, !is_unsigned);
-    }
-}
-
-/* CIntToPy */
   static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
 #pragma GCC diagnostic push
 #pragma GCC diagnostic ignored "-Wconversion"
 #endif
     const long neg_one = (long) -1, const_zero = (long) 0;
 #ifdef __Pyx_HAS_GCC_DIAGNOSTIC
@@ -31358,15 +33091,15 @@
 static __Pyx_TypeName
 __Pyx_PyType_GetName(PyTypeObject* tp)
 {
     PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
                                                __pyx_n_s_name_2);
     if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
         PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__28));
+        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__30));
     }
     return name;
 }
 #endif
 
 /* CheckBinaryVersion */
   static int __Pyx_check_binary_version(void) {
```

### Comparing `CyRK-0.6.0/CyRK/array/interp.pxd` & `CyRK-0.6.1/CyRK/array/interp.pxd`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 # distutils: language = c++
 
 cdef unsigned int binary_search_with_guess(double key, double[:] array, unsigned int length, unsigned int guess) nogil
 
-cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values) nogil
+cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,
+                            int provided_j = *) nogil
 
-cpdef double complex interp_complex(double desired_x, double[:] x_domain, double complex[:] dependent_values) nogil
+cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,
+                                            double complex[:] dependent_values, int provided_j = *) nogil
+
+cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values,
+                    int provided_j = *) nogil
+
+cpdef double complex interp_complex(double desired_x, double[:] x_domain, double complex[:] dependent_values,
+                                    int provided_j = *) nogil
 
 cpdef void interp_array(double[:] desired_x_array, double[:] x_domain, double[:] dependent_values,
                         double[:] desired_dependent_array) nogil
 
 cpdef void interp_complex_array(double[:] desired_x_array, double[:] x_domain, double complex[:] dependent_values,
                                 double complex[:] desired_dependent_array) nogil
```

### Comparing `CyRK-0.6.0/CyRK/array/interp.pyx` & `CyRK-0.6.1/CyRK/array/interp.pyx`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # distutils: language = c++
-# cython: boundscheck=False, wraparound=False, nonecheck=False, cdivision=True
+# cython: boundscheck=False, wraparound=False, nonecheck=False, cdivision=True, initializedcheck=False
 import cython
 from cython.parallel import parallel, prange
 cimport cython
 
 cimport openmp
 
 import numpy as np
@@ -89,15 +89,227 @@
             imin = imid + 1
         else:
             imax = imid
 
     return imin - 1
 
 
-cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values) nogil:
+cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,
+                            int provided_j = -1) nogil:
+    """ Interpolation function for floats. This function will return the index that it found during interpolation.
+
+    Provided a domain, `x_domain` and a dependent array `dependent_values` search domain for value closest to 
+    `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local 
+    slopes of `x_domain` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.
+
+    Based on `numpy`'s `interp` function.
+
+    Parameters
+    ----------
+    desired_x : float
+        Location where `dependent_variables` is desired.
+    x_domain : np.ndarray[float]
+        Domain to search for the correct location.
+    dependent_values : np.ndarray[float]
+        Dependent values that are to be returned after search and interpolation.
+    provided_j : int
+        Give a j index from a previous interpolation to improve performance.
+
+    Returns
+    -------
+    result : float
+        Desired value of `dependent_values`.
+    j_out : int
+        The index that was found during binary_search_with_guess which can be used by other interpolation functions 
+        to improve performance.
+
+    """
+
+    cdef unsigned int lenx
+    lenx = len(x_domain)
+    # TODO: Needs to be at least 3 item long array. Add exception here?
+
+    cdef double left_value
+    left_value = dependent_values[0]
+    cdef double right_value
+    right_value = dependent_values[lenx - 1]
+
+    # Binary Search with Guess
+    cdef unsigned int j
+    j = 0
+    cdef double slope
+
+    cdef double result
+    cdef double fp_at_j
+    cdef double xp_at_j
+    cdef double fp_at_jp1
+    cdef double xp_at_jp1
+
+    # Perform binary search with guess
+    if provided_j == -1:
+        # No j provided; search for it instead.
+        j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    elif provided_j < -1:
+        # Error
+        # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+        j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    else:
+        # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+        j = <unsigned int>provided_j
+
+    cdef int j_out
+    j_out = <int>j
+
+    if j == 0:
+        result = left_value
+    elif j == lenx:
+        result = right_value
+    else:
+        fp_at_j = dependent_values[j]
+        xp_at_j = x_domain[j]
+        if j == lenx - 1:
+            result = fp_at_j
+        elif xp_at_j == desired_x:
+            result = fp_at_j
+        else:
+            fp_at_jp1 = dependent_values[j + 1]
+            xp_at_jp1 = x_domain[j + 1]
+            slope = (fp_at_jp1 - fp_at_j) / (xp_at_jp1 - xp_at_j)
+
+            # If we get nan in one direction, try the other
+            result = slope * (desired_x - xp_at_j) + fp_at_j
+            if isnan(result):
+                result = slope * (desired_x - xp_at_jp1) + fp_at_jp1
+                if isnan(result) and (fp_at_jp1 == fp_at_j):
+                    result = fp_at_j
+
+    return result, j_out
+
+
+cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,
+                                            double complex[:] dependent_values, int provided_j = -1) nogil:
+    """ Interpolation function for complex numbers.
+
+    Provided a domain, `desired_x` and a dependent array `dependent_values` search domain for value closest to 
+    `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local 
+    slopes of `desired_x` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.
+
+    Based on `numpy`'s `interp` function.
+
+    Parameters
+    ----------
+    desired_x : float
+        Location where `dependent_variables` is desired.
+    x_domain : np.ndarray[float]
+        Domain to search for the correct location.
+    dependent_values : np.ndarray[complex]
+        Dependent values that are to be returned after search and interpolation.
+    provided_j : int
+        Give a j index from a previous interpolation to improve performance.
+
+    Returns
+    -------
+    result : complex
+        Desired value of `dependent_values`.
+    j_out : int
+        The index that was found during binary_search_with_guess which can be used by other interpolation functions 
+        to improve performance.
+
+    """
+
+    cdef unsigned int lenx
+    lenx = len(x_domain)
+    # Note: Needs to be at least 3 item long array. Add exception here?
+
+    cdef double complex left_value
+    left_value = dependent_values[0]
+    cdef double complex right_value
+    right_value = dependent_values[lenx - 1]
+
+    # Binary Search with Guess
+    cdef unsigned int j
+    j = 0
+    cdef double slope_real
+    cdef double slope_imag
+    cdef double x_slope_inverse
+
+    cdef double result_real
+    cdef double result_imag
+    cdef double complex fp_at_j
+    cdef double fp_at_j_real
+    cdef double fp_at_j_imag
+    cdef double xp_at_j
+    cdef double complex fp_at_jp1
+    cdef double fp_at_jp1_real
+    cdef double fp_at_jp1_imag
+    cdef double xp_at_jp1
+
+    # Perform binary search with guess
+    if provided_j == -1:
+        # No j provided; search for it instead.
+        j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    elif provided_j < -1:
+        # Error
+        # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+        j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    else:
+        # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+        j = <unsigned int> provided_j
+
+    cdef int j_out
+    j_out = <int> j
+
+    if j == 0:
+        result_real = left_value.real
+        result_imag = left_value.imag
+    elif j == lenx:
+        result_real = right_value.real
+        result_imag = right_value.imag
+    else:
+        fp_at_j = dependent_values[j]
+        fp_at_j_real = fp_at_j.real
+        fp_at_j_imag = fp_at_j.imag
+        xp_at_j = x_domain[j]
+        if j == lenx - 1:
+            result_real = fp_at_j_real
+            result_imag = fp_at_j_imag
+        elif xp_at_j == desired_x:
+            result_real = fp_at_j_real
+            result_imag = fp_at_j_imag
+        else:
+            fp_at_jp1 = dependent_values[j + 1]
+            fp_at_jp1_real = fp_at_jp1.real
+            fp_at_jp1_imag = fp_at_jp1.imag
+            xp_at_jp1 = x_domain[j + 1]
+            x_slope_inverse = 1.0 / (xp_at_jp1 - xp_at_j)
+            slope_real = (fp_at_jp1_real - fp_at_j_real) * x_slope_inverse
+            slope_imag = (fp_at_jp1_imag - fp_at_j_imag) * x_slope_inverse
+
+            # If we get nan in one direction try the other
+            # Real Part
+            result_real = slope_real * (desired_x - xp_at_j) + fp_at_j_real
+            if isnan(result_real):
+                result_real = slope_real * (desired_x - xp_at_jp1) + fp_at_jp1_real
+                if isnan(result_real) and (fp_at_jp1_real == fp_at_j_real):
+                    result_real = fp_at_j_real
+
+            # Imaginary Part
+            result_imag = slope_imag * (desired_x - xp_at_j) + fp_at_j_imag
+            if isnan(result_imag):
+                result_imag = slope_imag * (desired_x - xp_at_jp1) + fp_at_jp1_imag
+                if isnan(result_imag) and (fp_at_jp1_imag == fp_at_j_imag):
+                    result_imag = fp_at_j_imag
+
+    cdef double complex result
+    result = result_real + 1.0j * result_imag
+
+    return result, j_out
+
+
+cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values, int provided_j = -1) nogil:
     """ Interpolation function for floats.
 
     Provided a domain, `x_domain` and a dependent array `dependent_values` search domain for value closest to 
     `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local 
     slopes of `x_domain` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.
 
     Based on `numpy`'s `interp` function.
@@ -106,14 +318,16 @@
     ----------
     desired_x : float
         Location where `dependent_variables` is desired.
     x_domain : np.ndarray[float]
         Domain to search for the correct location.
     dependent_values : np.ndarray[float]
         Dependent values that are to be returned after search and interpolation.
+    provided_j : int
+        Give a j index from a previous interpolation to improve performance.
 
     Returns
     -------
     result : float
         Desired value of `dependent_values`.
 
     """
@@ -135,15 +349,24 @@
     cdef double result
     cdef double fp_at_j
     cdef double xp_at_j
     cdef double fp_at_jp1
     cdef double xp_at_jp1
 
     # Perform binary search with guess
-    j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    if provided_j == -1:
+        # No j provided; search for it instead.
+        j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    elif provided_j < -1:
+        # Error
+        # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+        j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    else:
+        # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+        j = <unsigned int>provided_j
 
     if j == 0:
         result = left_value
     elif j == lenx:
         result = right_value
     else:
         fp_at_j = dependent_values[j]
@@ -164,15 +387,15 @@
                 if isnan(result) and (fp_at_jp1 == fp_at_j):
                     result = fp_at_j
 
     return result
 
 
 cpdef double complex interp_complex(double desired_x, double[:] x_domain,
-                                    double complex[:] dependent_values) nogil:
+                                    double complex[:] dependent_values, int provided_j = -1) nogil:
     """ Interpolation function for complex numbers.
 
     Provided a domain, `desired_x` and a dependent array `dependent_values` search domain for value closest to 
     `desired_x` and return the value of `dependent_values` at that location if it is defined. Otherwise, use local 
     slopes of `desired_x` and `dependent_values` to interpolate a value of `dependent_values` at `desired_x`.
 
     Based on `numpy`'s `interp` function.
@@ -181,14 +404,16 @@
     ----------
     desired_x : float
         Location where `dependent_variables` is desired.
     x_domain : np.ndarray[float]
         Domain to search for the correct location.
     dependent_values : np.ndarray[complex]
         Dependent values that are to be returned after search and interpolation.
+    provided_j : int
+        Give a j index from a previous interpolation to improve performance.
 
     Returns
     -------
     result : complex
         Desired value of `dependent_values`.
 
     """
@@ -217,15 +442,24 @@
     cdef double xp_at_j
     cdef double complex fp_at_jp1
     cdef double fp_at_jp1_real
     cdef double fp_at_jp1_imag
     cdef double xp_at_jp1
 
     # Perform binary search with guess
-    j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    if provided_j == -1:
+        # No j provided; search for it instead.
+        j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    elif provided_j < -1:
+        # Error
+        # TODO: How to handle exception handling in a cdef function... For now just repeat the search.
+        j = binary_search_with_guess(desired_x, x_domain, lenx, j)
+    else:
+        # provided_j is strictly positive and smaller size in this block so the conversion is safe.
+        j = <unsigned int> provided_j
 
     if j == 0:
         result_real = left_value.real
         result_imag = left_value.imag
     elif j == lenx:
         result_real = right_value.real
         result_imag = right_value.imag
```

### Comparing `CyRK-0.6.0/CyRK/cy/cyrk.cpp` & `CyRK-0.6.1/CyRK/cy/cyrk.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 /* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
             "CyRK/cy",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "CyRK.cy.cyrk",
         "sources": [
             "CyRK/cy/cyrk.pyx"
         ]
     },
@@ -1559,177 +1559,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1762,49 +1762,113 @@
 
 /*--- Type declarations ---*/
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
+struct __pyx_ctuple_double__and_int;
+typedef struct __pyx_ctuple_double__and_int __pyx_ctuple_double__and_int;
+struct __pyx_opt_args_4CyRK_5array_6interp_interpj;
+struct __pyx_ctuple___dunderpyx_t_double_complex__and_int;
+typedef struct __pyx_ctuple___dunderpyx_t_double_complex__and_int __pyx_ctuple___dunderpyx_t_double_complex__and_int;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex;
+
+/* "CyRK/array/interp.pxd":5
+ * cdef unsigned int binary_search_with_guess(double key, double[:] array, unsigned int length, unsigned int guess) nogil
+ * 
+ * cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                             int provided_j = *) nogil
+ * 
+ */
+struct __pyx_ctuple_double__and_int {
+  double f0;
+  int f1;
+};
+struct __pyx_opt_args_4CyRK_5array_6interp_interpj {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":8
+ *                             int provided_j = *) nogil
+ * 
+ * cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
+ *                                             double complex[:] dependent_values, int provided_j = *) nogil
+ * 
+ */
+struct __pyx_ctuple___dunderpyx_t_double_complex__and_int {
+  __pyx_t_double_complex f0;
+  int f1;
+};
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":11
+ *                                             double complex[:] dependent_values, int provided_j = *) nogil
+ * 
+ * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                     int provided_j = *) nogil
+ * 
+ */
+struct __pyx_opt_args_4CyRK_5array_6interp_interp {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":14
+ *                     int provided_j = *) nogil
+ * 
+ * cpdef double complex interp_complex(double desired_x, double[:] x_domain, double complex[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                                     int provided_j = *) nogil
+ * 
+ */
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex {
+  int __pyx_n;
+  int provided_j;
+};
 struct __pyx_ctuple_double__and_double;
 typedef struct __pyx_ctuple_double__and_double __pyx_ctuple_double__and_double;
 struct __pyx_defaults;
 typedef struct __pyx_defaults __pyx_defaults;
 struct __pyx_defaults1;
 typedef struct __pyx_defaults1 __pyx_defaults1;
 struct __pyx_defaults2;
@@ -18710,261 +18774,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18973,29 +19037,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -19006,15 +19070,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19023,29 +19087,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -19056,15 +19120,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19073,29 +19137,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -19106,15 +19170,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19123,29 +19187,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -19156,15 +19220,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19173,29 +19237,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -19206,89 +19270,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -19296,33 +19360,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -19330,96 +19394,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19435,15 +19499,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -19451,68 +19515,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19520,15 +19584,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -19543,15 +19607,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19567,15 +19631,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19583,68 +19647,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19652,15 +19716,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19675,15 +19739,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19699,15 +19763,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19715,68 +19779,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19784,15 +19848,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19807,176 +19871,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -36122,26 +36186,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 989, __pyx_L1_error)
```

### Comparing `CyRK-0.6.0/CyRK/cy/cyrk.pyx` & `CyRK-0.6.1/CyRK/cy/cyrk.pyx`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/CyRK/cy/cysolver.cpp` & `CyRK-0.6.1/CyRK/cy/cysolver.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 /* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
             "CyRK/cy",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "CyRK.cy.cysolver",
         "sources": [
             "CyRK/cy/cysolver.pyx"
         ]
     },
@@ -1560,177 +1560,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1764,49 +1764,113 @@
 /*--- Type declarations ---*/
 struct __pyx_obj_4CyRK_2cy_8cysolver_CySolver;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
+struct __pyx_ctuple_double__and_int;
+typedef struct __pyx_ctuple_double__and_int __pyx_ctuple_double__and_int;
+struct __pyx_opt_args_4CyRK_5array_6interp_interpj;
+struct __pyx_ctuple___dunderpyx_t_double_complex__and_int;
+typedef struct __pyx_ctuple___dunderpyx_t_double_complex__and_int __pyx_ctuple___dunderpyx_t_double_complex__and_int;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp;
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex;
+
+/* "CyRK/array/interp.pxd":5
+ * cdef unsigned int binary_search_with_guess(double key, double[:] array, unsigned int length, unsigned int guess) nogil
+ * 
+ * cpdef (double, int) interpj(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                             int provided_j = *) nogil
+ * 
+ */
+struct __pyx_ctuple_double__and_int {
+  double f0;
+  int f1;
+};
+struct __pyx_opt_args_4CyRK_5array_6interp_interpj {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":8
+ *                             int provided_j = *) nogil
+ * 
+ * cpdef (double complex, int) interp_complexj(double desired_x, double[:] x_domain,             # <<<<<<<<<<<<<<
+ *                                             double complex[:] dependent_values, int provided_j = *) nogil
+ * 
+ */
+struct __pyx_ctuple___dunderpyx_t_double_complex__and_int {
+  __pyx_t_double_complex f0;
+  int f1;
+};
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complexj {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":11
+ *                                             double complex[:] dependent_values, int provided_j = *) nogil
+ * 
+ * cpdef double interp(double desired_x, double[:] x_domain, double[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                     int provided_j = *) nogil
+ * 
+ */
+struct __pyx_opt_args_4CyRK_5array_6interp_interp {
+  int __pyx_n;
+  int provided_j;
+};
+
+/* "CyRK/array/interp.pxd":14
+ *                     int provided_j = *) nogil
+ * 
+ * cpdef double complex interp_complex(double desired_x, double[:] x_domain, double complex[:] dependent_values,             # <<<<<<<<<<<<<<
+ *                                     int provided_j = *) nogil
+ * 
+ */
+struct __pyx_opt_args_4CyRK_5array_6interp_interp_complex {
+  int __pyx_n;
+  int provided_j;
+};
 struct __pyx_ctuple_double__and_double;
 typedef struct __pyx_ctuple_double__and_double __pyx_ctuple_double__and_double;
 
 /* "CyRK/cy/cysolver.pyx":34
  * 
  *     def __init__(self,
  *                  (double, double) t_span,             # <<<<<<<<<<<<<<
@@ -1814,17 +1878,17 @@
  *                   tuple args = None,
  */
 struct __pyx_ctuple_double__and_double {
   double f0;
   double f1;
 };
 
-/* "CyRK/cy/cysolver.pxd":3
- * cimport numpy as np
- * from libcpp cimport bool as bool_cpp_t
+/* "CyRK/cy/cysolver.pxd":13
+ * cdef double EPS_100
+ * 
  * cdef class CySolver:             # <<<<<<<<<<<<<<
  * 
  *     # Class attributes
  */
 struct __pyx_obj_4CyRK_2cy_8cysolver_CySolver {
   PyObject_HEAD
   struct __pyx_vtabstruct_4CyRK_2cy_8cysolver_CySolver *__pyx_vtab;
@@ -3068,14 +3132,26 @@
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
+/* PyObjectSetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+#define __Pyx_PyObject_DelAttrStr(o,n) __Pyx_PyObject_SetAttrStr(o, n, NULL)
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value);
+#else
+#define __Pyx_PyObject_DelAttrStr(o,n)   PyObject_DelAttr(o,n)
+#define __Pyx_PyObject_SetAttrStr(o,n,v) PyObject_SetAttr(o,n,v)
+#endif
+
+/* VoidPtrExport.proto */
+static int __Pyx_ExportVoidPtr(PyObject *name, void *p, const char *sig);
+
 /* VoidPtrImport.proto */
 static int __Pyx_ImportVoidPtr_3_0_0(PyObject *module, const char *name, void **p, const char *sig);
 
 /* FunctionImport.proto */
 static int __Pyx_ImportFunction_3_0_0(PyObject *module, const char *funcname, void (**f)(void), const char *sig);
 
 /* InitStrings.proto */
@@ -3316,14 +3392,16 @@
 static const char __pyx_k__3[] = "*";
 static const char __pyx_k__6[] = "'";
 static const char __pyx_k__7[] = ")";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_np[] = "np";
 static const char __pyx_k_y0[] = "y0";
+static const char __pyx_k_EPS[] = "EPS";
+static const char __pyx_k_INF[] = "INF";
 static const char __pyx_k__38[] = "?";
 static const char __pyx_k_abc[] = "abc";
 static const char __pyx_k_and[] = " and ";
 static const char __pyx_k_eps[] = "eps";
 static const char __pyx_k_got[] = " (got ";
 static const char __pyx_k_inf[] = "inf";
 static const char __pyx_k_nan[] = "nan";
@@ -3360,49 +3438,56 @@
 static const char __pyx_k_order[] = "order";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_solve[] = "solve";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_state[] = "state";
 static const char __pyx_k_zeros[] = "zeros";
+static const char __pyx_k_EPS_10[] = "EPS_10";
+static const char __pyx_k_SAFETY[] = "SAFETY";
 static const char __pyx_k_dict_2[] = "_dict";
 static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_t_eval[] = "t_eval";
 static const char __pyx_k_t_span[] = "t_span";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
+static const char __pyx_k_EPS_100[] = "EPS_100";
 static const char __pyx_k_asarray[] = "asarray";
 static const char __pyx_k_disable[] = "disable";
 static const char __pyx_k_float64[] = "float64";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_CySolver[] = "CySolver";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
+static const char __pyx_k_MAX_STEP[] = "MAX_STEP";
 static const char __pyx_k_Sequence[] = "Sequence";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_max_step[] = "max_step";
+static const char __pyx_k_pyx_capi[] = "__pyx_capi__";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_register[] = "register";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_num_extra[] = "num_extra";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_rk_method[] = "rk_method";
 static const char __pyx_k_IndexError[] = "IndexError";
+static const char __pyx_k_MAX_FACTOR[] = "MAX_FACTOR";
+static const char __pyx_k_MIN_FACTOR[] = "MIN_FACTOR";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_first_step[] = "first_step";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
@@ -3641,18 +3726,22 @@
   PyObject *__pyx_n_s_CyRK_cy_cysolver;
   PyObject *__pyx_kp_s_CyRK_cy_cysolver_pyx;
   PyObject *__pyx_n_s_CySolver;
   PyObject *__pyx_n_s_CySolver___reduce_cython;
   PyObject *__pyx_n_s_CySolver___setstate_cython;
   PyObject *__pyx_n_s_CySolver_solve;
   PyObject *__pyx_kp_s_Dimension_d_is_not_direct;
+  PyObject *__pyx_n_s_EPS;
+  PyObject *__pyx_n_s_EPS_10;
+  PyObject *__pyx_n_s_EPS_100;
   PyObject *__pyx_n_s_Ellipsis;
   PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
   PyObject *__pyx_kp_u_Error_in_user_provided_step_size;
   PyObject *__pyx_kp_u_Error_in_user_provided_step_size_2;
+  PyObject *__pyx_n_s_INF;
   PyObject *__pyx_n_s_ImportError;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
   PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2;
   PyObject *__pyx_n_s_IndexError;
   PyObject *__pyx_kp_s_Index_out_of_bounds_axis_d;
   PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
   PyObject *__pyx_kp_u_Integration_Failed;
@@ -3661,20 +3750,24 @@
   PyObject *__pyx_kp_u_Integration_completed;
   PyObject *__pyx_kp_u_Integration_finished_with_no_iss;
   PyObject *__pyx_kp_u_Integration_has_not_started;
   PyObject *__pyx_kp_u_Integration_never_started;
   PyObject *__pyx_kp_u_Integrator_is_running;
   PyObject *__pyx_kp_u_Invalid_mode_expected_c_or_fortr;
   PyObject *__pyx_kp_u_Invalid_shape_in_axis;
+  PyObject *__pyx_n_s_MAX_FACTOR;
+  PyObject *__pyx_n_s_MAX_STEP;
+  PyObject *__pyx_n_s_MIN_FACTOR;
   PyObject *__pyx_n_s_MemoryError;
   PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
   PyObject *__pyx_kp_s_MemoryView_of_r_object;
   PyObject *__pyx_n_b_O;
   PyObject *__pyx_kp_u_Out_of_bounds_on_buffer_access_a;
   PyObject *__pyx_n_s_PickleError;
+  PyObject *__pyx_n_s_SAFETY;
   PyObject *__pyx_n_s_Sequence;
   PyObject *__pyx_kp_s_Step_may_not_be_zero_axis_d;
   PyObject *__pyx_n_s_TypeError;
   PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
   PyObject *__pyx_kp_u_Unexpected_rk_method_provided_Cu;
   PyObject *__pyx_n_s_ValueError;
   PyObject *__pyx_n_s_View_MemoryView;
@@ -3752,14 +3845,15 @@
   PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
   PyObject *__pyx_n_s_obj;
   PyObject *__pyx_n_s_ones;
   PyObject *__pyx_n_s_order;
   PyObject *__pyx_n_s_pack;
   PyObject *__pyx_n_s_pickle;
   PyObject *__pyx_n_s_pyx_PickleError;
+  PyObject *__pyx_n_s_pyx_capi;
   PyObject *__pyx_n_s_pyx_checksum;
   PyObject *__pyx_n_s_pyx_result;
   PyObject *__pyx_n_s_pyx_state;
   PyObject *__pyx_n_s_pyx_type;
   PyObject *__pyx_n_s_pyx_unpickle_CySolver;
   PyObject *__pyx_n_s_pyx_unpickle_Enum;
   PyObject *__pyx_n_s_pyx_vtable;
@@ -3922,18 +4016,22 @@
   Py_CLEAR(clear_module_state->__pyx_n_s_CyRK_cy_cysolver);
   Py_CLEAR(clear_module_state->__pyx_kp_s_CyRK_cy_cysolver_pyx);
   Py_CLEAR(clear_module_state->__pyx_n_s_CySolver);
   Py_CLEAR(clear_module_state->__pyx_n_s_CySolver___reduce_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_CySolver___setstate_cython);
   Py_CLEAR(clear_module_state->__pyx_n_s_CySolver_solve);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Dimension_d_is_not_direct);
+  Py_CLEAR(clear_module_state->__pyx_n_s_EPS);
+  Py_CLEAR(clear_module_state->__pyx_n_s_EPS_10);
+  Py_CLEAR(clear_module_state->__pyx_n_s_EPS_100);
   Py_CLEAR(clear_module_state->__pyx_n_s_Ellipsis);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Empty_shape_tuple_for_cython_arr);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Error_in_user_provided_step_size);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Error_in_user_provided_step_size_2);
+  Py_CLEAR(clear_module_state->__pyx_n_s_INF);
   Py_CLEAR(clear_module_state->__pyx_n_s_ImportError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2);
   Py_CLEAR(clear_module_state->__pyx_n_s_IndexError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Index_out_of_bounds_axis_d);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Indirect_dimensions_not_supporte);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Integration_Failed);
@@ -3942,20 +4040,24 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_Integration_completed);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Integration_finished_with_no_iss);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Integration_has_not_started);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Integration_never_started);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Integrator_is_running);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_mode_expected_c_or_fortr);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Invalid_shape_in_axis);
+  Py_CLEAR(clear_module_state->__pyx_n_s_MAX_FACTOR);
+  Py_CLEAR(clear_module_state->__pyx_n_s_MAX_STEP);
+  Py_CLEAR(clear_module_state->__pyx_n_s_MIN_FACTOR);
   Py_CLEAR(clear_module_state->__pyx_n_s_MemoryError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_MemoryView_of_r_at_0x_x);
   Py_CLEAR(clear_module_state->__pyx_kp_s_MemoryView_of_r_object);
   Py_CLEAR(clear_module_state->__pyx_n_b_O);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Out_of_bounds_on_buffer_access_a);
   Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_SAFETY);
   Py_CLEAR(clear_module_state->__pyx_n_s_Sequence);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_CLEAR(clear_module_state->__pyx_n_s_TypeError);
   Py_CLEAR(clear_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_CLEAR(clear_module_state->__pyx_kp_u_Unexpected_rk_method_provided_Cu);
   Py_CLEAR(clear_module_state->__pyx_n_s_ValueError);
   Py_CLEAR(clear_module_state->__pyx_n_s_View_MemoryView);
@@ -4033,14 +4135,15 @@
   Py_CLEAR(clear_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
   Py_CLEAR(clear_module_state->__pyx_n_s_obj);
   Py_CLEAR(clear_module_state->__pyx_n_s_ones);
   Py_CLEAR(clear_module_state->__pyx_n_s_order);
   Py_CLEAR(clear_module_state->__pyx_n_s_pack);
   Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
+  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_capi);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_CySolver);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_Enum);
   Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
@@ -4180,18 +4283,22 @@
   Py_VISIT(traverse_module_state->__pyx_n_s_CyRK_cy_cysolver);
   Py_VISIT(traverse_module_state->__pyx_kp_s_CyRK_cy_cysolver_pyx);
   Py_VISIT(traverse_module_state->__pyx_n_s_CySolver);
   Py_VISIT(traverse_module_state->__pyx_n_s_CySolver___reduce_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_CySolver___setstate_cython);
   Py_VISIT(traverse_module_state->__pyx_n_s_CySolver_solve);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Dimension_d_is_not_direct);
+  Py_VISIT(traverse_module_state->__pyx_n_s_EPS);
+  Py_VISIT(traverse_module_state->__pyx_n_s_EPS_10);
+  Py_VISIT(traverse_module_state->__pyx_n_s_EPS_100);
   Py_VISIT(traverse_module_state->__pyx_n_s_Ellipsis);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Empty_shape_tuple_for_cython_arr);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Error_in_user_provided_step_size);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Error_in_user_provided_step_size_2);
+  Py_VISIT(traverse_module_state->__pyx_n_s_INF);
   Py_VISIT(traverse_module_state->__pyx_n_s_ImportError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2);
   Py_VISIT(traverse_module_state->__pyx_n_s_IndexError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Index_out_of_bounds_axis_d);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Indirect_dimensions_not_supporte);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Integration_Failed);
@@ -4200,20 +4307,24 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_Integration_completed);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Integration_finished_with_no_iss);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Integration_has_not_started);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Integration_never_started);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Integrator_is_running);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_mode_expected_c_or_fortr);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Invalid_shape_in_axis);
+  Py_VISIT(traverse_module_state->__pyx_n_s_MAX_FACTOR);
+  Py_VISIT(traverse_module_state->__pyx_n_s_MAX_STEP);
+  Py_VISIT(traverse_module_state->__pyx_n_s_MIN_FACTOR);
   Py_VISIT(traverse_module_state->__pyx_n_s_MemoryError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_MemoryView_of_r_at_0x_x);
   Py_VISIT(traverse_module_state->__pyx_kp_s_MemoryView_of_r_object);
   Py_VISIT(traverse_module_state->__pyx_n_b_O);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Out_of_bounds_on_buffer_access_a);
   Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_SAFETY);
   Py_VISIT(traverse_module_state->__pyx_n_s_Sequence);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Step_may_not_be_zero_axis_d);
   Py_VISIT(traverse_module_state->__pyx_n_s_TypeError);
   Py_VISIT(traverse_module_state->__pyx_kp_s_Unable_to_convert_item_to_object);
   Py_VISIT(traverse_module_state->__pyx_kp_u_Unexpected_rk_method_provided_Cu);
   Py_VISIT(traverse_module_state->__pyx_n_s_ValueError);
   Py_VISIT(traverse_module_state->__pyx_n_s_View_MemoryView);
@@ -4291,14 +4402,15 @@
   Py_VISIT(traverse_module_state->__pyx_kp_u_numpy_core_umath_failed_to_impor);
   Py_VISIT(traverse_module_state->__pyx_n_s_obj);
   Py_VISIT(traverse_module_state->__pyx_n_s_ones);
   Py_VISIT(traverse_module_state->__pyx_n_s_order);
   Py_VISIT(traverse_module_state->__pyx_n_s_pack);
   Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
+  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_capi);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_CySolver);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_Enum);
   Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
@@ -4480,18 +4592,22 @@
 #define __pyx_n_s_CyRK_cy_cysolver __pyx_mstate_global->__pyx_n_s_CyRK_cy_cysolver
 #define __pyx_kp_s_CyRK_cy_cysolver_pyx __pyx_mstate_global->__pyx_kp_s_CyRK_cy_cysolver_pyx
 #define __pyx_n_s_CySolver __pyx_mstate_global->__pyx_n_s_CySolver
 #define __pyx_n_s_CySolver___reduce_cython __pyx_mstate_global->__pyx_n_s_CySolver___reduce_cython
 #define __pyx_n_s_CySolver___setstate_cython __pyx_mstate_global->__pyx_n_s_CySolver___setstate_cython
 #define __pyx_n_s_CySolver_solve __pyx_mstate_global->__pyx_n_s_CySolver_solve
 #define __pyx_kp_s_Dimension_d_is_not_direct __pyx_mstate_global->__pyx_kp_s_Dimension_d_is_not_direct
+#define __pyx_n_s_EPS __pyx_mstate_global->__pyx_n_s_EPS
+#define __pyx_n_s_EPS_10 __pyx_mstate_global->__pyx_n_s_EPS_10
+#define __pyx_n_s_EPS_100 __pyx_mstate_global->__pyx_n_s_EPS_100
 #define __pyx_n_s_Ellipsis __pyx_mstate_global->__pyx_n_s_Ellipsis
 #define __pyx_kp_s_Empty_shape_tuple_for_cython_arr __pyx_mstate_global->__pyx_kp_s_Empty_shape_tuple_for_cython_arr
 #define __pyx_kp_u_Error_in_user_provided_step_size __pyx_mstate_global->__pyx_kp_u_Error_in_user_provided_step_size
 #define __pyx_kp_u_Error_in_user_provided_step_size_2 __pyx_mstate_global->__pyx_kp_u_Error_in_user_provided_step_size_2
+#define __pyx_n_s_INF __pyx_mstate_global->__pyx_n_s_INF
 #define __pyx_n_s_ImportError __pyx_mstate_global->__pyx_n_s_ImportError
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
 #define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2
 #define __pyx_n_s_IndexError __pyx_mstate_global->__pyx_n_s_IndexError
 #define __pyx_kp_s_Index_out_of_bounds_axis_d __pyx_mstate_global->__pyx_kp_s_Index_out_of_bounds_axis_d
 #define __pyx_kp_s_Indirect_dimensions_not_supporte __pyx_mstate_global->__pyx_kp_s_Indirect_dimensions_not_supporte
 #define __pyx_kp_u_Integration_Failed __pyx_mstate_global->__pyx_kp_u_Integration_Failed
@@ -4500,20 +4616,24 @@
 #define __pyx_kp_u_Integration_completed __pyx_mstate_global->__pyx_kp_u_Integration_completed
 #define __pyx_kp_u_Integration_finished_with_no_iss __pyx_mstate_global->__pyx_kp_u_Integration_finished_with_no_iss
 #define __pyx_kp_u_Integration_has_not_started __pyx_mstate_global->__pyx_kp_u_Integration_has_not_started
 #define __pyx_kp_u_Integration_never_started __pyx_mstate_global->__pyx_kp_u_Integration_never_started
 #define __pyx_kp_u_Integrator_is_running __pyx_mstate_global->__pyx_kp_u_Integrator_is_running
 #define __pyx_kp_u_Invalid_mode_expected_c_or_fortr __pyx_mstate_global->__pyx_kp_u_Invalid_mode_expected_c_or_fortr
 #define __pyx_kp_u_Invalid_shape_in_axis __pyx_mstate_global->__pyx_kp_u_Invalid_shape_in_axis
+#define __pyx_n_s_MAX_FACTOR __pyx_mstate_global->__pyx_n_s_MAX_FACTOR
+#define __pyx_n_s_MAX_STEP __pyx_mstate_global->__pyx_n_s_MAX_STEP
+#define __pyx_n_s_MIN_FACTOR __pyx_mstate_global->__pyx_n_s_MIN_FACTOR
 #define __pyx_n_s_MemoryError __pyx_mstate_global->__pyx_n_s_MemoryError
 #define __pyx_kp_s_MemoryView_of_r_at_0x_x __pyx_mstate_global->__pyx_kp_s_MemoryView_of_r_at_0x_x
 #define __pyx_kp_s_MemoryView_of_r_object __pyx_mstate_global->__pyx_kp_s_MemoryView_of_r_object
 #define __pyx_n_b_O __pyx_mstate_global->__pyx_n_b_O
 #define __pyx_kp_u_Out_of_bounds_on_buffer_access_a __pyx_mstate_global->__pyx_kp_u_Out_of_bounds_on_buffer_access_a
 #define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
+#define __pyx_n_s_SAFETY __pyx_mstate_global->__pyx_n_s_SAFETY
 #define __pyx_n_s_Sequence __pyx_mstate_global->__pyx_n_s_Sequence
 #define __pyx_kp_s_Step_may_not_be_zero_axis_d __pyx_mstate_global->__pyx_kp_s_Step_may_not_be_zero_axis_d
 #define __pyx_n_s_TypeError __pyx_mstate_global->__pyx_n_s_TypeError
 #define __pyx_kp_s_Unable_to_convert_item_to_object __pyx_mstate_global->__pyx_kp_s_Unable_to_convert_item_to_object
 #define __pyx_kp_u_Unexpected_rk_method_provided_Cu __pyx_mstate_global->__pyx_kp_u_Unexpected_rk_method_provided_Cu
 #define __pyx_n_s_ValueError __pyx_mstate_global->__pyx_n_s_ValueError
 #define __pyx_n_s_View_MemoryView __pyx_mstate_global->__pyx_n_s_View_MemoryView
@@ -4591,14 +4711,15 @@
 #define __pyx_kp_u_numpy_core_umath_failed_to_impor __pyx_mstate_global->__pyx_kp_u_numpy_core_umath_failed_to_impor
 #define __pyx_n_s_obj __pyx_mstate_global->__pyx_n_s_obj
 #define __pyx_n_s_ones __pyx_mstate_global->__pyx_n_s_ones
 #define __pyx_n_s_order __pyx_mstate_global->__pyx_n_s_order
 #define __pyx_n_s_pack __pyx_mstate_global->__pyx_n_s_pack
 #define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
 #define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
+#define __pyx_n_s_pyx_capi __pyx_mstate_global->__pyx_n_s_pyx_capi
 #define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
 #define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
 #define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
 #define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
 #define __pyx_n_s_pyx_unpickle_CySolver __pyx_mstate_global->__pyx_n_s_pyx_unpickle_CySolver
 #define __pyx_n_s_pyx_unpickle_Enum __pyx_mstate_global->__pyx_n_s_pyx_unpickle_Enum
 #define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
@@ -17983,261 +18104,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18246,29 +18367,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18279,15 +18400,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18296,29 +18417,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18329,15 +18450,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18346,29 +18467,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18379,15 +18500,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18396,29 +18517,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18429,15 +18550,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18446,29 +18567,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18479,89 +18600,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18569,33 +18690,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18603,96 +18724,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18708,15 +18829,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18724,68 +18845,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18793,15 +18914,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18816,15 +18937,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18840,15 +18961,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18856,68 +18977,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18925,15 +19046,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18948,15 +19069,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18972,15 +19093,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18988,68 +19109,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19057,15 +19178,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19080,176 +19201,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -28441,15 +28562,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "CyRK/cy/cysolver.pxd":26
+/* "CyRK/cy/cysolver.pxd":36
  * 
  *     # -- Integration information
  *     cdef public char status             # <<<<<<<<<<<<<<
  *     cdef public str message
  *     cdef public bool_cpp_t success
  */
 
@@ -28472,15 +28593,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyInt_From_char(__pyx_v_self->status); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 26, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_char(__pyx_v_self->status); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 36, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -28511,29 +28632,29 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   char __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyInt_As_char(__pyx_v_value); if (unlikely((__pyx_t_1 == (char)-1) && PyErr_Occurred())) __PYX_ERR(3, 26, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_As_char(__pyx_v_value); if (unlikely((__pyx_t_1 == (char)-1) && PyErr_Occurred())) __PYX_ERR(3, 36, __pyx_L1_error)
   __pyx_v_self->status = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("CyRK.cy.cysolver.CySolver.status.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "CyRK/cy/cysolver.pxd":27
+/* "CyRK/cy/cysolver.pxd":37
  *     # -- Integration information
  *     cdef public char status
  *     cdef public str message             # <<<<<<<<<<<<<<
  *     cdef public bool_cpp_t success
  *     cdef double t_start, t_end, t_delta, t_delta_abs, direction, direction_inf
  */
 
@@ -28585,15 +28706,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(3, 27, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(3, 37, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->message);
   __Pyx_DECREF(__pyx_v_self->message);
   __pyx_v_self->message = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
@@ -28636,15 +28757,15 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "CyRK/cy/cysolver.pxd":28
+/* "CyRK/cy/cysolver.pxd":38
  *     cdef public char status
  *     cdef public str message
  *     cdef public bool_cpp_t success             # <<<<<<<<<<<<<<
  *     cdef double t_start, t_end, t_delta, t_delta_abs, direction, direction_inf
  *     cdef double rtol, atol
  */
 
@@ -28667,15 +28788,15 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->success); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBool_FromLong(__pyx_v_self->success); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 38, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
@@ -28706,15 +28827,15 @@
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   bool __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(3, 28, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_IsTrue(__pyx_v_value); if (unlikely((__pyx_t_1 == ((bool)-1)) && PyErr_Occurred())) __PYX_ERR(3, 38, __pyx_L1_error)
   __pyx_v_self->success = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("CyRK.cy.cysolver.CySolver.success.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
@@ -31550,18 +31671,22 @@
     {&__pyx_n_s_CyRK_cy_cysolver, __pyx_k_CyRK_cy_cysolver, sizeof(__pyx_k_CyRK_cy_cysolver), 0, 0, 1, 1},
     {&__pyx_kp_s_CyRK_cy_cysolver_pyx, __pyx_k_CyRK_cy_cysolver_pyx, sizeof(__pyx_k_CyRK_cy_cysolver_pyx), 0, 0, 1, 0},
     {&__pyx_n_s_CySolver, __pyx_k_CySolver, sizeof(__pyx_k_CySolver), 0, 0, 1, 1},
     {&__pyx_n_s_CySolver___reduce_cython, __pyx_k_CySolver___reduce_cython, sizeof(__pyx_k_CySolver___reduce_cython), 0, 0, 1, 1},
     {&__pyx_n_s_CySolver___setstate_cython, __pyx_k_CySolver___setstate_cython, sizeof(__pyx_k_CySolver___setstate_cython), 0, 0, 1, 1},
     {&__pyx_n_s_CySolver_solve, __pyx_k_CySolver_solve, sizeof(__pyx_k_CySolver_solve), 0, 0, 1, 1},
     {&__pyx_kp_s_Dimension_d_is_not_direct, __pyx_k_Dimension_d_is_not_direct, sizeof(__pyx_k_Dimension_d_is_not_direct), 0, 0, 1, 0},
+    {&__pyx_n_s_EPS, __pyx_k_EPS, sizeof(__pyx_k_EPS), 0, 0, 1, 1},
+    {&__pyx_n_s_EPS_10, __pyx_k_EPS_10, sizeof(__pyx_k_EPS_10), 0, 0, 1, 1},
+    {&__pyx_n_s_EPS_100, __pyx_k_EPS_100, sizeof(__pyx_k_EPS_100), 0, 0, 1, 1},
     {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
     {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
     {&__pyx_kp_u_Error_in_user_provided_step_size, __pyx_k_Error_in_user_provided_step_size, sizeof(__pyx_k_Error_in_user_provided_step_size), 0, 1, 0, 0},
     {&__pyx_kp_u_Error_in_user_provided_step_size_2, __pyx_k_Error_in_user_provided_step_size_2, sizeof(__pyx_k_Error_in_user_provided_step_size_2), 0, 1, 0, 0},
+    {&__pyx_n_s_INF, __pyx_k_INF, sizeof(__pyx_k_INF), 0, 0, 1, 1},
     {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
     {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0_2, __pyx_k_Incompatible_checksums_0x_x_vs_0_2, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0_2), 0, 0, 1, 0},
     {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
     {&__pyx_kp_s_Index_out_of_bounds_axis_d, __pyx_k_Index_out_of_bounds_axis_d, sizeof(__pyx_k_Index_out_of_bounds_axis_d), 0, 0, 1, 0},
     {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
     {&__pyx_kp_u_Integration_Failed, __pyx_k_Integration_Failed, sizeof(__pyx_k_Integration_Failed), 0, 1, 0, 0},
@@ -31570,20 +31695,24 @@
     {&__pyx_kp_u_Integration_completed, __pyx_k_Integration_completed, sizeof(__pyx_k_Integration_completed), 0, 1, 0, 0},
     {&__pyx_kp_u_Integration_finished_with_no_iss, __pyx_k_Integration_finished_with_no_iss, sizeof(__pyx_k_Integration_finished_with_no_iss), 0, 1, 0, 0},
     {&__pyx_kp_u_Integration_has_not_started, __pyx_k_Integration_has_not_started, sizeof(__pyx_k_Integration_has_not_started), 0, 1, 0, 0},
     {&__pyx_kp_u_Integration_never_started, __pyx_k_Integration_never_started, sizeof(__pyx_k_Integration_never_started), 0, 1, 0, 0},
     {&__pyx_kp_u_Integrator_is_running, __pyx_k_Integrator_is_running, sizeof(__pyx_k_Integrator_is_running), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 1, 0, 0},
     {&__pyx_kp_u_Invalid_shape_in_axis, __pyx_k_Invalid_shape_in_axis, sizeof(__pyx_k_Invalid_shape_in_axis), 0, 1, 0, 0},
+    {&__pyx_n_s_MAX_FACTOR, __pyx_k_MAX_FACTOR, sizeof(__pyx_k_MAX_FACTOR), 0, 0, 1, 1},
+    {&__pyx_n_s_MAX_STEP, __pyx_k_MAX_STEP, sizeof(__pyx_k_MAX_STEP), 0, 0, 1, 1},
+    {&__pyx_n_s_MIN_FACTOR, __pyx_k_MIN_FACTOR, sizeof(__pyx_k_MIN_FACTOR), 0, 0, 1, 1},
     {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
     {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
     {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
     {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
     {&__pyx_kp_u_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 1, 0, 0},
     {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
+    {&__pyx_n_s_SAFETY, __pyx_k_SAFETY, sizeof(__pyx_k_SAFETY), 0, 0, 1, 1},
     {&__pyx_n_s_Sequence, __pyx_k_Sequence, sizeof(__pyx_k_Sequence), 0, 0, 1, 1},
     {&__pyx_kp_s_Step_may_not_be_zero_axis_d, __pyx_k_Step_may_not_be_zero_axis_d, sizeof(__pyx_k_Step_may_not_be_zero_axis_d), 0, 0, 1, 0},
     {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
     {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
     {&__pyx_kp_u_Unexpected_rk_method_provided_Cu, __pyx_k_Unexpected_rk_method_provided_Cu, sizeof(__pyx_k_Unexpected_rk_method_provided_Cu), 0, 1, 0, 0},
     {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
     {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
@@ -31661,14 +31790,15 @@
     {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
     {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
     {&__pyx_n_s_ones, __pyx_k_ones, sizeof(__pyx_k_ones), 0, 0, 1, 1},
     {&__pyx_n_s_order, __pyx_k_order, sizeof(__pyx_k_order), 0, 0, 1, 1},
     {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
     {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
+    {&__pyx_n_s_pyx_capi, __pyx_k_pyx_capi, sizeof(__pyx_k_pyx_capi), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_CySolver, __pyx_k_pyx_unpickle_CySolver, sizeof(__pyx_k_pyx_unpickle_CySolver), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
     {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
@@ -31766,26 +31896,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 989, __pyx_L1_error)
@@ -32059,18 +32189,32 @@
   indirect_contiguous = Py_None; Py_INCREF(Py_None);
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 static int __Pyx_modinit_variable_export_code(void) {
   __Pyx_RefNannyDeclarations
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_export_code", 0);
   /*--- Variable export code ---*/
+  if (__Pyx_ExportVoidPtr(__pyx_n_s_SAFETY, (void *)&__pyx_v_4CyRK_2cy_8cysolver_SAFETY, "double") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportVoidPtr(__pyx_n_s_MIN_FACTOR, (void *)&__pyx_v_4CyRK_2cy_8cysolver_MIN_FACTOR, "double") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportVoidPtr(__pyx_n_s_MAX_FACTOR, (void *)&__pyx_v_4CyRK_2cy_8cysolver_MAX_FACTOR, "double") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportVoidPtr(__pyx_n_s_MAX_STEP, (void *)&__pyx_v_4CyRK_2cy_8cysolver_MAX_STEP, "double") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportVoidPtr(__pyx_n_s_INF, (void *)&__pyx_v_4CyRK_2cy_8cysolver_INF, "double") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportVoidPtr(__pyx_n_s_EPS, (void *)&__pyx_v_4CyRK_2cy_8cysolver_EPS, "double") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportVoidPtr(__pyx_n_s_EPS_10, (void *)&__pyx_v_4CyRK_2cy_8cysolver_EPS_10, "double") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__Pyx_ExportVoidPtr(__pyx_n_s_EPS_100, (void *)&__pyx_v_4CyRK_2cy_8cysolver_EPS_100, "double") < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
+  __pyx_L1_error:;
+  __Pyx_RefNannyFinishContext();
+  return -1;
 }
 
 static int __Pyx_modinit_function_export_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_export_code", 0);
   /*--- Function export code ---*/
   __Pyx_RefNannyFinishContext();
@@ -32671,15 +32815,15 @@
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
-  (void)__Pyx_modinit_variable_export_code();
+  if (unlikely((__Pyx_modinit_variable_export_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_function_export_code();
   if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   if (unlikely((__Pyx_modinit_variable_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   if (unlikely((__Pyx_modinit_function_import_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
@@ -41218,14 +41362,55 @@
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
+/* PyObjectSetAttrStr */
+  #if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE int __Pyx_PyObject_SetAttrStr(PyObject* obj, PyObject* attr_name, PyObject* value) {
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_setattro))
+        return tp->tp_setattro(obj, attr_name, value);
+#if PY_MAJOR_VERSION < 3
+    if (likely(tp->tp_setattr))
+        return tp->tp_setattr(obj, PyString_AS_STRING(attr_name), value);
+#endif
+    return PyObject_SetAttr(obj, attr_name, value);
+}
+#endif
+
+/* VoidPtrExport */
+  static int __Pyx_ExportVoidPtr(PyObject *name, void *p, const char *sig) {
+    PyObject *d;
+    PyObject *cobj = 0;
+    d = PyDict_GetItem(__pyx_d, __pyx_n_s_pyx_capi);
+    Py_XINCREF(d);
+    if (!d) {
+        d = PyDict_New();
+        if (!d)
+            goto bad;
+        if (__Pyx_PyObject_SetAttrStr(__pyx_m, __pyx_n_s_pyx_capi, d) < 0)
+            goto bad;
+    }
+    cobj = PyCapsule_New(p, sig, 0);
+    if (!cobj)
+        goto bad;
+    if (PyDict_SetItem(d, name, cobj) < 0)
+        goto bad;
+    Py_DECREF(cobj);
+    Py_DECREF(d);
+    return 0;
+bad:
+    Py_XDECREF(cobj);
+    Py_XDECREF(d);
+    return -1;
+}
+
 /* VoidPtrImport */
   #ifndef __PYX_HAVE_RT_ImportVoidPtr_3_0_0
 #define __PYX_HAVE_RT_ImportVoidPtr_3_0_0
 static int __Pyx_ImportVoidPtr_3_0_0(PyObject *module, const char *name, void **p, const char *sig) {
     PyObject *d = 0;
     PyObject *cobj = 0;
     d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
```

### Comparing `CyRK-0.6.0/CyRK/cy/cysolver.pxd` & `CyRK-0.6.1/CyRK/cy/cysolver.pxd`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,19 @@
 cimport numpy as np
 from libcpp cimport bool as bool_cpp_t
+
+cdef double SAFETY
+cdef double MIN_FACTOR
+cdef double MAX_FACTOR
+cdef double MAX_STEP
+cdef double INF
+cdef double EPS
+cdef double EPS_10
+cdef double EPS_100
+
 cdef class CySolver:
 
     # Class attributes    
     # -- Live variables
     cdef double t_new, t_old
     cdef unsigned int len_t
     cdef double[:] y_new_view, y_old_view, dy_new_view, dy_old_view
```

### Comparing `CyRK-0.6.0/CyRK/cy/cysolver.pyx` & `CyRK-0.6.1/CyRK/cy/cysolver.pyx`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/CyRK/cy/cysolvertest.cpp` & `CyRK-0.6.1/CyRK/cy/cysolvertest.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 /* Generated by Cython 3.0.0 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
             "CyRK/cy",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "CyRK.cy.cysolvertest",
         "sources": [
             "CyRK/cy/cysolvertest.pyx"
         ]
     },
@@ -1559,177 +1559,177 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1770,53 +1770,53 @@
 struct __pyx_obj_4CyRK_2cy_12cysolvertest_CySolverLotkavolterra;
 struct __pyx_obj_4CyRK_2cy_12cysolvertest_CySolverPendulum;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
 
-/* "CyRK/cy/cysolver.pxd":3
- * cimport numpy as np
- * from libcpp cimport bool as bool_cpp_t
+/* "CyRK/cy/cysolver.pxd":13
+ * cdef double EPS_100
+ * 
  * cdef class CySolver:             # <<<<<<<<<<<<<<
  * 
  *     # Class attributes
  */
 struct __pyx_obj_4CyRK_2cy_8cysolver_CySolver {
   PyObject_HEAD
   struct __pyx_vtabstruct_4CyRK_2cy_8cysolver_CySolver *__pyx_vtab;
@@ -2037,17 +2037,17 @@
   PyObject *from_object;
   PyObject *(*to_object_func)(char *);
   int (*to_dtype_func)(char *, PyObject *);
 };
 
 
 
-/* "CyRK/cy/cysolver.pxd":3
- * cimport numpy as np
- * from libcpp cimport bool as bool_cpp_t
+/* "CyRK/cy/cysolver.pxd":13
+ * cdef double EPS_100
+ * 
  * cdef class CySolver:             # <<<<<<<<<<<<<<
  * 
  *     # Class attributes
  */
 
 struct __pyx_vtabstruct_4CyRK_2cy_8cysolver_CySolver {
   double (*calc_first_step)(struct __pyx_obj_4CyRK_2cy_8cysolver_CySolver *);
@@ -3224,14 +3224,17 @@
 #define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
 #define __Pyx_DECREF_TypeName(obj)
 #endif
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
+/* VoidPtrImport.proto */
+static int __Pyx_ImportVoidPtr_3_0_0(PyObject *module, const char *name, void **p, const char *sig);
+
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
 /* #### Code section: module_declarations ### */
 static PyObject *__pyx_array_get_memview(struct __pyx_array_obj *__pyx_v_self); /* proto*/
 static char *__pyx_memoryview_get_item_pointer(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_index); /* proto*/
 static PyObject *__pyx_memoryview_is_slice(struct __pyx_memoryview_obj *__pyx_v_self, PyObject *__pyx_v_obj); /* proto*/
@@ -3285,14 +3288,30 @@
 static CYTHON_INLINE int __pyx_f_5numpy_import_array(void); /*proto*/
 
 /* Module declarations from "libc.math" */
 
 /* Module declarations from "libcpp" */
 
 /* Module declarations from "CyRK.cy.cysolver" */
+static double *__pyx_vp_4CyRK_2cy_8cysolver_SAFETY = 0;
+#define __pyx_v_4CyRK_2cy_8cysolver_SAFETY (*__pyx_vp_4CyRK_2cy_8cysolver_SAFETY)
+static double *__pyx_vp_4CyRK_2cy_8cysolver_MIN_FACTOR = 0;
+#define __pyx_v_4CyRK_2cy_8cysolver_MIN_FACTOR (*__pyx_vp_4CyRK_2cy_8cysolver_MIN_FACTOR)
+static double *__pyx_vp_4CyRK_2cy_8cysolver_MAX_FACTOR = 0;
+#define __pyx_v_4CyRK_2cy_8cysolver_MAX_FACTOR (*__pyx_vp_4CyRK_2cy_8cysolver_MAX_FACTOR)
+static double *__pyx_vp_4CyRK_2cy_8cysolver_MAX_STEP = 0;
+#define __pyx_v_4CyRK_2cy_8cysolver_MAX_STEP (*__pyx_vp_4CyRK_2cy_8cysolver_MAX_STEP)
+static double *__pyx_vp_4CyRK_2cy_8cysolver_INF = 0;
+#define __pyx_v_4CyRK_2cy_8cysolver_INF (*__pyx_vp_4CyRK_2cy_8cysolver_INF)
+static double *__pyx_vp_4CyRK_2cy_8cysolver_EPS = 0;
+#define __pyx_v_4CyRK_2cy_8cysolver_EPS (*__pyx_vp_4CyRK_2cy_8cysolver_EPS)
+static double *__pyx_vp_4CyRK_2cy_8cysolver_EPS_10 = 0;
+#define __pyx_v_4CyRK_2cy_8cysolver_EPS_10 (*__pyx_vp_4CyRK_2cy_8cysolver_EPS_10)
+static double *__pyx_vp_4CyRK_2cy_8cysolver_EPS_100 = 0;
+#define __pyx_v_4CyRK_2cy_8cysolver_EPS_100 (*__pyx_vp_4CyRK_2cy_8cysolver_EPS_100)
 
 /* Module declarations from "CyRK.cy.cysolvertest" */
 static PyObject *__pyx_collections_abc_Sequence = 0;
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
@@ -18055,261 +18074,261 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18318,29 +18337,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -18351,15 +18370,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18368,29 +18387,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -18401,15 +18420,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18418,29 +18437,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -18451,15 +18470,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18468,29 +18487,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -18501,15 +18520,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18518,29 +18537,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(2, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -18551,89 +18570,89 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18641,33 +18660,33 @@
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":968
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":969
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(2, 969, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":967
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
@@ -18675,96 +18694,96 @@
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":972
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":974
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":973
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":975
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":971
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18780,15 +18799,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -18796,68 +18815,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":981
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 981, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":982
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 982, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 983, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 983, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":980
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18865,15 +18884,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":979
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -18888,15 +18907,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -18912,15 +18931,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -18928,68 +18947,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":987
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 987, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":988
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 988, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 989, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 989, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":986
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -18997,15 +19016,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":985
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19020,15 +19039,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19044,15 +19063,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -19060,68 +19079,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":993
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(2, 993, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":994
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(2, 994, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":995
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(2, 995, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(2, 995, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
+    /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":992
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -19129,15 +19148,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":991
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -19152,176 +19171,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1010
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":998
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1025
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1013
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1035
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1028
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1042
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1038
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+/* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1049
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":1045
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -33051,26 +33070,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(0, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":983
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(2, 983, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../../tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../../tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/__init__.cython-30.pxd":989
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(2, 989, __pyx_L1_error)
@@ -33841,18 +33860,37 @@
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static int __Pyx_modinit_variable_import_code(void) {
   __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_variable_import_code", 0);
   /*--- Variable import code ---*/
+  __pyx_t_1 = PyImport_ImportModule("CyRK.cy.cysolver"); if (!__pyx_t_1) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (__Pyx_ImportVoidPtr_3_0_0(__pyx_t_1, "SAFETY", (void **)&__pyx_vp_4CyRK_2cy_8cysolver_SAFETY, "double") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_3_0_0(__pyx_t_1, "MIN_FACTOR", (void **)&__pyx_vp_4CyRK_2cy_8cysolver_MIN_FACTOR, "double") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_3_0_0(__pyx_t_1, "MAX_FACTOR", (void **)&__pyx_vp_4CyRK_2cy_8cysolver_MAX_FACTOR, "double") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_3_0_0(__pyx_t_1, "MAX_STEP", (void **)&__pyx_vp_4CyRK_2cy_8cysolver_MAX_STEP, "double") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_3_0_0(__pyx_t_1, "INF", (void **)&__pyx_vp_4CyRK_2cy_8cysolver_INF, "double") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_3_0_0(__pyx_t_1, "EPS", (void **)&__pyx_vp_4CyRK_2cy_8cysolver_EPS, "double") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_3_0_0(__pyx_t_1, "EPS_10", (void **)&__pyx_vp_4CyRK_2cy_8cysolver_EPS_10, "double") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  if (__Pyx_ImportVoidPtr_3_0_0(__pyx_t_1, "EPS_100", (void **)&__pyx_vp_4CyRK_2cy_8cysolver_EPS_100, "double") < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_RefNannyFinishContext();
+  return -1;
 }
 
 static int __Pyx_modinit_function_import_code(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
@@ -34135,15 +34173,15 @@
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
   if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(1, 1, __pyx_L1_error)
   if (unlikely((__Pyx_modinit_type_import_code() < 0))) __PYX_ERR(1, 1, __pyx_L1_error)
-  (void)__Pyx_modinit_variable_import_code();
+  if (unlikely((__Pyx_modinit_variable_import_code() < 0))) __PYX_ERR(1, 1, __pyx_L1_error)
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(1, 1, __pyx_L1_error)
   #endif
 
   /* "View.MemoryView":99
@@ -42626,14 +42664,47 @@
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
+/* VoidPtrImport */
+  #ifndef __PYX_HAVE_RT_ImportVoidPtr_3_0_0
+#define __PYX_HAVE_RT_ImportVoidPtr_3_0_0
+static int __Pyx_ImportVoidPtr_3_0_0(PyObject *module, const char *name, void **p, const char *sig) {
+    PyObject *d = 0;
+    PyObject *cobj = 0;
+    d = PyObject_GetAttrString(module, (char *)"__pyx_capi__");
+    if (!d)
+        goto bad;
+    cobj = PyDict_GetItemString(d, name);
+    if (!cobj) {
+        PyErr_Format(PyExc_ImportError,
+            "%.200s does not export expected C variable %.200s",
+                PyModule_GetName(module), name);
+        goto bad;
+    }
+    if (!PyCapsule_IsValid(cobj, sig)) {
+        PyErr_Format(PyExc_TypeError,
+            "C variable %.200s.%.200s has wrong signature (expected %.500s, got %.500s)",
+             PyModule_GetName(module), name, sig, PyCapsule_GetName(cobj));
+        goto bad;
+    }
+    *p = PyCapsule_GetPointer(cobj, sig);
+    if (!(*p))
+        goto bad;
+    Py_DECREF(d);
+    return 0;
+bad:
+    Py_XDECREF(d);
+    return -1;
+}
+#endif
+
 /* InitStrings */
   #if PY_MAJOR_VERSION >= 3
 static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
     if (t.is_unicode | t.is_str) {
         if (t.intern) {
             *str = PyUnicode_InternFromString(t.s);
         } else if (t.encoding) {
```

### Comparing `CyRK-0.6.0/CyRK/cy/cysolvertest.pyx` & `CyRK-0.6.1/CyRK/cy/cysolvertest.pyx`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/CyRK/helper.py` & `CyRK-0.6.1/CyRK/helper.py`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/CyRK/nb/dop_coefficients.py` & `CyRK-0.6.1/CyRK/nb/dop_coefficients.py`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/CyRK/nb/nbrk.py` & `CyRK-0.6.1/CyRK/nb/nbrk.py`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/CyRK/rk/rk.cpp` & `CyRK-0.6.1/CyRK/rk/rk.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
             "-fopenmp"
         ],
         "extra_link_args": [
             "-fopenmp"
         ],
         "include_dirs": [
             "CyRK/rk",
-            "/tmp/build-env-z2z0y6y4/lib/python3.10/site-packages/numpy/core/include"
+            "/tmp/build-env-v1jyxftm/lib/python3.10/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "CyRK.rk.rk",
         "sources": [
             "CyRK/rk/rk.pyx"
         ]
     },
```

### Comparing `CyRK-0.6.0/CyRK/rk/rk.pxd` & `CyRK-0.6.1/CyRK/rk/rk.pxd`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/CyRK/rk/rk.pyx` & `CyRK-0.6.1/CyRK/rk/rk.pyx`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/CyRK.egg-info/PKG-INFO` & `CyRK-0.6.1/CyRK.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CyRK
-Version: 0.6.0
+Version: 0.6.1
 Summary: Runge-Kutta ODE Integrator Implemented in Cython and Numba.
 Author-email: "Joe P. Renaud" <joe.p.renaud@gmail.com>
 License: # Creative Commons Attribution-ShareAlike 4.0 International
         
         Creative Commons Corporation (“Creative Commons”) is not a law firm and does not provide legal services or legal advice. Distribution of Creative Commons public licenses does not create a lawyer-client or other relationship. Creative Commons makes its licenses and related information available on an “as-is” basis. Creative Commons gives no warranties regarding its licenses, any material licensed under their terms and conditions, or any related information. Creative Commons disclaims all liability for damages resulting from their use to the fullest extent possible.
         
         **Using Creative Commons Public Licenses**
@@ -208,115 +208,112 @@
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_win.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_win.yml/badge.svg?branch=main" alt="Windows Tests" /></a>
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_mac.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_mac.yml/badge.svg?branch=main" alt="MacOS Tests" /></a>
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_ubun.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_ubun.yml/badge.svg?branch=main" alt="Ubuntu Tests" /></a>
 </div>
 
 ---
 
-<a href="https://github.com/jrenaud90/CyRK/releases"><img src="https://img.shields.io/badge/CyRK-0.6.0 Alpha-orange" alt="CyRK Version 0.6.0 Alpha" /></a>
+<a href="https://github.com/jrenaud90/CyRK/releases"><img src="https://img.shields.io/badge/CyRK-0.6.1 Alpha-orange" alt="CyRK Version 0.6.1 Alpha" /></a>
 
 
 **Runge-Kutta ODE Integrator Implemented in Cython and Numba**
 
-CyRK provides fast integration tools to solve systems of ODEs using an adaptive time stepping scheme. CyRK can, usually, accept differential equation functions 
-that are written in pure Python, njited numba, or cython-based cdef classes. These kinds of functions are generally easier to implement than pure c functions. Using CyRK can speed up development time while not making a huge sacrifice when it comes to performance. 
+CyRK provides fast integration tools to solve systems of ODEs using an adaptive time stepping scheme. CyRK can accept differential equations that are written in pure Python, njited numba, or cython-based cdef classes. These kinds of functions are generally easier to implement than pure c functions. Using CyRK can speed up development time while not making a huge sacrifice when it comes to performance. 
 
 The purpose of this package is to provide some 
 functionality of [scipy's solve_ivp](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html) with greatly improved performance.
 
 Currently, CyRK's [numba](https://numba.discourse.group/) (njit-safe) implementation is **10-100x faster** than scipy's solve_ivp function.
 The [cython](https://cython.org/) `cyrk_ode` function that works with python (or numba) functions is **5-40x faster** than scipy.
 The [cython](https://cython.org/) `CySolver` class that works with cython-based cdef classes is **5-400x faster** than scipy.
 
 An additional benefit of the two cython implementations is that they are pre-compiled. This avoids most of the start-up performance hit experienced by just-in-time compilers like numba.
 
 <img style="text-align: center" src="https://github.com/jrenaud90/CyRK/blob/main/Benchmarks/CyRK_SciPy_Compare_v0-6-0a4.png" alt="CyRK Performance" />
 
 ## Installation
 
-It is recommended you use an [Anaconda](https://www.anaconda.com/products/distribution) environment. CyRK has been tested on Python 3.8--3.10
+*CyRK has been tested on Python 3.8--3.11; Windows, Ubuntu, and MacOS.*
 
 To install simply open a terminal and call:
 
 `pip install CyRK`
 
-If not installing from a wheel, CyRK will attempt to install `Cython` and `Numpy` in order to compile the cython code. 
-After the files have been compiled, cython will be uninstalled and CyRK's runtime dependencies 
-(see the pyproject.toml file for the latest list) will be installed instead.
+If not installing from a wheel, CyRK will attempt to install `Cython` and `Numpy` in order to compile the source code. 
+After everything has been compiled, cython will be uninstalled and CyRK's runtime dependencies (see the pyproject.toml file for the latest list) will be installed instead.
 
 A new installation of CyRK can be tested quickly by running the following from a python console.
 ```python
 from CyRK import test_cyrk, test_nbrk, test_cysolver
 test_cyrk()
-# You will hopefully see the message "CyRK's cyrk_ode was tested successfully."
+# Should see "CyRK's cyrk_ode was tested successfully."
 test_nbrk()
-# You will hopefully see the message "CyRK's nbrk_ode was tested successfully."
+# Should see "CyRK's nbrk_ode was tested successfully."
 test_cysolver()
-# You will hopefully see the message "CyRK's CySolver was tested successfully."
+# Should see "CyRK's CySolver was tested successfully."
 ```
 
 ### Installation Troubleshooting
 
 *Please [report](https://github.com/jrenaud90/CyRK/issues) installation issues. We will work on a fix and/or add workaround information here.*
 
 - If you see a "Can not load module: CyRK.cy" or similar error then the cython extensions likely did not compile during installation. Try running `pip install CyRK --no-binary="CyRK"` 
 to force python to recompile the cython extensions locally (rather than via a prebuilt wheel).
-- On MacOS: If you run into problems installing CyRK then reinstall using the verbose flag (`pip install -v .`) to look at the installation log. If you see an error that looks like "clang: error: unsupported option '-fopenmp'" then you may have a problem with your `llvm` or `libomp` libraries. It is recommended that you install CyRK in an anaconda environment with the following packages `conda install numpy scipy cython llvm-openmp`. See more discussion [here](https://github.com/facebookresearch/xformers/issues/157) and the steps taken [here](https://github.com/jrenaud90/CyRK/blob/main/.github/workflows/push_tests_mac.yml).
+- On MacOS: If you run into problems installing CyRK then reinstall using the verbose flag (`pip install -v .`) to look at the installation log. If you see an error that looks like "clang: error: unsupported option '-fopenmp'" then you may have a problem with your `llvm` or `libomp` libraries. It is recommended that you install CyRK in an [Anaconda](https://www.anaconda.com/download) environment with the following packages `conda install numpy scipy cython llvm-openmp`. See more discussion [here](https://github.com/facebookresearch/xformers/issues/157) and the steps taken [here](https://github.com/jrenaud90/CyRK/blob/main/.github/workflows/push_tests_mac.yml).
 
 ### Development and Testing Dependencies
 
-If you intend to work on CyRK's code base you will want to install the following dependencies in order to run CyRK's
-test suite.
+If you intend to work on CyRK's code base you will want to install the following dependencies in order to run CyRK's test suite and experimental notebooks.
 
 `conda install pytest scipy matplotlib jupyter`
 
 `conda install` can be replaced with `pip install` if you prefer.
 
 ## Using CyRK
 CyRK's API is similar to SciPy's solve_ivp function. A differential equation can be defined in python such as:
 
 ```python
 import numpy as np
-from numba import njit
+
 # For even more speed up you can use numba's njit to compile the diffeq
+from numba import njit
 @njit
 def diffeq_nb(t, y):
     dy = np.empty_like(y)
     dy[0] = (1. - 0.01 * y[1]) * y[0]
     dy[1] = (0.02 * y[0] - 1.) * y[1]
     return dy
 
 initial_conds = np.asarray((20., 20.), dtype=np.complex128)
 time_span = (0., 50.)
 rtol = 1.0e-7
 atol = 1.0e-8
 ```
 
 ### Numba-based `nbrk_ode`
-The ODE can then be solved using the numba function by calling CyRK's `nbrk_ode`:
+The system of ODEs can then be solved using CyRK's numba solver by,
 
 ```python
 from CyRK import nbrk_ode
 time_domain, y_results, success, message = \
     nbrk_ode(diffeq_nb, time_span, initial_conds, rk_method=1, rtol=rtol, atol=atol)
 ```
 
 ### Cython-based `cyrk_ode`
 To call the cython version of the integrator you need to slightly edit the differential equation so that it does not
-return the derivative. Instead, the output is passed as an input argument (a np.ndarray) to the function. 
+return the derivative. Instead, the output is passed as an input argument (a `np.ndarray`) to the function. 
 
 ```python
 @njit
 def diffeq_cy(t, y, dy):
     dy[0] = (1. - 0.01 * y[1]) * y[0]
     dy[1] = (0.02 * y[0] - 1.) * y[1]
 ```
 
-Alternatively, you can use CyRK's conversion helper functions to automatically convert between numba/scipy and cyrk
-function calls.
+Alternatively, you can use CyRK's conversion helper functions to automatically convert between numba/scipy and cyrk function calls.
 
 ```python
 from CyRK import nb2cy, cy2nb
 
 @njit
 def diffeq_nb(t, y):
     dy = np.empty_like(y)
@@ -333,120 +330,113 @@
 ```python
 from CyRK import cyrk_ode
 time_domain, y_results, success, message = \
     cyrk_ode(diffeq_cy, time_span, initial_conds, rk_method=1, rtol=rtol, atol=atol)
 ```
 
 ### Cython-based `CySolver`
-The cython-based `CySolver` class requires writing a new cython cdef class. This can be done like so, note this is in a .pyx file that must be
-cythonized and compiled before it can be used.
+The cython-based `CySolver` class requires writing a new cython cdef class. This is done in a new cython .pyx file which must then be cythonized and compiled before it can be used.
 
 ```cython
 """ODE.pyx"""
 # distutils: language = c++
 # cython: boundscheck=False, wraparound=False, nonecheck=False, cdivision=True, initializedcheck=False
+
 from CyRK.cy.cysolver cimport CySolver
 # Note the `cimport` here^
 
-cdef class CySolverTester(CySolver):
+cdef class MyCyRKDiffeq(CySolver):
 
     @cython.exceptval(check=False)
     cdef void diffeq(self):
         
         # Unpack dependent variables using the `self.y_new_view` variable.
+        # In this example we have a system of two dependent variables, but any number can be used.
         cdef double y0, y1
         y0 = self.y_new_view[0]
         y1 = self.y_new_view[1]
 
         # Unpack any additional arguments that do not change with time using the `self.arg_array_view` variable.
         cdef double a, b
         # These must be float64s
         a  = self.arg_array_view[0]
         b  = self.arg_array_view[1]
 
         # If needed, unpack the time variable using `self.t_new`
         cdef double t
         t = self.t_new
 
-        # This function must set the dydt variable `self.dy_new_view`
+        # This then updates dydt by setting the values of `self.dy_new_view`
         self.dy_new_view[0] = (1. - a * y1) * y0
         self.dy_new_view[1] = (b * y0 - 1.) * y1
 ```
 
 Once you compile the differential equation it can be imported in a regular python file and used in a similar fashion to the other integrators.
 
 ```python
 """run.py"""
-from CyRK.cy.cysolvertest import CySolverTester
+from ODE import MyCyRKDiffeq
 
 # Need to make an instance of the integrator.
 # The diffeq no longer needs to be passed to the class.
-CySolverTesterInst = CySolverTester(time_span, initial_conds, args=(0.01, 0.02), rk_method=1, rtol=rtol, atol=atol)
+MyCyRKDiffeqInst = MyCyRKDiffeq(time_span, initial_conds, args=(0.01, 0.02), rk_method=1, rtol=rtol, atol=atol)
 
 # To perform the integration make a call to the solve method.
-CySolverTesterInst.solve()
+MyCyRKDiffeqInst.solve()
 
 # Once complete, you can access the results via...
-CySolverTesterInst.success     # True / False
-CySolverTesterInst.message     # Note about integration
-CySolverTesterInst.solution_t  # Time domain
-CySolverTesterInst.solution_y  # y dependent variables
-CySolverTesterInst.solution_extra  # Extra output that was captured during integration.
+MyCyRKDiffeqInst.success     # True / False
+MyCyRKDiffeqInst.message     # Note about integration
+MyCyRKDiffeqInst.solution_t  # Time domain
+MyCyRKDiffeqInst.solution_y  # y dependent variables
+MyCyRKDiffeqInst.solution_extra  # Extra output that was captured during integration.
 # See Documentation/Extra Output.md for more information on `solution_extra`
 ```
 
 ## Optional Arguments
 
-Both the numba and cython versions of the ODE solver have the following optional inputs:
+All three integrators can take the following optional inputs:
 - `rtol`: Relative Tolerance (default is 1.0e-6).
 - `atol`: Absolute Tolerance (default is 1.0e-8).
 - `max_step`: Maximum step size (default is +infinity).
 - `first_step`: Initial step size (default is 0).
   - If 0, then the solver will try to determine an ideal value.
 - `args`: Python tuple of additional arguments passed to the `diffeq`.
-- `t_eval`: Both solvers uses an adaptive time stepping protocol based on the recent error at each step. This results in
-a final non-uniform time domain of variable size. If the user would like the results at specific time steps then 
-they can provide a np.ndarray array at the desired steps to `t_eval`.
-The solver will then interpolate the results to fit this array.
+  - For the cython solvers these arguments must be floating point numbers only.
+- `t_eval`: Both solvers uses an adaptive time stepping protocol based on the recent error at each step. This results in a final non-uniform time domain of variable size. If the user would like the results at specific time steps then they can provide a np.ndarray array at the desired steps via `t_eval`. The solver will then interpolate the results to fit this array.
 - `rk_method`: Runge-Kutta method (default is 1; all of these methods are based off of
 [SciPy implementations](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html)):
   - `0` - "RK23" Explicit Runge-Kutta method of order 3(2).
   - `1` - "RK45" Explicit Runge-Kutta method of order 5(4).
   - `2` - "DOP853" Explicit Runge-Kutta method of order 8.
 - `capture_extra` and `interpolate_extra`: CyRK has the capability of capturing additional parameters during integration. Please see `Documentation\Extra Output.md` for more details.
 
 ### Additional Arguments for `cyrk_ode` and `CySolver`
 - `num_extra` : The number of extra outputs the integrator should expect.
+  - Please see `Documentation\Extra Output.md` for more details.
 - `expected_size` : Best guess on the expected size of the final time domain (number of points).
-    - The integrator must pre-allocate memory to store results from the integration. It will attempt to use arrays sized to `expected_size`. However, if this is too small or too large then performance will be impacted. It is recommended you try out different values based on the problem you are trying to solve.
+    - The integrator must pre-allocate memory to store results from the integration. It will attempt to use arrays sized to `expected_size`. However, if this is too small or too large then performance will be negatively impacted. It is recommended you try out different values based on the problem you are trying to solve.
     - If `expected_size=0` (the default) then the solver will attempt to guess a best size. Currently this is a very basic guess so it is not recommended.
     - It is better to overshoot than undershoot this guess.
 
 ## Limitations and Known Issues
 
-- [Issue 1](https://github.com/jrenaud90/CyRK/issues/1): Absolute tolerance can only be passed as a single value
-(same for all y's).
+- [Issue 1](https://github.com/jrenaud90/CyRK/issues/1): Absolute tolerance can only be passed as a single value (same for all y's).
+- [Issue 30](https://github.com/jrenaud90/CyRK/issues/30): CyRK's CySolver does not allow for complex-valued dependent variables. 
 
 ## Citing CyRK
 
-It is great to see CyRK used in other software or in scientific studies. We ask that you cite back to CyRK's 
-[GitHub](https://github.com/jrenaud90/CyRK) website so interested parties can learn about this package. 
+It is great to see CyRK used in other software or in scientific studies. We ask that you cite back to CyRK's [GitHub](https://github.com/jrenaud90/CyRK) website so interested parties can learn about this package. It would also be great to hear about the work being done with CyRK, so get in touch!
 
 Renaud, Joe P. (2022). CyRK - ODE Integrator Implemented in Cython and Numba. Zenodo. https://doi.org/10.5281/zenodo.7093266
 
-In addition to citing CyRK, please consider citing SciPy and its references for the specific Runge-Kutta model that
-was used in your work. CyRK is largely an adaptation of SciPy's functionality.
-Find more details [here](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
+In addition to citing CyRK, please consider citing SciPy and its references for the specific Runge-Kutta model that was used in your work. CyRK is largely an adaptation of SciPy's functionality. Find more details [here](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
 
 Pauli Virtanen, Ralf Gommers, Travis E. Oliphant, Matt Haberland, Tyler Reddy, David Cournapeau, Evgeni Burovski, Pearu Peterson, Warren Weckesser, Jonathan Bright, Stéfan J. van der Walt, Matthew Brett, Joshua Wilson, K. Jarrod Millman, Nikolay Mayorov, Andrew R. J. Nelson, Eric Jones, Robert Kern, Eric Larson, CJ Carey, İlhan Polat, Yu Feng, Eric W. Moore, Jake VanderPlas, Denis Laxalde, Josef Perktold, Robert Cimrman, Ian Henriksen, E.A. Quintero, Charles R Harris, Anne M. Archibald, Antônio H. Ribeiro, Fabian Pedregosa, Paul van Mulbregt, and SciPy 1.0 Contributors. (2020) SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. Nature Methods, 17(3), 261-272.
 
 ## Contribute to CyRK
 _Please look [here](https://github.com/jrenaud90/CyRK/graphs/contributors) for an up-to-date list of contributors to the CyRK package._
 
-CyRK is open-source and is distributed under the Creative Commons Attribution-ShareAlike 4.0 International license. 
-You are welcome to fork this repository and make any edits with attribution back to this project (please see the 
-`Citing CyRK` section).
+CyRK is open-source and is distributed under the Creative Commons Attribution-ShareAlike 4.0 International license. You are welcome to fork this repository and make any edits with attribution back to this project (please see the `Citing CyRK` section).
 - We encourage users to report bugs or feature requests using [GitHub Issues](https://github.com/jrenaud90/CyRK/issues).
-- If you would like to contribute but don't know where to start, check out the 
-[good first issue](https://github.com/jrenaud90/CyRK/labels/good%20first%20issue) tag on GitHub.
-- Users are welcome to submit pull requests and should feel free to create them before the final code is completed so
-that feedback and suggestions can be given early on.
+- If you would like to contribute but don't know where to start, check out the [good first issue](https://github.com/jrenaud90/CyRK/labels/good%20first%20issue) tag on GitHub.
+- Users are welcome to submit pull requests and should feel free to create them before the final code is completed so that feedback and suggestions can be given early on.
```

### Comparing `CyRK-0.6.0/CyRK.egg-info/SOURCES.txt` & `CyRK-0.6.1/CyRK.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,15 +8,17 @@
 CyRK/_test.py
 CyRK/helper.py
 CyRK.egg-info/PKG-INFO
 CyRK.egg-info/SOURCES.txt
 CyRK.egg-info/dependency_links.txt
 CyRK.egg-info/requires.txt
 CyRK.egg-info/top_level.txt
+CyRK/array/__init__.pxd
 CyRK/array/__init__.py
+CyRK/array/__init__.pyx
 CyRK/array/interp.cpp
 CyRK/array/interp.pxd
 CyRK/array/interp.pyx
 CyRK/cy/__init__.pxd
 CyRK/cy/__init__.py
 CyRK/cy/__init__.pyx
 CyRK/cy/cyrk.cpp
```

### Comparing `CyRK-0.6.0/LICENSE.md` & `CyRK-0.6.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/PKG-INFO` & `CyRK-0.6.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CyRK
-Version: 0.6.0
+Version: 0.6.1
 Summary: Runge-Kutta ODE Integrator Implemented in Cython and Numba.
 Author-email: "Joe P. Renaud" <joe.p.renaud@gmail.com>
 License: # Creative Commons Attribution-ShareAlike 4.0 International
         
         Creative Commons Corporation (“Creative Commons”) is not a law firm and does not provide legal services or legal advice. Distribution of Creative Commons public licenses does not create a lawyer-client or other relationship. Creative Commons makes its licenses and related information available on an “as-is” basis. Creative Commons gives no warranties regarding its licenses, any material licensed under their terms and conditions, or any related information. Creative Commons disclaims all liability for damages resulting from their use to the fullest extent possible.
         
         **Using Creative Commons Public Licenses**
@@ -208,115 +208,112 @@
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_win.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_win.yml/badge.svg?branch=main" alt="Windows Tests" /></a>
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_mac.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_mac.yml/badge.svg?branch=main" alt="MacOS Tests" /></a>
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_ubun.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_ubun.yml/badge.svg?branch=main" alt="Ubuntu Tests" /></a>
 </div>
 
 ---
 
-<a href="https://github.com/jrenaud90/CyRK/releases"><img src="https://img.shields.io/badge/CyRK-0.6.0 Alpha-orange" alt="CyRK Version 0.6.0 Alpha" /></a>
+<a href="https://github.com/jrenaud90/CyRK/releases"><img src="https://img.shields.io/badge/CyRK-0.6.1 Alpha-orange" alt="CyRK Version 0.6.1 Alpha" /></a>
 
 
 **Runge-Kutta ODE Integrator Implemented in Cython and Numba**
 
-CyRK provides fast integration tools to solve systems of ODEs using an adaptive time stepping scheme. CyRK can, usually, accept differential equation functions 
-that are written in pure Python, njited numba, or cython-based cdef classes. These kinds of functions are generally easier to implement than pure c functions. Using CyRK can speed up development time while not making a huge sacrifice when it comes to performance. 
+CyRK provides fast integration tools to solve systems of ODEs using an adaptive time stepping scheme. CyRK can accept differential equations that are written in pure Python, njited numba, or cython-based cdef classes. These kinds of functions are generally easier to implement than pure c functions. Using CyRK can speed up development time while not making a huge sacrifice when it comes to performance. 
 
 The purpose of this package is to provide some 
 functionality of [scipy's solve_ivp](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html) with greatly improved performance.
 
 Currently, CyRK's [numba](https://numba.discourse.group/) (njit-safe) implementation is **10-100x faster** than scipy's solve_ivp function.
 The [cython](https://cython.org/) `cyrk_ode` function that works with python (or numba) functions is **5-40x faster** than scipy.
 The [cython](https://cython.org/) `CySolver` class that works with cython-based cdef classes is **5-400x faster** than scipy.
 
 An additional benefit of the two cython implementations is that they are pre-compiled. This avoids most of the start-up performance hit experienced by just-in-time compilers like numba.
 
 <img style="text-align: center" src="https://github.com/jrenaud90/CyRK/blob/main/Benchmarks/CyRK_SciPy_Compare_v0-6-0a4.png" alt="CyRK Performance" />
 
 ## Installation
 
-It is recommended you use an [Anaconda](https://www.anaconda.com/products/distribution) environment. CyRK has been tested on Python 3.8--3.10
+*CyRK has been tested on Python 3.8--3.11; Windows, Ubuntu, and MacOS.*
 
 To install simply open a terminal and call:
 
 `pip install CyRK`
 
-If not installing from a wheel, CyRK will attempt to install `Cython` and `Numpy` in order to compile the cython code. 
-After the files have been compiled, cython will be uninstalled and CyRK's runtime dependencies 
-(see the pyproject.toml file for the latest list) will be installed instead.
+If not installing from a wheel, CyRK will attempt to install `Cython` and `Numpy` in order to compile the source code. 
+After everything has been compiled, cython will be uninstalled and CyRK's runtime dependencies (see the pyproject.toml file for the latest list) will be installed instead.
 
 A new installation of CyRK can be tested quickly by running the following from a python console.
 ```python
 from CyRK import test_cyrk, test_nbrk, test_cysolver
 test_cyrk()
-# You will hopefully see the message "CyRK's cyrk_ode was tested successfully."
+# Should see "CyRK's cyrk_ode was tested successfully."
 test_nbrk()
-# You will hopefully see the message "CyRK's nbrk_ode was tested successfully."
+# Should see "CyRK's nbrk_ode was tested successfully."
 test_cysolver()
-# You will hopefully see the message "CyRK's CySolver was tested successfully."
+# Should see "CyRK's CySolver was tested successfully."
 ```
 
 ### Installation Troubleshooting
 
 *Please [report](https://github.com/jrenaud90/CyRK/issues) installation issues. We will work on a fix and/or add workaround information here.*
 
 - If you see a "Can not load module: CyRK.cy" or similar error then the cython extensions likely did not compile during installation. Try running `pip install CyRK --no-binary="CyRK"` 
 to force python to recompile the cython extensions locally (rather than via a prebuilt wheel).
-- On MacOS: If you run into problems installing CyRK then reinstall using the verbose flag (`pip install -v .`) to look at the installation log. If you see an error that looks like "clang: error: unsupported option '-fopenmp'" then you may have a problem with your `llvm` or `libomp` libraries. It is recommended that you install CyRK in an anaconda environment with the following packages `conda install numpy scipy cython llvm-openmp`. See more discussion [here](https://github.com/facebookresearch/xformers/issues/157) and the steps taken [here](https://github.com/jrenaud90/CyRK/blob/main/.github/workflows/push_tests_mac.yml).
+- On MacOS: If you run into problems installing CyRK then reinstall using the verbose flag (`pip install -v .`) to look at the installation log. If you see an error that looks like "clang: error: unsupported option '-fopenmp'" then you may have a problem with your `llvm` or `libomp` libraries. It is recommended that you install CyRK in an [Anaconda](https://www.anaconda.com/download) environment with the following packages `conda install numpy scipy cython llvm-openmp`. See more discussion [here](https://github.com/facebookresearch/xformers/issues/157) and the steps taken [here](https://github.com/jrenaud90/CyRK/blob/main/.github/workflows/push_tests_mac.yml).
 
 ### Development and Testing Dependencies
 
-If you intend to work on CyRK's code base you will want to install the following dependencies in order to run CyRK's
-test suite.
+If you intend to work on CyRK's code base you will want to install the following dependencies in order to run CyRK's test suite and experimental notebooks.
 
 `conda install pytest scipy matplotlib jupyter`
 
 `conda install` can be replaced with `pip install` if you prefer.
 
 ## Using CyRK
 CyRK's API is similar to SciPy's solve_ivp function. A differential equation can be defined in python such as:
 
 ```python
 import numpy as np
-from numba import njit
+
 # For even more speed up you can use numba's njit to compile the diffeq
+from numba import njit
 @njit
 def diffeq_nb(t, y):
     dy = np.empty_like(y)
     dy[0] = (1. - 0.01 * y[1]) * y[0]
     dy[1] = (0.02 * y[0] - 1.) * y[1]
     return dy
 
 initial_conds = np.asarray((20., 20.), dtype=np.complex128)
 time_span = (0., 50.)
 rtol = 1.0e-7
 atol = 1.0e-8
 ```
 
 ### Numba-based `nbrk_ode`
-The ODE can then be solved using the numba function by calling CyRK's `nbrk_ode`:
+The system of ODEs can then be solved using CyRK's numba solver by,
 
 ```python
 from CyRK import nbrk_ode
 time_domain, y_results, success, message = \
     nbrk_ode(diffeq_nb, time_span, initial_conds, rk_method=1, rtol=rtol, atol=atol)
 ```
 
 ### Cython-based `cyrk_ode`
 To call the cython version of the integrator you need to slightly edit the differential equation so that it does not
-return the derivative. Instead, the output is passed as an input argument (a np.ndarray) to the function. 
+return the derivative. Instead, the output is passed as an input argument (a `np.ndarray`) to the function. 
 
 ```python
 @njit
 def diffeq_cy(t, y, dy):
     dy[0] = (1. - 0.01 * y[1]) * y[0]
     dy[1] = (0.02 * y[0] - 1.) * y[1]
 ```
 
-Alternatively, you can use CyRK's conversion helper functions to automatically convert between numba/scipy and cyrk
-function calls.
+Alternatively, you can use CyRK's conversion helper functions to automatically convert between numba/scipy and cyrk function calls.
 
 ```python
 from CyRK import nb2cy, cy2nb
 
 @njit
 def diffeq_nb(t, y):
     dy = np.empty_like(y)
@@ -333,120 +330,113 @@
 ```python
 from CyRK import cyrk_ode
 time_domain, y_results, success, message = \
     cyrk_ode(diffeq_cy, time_span, initial_conds, rk_method=1, rtol=rtol, atol=atol)
 ```
 
 ### Cython-based `CySolver`
-The cython-based `CySolver` class requires writing a new cython cdef class. This can be done like so, note this is in a .pyx file that must be
-cythonized and compiled before it can be used.
+The cython-based `CySolver` class requires writing a new cython cdef class. This is done in a new cython .pyx file which must then be cythonized and compiled before it can be used.
 
 ```cython
 """ODE.pyx"""
 # distutils: language = c++
 # cython: boundscheck=False, wraparound=False, nonecheck=False, cdivision=True, initializedcheck=False
+
 from CyRK.cy.cysolver cimport CySolver
 # Note the `cimport` here^
 
-cdef class CySolverTester(CySolver):
+cdef class MyCyRKDiffeq(CySolver):
 
     @cython.exceptval(check=False)
     cdef void diffeq(self):
         
         # Unpack dependent variables using the `self.y_new_view` variable.
+        # In this example we have a system of two dependent variables, but any number can be used.
         cdef double y0, y1
         y0 = self.y_new_view[0]
         y1 = self.y_new_view[1]
 
         # Unpack any additional arguments that do not change with time using the `self.arg_array_view` variable.
         cdef double a, b
         # These must be float64s
         a  = self.arg_array_view[0]
         b  = self.arg_array_view[1]
 
         # If needed, unpack the time variable using `self.t_new`
         cdef double t
         t = self.t_new
 
-        # This function must set the dydt variable `self.dy_new_view`
+        # This then updates dydt by setting the values of `self.dy_new_view`
         self.dy_new_view[0] = (1. - a * y1) * y0
         self.dy_new_view[1] = (b * y0 - 1.) * y1
 ```
 
 Once you compile the differential equation it can be imported in a regular python file and used in a similar fashion to the other integrators.
 
 ```python
 """run.py"""
-from CyRK.cy.cysolvertest import CySolverTester
+from ODE import MyCyRKDiffeq
 
 # Need to make an instance of the integrator.
 # The diffeq no longer needs to be passed to the class.
-CySolverTesterInst = CySolverTester(time_span, initial_conds, args=(0.01, 0.02), rk_method=1, rtol=rtol, atol=atol)
+MyCyRKDiffeqInst = MyCyRKDiffeq(time_span, initial_conds, args=(0.01, 0.02), rk_method=1, rtol=rtol, atol=atol)
 
 # To perform the integration make a call to the solve method.
-CySolverTesterInst.solve()
+MyCyRKDiffeqInst.solve()
 
 # Once complete, you can access the results via...
-CySolverTesterInst.success     # True / False
-CySolverTesterInst.message     # Note about integration
-CySolverTesterInst.solution_t  # Time domain
-CySolverTesterInst.solution_y  # y dependent variables
-CySolverTesterInst.solution_extra  # Extra output that was captured during integration.
+MyCyRKDiffeqInst.success     # True / False
+MyCyRKDiffeqInst.message     # Note about integration
+MyCyRKDiffeqInst.solution_t  # Time domain
+MyCyRKDiffeqInst.solution_y  # y dependent variables
+MyCyRKDiffeqInst.solution_extra  # Extra output that was captured during integration.
 # See Documentation/Extra Output.md for more information on `solution_extra`
 ```
 
 ## Optional Arguments
 
-Both the numba and cython versions of the ODE solver have the following optional inputs:
+All three integrators can take the following optional inputs:
 - `rtol`: Relative Tolerance (default is 1.0e-6).
 - `atol`: Absolute Tolerance (default is 1.0e-8).
 - `max_step`: Maximum step size (default is +infinity).
 - `first_step`: Initial step size (default is 0).
   - If 0, then the solver will try to determine an ideal value.
 - `args`: Python tuple of additional arguments passed to the `diffeq`.
-- `t_eval`: Both solvers uses an adaptive time stepping protocol based on the recent error at each step. This results in
-a final non-uniform time domain of variable size. If the user would like the results at specific time steps then 
-they can provide a np.ndarray array at the desired steps to `t_eval`.
-The solver will then interpolate the results to fit this array.
+  - For the cython solvers these arguments must be floating point numbers only.
+- `t_eval`: Both solvers uses an adaptive time stepping protocol based on the recent error at each step. This results in a final non-uniform time domain of variable size. If the user would like the results at specific time steps then they can provide a np.ndarray array at the desired steps via `t_eval`. The solver will then interpolate the results to fit this array.
 - `rk_method`: Runge-Kutta method (default is 1; all of these methods are based off of
 [SciPy implementations](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html)):
   - `0` - "RK23" Explicit Runge-Kutta method of order 3(2).
   - `1` - "RK45" Explicit Runge-Kutta method of order 5(4).
   - `2` - "DOP853" Explicit Runge-Kutta method of order 8.
 - `capture_extra` and `interpolate_extra`: CyRK has the capability of capturing additional parameters during integration. Please see `Documentation\Extra Output.md` for more details.
 
 ### Additional Arguments for `cyrk_ode` and `CySolver`
 - `num_extra` : The number of extra outputs the integrator should expect.
+  - Please see `Documentation\Extra Output.md` for more details.
 - `expected_size` : Best guess on the expected size of the final time domain (number of points).
-    - The integrator must pre-allocate memory to store results from the integration. It will attempt to use arrays sized to `expected_size`. However, if this is too small or too large then performance will be impacted. It is recommended you try out different values based on the problem you are trying to solve.
+    - The integrator must pre-allocate memory to store results from the integration. It will attempt to use arrays sized to `expected_size`. However, if this is too small or too large then performance will be negatively impacted. It is recommended you try out different values based on the problem you are trying to solve.
     - If `expected_size=0` (the default) then the solver will attempt to guess a best size. Currently this is a very basic guess so it is not recommended.
     - It is better to overshoot than undershoot this guess.
 
 ## Limitations and Known Issues
 
-- [Issue 1](https://github.com/jrenaud90/CyRK/issues/1): Absolute tolerance can only be passed as a single value
-(same for all y's).
+- [Issue 1](https://github.com/jrenaud90/CyRK/issues/1): Absolute tolerance can only be passed as a single value (same for all y's).
+- [Issue 30](https://github.com/jrenaud90/CyRK/issues/30): CyRK's CySolver does not allow for complex-valued dependent variables. 
 
 ## Citing CyRK
 
-It is great to see CyRK used in other software or in scientific studies. We ask that you cite back to CyRK's 
-[GitHub](https://github.com/jrenaud90/CyRK) website so interested parties can learn about this package. 
+It is great to see CyRK used in other software or in scientific studies. We ask that you cite back to CyRK's [GitHub](https://github.com/jrenaud90/CyRK) website so interested parties can learn about this package. It would also be great to hear about the work being done with CyRK, so get in touch!
 
 Renaud, Joe P. (2022). CyRK - ODE Integrator Implemented in Cython and Numba. Zenodo. https://doi.org/10.5281/zenodo.7093266
 
-In addition to citing CyRK, please consider citing SciPy and its references for the specific Runge-Kutta model that
-was used in your work. CyRK is largely an adaptation of SciPy's functionality.
-Find more details [here](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
+In addition to citing CyRK, please consider citing SciPy and its references for the specific Runge-Kutta model that was used in your work. CyRK is largely an adaptation of SciPy's functionality. Find more details [here](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
 
 Pauli Virtanen, Ralf Gommers, Travis E. Oliphant, Matt Haberland, Tyler Reddy, David Cournapeau, Evgeni Burovski, Pearu Peterson, Warren Weckesser, Jonathan Bright, Stéfan J. van der Walt, Matthew Brett, Joshua Wilson, K. Jarrod Millman, Nikolay Mayorov, Andrew R. J. Nelson, Eric Jones, Robert Kern, Eric Larson, CJ Carey, İlhan Polat, Yu Feng, Eric W. Moore, Jake VanderPlas, Denis Laxalde, Josef Perktold, Robert Cimrman, Ian Henriksen, E.A. Quintero, Charles R Harris, Anne M. Archibald, Antônio H. Ribeiro, Fabian Pedregosa, Paul van Mulbregt, and SciPy 1.0 Contributors. (2020) SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. Nature Methods, 17(3), 261-272.
 
 ## Contribute to CyRK
 _Please look [here](https://github.com/jrenaud90/CyRK/graphs/contributors) for an up-to-date list of contributors to the CyRK package._
 
-CyRK is open-source and is distributed under the Creative Commons Attribution-ShareAlike 4.0 International license. 
-You are welcome to fork this repository and make any edits with attribution back to this project (please see the 
-`Citing CyRK` section).
+CyRK is open-source and is distributed under the Creative Commons Attribution-ShareAlike 4.0 International license. You are welcome to fork this repository and make any edits with attribution back to this project (please see the `Citing CyRK` section).
 - We encourage users to report bugs or feature requests using [GitHub Issues](https://github.com/jrenaud90/CyRK/issues).
-- If you would like to contribute but don't know where to start, check out the 
-[good first issue](https://github.com/jrenaud90/CyRK/labels/good%20first%20issue) tag on GitHub.
-- Users are welcome to submit pull requests and should feel free to create them before the final code is completed so
-that feedback and suggestions can be given early on.
+- If you would like to contribute but don't know where to start, check out the [good first issue](https://github.com/jrenaud90/CyRK/labels/good%20first%20issue) tag on GitHub.
+- Users are welcome to submit pull requests and should feel free to create them before the final code is completed so that feedback and suggestions can be given early on.
```

### Comparing `CyRK-0.6.0/README.md` & `CyRK-0.6.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -7,115 +7,112 @@
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_win.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_win.yml/badge.svg?branch=main" alt="Windows Tests" /></a>
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_mac.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_mac.yml/badge.svg?branch=main" alt="MacOS Tests" /></a>
 <a href="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_ubun.yml"><img src="https://github.com/jrenaud90/CyRK/actions/workflows/push_tests_ubun.yml/badge.svg?branch=main" alt="Ubuntu Tests" /></a>
 </div>
 
 ---
 
-<a href="https://github.com/jrenaud90/CyRK/releases"><img src="https://img.shields.io/badge/CyRK-0.6.0 Alpha-orange" alt="CyRK Version 0.6.0 Alpha" /></a>
+<a href="https://github.com/jrenaud90/CyRK/releases"><img src="https://img.shields.io/badge/CyRK-0.6.1 Alpha-orange" alt="CyRK Version 0.6.1 Alpha" /></a>
 
 
 **Runge-Kutta ODE Integrator Implemented in Cython and Numba**
 
-CyRK provides fast integration tools to solve systems of ODEs using an adaptive time stepping scheme. CyRK can, usually, accept differential equation functions 
-that are written in pure Python, njited numba, or cython-based cdef classes. These kinds of functions are generally easier to implement than pure c functions. Using CyRK can speed up development time while not making a huge sacrifice when it comes to performance. 
+CyRK provides fast integration tools to solve systems of ODEs using an adaptive time stepping scheme. CyRK can accept differential equations that are written in pure Python, njited numba, or cython-based cdef classes. These kinds of functions are generally easier to implement than pure c functions. Using CyRK can speed up development time while not making a huge sacrifice when it comes to performance. 
 
 The purpose of this package is to provide some 
 functionality of [scipy's solve_ivp](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html) with greatly improved performance.
 
 Currently, CyRK's [numba](https://numba.discourse.group/) (njit-safe) implementation is **10-100x faster** than scipy's solve_ivp function.
 The [cython](https://cython.org/) `cyrk_ode` function that works with python (or numba) functions is **5-40x faster** than scipy.
 The [cython](https://cython.org/) `CySolver` class that works with cython-based cdef classes is **5-400x faster** than scipy.
 
 An additional benefit of the two cython implementations is that they are pre-compiled. This avoids most of the start-up performance hit experienced by just-in-time compilers like numba.
 
 <img style="text-align: center" src="https://github.com/jrenaud90/CyRK/blob/main/Benchmarks/CyRK_SciPy_Compare_v0-6-0a4.png" alt="CyRK Performance" />
 
 ## Installation
 
-It is recommended you use an [Anaconda](https://www.anaconda.com/products/distribution) environment. CyRK has been tested on Python 3.8--3.10
+*CyRK has been tested on Python 3.8--3.11; Windows, Ubuntu, and MacOS.*
 
 To install simply open a terminal and call:
 
 `pip install CyRK`
 
-If not installing from a wheel, CyRK will attempt to install `Cython` and `Numpy` in order to compile the cython code. 
-After the files have been compiled, cython will be uninstalled and CyRK's runtime dependencies 
-(see the pyproject.toml file for the latest list) will be installed instead.
+If not installing from a wheel, CyRK will attempt to install `Cython` and `Numpy` in order to compile the source code. 
+After everything has been compiled, cython will be uninstalled and CyRK's runtime dependencies (see the pyproject.toml file for the latest list) will be installed instead.
 
 A new installation of CyRK can be tested quickly by running the following from a python console.
 ```python
 from CyRK import test_cyrk, test_nbrk, test_cysolver
 test_cyrk()
-# You will hopefully see the message "CyRK's cyrk_ode was tested successfully."
+# Should see "CyRK's cyrk_ode was tested successfully."
 test_nbrk()
-# You will hopefully see the message "CyRK's nbrk_ode was tested successfully."
+# Should see "CyRK's nbrk_ode was tested successfully."
 test_cysolver()
-# You will hopefully see the message "CyRK's CySolver was tested successfully."
+# Should see "CyRK's CySolver was tested successfully."
 ```
 
 ### Installation Troubleshooting
 
 *Please [report](https://github.com/jrenaud90/CyRK/issues) installation issues. We will work on a fix and/or add workaround information here.*
 
 - If you see a "Can not load module: CyRK.cy" or similar error then the cython extensions likely did not compile during installation. Try running `pip install CyRK --no-binary="CyRK"` 
 to force python to recompile the cython extensions locally (rather than via a prebuilt wheel).
-- On MacOS: If you run into problems installing CyRK then reinstall using the verbose flag (`pip install -v .`) to look at the installation log. If you see an error that looks like "clang: error: unsupported option '-fopenmp'" then you may have a problem with your `llvm` or `libomp` libraries. It is recommended that you install CyRK in an anaconda environment with the following packages `conda install numpy scipy cython llvm-openmp`. See more discussion [here](https://github.com/facebookresearch/xformers/issues/157) and the steps taken [here](https://github.com/jrenaud90/CyRK/blob/main/.github/workflows/push_tests_mac.yml).
+- On MacOS: If you run into problems installing CyRK then reinstall using the verbose flag (`pip install -v .`) to look at the installation log. If you see an error that looks like "clang: error: unsupported option '-fopenmp'" then you may have a problem with your `llvm` or `libomp` libraries. It is recommended that you install CyRK in an [Anaconda](https://www.anaconda.com/download) environment with the following packages `conda install numpy scipy cython llvm-openmp`. See more discussion [here](https://github.com/facebookresearch/xformers/issues/157) and the steps taken [here](https://github.com/jrenaud90/CyRK/blob/main/.github/workflows/push_tests_mac.yml).
 
 ### Development and Testing Dependencies
 
-If you intend to work on CyRK's code base you will want to install the following dependencies in order to run CyRK's
-test suite.
+If you intend to work on CyRK's code base you will want to install the following dependencies in order to run CyRK's test suite and experimental notebooks.
 
 `conda install pytest scipy matplotlib jupyter`
 
 `conda install` can be replaced with `pip install` if you prefer.
 
 ## Using CyRK
 CyRK's API is similar to SciPy's solve_ivp function. A differential equation can be defined in python such as:
 
 ```python
 import numpy as np
-from numba import njit
+
 # For even more speed up you can use numba's njit to compile the diffeq
+from numba import njit
 @njit
 def diffeq_nb(t, y):
     dy = np.empty_like(y)
     dy[0] = (1. - 0.01 * y[1]) * y[0]
     dy[1] = (0.02 * y[0] - 1.) * y[1]
     return dy
 
 initial_conds = np.asarray((20., 20.), dtype=np.complex128)
 time_span = (0., 50.)
 rtol = 1.0e-7
 atol = 1.0e-8
 ```
 
 ### Numba-based `nbrk_ode`
-The ODE can then be solved using the numba function by calling CyRK's `nbrk_ode`:
+The system of ODEs can then be solved using CyRK's numba solver by,
 
 ```python
 from CyRK import nbrk_ode
 time_domain, y_results, success, message = \
     nbrk_ode(diffeq_nb, time_span, initial_conds, rk_method=1, rtol=rtol, atol=atol)
 ```
 
 ### Cython-based `cyrk_ode`
 To call the cython version of the integrator you need to slightly edit the differential equation so that it does not
-return the derivative. Instead, the output is passed as an input argument (a np.ndarray) to the function. 
+return the derivative. Instead, the output is passed as an input argument (a `np.ndarray`) to the function. 
 
 ```python
 @njit
 def diffeq_cy(t, y, dy):
     dy[0] = (1. - 0.01 * y[1]) * y[0]
     dy[1] = (0.02 * y[0] - 1.) * y[1]
 ```
 
-Alternatively, you can use CyRK's conversion helper functions to automatically convert between numba/scipy and cyrk
-function calls.
+Alternatively, you can use CyRK's conversion helper functions to automatically convert between numba/scipy and cyrk function calls.
 
 ```python
 from CyRK import nb2cy, cy2nb
 
 @njit
 def diffeq_nb(t, y):
     dy = np.empty_like(y)
@@ -132,120 +129,113 @@
 ```python
 from CyRK import cyrk_ode
 time_domain, y_results, success, message = \
     cyrk_ode(diffeq_cy, time_span, initial_conds, rk_method=1, rtol=rtol, atol=atol)
 ```
 
 ### Cython-based `CySolver`
-The cython-based `CySolver` class requires writing a new cython cdef class. This can be done like so, note this is in a .pyx file that must be
-cythonized and compiled before it can be used.
+The cython-based `CySolver` class requires writing a new cython cdef class. This is done in a new cython .pyx file which must then be cythonized and compiled before it can be used.
 
 ```cython
 """ODE.pyx"""
 # distutils: language = c++
 # cython: boundscheck=False, wraparound=False, nonecheck=False, cdivision=True, initializedcheck=False
+
 from CyRK.cy.cysolver cimport CySolver
 # Note the `cimport` here^
 
-cdef class CySolverTester(CySolver):
+cdef class MyCyRKDiffeq(CySolver):
 
     @cython.exceptval(check=False)
     cdef void diffeq(self):
         
         # Unpack dependent variables using the `self.y_new_view` variable.
+        # In this example we have a system of two dependent variables, but any number can be used.
         cdef double y0, y1
         y0 = self.y_new_view[0]
         y1 = self.y_new_view[1]
 
         # Unpack any additional arguments that do not change with time using the `self.arg_array_view` variable.
         cdef double a, b
         # These must be float64s
         a  = self.arg_array_view[0]
         b  = self.arg_array_view[1]
 
         # If needed, unpack the time variable using `self.t_new`
         cdef double t
         t = self.t_new
 
-        # This function must set the dydt variable `self.dy_new_view`
+        # This then updates dydt by setting the values of `self.dy_new_view`
         self.dy_new_view[0] = (1. - a * y1) * y0
         self.dy_new_view[1] = (b * y0 - 1.) * y1
 ```
 
 Once you compile the differential equation it can be imported in a regular python file and used in a similar fashion to the other integrators.
 
 ```python
 """run.py"""
-from CyRK.cy.cysolvertest import CySolverTester
+from ODE import MyCyRKDiffeq
 
 # Need to make an instance of the integrator.
 # The diffeq no longer needs to be passed to the class.
-CySolverTesterInst = CySolverTester(time_span, initial_conds, args=(0.01, 0.02), rk_method=1, rtol=rtol, atol=atol)
+MyCyRKDiffeqInst = MyCyRKDiffeq(time_span, initial_conds, args=(0.01, 0.02), rk_method=1, rtol=rtol, atol=atol)
 
 # To perform the integration make a call to the solve method.
-CySolverTesterInst.solve()
+MyCyRKDiffeqInst.solve()
 
 # Once complete, you can access the results via...
-CySolverTesterInst.success     # True / False
-CySolverTesterInst.message     # Note about integration
-CySolverTesterInst.solution_t  # Time domain
-CySolverTesterInst.solution_y  # y dependent variables
-CySolverTesterInst.solution_extra  # Extra output that was captured during integration.
+MyCyRKDiffeqInst.success     # True / False
+MyCyRKDiffeqInst.message     # Note about integration
+MyCyRKDiffeqInst.solution_t  # Time domain
+MyCyRKDiffeqInst.solution_y  # y dependent variables
+MyCyRKDiffeqInst.solution_extra  # Extra output that was captured during integration.
 # See Documentation/Extra Output.md for more information on `solution_extra`
 ```
 
 ## Optional Arguments
 
-Both the numba and cython versions of the ODE solver have the following optional inputs:
+All three integrators can take the following optional inputs:
 - `rtol`: Relative Tolerance (default is 1.0e-6).
 - `atol`: Absolute Tolerance (default is 1.0e-8).
 - `max_step`: Maximum step size (default is +infinity).
 - `first_step`: Initial step size (default is 0).
   - If 0, then the solver will try to determine an ideal value.
 - `args`: Python tuple of additional arguments passed to the `diffeq`.
-- `t_eval`: Both solvers uses an adaptive time stepping protocol based on the recent error at each step. This results in
-a final non-uniform time domain of variable size. If the user would like the results at specific time steps then 
-they can provide a np.ndarray array at the desired steps to `t_eval`.
-The solver will then interpolate the results to fit this array.
+  - For the cython solvers these arguments must be floating point numbers only.
+- `t_eval`: Both solvers uses an adaptive time stepping protocol based on the recent error at each step. This results in a final non-uniform time domain of variable size. If the user would like the results at specific time steps then they can provide a np.ndarray array at the desired steps via `t_eval`. The solver will then interpolate the results to fit this array.
 - `rk_method`: Runge-Kutta method (default is 1; all of these methods are based off of
 [SciPy implementations](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html)):
   - `0` - "RK23" Explicit Runge-Kutta method of order 3(2).
   - `1` - "RK45" Explicit Runge-Kutta method of order 5(4).
   - `2` - "DOP853" Explicit Runge-Kutta method of order 8.
 - `capture_extra` and `interpolate_extra`: CyRK has the capability of capturing additional parameters during integration. Please see `Documentation\Extra Output.md` for more details.
 
 ### Additional Arguments for `cyrk_ode` and `CySolver`
 - `num_extra` : The number of extra outputs the integrator should expect.
+  - Please see `Documentation\Extra Output.md` for more details.
 - `expected_size` : Best guess on the expected size of the final time domain (number of points).
-    - The integrator must pre-allocate memory to store results from the integration. It will attempt to use arrays sized to `expected_size`. However, if this is too small or too large then performance will be impacted. It is recommended you try out different values based on the problem you are trying to solve.
+    - The integrator must pre-allocate memory to store results from the integration. It will attempt to use arrays sized to `expected_size`. However, if this is too small or too large then performance will be negatively impacted. It is recommended you try out different values based on the problem you are trying to solve.
     - If `expected_size=0` (the default) then the solver will attempt to guess a best size. Currently this is a very basic guess so it is not recommended.
     - It is better to overshoot than undershoot this guess.
 
 ## Limitations and Known Issues
 
-- [Issue 1](https://github.com/jrenaud90/CyRK/issues/1): Absolute tolerance can only be passed as a single value
-(same for all y's).
+- [Issue 1](https://github.com/jrenaud90/CyRK/issues/1): Absolute tolerance can only be passed as a single value (same for all y's).
+- [Issue 30](https://github.com/jrenaud90/CyRK/issues/30): CyRK's CySolver does not allow for complex-valued dependent variables. 
 
 ## Citing CyRK
 
-It is great to see CyRK used in other software or in scientific studies. We ask that you cite back to CyRK's 
-[GitHub](https://github.com/jrenaud90/CyRK) website so interested parties can learn about this package. 
+It is great to see CyRK used in other software or in scientific studies. We ask that you cite back to CyRK's [GitHub](https://github.com/jrenaud90/CyRK) website so interested parties can learn about this package. It would also be great to hear about the work being done with CyRK, so get in touch!
 
 Renaud, Joe P. (2022). CyRK - ODE Integrator Implemented in Cython and Numba. Zenodo. https://doi.org/10.5281/zenodo.7093266
 
-In addition to citing CyRK, please consider citing SciPy and its references for the specific Runge-Kutta model that
-was used in your work. CyRK is largely an adaptation of SciPy's functionality.
-Find more details [here](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
+In addition to citing CyRK, please consider citing SciPy and its references for the specific Runge-Kutta model that was used in your work. CyRK is largely an adaptation of SciPy's functionality. Find more details [here](https://docs.scipy.org/doc/scipy/reference/generated/scipy.integrate.solve_ivp.html).
 
 Pauli Virtanen, Ralf Gommers, Travis E. Oliphant, Matt Haberland, Tyler Reddy, David Cournapeau, Evgeni Burovski, Pearu Peterson, Warren Weckesser, Jonathan Bright, Stéfan J. van der Walt, Matthew Brett, Joshua Wilson, K. Jarrod Millman, Nikolay Mayorov, Andrew R. J. Nelson, Eric Jones, Robert Kern, Eric Larson, CJ Carey, İlhan Polat, Yu Feng, Eric W. Moore, Jake VanderPlas, Denis Laxalde, Josef Perktold, Robert Cimrman, Ian Henriksen, E.A. Quintero, Charles R Harris, Anne M. Archibald, Antônio H. Ribeiro, Fabian Pedregosa, Paul van Mulbregt, and SciPy 1.0 Contributors. (2020) SciPy 1.0: Fundamental Algorithms for Scientific Computing in Python. Nature Methods, 17(3), 261-272.
 
 ## Contribute to CyRK
 _Please look [here](https://github.com/jrenaud90/CyRK/graphs/contributors) for an up-to-date list of contributors to the CyRK package._
 
-CyRK is open-source and is distributed under the Creative Commons Attribution-ShareAlike 4.0 International license. 
-You are welcome to fork this repository and make any edits with attribution back to this project (please see the 
-`Citing CyRK` section).
+CyRK is open-source and is distributed under the Creative Commons Attribution-ShareAlike 4.0 International license. You are welcome to fork this repository and make any edits with attribution back to this project (please see the `Citing CyRK` section).
 - We encourage users to report bugs or feature requests using [GitHub Issues](https://github.com/jrenaud90/CyRK/issues).
-- If you would like to contribute but don't know where to start, check out the 
-[good first issue](https://github.com/jrenaud90/CyRK/labels/good%20first%20issue) tag on GitHub.
-- Users are welcome to submit pull requests and should feel free to create them before the final code is completed so
-that feedback and suggestions can be given early on.
+- If you would like to contribute but don't know where to start, check out the [good first issue](https://github.com/jrenaud90/CyRK/labels/good%20first%20issue) tag on GitHub.
+- Users are welcome to submit pull requests and should feel free to create them before the final code is completed so that feedback and suggestions can be given early on.
```

### Comparing `CyRK-0.6.0/_build_cyrk.py` & `CyRK-0.6.1/_build_cyrk.py`

 * *Files identical despite different names*

### Comparing `CyRK-0.6.0/pyproject.toml` & `CyRK-0.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name='CyRK'
-version = '0.6.0'
+version = '0.6.1'
 description='Runge-Kutta ODE Integrator Implemented in Cython and Numba.'
 authors= [
     {name = 'Joe P. Renaud', email = 'joe.p.renaud@gmail.com'}
     ]
 requires-python = ">=3.8,<3.12"
 dependencies = [
     'numba>=0.54.1',
```

### Comparing `CyRK-0.6.0/setup.py` & `CyRK-0.6.1/setup.py`

 * *Files identical despite different names*

