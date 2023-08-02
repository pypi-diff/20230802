# Comparing `tmp/lfdfiles-2023.4.20.tar.gz` & `tmp/lfdfiles-2023.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lfdfiles-2023.4.20.tar", last modified: Thu Apr 20 18:59:25 2023, max compression
+gzip compressed data, was "lfdfiles-2023.8.1.tar", last modified: Tue Aug  1 23:48:01 2023, max compression
```

## Comparing `lfdfiles-2023.4.20.tar` & `lfdfiles-2023.8.1.tar`

### file list

```diff
@@ -1,32 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 18:59:25.025725 lfdfiles-2023.4.20/
-drwxrwxrwx   0        0        0        0 2023-04-20 18:59:24.961266 lfdfiles-2023.4.20/.github/
-drwxrwxrwx   0        0        0        0 2023-04-20 18:59:24.989968 lfdfiles-2023.4.20/.github/workflows/
--rw-rw-rw-   0        0        0     1051 2023-04-20 18:31:22.000000 lfdfiles-2023.4.20/.github/workflows/wheel.yml
--rw-rw-rw-   0        0        0     3093 2023-04-20 18:59:21.000000 lfdfiles-2023.4.20/CHANGES.rst
--rw-rw-rw-   0        0        0     1559 2023-04-20 18:59:21.000000 lfdfiles-2023.4.20/LICENSE
--rw-rw-rw-   0        0        0      459 2023-04-20 18:45:59.000000 lfdfiles-2023.4.20/MANIFEST.in
--rw-rw-rw-   0        0        0     7442 2023-04-20 18:59:25.015562 lfdfiles-2023.4.20/PKG-INFO
--rw-rw-rw-   0        0        0     6492 2023-04-20 18:59:21.000000 lfdfiles-2023.4.20/README.rst
-drwxrwxrwx   0        0        0        0 2023-04-20 18:59:24.989968 lfdfiles-2023.4.20/docs/
-drwxrwxrwx   0        0        0        0 2023-04-20 18:59:24.989968 lfdfiles-2023.4.20/docs/_static/
--rw-rw-rw-   0        0        0      127 2022-05-28 19:33:31.000000 lfdfiles-2023.4.20/docs/_static/custom.css
--rw-rw-rw-   0        0        0     1285 2023-04-20 01:18:18.000000 lfdfiles-2023.4.20/docs/conf.py
--rw-rw-rw-   0        0        0      328 2022-06-11 02:47:09.000000 lfdfiles-2023.4.20/docs/index.rst
--rw-rw-rw-   0        0        0     2809 2022-01-30 04:01:44.000000 lfdfiles-2023.4.20/fbdfix.py
-drwxrwxrwx   0        0        0        0 2023-04-20 18:59:25.005357 lfdfiles-2023.4.20/lfdfiles/
--rw-rw-rw-   0        0        0      104 2020-01-01 02:24:19.000000 lfdfiles-2023.4.20/lfdfiles/__init__.py
--rw-rw-rw-   0        0        0      135 2020-01-01 02:24:17.000000 lfdfiles-2023.4.20/lfdfiles/__main__.py
--rw-rw-rw-   0        0        0  1352369 2023-04-20 18:57:37.000000 lfdfiles-2023.4.20/lfdfiles/_lfdfiles.c
--rw-rw-rw-   0        0        0    15864 2023-04-20 18:47:26.000000 lfdfiles-2023.4.20/lfdfiles/_lfdfiles.pyx
--rw-rw-rw-   0        0        0     6444 2022-06-11 06:33:29.000000 lfdfiles-2023.4.20/lfdfiles/fbd2b64.py
--rw-rw-rw-   0        0        0   212656 2023-04-20 18:52:14.000000 lfdfiles-2023.4.20/lfdfiles/lfdfiles.py
-drwxrwxrwx   0        0        0        0 2023-04-20 18:59:25.015562 lfdfiles-2023.4.20/lfdfiles.egg-info/
--rw-rw-rw-   0        0        0     7442 2023-04-20 18:59:23.000000 lfdfiles-2023.4.20/lfdfiles.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      493 2023-04-20 18:59:24.000000 lfdfiles-2023.4.20/lfdfiles.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 18:59:23.000000 lfdfiles-2023.4.20/lfdfiles.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-04-20 18:59:23.000000 lfdfiles-2023.4.20/lfdfiles.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-20 18:59:23.000000 lfdfiles-2023.4.20/lfdfiles.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       78 2023-04-20 18:59:23.000000 lfdfiles-2023.4.20/lfdfiles.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 18:59:23.000000 lfdfiles-2023.4.20/lfdfiles.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 18:59:25.025725 lfdfiles-2023.4.20/setup.cfg
--rw-rw-rw-   0        0        0     4518 2023-04-20 18:46:25.000000 lfdfiles-2023.4.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:48:01.962519 lfdfiles-2023.8.1/
+drwxrwxrwx   0        0        0        0 2023-08-01 23:48:01.912284 lfdfiles-2023.8.1/.github/
+drwxrwxrwx   0        0        0        0 2023-08-01 23:48:01.940426 lfdfiles-2023.8.1/.github/workflows/
+-rw-rw-rw-   0        0        0     1074 2023-08-01 22:38:10.000000 lfdfiles-2023.8.1/.github/workflows/wheel.yml
+-rw-rw-rw-   0        0        0     3165 2023-08-01 23:47:56.000000 lfdfiles-2023.8.1/CHANGES.rst
+-rw-rw-rw-   0        0        0     1559 2023-08-01 23:47:56.000000 lfdfiles-2023.8.1/LICENSE
+-rw-rw-rw-   0        0        0      540 2023-04-21 16:58:28.000000 lfdfiles-2023.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7687 2023-08-01 23:48:01.962519 lfdfiles-2023.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6648 2023-08-01 23:47:56.000000 lfdfiles-2023.8.1/README.rst
+-rw-rw-rw-   0        0        0     2809 2022-01-30 04:01:44.000000 lfdfiles-2023.8.1/fbdfix.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:48:01.951016 lfdfiles-2023.8.1/lfdfiles/
+-rw-rw-rw-   0        0        0      104 2020-01-01 02:24:19.000000 lfdfiles-2023.8.1/lfdfiles/__init__.py
+-rw-rw-rw-   0        0        0      135 2020-01-01 02:24:17.000000 lfdfiles-2023.8.1/lfdfiles/__main__.py
+-rw-rw-rw-   0        0        0  1417911 2023-08-01 23:46:25.000000 lfdfiles-2023.8.1/lfdfiles/_lfdfiles.c
+-rw-rw-rw-   0        0        0    22458 2023-08-01 22:45:07.000000 lfdfiles-2023.8.1/lfdfiles/_lfdfiles.pyx
+-rw-rw-rw-   0        0        0     6444 2022-06-11 06:33:29.000000 lfdfiles-2023.8.1/lfdfiles/fbd2b64.py
+-rw-rw-rw-   0        0        0   213781 2023-08-01 22:45:01.000000 lfdfiles-2023.8.1/lfdfiles/lfdfiles.py
+drwxrwxrwx   0        0        0        0 2023-08-01 23:48:01.962519 lfdfiles-2023.8.1/lfdfiles.egg-info/
+-rw-rw-rw-   0        0        0     7687 2023-08-01 23:48:00.000000 lfdfiles-2023.8.1/lfdfiles.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      441 2023-08-01 23:48:01.000000 lfdfiles-2023.8.1/lfdfiles.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-01 23:48:00.000000 lfdfiles-2023.8.1/lfdfiles.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-08-01 23:48:00.000000 lfdfiles-2023.8.1/lfdfiles.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-01 23:48:00.000000 lfdfiles-2023.8.1/lfdfiles.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       78 2023-08-01 23:48:00.000000 lfdfiles-2023.8.1/lfdfiles.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-08-01 23:48:00.000000 lfdfiles-2023.8.1/lfdfiles.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-01 23:48:01.962519 lfdfiles-2023.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     4744 2023-07-05 15:06:23.000000 lfdfiles-2023.8.1/setup.py
```

### Comparing `lfdfiles-2023.4.20/.github/workflows/wheel.yml` & `lfdfiles-2023.8.1/.github/workflows/wheel.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,19 +8,19 @@
     name: Build wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04, macos-12, windows-2019]
     steps:
       - uses: actions/checkout@v3
-      - uses: pypa/cibuildwheel@v2.12.3
+      - uses: pypa/cibuildwheel@v2.14.1
         env:
-          CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x"
+          CIBW_SKIP: "pp* cp37* cp38* *musllinux* *i686 *ppc64le *s390x cp39*win*arm64 cp310*win*arm64"
           CIBW_BEFORE_ALL_MACOS: curl -O https://mac.r-project.org/openmp/openmp-14.0.6-darwin20-Release.tar.gz && sudo tar fvxz openmp-14.0.6-darwin20-Release.tar.gz -C /
-          CIBW_BEFORE_BUILD: python -m pip install oldest-supported-numpy cython
+          CIBW_BEFORE_BUILD: python -m pip install numpy Cython==0.29.36
           # CIBW_ARCHS_LINUX: auto aarch64
           CIBW_ARCHS_LINUX: auto
           CIBW_ARCHS_MACOS: x86_64 arm64
           CIBW_ARCHS_WINDOWS: AMD64 ARM64 x86
           CIBW_TEST_REQUIRES: numpy tifffile
           CIBW_TEST_COMMAND: python -c "import lfdfiles;from lfdfiles import _lfdfiles;print(lfdfiles.__version__)"
       - uses: actions/upload-artifact@v3
```

### Comparing `lfdfiles-2023.4.20/CHANGES.rst` & `lfdfiles-2023.8.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Revisions
 ---------
 
+2023.8.1
+
+- Specify encoding of text files.
+- Fix linting issues.
+
 2023.4.20
 
 - Improve type hints.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2022.9.29
```

### Comparing `lfdfiles-2023.4.20/LICENSE` & `lfdfiles-2023.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lfdfiles-2023.4.20/PKG-INFO` & `lfdfiles-2023.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfdfiles
-Version: 2023.4.20
+Version: 2023.8.1
 Summary: Laboratory for Fluorescence Dynamics (LFD) file formats
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/lfdfiles/issues
 Project-URL: Source Code, https://github.com/cgohlke/lfdfiles
@@ -15,15 +15,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 Provides-Extra: all
 License-File: LICENSE
 
 Laboratory for Fluorescence Dynamics (LFD) file formats
 =======================================================
 
 Lfdfiles is a Python library and console script for reading, writing,
@@ -39,54 +41,61 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.20
+:Version: 2023.8.1
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
 
     python -m pip install -U lfdfiles[all]
 
 Print the console script usage::
 
     python -m lfdfiles --help
 
+The lfdfiles library is type annotated and documented via docstrings.
+
 See `Examples`_ for using the programming interface.
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/lfdfiles>`_.
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
-- `Cython <https://pypi.org/project/cython/>`_ 0.29.34 (build)
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12(optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b4
+- `Cython <https://pypi.org/project/cython/>`_ 0.29.36 (build)
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.1
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.7.18 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile />`_ 2022.9.29 (optional)
-- `Netpbmfile <https://pypi.org/project/netpbmfile />`_ 2023.1.1 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+- `Netpbmfile <https://pypi.org/project/netpbmfile />`_ 2023.6.15 (optional)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
   (optional, for plotting)
-- `Click <https://pypi.python.org/pypi/click>`_ 8.1.3
+- `Click <https://pypi.python.org/pypi/click>`_ 8.1.6
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2023.8.1
+
+- Specify encoding of text files.
+- Fix linting issues.
+
 2023.4.20
 
 - Improve type hints.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2022.9.29
```

### Comparing `lfdfiles-2023.4.20/README.rst` & `lfdfiles-2023.8.1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -14,54 +14,61 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.20
+:Version: 2023.8.1
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
 
     python -m pip install -U lfdfiles[all]
 
 Print the console script usage::
 
     python -m lfdfiles --help
 
+The lfdfiles library is type annotated and documented via docstrings.
+
 See `Examples`_ for using the programming interface.
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/lfdfiles>`_.
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
-- `Cython <https://pypi.org/project/cython/>`_ 0.29.34 (build)
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12(optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b4
+- `Cython <https://pypi.org/project/cython/>`_ 0.29.36 (build)
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.1
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.7.18 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile />`_ 2022.9.29 (optional)
-- `Netpbmfile <https://pypi.org/project/netpbmfile />`_ 2023.1.1 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+- `Netpbmfile <https://pypi.org/project/netpbmfile />`_ 2023.6.15 (optional)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
   (optional, for plotting)
-- `Click <https://pypi.python.org/pypi/click>`_ 8.1.3
+- `Click <https://pypi.python.org/pypi/click>`_ 8.1.6
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2023.8.1
+
+- Specify encoding of text files.
+- Fix linting issues.
+
 2023.4.20
 
 - Improve type hints.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2022.9.29
```

### Comparing `lfdfiles-2023.4.20/fbdfix.py` & `lfdfiles-2023.8.1/fbdfix.py`

 * *Files identical despite different names*

### Comparing `lfdfiles-2023.4.20/lfdfiles/_lfdfiles.c` & `lfdfiles-2023.8.1/lfdfiles/_lfdfiles.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-/* Generated by Cython 0.29.34 */
+/* Generated by Cython 0.29.36 */
 
 #ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
 #endif /* PY_SSIZE_T_CLEAN */
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
 #elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
     #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "0_29_34"
-#define CYTHON_HEX_VERSION 0x001D22F0
+#define CYTHON_ABI "0_29_36"
+#define CYTHON_HEX_VERSION 0x001D24F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -74,18 +74,22 @@
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #if PY_VERSION_HEX < 0x03090000
+    #undef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
+    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
+  #endif
   #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
+  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
@@ -361,17 +365,14 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
-  #define Py_OptimizeFlag 0
-#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
   #define __Pyx_DefaultClassType PyClass_Type
@@ -441,14 +442,19 @@
     }
 #else
   #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
   #define __Pyx_DefaultClassType PyType_Type
 #endif
+#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
+  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
+#else
+  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
+#endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
@@ -1798,14 +1804,31 @@
     Py_DECREF(none);
     return 0;
 #else
     return PyList_SetSlice(L, PY_SSIZE_T_MAX, PY_SSIZE_T_MAX, v);
 #endif
 }
 
+/* AssertionsEnabled.proto */
+#define __Pyx_init_assertions_enabled()
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define __pyx_assertions_enabled() (1)
+#elif PY_VERSION_HEX < 0x03080000  ||  CYTHON_COMPILING_IN_PYPY  ||  defined(Py_LIMITED_API)
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#elif CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030900A6
+  static int __pyx_assertions_enabled_flag;
+  #define __pyx_assertions_enabled() (__pyx_assertions_enabled_flag)
+  #undef __Pyx_init_assertions_enabled
+  static void __Pyx_init_assertions_enabled(void) {
+    __pyx_assertions_enabled_flag = ! _PyInterpreterState_GetConfig(__Pyx_PyThreadState_Current->interp)->optimization_level;
+  }
+#else
+  #define __pyx_assertions_enabled() (!Py_OptimizeFlag)
+#endif
+
 /* None.proto */
 static CYTHON_INLINE void __Pyx_RaiseUnboundLocalError(const char *varname);
 
 /* PySequenceContains.proto */
 static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
     int result = PySequence_Contains(seq, item);
     return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
@@ -2021,14 +2044,17 @@
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dsds_nn_int16_t(PyObject *, int writable_flag);
 
 /* ObjectToMemviewSlice.proto */
 static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_dc_nn_uint32_t__const__(PyObject *, int writable_flag);
 
+/* ObjectToMemviewSlice.proto */
+static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn_uint16_t(PyObject *, int writable_flag);
+
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_Py_ssize_t(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_Py_ssize_t(const char *itemp, PyObject *obj);
 
 /* MemviewDtypeToObject.proto */
 static CYTHON_INLINE PyObject *__pyx_memview_get_nn_uint32_t(const char *itemp);
 static CYTHON_INLINE int __pyx_memview_set_nn_uint32_t(const char *itemp, PyObject *obj);
@@ -2116,16 +2142,17 @@
 static PyObject *generic = 0;
 static PyObject *strided = 0;
 static PyObject *indirect = 0;
 static PyObject *contiguous = 0;
 static PyObject *indirect_contiguous = 0;
 static int __pyx_memoryview_thread_locks_used;
 static PyThread_type_lock __pyx_memoryview_thread_locks[8];
-static int __pyx_fuse_0__pyx_f_8lfdfiles_9_lfdfiles__decode_address(Py_ssize_t const , __Pyx_memviewslice, __Pyx_memviewslice, Py_ssize_t const , uint64_t const , uint64_t const , Py_ssize_t const , omp_lock_t); /*proto*/
-static int __pyx_fuse_1__pyx_f_8lfdfiles_9_lfdfiles__decode_address(Py_ssize_t const , __Pyx_memviewslice, __Pyx_memviewslice, Py_ssize_t const , uint64_t const , uint64_t const , Py_ssize_t const , omp_lock_t); /*proto*/
+static Py_ssize_t __pyx_f_8lfdfiles_9_lfdfiles__decode_address_photons(Py_ssize_t const , __Pyx_memviewslice, __Pyx_memviewslice, Py_ssize_t const , Py_ssize_t const , Py_ssize_t const , uint64_t const , uint64_t const , Py_ssize_t const ); /*proto*/
+static Py_ssize_t __pyx_fuse_0__pyx_f_8lfdfiles_9_lfdfiles__decode_address(Py_ssize_t const , __Pyx_memviewslice, __Pyx_memviewslice, Py_ssize_t const , uint64_t const , uint64_t const , Py_ssize_t const , omp_lock_t); /*proto*/
+static Py_ssize_t __pyx_fuse_1__pyx_f_8lfdfiles_9_lfdfiles__decode_address(Py_ssize_t const , __Pyx_memviewslice, __Pyx_memviewslice, Py_ssize_t const , uint64_t const , uint64_t const , Py_ssize_t const , omp_lock_t); /*proto*/
 static CYTHON_INLINE PyObject *__Pyx_carray_to_py_Py_ssize_t(Py_ssize_t *, Py_ssize_t); /*proto*/
 static CYTHON_INLINE PyObject *__Pyx_carray_to_tuple_Py_ssize_t(Py_ssize_t *, Py_ssize_t); /*proto*/
 static struct __pyx_array_obj *__pyx_array_new(PyObject *, Py_ssize_t, char *, char *, char *); /*proto*/
 static void *__pyx_align_pointer(void *, size_t); /*proto*/
 static PyObject *__pyx_memoryview_new(PyObject *, int, int, __Pyx_TypeInfo *); /*proto*/
 static CYTHON_INLINE int __pyx_memoryview_check(PyObject *); /*proto*/
 static PyObject *_unellipsify(PyObject *, int); /*proto*/
@@ -2188,16 +2215,18 @@
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_s[] = "s";
 static const char __pyx_k_w[] = "w";
 static const char __pyx_k__2[] = "|";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_m0[] = "m0";
 static const char __pyx_k_m1[] = "m1";
+static const char __pyx_k_np[] = "np";
 static const char __pyx_k_t0[] = "t0";
 static const char __pyx_k_t1[] = "t1";
+static const char __pyx_k_1_5[] = " != (-1, 5)";
 static const char __pyx_k_idx[] = "idx";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_pcc[] = "pcc";
 static const char __pyx_k_ret[] = "ret";
 static const char __pyx_k_win[] = "win";
 static const char __pyx_k_args[] = "args";
@@ -2227,35 +2256,39 @@
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_sflim[] = "sflim";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_split[] = "split";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_strip[] = "strip";
 static const char __pyx_k_times[] = "times";
+static const char __pyx_k_width[] = "width";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
+static const char __pyx_k_height[] = "height";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_kwargs[] = "kwargs";
 static const char __pyx_k_name_2[] = "__name__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_struct[] = "struct";
 static const char __pyx_k_unpack[] = "unpack";
 static const char __pyx_k_update[] = "update";
 static const char __pyx_k_address[] = "address";
 static const char __pyx_k_fortran[] = "fortran";
 static const char __pyx_k_memview[] = "memview";
 static const char __pyx_k_nframes[] = "nframes";
 static const char __pyx_k_pcc_shr[] = "pcc_shr";
+static const char __pyx_k_photons[] = "photons";
 static const char __pyx_k_tcc_max[] = "tcc_max";
 static const char __pyx_k_tcc_shr[] = "tcc_shr";
 static const char __pyx_k_uint8_t[] = "uint8_t";
 static const char __pyx_k_version[] = "__version__";
 static const char __pyx_k_win_shr[] = "win_shr";
 static const char __pyx_k_windows[] = "windows";
+static const char __pyx_k_2023_8_1[] = "2023.8.1";
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_bins_out[] = "bins_out";
 static const char __pyx_k_datasize[] = "datasize";
 static const char __pyx_k_defaults[] = "defaults";
 static const char __pyx_k_framelen[] = "framelen";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_hist_out[] = "hist_out";
@@ -2267,30 +2300,31 @@
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
 static const char __pyx_k_tcc_mask[] = "tcc_mask";
 static const char __pyx_k_uint16_t[] = "uint16_t";
 static const char __pyx_k_uint32_t[] = "uint32_t";
 static const char __pyx_k_uint64_t[] = "uint64_t";
 static const char __pyx_k_win_mask[] = "win_mask";
-static const char __pyx_k_2023_4_20[] = "2023.4.20";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_harmonics[] = "harmonics";
 static const char __pyx_k_maxframes[] = "maxframes";
 static const char __pyx_k_maxmarker[] = "maxmarker";
 static const char __pyx_k_maxwindex[] = "maxwindex";
 static const char __pyx_k_nchannels[] = "nchannels";
 static const char __pyx_k_pixeltime[] = "pixeltime";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_times_out[] = "times_out";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_ValueError[] = "ValueError";
 static const char __pyx_k_enabletime[] = "enabletime";
+static const char __pyx_k_frameshape[] = "frameshape";
 static const char __pyx_k_marker_shr[] = "marker_shr";
+static const char __pyx_k_maxphotons[] = "maxphotons";
 static const char __pyx_k_numthreads[] = "numthreads";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_signatures[] = "signatures";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
 static const char __pyx_k_marker_mask[] = "marker_mask";
@@ -2311,32 +2345,36 @@
 static const char __pyx_k_units_per_sample[] = "units_per_sample";
 static const char __pyx_k_pyx_unpickle_Enum[] = "__pyx_unpickle_Enum";
 static const char __pyx_k_uint16_t_uint32_t[] = "uint16_t|uint32_t";
 static const char __pyx_k_uint16_t_uint64_t[] = "uint16_t|uint64_t";
 static const char __pyx_k_uint32_t_uint32_t[] = "uint32_t|uint32_t";
 static const char __pyx_k_uint32_t_uint64_t[] = "uint32_t|uint64_t";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
+static const char __pyx_k_invalid_frameshape[] = "invalid frameshape";
 static const char __pyx_k_invalid_parameters[] = "invalid parameters";
 static const char __pyx_k_lfdfiles__lfdfiles[] = "lfdfiles._lfdfiles";
 static const char __pyx_k_strided_and_direct[] = "<strided and direct>";
 static const char __pyx_k_32_256_height_width[] = " != (32, 256, height, width)";
 static const char __pyx_k_invalid_sflim_shape[] = "invalid sflim shape ";
 static const char __pyx_k_scanner_frame_start[] = "scanner_frame_start";
 static const char __pyx_k_simfcsfbd_histogram[] = "simfcsfbd_histogram";
+static const char __pyx_k_sflim_decode_photons[] = "sflim_decode_photons";
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
+static const char __pyx_k_invalid_photons_shape[] = "invalid photons shape ";
 static const char __pyx_k_sflim_decode_line_274[] = "sflim_decode (line 274)";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_lfdfiles__lfdfiles_pyx[] = "lfdfiles\\_lfdfiles.pyx";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_No_matching_signature_found[] = "No matching signature found";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
+static const char __pyx_k_sflim_decode_photons_line_460[] = "sflim_decode_photons (line 460)";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_shape_mismatch_between_bins_and[] = "shape mismatch between bins and decoder_table";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
 static const char __pyx_k_Can_only_create_a_buffer_that_is[] = "Can only create a buffer that is contiguous in memory.";
 static const char __pyx_k_Cannot_assign_to_read_only_memor[] = "Cannot assign to read-only memoryview";
 static const char __pyx_k_Cannot_create_writable_memory_vi[] = "Cannot create writable memory view from read-only memoryview";
@@ -2353,24 +2391,27 @@
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_no_start_of_frame_found_for_addr[] = "no start of frame found for address ";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
 static const char __pyx_k_shape_mismatch_between_bins_and_2[] = "shape mismatch between bins and time";
 static const char __pyx_k_shape_mismatch_between_bins_and_3[] = "shape mismatch between bins and hist_out";
 static const char __pyx_k_shape_mismatch_between_bins_and_4[] = "shape mismatch between bins and times";
+static const char __pyx_k_Decode_Kintex_FLIMbox_data_to_SL_2[] = "Decode Kintex FLIMbox data to SLIM photon array.\n\n    This function is private and may change or be removed in future versions.\n\n    Parameters:\n        data (numpy.ndarray):\n            Data stream from Kintex FLIMbox. A `uint32` array.\n        photons (numpy.ndarray):\n            `uint16` array of shape `(number of photons, 5)`,\n            where arrival time, frame, channel, y and x position are stored for\n            each photon.\n        frameshape (tuple):\n            Shape of image frame.\n        pixeltime (int):\n            Pixel dwell time in FLIMbox units.\n            ``math.ceil(dwelltime * 256 / 255 * frequency_factor * frequency)``\n        enabletime (int):\n            Time in FLIMbox units to wait after detecting enable bit before\n            detecting next enable bit.\n        maxframes (int):\n            Maximum number of image frames to decode.\n\n    Returns:\n        Number of photons decoded.\n\n    Examples:\n        >>> import numpy, math\n        >>> from lfdfiles._lfdfiles import sflim_decode_photons\n        >>> data = numpy.fromfile(\n        ...     '20210123488_100x_NSC_166_TMRM_4_zoom4000_L115.bin',\n        ...      dtype=numpy.uint32\n        ... )\n        >>> frequency = 78e6\n        >>> frequency_factor = 0.9976\n        >>> dwelltime = 16e-6\n        >>> pixeltime = math.ceil(\n        ...     dwelltime * 256 / 255 * frequency_factor * frequency\n        ... )\n        >>> photons = numpy.zeros((2035488, 5), dtype=numpy.uint6)\n        >>> sflim_decode_photons(\n        ...     data, photons, (256, 342), pixeltime=pixeltime, maxframes=20\n        ... )\n        2035488\n        >>> photons[12345].tolist()\n        [205, 3, 2, 181, 51]\n\n    ";
 static PyObject *__pyx_kp_s_;
-static PyObject *__pyx_kp_u_2023_4_20;
+static PyObject *__pyx_kp_u_1_5;
+static PyObject *__pyx_kp_u_2023_8_1;
 static PyObject *__pyx_kp_u_32_256_height_width;
 static PyObject *__pyx_n_s_ASCII;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
 static PyObject *__pyx_kp_u_Decode_Kintex_FLIMbox_data_to_SL;
+static PyObject *__pyx_kp_u_Decode_Kintex_FLIMbox_data_to_SL_2;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
 static PyObject *__pyx_kp_s_Expected_at_least_d_argument_s_g;
 static PyObject *__pyx_kp_s_Function_call_with_ambiguous_arg;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
@@ -2415,23 +2456,27 @@
 static PyObject *__pyx_n_s_f;
 static PyObject *__pyx_n_s_flags;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_fortran;
 static PyObject *__pyx_n_u_fortran;
 static PyObject *__pyx_n_s_frame_markers;
 static PyObject *__pyx_n_s_framelen;
+static PyObject *__pyx_n_s_frameshape;
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_s_harmonics;
+static PyObject *__pyx_n_s_height;
 static PyObject *__pyx_n_s_hist_out;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_idx;
 static PyObject *__pyx_n_s_import;
+static PyObject *__pyx_kp_u_invalid_frameshape;
 static PyObject *__pyx_kp_u_invalid_parameters;
+static PyObject *__pyx_kp_u_invalid_photons_shape;
 static PyObject *__pyx_kp_u_invalid_sflim_shape;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_j;
 static PyObject *__pyx_n_s_k;
 static PyObject *__pyx_n_s_kind;
 static PyObject *__pyx_n_s_kwargs;
@@ -2442,35 +2487,38 @@
 static PyObject *__pyx_n_s_m1;
 static PyObject *__pyx_n_s_main;
 static PyObject *__pyx_n_s_marker_mask;
 static PyObject *__pyx_n_s_marker_shr;
 static PyObject *__pyx_n_s_markers_out;
 static PyObject *__pyx_n_s_maxframes;
 static PyObject *__pyx_n_s_maxmarker;
+static PyObject *__pyx_n_s_maxphotons;
 static PyObject *__pyx_n_s_maxwindex;
 static PyObject *__pyx_n_s_memview;
 static PyObject *__pyx_n_s_mode;
 static PyObject *__pyx_n_s_name;
 static PyObject *__pyx_n_s_name_2;
 static PyObject *__pyx_n_s_nchannel;
 static PyObject *__pyx_n_s_nchannels;
 static PyObject *__pyx_n_s_ndim;
 static PyObject *__pyx_n_s_new;
 static PyObject *__pyx_n_s_nframes;
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_kp_u_no_start_of_frame_found_for_addr;
+static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_n_s_numthreads;
 static PyObject *__pyx_n_s_nwindows;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_pack;
 static PyObject *__pyx_n_s_pcc;
 static PyObject *__pyx_n_s_pcc_mask;
 static PyObject *__pyx_n_s_pcc_shr;
 static PyObject *__pyx_n_s_pdiv;
+static PyObject *__pyx_n_s_photons;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_pixeltime;
 static PyObject *__pyx_n_s_pmax;
 static PyObject *__pyx_n_s_pmax_win;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
@@ -2487,14 +2535,16 @@
 static PyObject *__pyx_n_s_s;
 static PyObject *__pyx_n_s_scanner_frame_start;
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_sflim;
 static PyObject *__pyx_n_s_sflim_decode;
 static PyObject *__pyx_kp_u_sflim_decode_line_274;
+static PyObject *__pyx_n_s_sflim_decode_photons;
+static PyObject *__pyx_kp_u_sflim_decode_photons_line_460;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_kp_u_shape_mismatch_between_bins_and;
 static PyObject *__pyx_kp_u_shape_mismatch_between_bins_and_2;
 static PyObject *__pyx_kp_u_shape_mismatch_between_bins_and_3;
 static PyObject *__pyx_kp_u_shape_mismatch_between_bins_and_4;
 static PyObject *__pyx_n_s_signatures;
 static PyObject *__pyx_n_s_simfcsfbd_decode;
@@ -2529,31 +2579,33 @@
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_units_per_sample;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_version;
 static PyObject *__pyx_n_s_w;
+static PyObject *__pyx_n_s_width;
 static PyObject *__pyx_n_s_win;
 static PyObject *__pyx_n_s_win_mask;
 static PyObject *__pyx_n_s_win_shr;
 static PyObject *__pyx_n_s_windows;
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_6simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint16_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint16_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint16_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint16_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr); /* proto */
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_8simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint16_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint16_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint16_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint16_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr); /* proto */
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_10simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint32_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint32_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint32_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint32_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr); /* proto */
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_10simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint16_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint16_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint16_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint16_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr); /* proto */
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_12simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint32_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint32_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint32_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint32_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr); /* proto */
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_14simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint32_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint32_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint32_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint32_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr); /* proto */
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_2simfcsfbd_histogram(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_16simfcsfbd_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out); /* proto */
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_18simfcsfbd_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out); /* proto */
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_20simfcsfbd_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out); /* proto */
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_4sflim_decode(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_signatures, PyObject *__pyx_v_args, PyObject *__pyx_v_kwargs, CYTHON_UNUSED PyObject *__pyx_v_defaults); /* proto */
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_32__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_22sflim_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes, int __pyx_v_numthreads); /* proto */
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_34__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
 static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_24sflim_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes, int __pyx_v_numthreads); /* proto */
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_36__defaults__(CYTHON_UNUSED PyObject *__pyx_self); /* proto */
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_26sflim_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes, int __pyx_v_numthreads); /* proto */
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_6sflim_decode_photons(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_photons, PyObject *__pyx_v_frameshape, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2609,46 +2661,49 @@
 static PyObject *__pyx_tuple__3;
 static PyObject *__pyx_tuple__4;
 static PyObject *__pyx_tuple__5;
 static PyObject *__pyx_tuple__6;
 static PyObject *__pyx_tuple__7;
 static PyObject *__pyx_tuple__8;
 static PyObject *__pyx_tuple__9;
-static PyObject *__pyx_slice__25;
+static PyObject *__pyx_slice__26;
 static PyObject *__pyx_tuple__11;
 static PyObject *__pyx_tuple__12;
 static PyObject *__pyx_tuple__13;
 static PyObject *__pyx_tuple__14;
 static PyObject *__pyx_tuple__15;
 static PyObject *__pyx_tuple__16;
 static PyObject *__pyx_tuple__17;
 static PyObject *__pyx_tuple__18;
 static PyObject *__pyx_tuple__19;
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__23;
 static PyObject *__pyx_tuple__24;
-static PyObject *__pyx_tuple__26;
+static PyObject *__pyx_tuple__25;
 static PyObject *__pyx_tuple__27;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__29;
 static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_tuple__32;
-static PyObject *__pyx_tuple__34;
-static PyObject *__pyx_tuple__36;
+static PyObject *__pyx_tuple__31;
+static PyObject *__pyx_tuple__33;
+static PyObject *__pyx_tuple__35;
 static PyObject *__pyx_tuple__37;
-static PyObject *__pyx_tuple__38;
 static PyObject *__pyx_tuple__39;
 static PyObject *__pyx_tuple__40;
 static PyObject *__pyx_tuple__41;
-static PyObject *__pyx_codeobj__31;
-static PyObject *__pyx_codeobj__33;
-static PyObject *__pyx_codeobj__35;
-static PyObject *__pyx_codeobj__42;
+static PyObject *__pyx_tuple__42;
+static PyObject *__pyx_tuple__43;
+static PyObject *__pyx_tuple__44;
+static PyObject *__pyx_codeobj__32;
+static PyObject *__pyx_codeobj__34;
+static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__38;
+static PyObject *__pyx_codeobj__45;
 /* Late includes */
 
 /* "lfdfiles/_lfdfiles.pyx":67
  * 
  * 
  * def simfcsfbd_decode(             # <<<<<<<<<<<<<<
  *     data_t[::] data,
@@ -3442,17 +3497,17 @@
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0_0__pyx_pw_8lfdfiles_9_lfdfiles_7simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0_0__pyx_mdef_8lfdfiles_9_lfdfiles_7simfcsfbd_decode = {"__pyx_fuse_0_0simfcsfbd_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_0__pyx_pw_8lfdfiles_9_lfdfiles_7simfcsfbd_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_simfcsfbd_decode};
-static PyObject *__pyx_fuse_0_0__pyx_pw_8lfdfiles_9_lfdfiles_7simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0_0__pyx_pw_8lfdfiles_9_lfdfiles_9simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0_0__pyx_mdef_8lfdfiles_9_lfdfiles_9simfcsfbd_decode = {"__pyx_fuse_0_0simfcsfbd_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_0__pyx_pw_8lfdfiles_9_lfdfiles_9simfcsfbd_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_simfcsfbd_decode};
+static PyObject *__pyx_fuse_0_0__pyx_pw_8lfdfiles_9_lfdfiles_9simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_data = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_bins_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_times_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_markers_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_v_windows;
   int __pyx_v_pdiv;
   int __pyx_v_harmonics;
@@ -3653,22 +3708,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("simfcsfbd_decode", 1, 16, 16, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 67, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lfdfiles._lfdfiles.simfcsfbd_decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_6simfcsfbd_decode(__pyx_self, __pyx_v_data, __pyx_v_bins_out, __pyx_v_times_out, __pyx_v_markers_out, __pyx_v_windows, __pyx_v_pdiv, __pyx_v_harmonics, __pyx_v_decoder_table, __pyx_v_tcc_mask, __pyx_v_tcc_shr, __pyx_v_pcc_mask, __pyx_v_pcc_shr, __pyx_v_marker_mask, __pyx_v_marker_shr, __pyx_v_win_mask, __pyx_v_win_shr);
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_8simfcsfbd_decode(__pyx_self, __pyx_v_data, __pyx_v_bins_out, __pyx_v_times_out, __pyx_v_markers_out, __pyx_v_windows, __pyx_v_pdiv, __pyx_v_harmonics, __pyx_v_decoder_table, __pyx_v_tcc_mask, __pyx_v_tcc_shr, __pyx_v_pcc_mask, __pyx_v_pcc_shr, __pyx_v_marker_mask, __pyx_v_marker_shr, __pyx_v_win_mask, __pyx_v_win_shr);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_6simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint16_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint16_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint16_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint16_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_8simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint16_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint16_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint16_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint16_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr) {
   int __pyx_v_maxwindex;
   Py_ssize_t __pyx_v_maxmarker;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannel;
   Py_ssize_t __pyx_v_datasize;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_c;
@@ -4353,17 +4408,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_decoder_table, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0_1__pyx_pw_8lfdfiles_9_lfdfiles_9simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0_1__pyx_mdef_8lfdfiles_9_lfdfiles_9simfcsfbd_decode = {"__pyx_fuse_0_1simfcsfbd_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_1__pyx_pw_8lfdfiles_9_lfdfiles_9simfcsfbd_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_simfcsfbd_decode};
-static PyObject *__pyx_fuse_0_1__pyx_pw_8lfdfiles_9_lfdfiles_9simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0_1__pyx_pw_8lfdfiles_9_lfdfiles_11simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0_1__pyx_mdef_8lfdfiles_9_lfdfiles_11simfcsfbd_decode = {"__pyx_fuse_0_1simfcsfbd_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0_1__pyx_pw_8lfdfiles_9_lfdfiles_11simfcsfbd_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_simfcsfbd_decode};
+static PyObject *__pyx_fuse_0_1__pyx_pw_8lfdfiles_9_lfdfiles_11simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_data = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_bins_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_times_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_markers_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_v_windows;
   int __pyx_v_pdiv;
   int __pyx_v_harmonics;
@@ -4564,22 +4619,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("simfcsfbd_decode", 1, 16, 16, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 67, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lfdfiles._lfdfiles.simfcsfbd_decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_8simfcsfbd_decode(__pyx_self, __pyx_v_data, __pyx_v_bins_out, __pyx_v_times_out, __pyx_v_markers_out, __pyx_v_windows, __pyx_v_pdiv, __pyx_v_harmonics, __pyx_v_decoder_table, __pyx_v_tcc_mask, __pyx_v_tcc_shr, __pyx_v_pcc_mask, __pyx_v_pcc_shr, __pyx_v_marker_mask, __pyx_v_marker_shr, __pyx_v_win_mask, __pyx_v_win_shr);
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_10simfcsfbd_decode(__pyx_self, __pyx_v_data, __pyx_v_bins_out, __pyx_v_times_out, __pyx_v_markers_out, __pyx_v_windows, __pyx_v_pdiv, __pyx_v_harmonics, __pyx_v_decoder_table, __pyx_v_tcc_mask, __pyx_v_tcc_shr, __pyx_v_pcc_mask, __pyx_v_pcc_shr, __pyx_v_marker_mask, __pyx_v_marker_shr, __pyx_v_win_mask, __pyx_v_win_shr);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_8simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint16_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint16_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint16_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint16_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_10simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint16_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint16_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint16_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint16_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr) {
   int __pyx_v_maxwindex;
   Py_ssize_t __pyx_v_maxmarker;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannel;
   Py_ssize_t __pyx_v_datasize;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_c;
@@ -5264,17 +5319,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_decoder_table, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1_0__pyx_pw_8lfdfiles_9_lfdfiles_11simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1_0__pyx_mdef_8lfdfiles_9_lfdfiles_11simfcsfbd_decode = {"__pyx_fuse_1_0simfcsfbd_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_0__pyx_pw_8lfdfiles_9_lfdfiles_11simfcsfbd_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_simfcsfbd_decode};
-static PyObject *__pyx_fuse_1_0__pyx_pw_8lfdfiles_9_lfdfiles_11simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1_0__pyx_pw_8lfdfiles_9_lfdfiles_13simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1_0__pyx_mdef_8lfdfiles_9_lfdfiles_13simfcsfbd_decode = {"__pyx_fuse_1_0simfcsfbd_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_0__pyx_pw_8lfdfiles_9_lfdfiles_13simfcsfbd_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_simfcsfbd_decode};
+static PyObject *__pyx_fuse_1_0__pyx_pw_8lfdfiles_9_lfdfiles_13simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_data = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_bins_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_times_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_markers_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_v_windows;
   int __pyx_v_pdiv;
   int __pyx_v_harmonics;
@@ -5475,22 +5530,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("simfcsfbd_decode", 1, 16, 16, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 67, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lfdfiles._lfdfiles.simfcsfbd_decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_10simfcsfbd_decode(__pyx_self, __pyx_v_data, __pyx_v_bins_out, __pyx_v_times_out, __pyx_v_markers_out, __pyx_v_windows, __pyx_v_pdiv, __pyx_v_harmonics, __pyx_v_decoder_table, __pyx_v_tcc_mask, __pyx_v_tcc_shr, __pyx_v_pcc_mask, __pyx_v_pcc_shr, __pyx_v_marker_mask, __pyx_v_marker_shr, __pyx_v_win_mask, __pyx_v_win_shr);
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_12simfcsfbd_decode(__pyx_self, __pyx_v_data, __pyx_v_bins_out, __pyx_v_times_out, __pyx_v_markers_out, __pyx_v_windows, __pyx_v_pdiv, __pyx_v_harmonics, __pyx_v_decoder_table, __pyx_v_tcc_mask, __pyx_v_tcc_shr, __pyx_v_pcc_mask, __pyx_v_pcc_shr, __pyx_v_marker_mask, __pyx_v_marker_shr, __pyx_v_win_mask, __pyx_v_win_shr);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_10simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint32_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint32_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint32_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint32_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_12simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint32_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint32_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint32_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint32_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr) {
   int __pyx_v_maxwindex;
   Py_ssize_t __pyx_v_maxmarker;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannel;
   Py_ssize_t __pyx_v_datasize;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_c;
@@ -6175,17 +6230,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_decoder_table, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1_1__pyx_pw_8lfdfiles_9_lfdfiles_13simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1_1__pyx_mdef_8lfdfiles_9_lfdfiles_13simfcsfbd_decode = {"__pyx_fuse_1_1simfcsfbd_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_1__pyx_pw_8lfdfiles_9_lfdfiles_13simfcsfbd_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_simfcsfbd_decode};
-static PyObject *__pyx_fuse_1_1__pyx_pw_8lfdfiles_9_lfdfiles_13simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1_1__pyx_pw_8lfdfiles_9_lfdfiles_15simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1_1__pyx_mdef_8lfdfiles_9_lfdfiles_15simfcsfbd_decode = {"__pyx_fuse_1_1simfcsfbd_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1_1__pyx_pw_8lfdfiles_9_lfdfiles_15simfcsfbd_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_simfcsfbd_decode};
+static PyObject *__pyx_fuse_1_1__pyx_pw_8lfdfiles_9_lfdfiles_15simfcsfbd_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_data = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_bins_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_times_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_markers_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_v_windows;
   int __pyx_v_pdiv;
   int __pyx_v_harmonics;
@@ -6386,22 +6441,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("simfcsfbd_decode", 1, 16, 16, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 67, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lfdfiles._lfdfiles.simfcsfbd_decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_12simfcsfbd_decode(__pyx_self, __pyx_v_data, __pyx_v_bins_out, __pyx_v_times_out, __pyx_v_markers_out, __pyx_v_windows, __pyx_v_pdiv, __pyx_v_harmonics, __pyx_v_decoder_table, __pyx_v_tcc_mask, __pyx_v_tcc_shr, __pyx_v_pcc_mask, __pyx_v_pcc_shr, __pyx_v_marker_mask, __pyx_v_marker_shr, __pyx_v_win_mask, __pyx_v_win_shr);
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_14simfcsfbd_decode(__pyx_self, __pyx_v_data, __pyx_v_bins_out, __pyx_v_times_out, __pyx_v_markers_out, __pyx_v_windows, __pyx_v_pdiv, __pyx_v_harmonics, __pyx_v_decoder_table, __pyx_v_tcc_mask, __pyx_v_tcc_shr, __pyx_v_pcc_mask, __pyx_v_pcc_shr, __pyx_v_marker_mask, __pyx_v_marker_shr, __pyx_v_win_mask, __pyx_v_win_shr);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_12simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint32_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint32_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint32_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint32_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_14simfcsfbd_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_bins_out, __Pyx_memviewslice __pyx_v_times_out, __Pyx_memviewslice __pyx_v_markers_out, int __pyx_v_windows, int __pyx_v_pdiv, int __pyx_v_harmonics, __Pyx_memviewslice __pyx_v_decoder_table, uint32_t __pyx_v_tcc_mask, uint32_t __pyx_v_tcc_shr, uint32_t __pyx_v_pcc_mask, uint32_t __pyx_v_pcc_shr, uint32_t __pyx_v_marker_mask, CYTHON_UNUSED uint32_t __pyx_v_marker_shr, uint32_t __pyx_v_win_mask, uint32_t __pyx_v_win_shr) {
   int __pyx_v_maxwindex;
   Py_ssize_t __pyx_v_maxmarker;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannel;
   Py_ssize_t __pyx_v_datasize;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_c;
@@ -7641,17 +7696,17 @@
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_17simfcsfbd_histogram(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0__pyx_mdef_8lfdfiles_9_lfdfiles_17simfcsfbd_histogram = {"__pyx_fuse_0simfcsfbd_histogram", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_17simfcsfbd_histogram, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_2simfcsfbd_histogram};
-static PyObject *__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_17simfcsfbd_histogram(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0__pyx_mdef_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram = {"__pyx_fuse_0simfcsfbd_histogram", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_2simfcsfbd_histogram};
+static PyObject *__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_bins = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_times = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_v_frame_markers = 0;
   double __pyx_v_units_per_sample;
   double __pyx_v_scanner_frame_start;
   __Pyx_memviewslice __pyx_v_hist_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
@@ -7742,22 +7797,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("simfcsfbd_histogram", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 191, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lfdfiles._lfdfiles.simfcsfbd_histogram", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_16simfcsfbd_histogram(__pyx_self, __pyx_v_bins, __pyx_v_times, __pyx_v_frame_markers, __pyx_v_units_per_sample, __pyx_v_scanner_frame_start, __pyx_v_hist_out);
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_18simfcsfbd_histogram(__pyx_self, __pyx_v_bins, __pyx_v_times, __pyx_v_frame_markers, __pyx_v_units_per_sample, __pyx_v_scanner_frame_start, __pyx_v_hist_out);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_16simfcsfbd_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_18simfcsfbd_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out) {
   Py_ssize_t __pyx_v_nframes;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannels;
   Py_ssize_t __pyx_v_framelen;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nwindows;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_k;
@@ -8232,17 +8287,17 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_hist_out, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1__pyx_mdef_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram = {"__pyx_fuse_1simfcsfbd_histogram", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_2simfcsfbd_histogram};
-static PyObject *__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_21simfcsfbd_histogram(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1__pyx_mdef_8lfdfiles_9_lfdfiles_21simfcsfbd_histogram = {"__pyx_fuse_1simfcsfbd_histogram", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_21simfcsfbd_histogram, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_2simfcsfbd_histogram};
+static PyObject *__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_21simfcsfbd_histogram(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_bins = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_times = { 0, 0, { 0 }, { 0 }, { 0 } };
   PyObject *__pyx_v_frame_markers = 0;
   double __pyx_v_units_per_sample;
   double __pyx_v_scanner_frame_start;
   __Pyx_memviewslice __pyx_v_hist_out = { 0, 0, { 0 }, { 0 }, { 0 } };
   int __pyx_lineno = 0;
@@ -8333,22 +8388,22 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("simfcsfbd_histogram", 1, 6, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 191, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lfdfiles._lfdfiles.simfcsfbd_histogram", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_18simfcsfbd_histogram(__pyx_self, __pyx_v_bins, __pyx_v_times, __pyx_v_frame_markers, __pyx_v_units_per_sample, __pyx_v_scanner_frame_start, __pyx_v_hist_out);
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_20simfcsfbd_histogram(__pyx_self, __pyx_v_bins, __pyx_v_times, __pyx_v_frame_markers, __pyx_v_units_per_sample, __pyx_v_scanner_frame_start, __pyx_v_hist_out);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_18simfcsfbd_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_20simfcsfbd_histogram(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_bins, __Pyx_memviewslice __pyx_v_times, PyObject *__pyx_v_frame_markers, double __pyx_v_units_per_sample, double __pyx_v_scanner_frame_start, __Pyx_memviewslice __pyx_v_hist_out) {
   Py_ssize_t __pyx_v_nframes;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nchannels;
   Py_ssize_t __pyx_v_framelen;
   CYTHON_UNUSED Py_ssize_t __pyx_v_nwindows;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_j;
   Py_ssize_t __pyx_v_k;
@@ -9378,15 +9433,15 @@
   __Pyx_XDECREF(__pyx_v_dst_type);
   __Pyx_XDECREF(__pyx_v_kwargs);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_32__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_34__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
@@ -9434,17 +9489,17 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_23sflim_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_0__pyx_mdef_8lfdfiles_9_lfdfiles_23sflim_decode = {"__pyx_fuse_0sflim_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_23sflim_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_4sflim_decode};
-static PyObject *__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_23sflim_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_25sflim_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_0__pyx_mdef_8lfdfiles_9_lfdfiles_25sflim_decode = {"__pyx_fuse_0sflim_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_25sflim_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_4sflim_decode};
+static PyObject *__pyx_fuse_0__pyx_pw_8lfdfiles_9_lfdfiles_25sflim_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_data = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sflim = { 0, 0, { 0 }, { 0 }, { 0 } };
   uint64_t __pyx_v_pixeltime;
   uint64_t __pyx_v_enabletime;
   Py_ssize_t __pyx_v_maxframes;
   int __pyx_v_numthreads;
   int __pyx_lineno = 0;
@@ -9553,26 +9608,26 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("sflim_decode", 0, 3, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 274, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lfdfiles._lfdfiles.sflim_decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_22sflim_decode(__pyx_self, __pyx_v_data, __pyx_v_sflim, __pyx_v_pixeltime, __pyx_v_enabletime, __pyx_v_maxframes, __pyx_v_numthreads);
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_24sflim_decode(__pyx_self, __pyx_v_data, __pyx_v_sflim, __pyx_v_pixeltime, __pyx_v_enabletime, __pyx_v_maxframes, __pyx_v_numthreads);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_22sflim_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes, int __pyx_v_numthreads) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_24sflim_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes, int __pyx_v_numthreads) {
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_v_address;
   omp_lock_t __pyx_v_lock;
-  int __pyx_v_ret;
+  Py_ssize_t __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
@@ -9607,15 +9662,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = PyInt_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_size = __pyx_t_3;
 
   /* "lfdfiles/_lfdfiles.pyx":328
- *         int ret
+ *         ssize_t ret
  * 
  *     if size == 0:             # <<<<<<<<<<<<<<
  *         return
  *     if sflim.shape[0] != 32 or sflim.shape[1] != 256:
  */
   __pyx_t_4 = ((__pyx_v_size == 0) != 0);
   if (__pyx_t_4) {
@@ -9628,15 +9683,15 @@
  *         raise ValueError(
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
     /* "lfdfiles/_lfdfiles.pyx":328
- *         int ret
+ *         ssize_t ret
  * 
  *     if size == 0:             # <<<<<<<<<<<<<<
  *         return
  *     if sflim.shape[0] != 32 or sflim.shape[1] != 256:
  */
   }
 
@@ -9802,15 +9857,15 @@
  *             for address in prange(8):             # <<<<<<<<<<<<<<
  *                 ret = _decode_address(
  *                     address,
  */
                   if ((1 == 0)) abort();
                   {
                       Py_ssize_t __pyx_parallel_temp0 = ((Py_ssize_t)0xbad0bad0);
-                      int __pyx_parallel_temp1 = ((int)0xbad0bad0);
+                      Py_ssize_t __pyx_parallel_temp1 = ((Py_ssize_t)0xbad0bad0);
                       const char *__pyx_parallel_filename = NULL; int __pyx_parallel_lineno = 0, __pyx_parallel_clineno = 0;
                       PyObject *__pyx_parallel_exc_type = NULL, *__pyx_parallel_exc_value = NULL, *__pyx_parallel_exc_tb = NULL;
                       int __pyx_parallel_why;
                       __pyx_parallel_why = 0;
                       __pyx_t_9 = (8 - 0 + 1 - 1/abs(1)) / 1;
                       if (__pyx_t_9 > 0)
                       {
@@ -9818,15 +9873,15 @@
                           #pragma omp for firstprivate(__pyx_v_address) lastprivate(__pyx_v_address) lastprivate(__pyx_v_ret)
                           #endif /* _OPENMP */
                           for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_9; __pyx_t_3++){
                               if (__pyx_parallel_why < 2)
                               {
                                   __pyx_v_address = (Py_ssize_t)(0 + 1 * __pyx_t_3);
                                   /* Initialize private variables to invalid values */
-                                  __pyx_v_ret = ((int)0xbad0bad0);
+                                  __pyx_v_ret = ((Py_ssize_t)0xbad0bad0);
 
                                   /* "lfdfiles/_lfdfiles.pyx":343
  *         with nogil, parallel(num_threads=numthreads):
  *             for address in prange(8):
  *                 ret = _decode_address(             # <<<<<<<<<<<<<<
  *                     address,
  *                     data,
@@ -10136,15 +10191,15 @@
   __PYX_XDEC_MEMVIEW(&__pyx_v_data, 1);
   __PYX_XDEC_MEMVIEW(&__pyx_v_sflim, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_34__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_36__defaults__(CYTHON_UNUSED PyObject *__pyx_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
   int __pyx_lineno = 0;
@@ -10192,17 +10247,17 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static PyObject *__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_25sflim_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static PyMethodDef __pyx_fuse_1__pyx_mdef_8lfdfiles_9_lfdfiles_25sflim_decode = {"__pyx_fuse_1sflim_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_25sflim_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_4sflim_decode};
-static PyObject *__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_25sflim_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static PyObject *__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_27sflim_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_fuse_1__pyx_mdef_8lfdfiles_9_lfdfiles_27sflim_decode = {"__pyx_fuse_1sflim_decode", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_27sflim_decode, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_4sflim_decode};
+static PyObject *__pyx_fuse_1__pyx_pw_8lfdfiles_9_lfdfiles_27sflim_decode(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   __Pyx_memviewslice __pyx_v_data = { 0, 0, { 0 }, { 0 }, { 0 } };
   __Pyx_memviewslice __pyx_v_sflim = { 0, 0, { 0 }, { 0 }, { 0 } };
   uint64_t __pyx_v_pixeltime;
   uint64_t __pyx_v_enabletime;
   Py_ssize_t __pyx_v_maxframes;
   int __pyx_v_numthreads;
   int __pyx_lineno = 0;
@@ -10311,26 +10366,26 @@
   __pyx_L5_argtuple_error:;
   __Pyx_RaiseArgtupleInvalid("sflim_decode", 0, 3, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 274, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("lfdfiles._lfdfiles.sflim_decode", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_24sflim_decode(__pyx_self, __pyx_v_data, __pyx_v_sflim, __pyx_v_pixeltime, __pyx_v_enabletime, __pyx_v_maxframes, __pyx_v_numthreads);
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_26sflim_decode(__pyx_self, __pyx_v_data, __pyx_v_sflim, __pyx_v_pixeltime, __pyx_v_enabletime, __pyx_v_maxframes, __pyx_v_numthreads);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_24sflim_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes, int __pyx_v_numthreads) {
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_26sflim_decode(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes, int __pyx_v_numthreads) {
   Py_ssize_t __pyx_v_size;
   Py_ssize_t __pyx_v_address;
   omp_lock_t __pyx_v_lock;
-  int __pyx_v_ret;
+  Py_ssize_t __pyx_v_ret;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   Py_ssize_t __pyx_t_3;
   int __pyx_t_4;
   int __pyx_t_5;
@@ -10365,15 +10420,15 @@
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = PyInt_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 323, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __pyx_v_size = __pyx_t_3;
 
   /* "lfdfiles/_lfdfiles.pyx":328
- *         int ret
+ *         ssize_t ret
  * 
  *     if size == 0:             # <<<<<<<<<<<<<<
  *         return
  *     if sflim.shape[0] != 32 or sflim.shape[1] != 256:
  */
   __pyx_t_4 = ((__pyx_v_size == 0) != 0);
   if (__pyx_t_4) {
@@ -10386,15 +10441,15 @@
  *         raise ValueError(
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
     /* "lfdfiles/_lfdfiles.pyx":328
- *         int ret
+ *         ssize_t ret
  * 
  *     if size == 0:             # <<<<<<<<<<<<<<
  *         return
  *     if sflim.shape[0] != 32 or sflim.shape[1] != 256:
  */
   }
 
@@ -10560,15 +10615,15 @@
  *             for address in prange(8):             # <<<<<<<<<<<<<<
  *                 ret = _decode_address(
  *                     address,
  */
                   if ((1 == 0)) abort();
                   {
                       Py_ssize_t __pyx_parallel_temp0 = ((Py_ssize_t)0xbad0bad0);
-                      int __pyx_parallel_temp1 = ((int)0xbad0bad0);
+                      Py_ssize_t __pyx_parallel_temp1 = ((Py_ssize_t)0xbad0bad0);
                       const char *__pyx_parallel_filename = NULL; int __pyx_parallel_lineno = 0, __pyx_parallel_clineno = 0;
                       PyObject *__pyx_parallel_exc_type = NULL, *__pyx_parallel_exc_value = NULL, *__pyx_parallel_exc_tb = NULL;
                       int __pyx_parallel_why;
                       __pyx_parallel_why = 0;
                       __pyx_t_9 = (8 - 0 + 1 - 1/abs(1)) / 1;
                       if (__pyx_t_9 > 0)
                       {
@@ -10576,15 +10631,15 @@
                           #pragma omp for firstprivate(__pyx_v_address) lastprivate(__pyx_v_address) lastprivate(__pyx_v_ret)
                           #endif /* _OPENMP */
                           for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_9; __pyx_t_3++){
                               if (__pyx_parallel_why < 2)
                               {
                                   __pyx_v_address = (Py_ssize_t)(0 + 1 * __pyx_t_3);
                                   /* Initialize private variables to invalid values */
-                                  __pyx_v_ret = ((int)0xbad0bad0);
+                                  __pyx_v_ret = ((Py_ssize_t)0xbad0bad0);
 
                                   /* "lfdfiles/_lfdfiles.pyx":343
  *         with nogil, parallel(num_threads=numthreads):
  *             for address in prange(8):
  *                 ret = _decode_address(             # <<<<<<<<<<<<<<
  *                     address,
  *                     data,
@@ -10897,20 +10952,20 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "lfdfiles/_lfdfiles.pyx":362
  * 
  * 
- * cdef int _decode_address(             # <<<<<<<<<<<<<<
+ * cdef ssize_t _decode_address(             # <<<<<<<<<<<<<<
  *     const ssize_t address,
  *     const uint32_t[::1] data,
  */
 
-static int __pyx_fuse_0__pyx_f_8lfdfiles_9_lfdfiles__decode_address(Py_ssize_t const __pyx_v_address, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, Py_ssize_t const __pyx_v_size, uint64_t const __pyx_v_pixeltime, uint64_t const __pyx_v_enabletime, Py_ssize_t const __pyx_v_maxframes, omp_lock_t __pyx_v_lock) {
+static Py_ssize_t __pyx_fuse_0__pyx_f_8lfdfiles_9_lfdfiles__decode_address(Py_ssize_t const __pyx_v_address, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, Py_ssize_t const __pyx_v_size, uint64_t const __pyx_v_pixeltime, uint64_t const __pyx_v_enabletime, Py_ssize_t const __pyx_v_maxframes, omp_lock_t __pyx_v_lock) {
   Py_ssize_t __pyx_v_width;
   Py_ssize_t __pyx_v_height;
   Py_ssize_t __pyx_v_framesize;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_c;
   Py_ssize_t __pyx_v_h;
   Py_ssize_t __pyx_v_y;
@@ -10922,15 +10977,15 @@
   uint64_t __pyx_v_macrotime0;
   uint32_t __pyx_v_d;
   uint32_t __pyx_v_pcc;
   uint32_t __pyx_v_tcc;
   uint32_t __pyx_v_tcc0;
   uint32_t __pyx_v_enable;
   uint32_t __pyx_v_ph;
-  int __pyx_r;
+  Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
@@ -11028,15 +11083,15 @@
     /* "lfdfiles/_lfdfiles.pyx":388
  *             break
  *     else:
  *         return -1             # <<<<<<<<<<<<<<
  * 
  *     tcc0 = data[start] & <uint32_t> MASK_TCC
  */
-    __pyx_r = -1;
+    __pyx_r = -1L;
     goto __pyx_L0;
   }
   __pyx_L4_break:;
 
   /* "lfdfiles/_lfdfiles.pyx":390
  *         return -1
  * 
@@ -11607,15 +11662,15 @@
       *((uint8_t *) ( /* dim=3 */ ((char *) (((uint8_t *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_sflim.data + __pyx_t_9 * __pyx_v_sflim.strides[0]) ) + __pyx_t_8 * __pyx_v_sflim.strides[1]) ) + __pyx_t_7 * __pyx_v_sflim.strides[2]) )) + __pyx_t_4)) )) += 1;
 
       /* "lfdfiles/_lfdfiles.pyx":455
  *             openmp.omp_set_lock(&lock)
  *             sflim[c, h, y, x] += 1
  *             openmp.omp_unset_lock(&lock)             # <<<<<<<<<<<<<<
  * 
- *     return <int> frames
+ *     return frames
  */
       omp_unset_lock((&__pyx_v_lock));
 
       /* "lfdfiles/_lfdfiles.pyx":450
  * 
  *         ph = (d & <uint32_t> MASK_PH3) >> SHR_PH3
  *         if ph:             # <<<<<<<<<<<<<<
@@ -11626,33 +11681,35 @@
     __pyx_L6_continue:;
   }
   __pyx_L7_break:;
 
   /* "lfdfiles/_lfdfiles.pyx":457
  *             openmp.omp_unset_lock(&lock)
  * 
- *     return <int> frames             # <<<<<<<<<<<<<<
+ *     return frames             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
-  __pyx_r = ((int)__pyx_v_frames);
+  __pyx_r = __pyx_v_frames;
   goto __pyx_L0;
 
   /* "lfdfiles/_lfdfiles.pyx":362
  * 
  * 
- * cdef int _decode_address(             # <<<<<<<<<<<<<<
+ * cdef ssize_t _decode_address(             # <<<<<<<<<<<<<<
  *     const ssize_t address,
  *     const uint32_t[::1] data,
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-static int __pyx_fuse_1__pyx_f_8lfdfiles_9_lfdfiles__decode_address(Py_ssize_t const __pyx_v_address, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, Py_ssize_t const __pyx_v_size, uint64_t const __pyx_v_pixeltime, uint64_t const __pyx_v_enabletime, Py_ssize_t const __pyx_v_maxframes, omp_lock_t __pyx_v_lock) {
+static Py_ssize_t __pyx_fuse_1__pyx_f_8lfdfiles_9_lfdfiles__decode_address(Py_ssize_t const __pyx_v_address, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_sflim, Py_ssize_t const __pyx_v_size, uint64_t const __pyx_v_pixeltime, uint64_t const __pyx_v_enabletime, Py_ssize_t const __pyx_v_maxframes, omp_lock_t __pyx_v_lock) {
   Py_ssize_t __pyx_v_width;
   Py_ssize_t __pyx_v_height;
   Py_ssize_t __pyx_v_framesize;
   Py_ssize_t __pyx_v_i;
   Py_ssize_t __pyx_v_c;
   Py_ssize_t __pyx_v_h;
   Py_ssize_t __pyx_v_y;
@@ -11664,15 +11721,15 @@
   uint64_t __pyx_v_macrotime0;
   uint32_t __pyx_v_d;
   uint32_t __pyx_v_pcc;
   uint32_t __pyx_v_tcc;
   uint32_t __pyx_v_tcc0;
   uint32_t __pyx_v_enable;
   uint32_t __pyx_v_ph;
-  int __pyx_r;
+  Py_ssize_t __pyx_r;
   Py_ssize_t __pyx_t_1;
   Py_ssize_t __pyx_t_2;
   Py_ssize_t __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
   int __pyx_t_6;
   Py_ssize_t __pyx_t_7;
@@ -11770,15 +11827,15 @@
     /* "lfdfiles/_lfdfiles.pyx":388
  *             break
  *     else:
  *         return -1             # <<<<<<<<<<<<<<
  * 
  *     tcc0 = data[start] & <uint32_t> MASK_TCC
  */
-    __pyx_r = -1;
+    __pyx_r = -1L;
     goto __pyx_L0;
   }
   __pyx_L4_break:;
 
   /* "lfdfiles/_lfdfiles.pyx":390
  *         return -1
  * 
@@ -12349,15 +12406,15 @@
       *((uint16_t *) ( /* dim=3 */ ((char *) (((uint16_t *) ( /* dim=2 */ (( /* dim=1 */ (( /* dim=0 */ (__pyx_v_sflim.data + __pyx_t_9 * __pyx_v_sflim.strides[0]) ) + __pyx_t_8 * __pyx_v_sflim.strides[1]) ) + __pyx_t_7 * __pyx_v_sflim.strides[2]) )) + __pyx_t_4)) )) += 1;
 
       /* "lfdfiles/_lfdfiles.pyx":455
  *             openmp.omp_set_lock(&lock)
  *             sflim[c, h, y, x] += 1
  *             openmp.omp_unset_lock(&lock)             # <<<<<<<<<<<<<<
  * 
- *     return <int> frames
+ *     return frames
  */
       omp_unset_lock((&__pyx_v_lock));
 
       /* "lfdfiles/_lfdfiles.pyx":450
  * 
  *         ph = (d & <uint32_t> MASK_PH3) >> SHR_PH3
  *         if ph:             # <<<<<<<<<<<<<<
@@ -12368,23 +12425,1574 @@
     __pyx_L6_continue:;
   }
   __pyx_L7_break:;
 
   /* "lfdfiles/_lfdfiles.pyx":457
  *             openmp.omp_unset_lock(&lock)
  * 
- *     return <int> frames             # <<<<<<<<<<<<<<
+ *     return frames             # <<<<<<<<<<<<<<
+ * 
+ * 
  */
-  __pyx_r = ((int)__pyx_v_frames);
+  __pyx_r = __pyx_v_frames;
   goto __pyx_L0;
 
   /* "lfdfiles/_lfdfiles.pyx":362
  * 
  * 
- * cdef int _decode_address(             # <<<<<<<<<<<<<<
+ * cdef ssize_t _decode_address(             # <<<<<<<<<<<<<<
+ *     const ssize_t address,
+ *     const uint32_t[::1] data,
+ */
+
+  /* function exit code */
+  __pyx_L0:;
+  return __pyx_r;
+}
+
+/* "lfdfiles/_lfdfiles.pyx":460
+ * 
+ * 
+ * def sflim_decode_photons(             # <<<<<<<<<<<<<<
+ *     const uint32_t[::1] data,
+ *     uint16_t[:, ::1] photons,
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_8lfdfiles_9_lfdfiles_7sflim_decode_photons(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_8lfdfiles_9_lfdfiles_6sflim_decode_photons[] = "Decode Kintex FLIMbox data to SLIM photon array.\n\n    This function is private and may change or be removed in future versions.\n\n    Parameters:\n        data (numpy.ndarray):\n            Data stream from Kintex FLIMbox. A `uint32` array.\n        photons (numpy.ndarray):\n            `uint16` array of shape `(number of photons, 5)`,\n            where arrival time, frame, channel, y and x position are stored for\n            each photon.\n        frameshape (tuple):\n            Shape of image frame.\n        pixeltime (int):\n            Pixel dwell time in FLIMbox units.\n            ``math.ceil(dwelltime * 256 / 255 * frequency_factor * frequency)``\n        enabletime (int):\n            Time in FLIMbox units to wait after detecting enable bit before\n            detecting next enable bit.\n        maxframes (int):\n            Maximum number of image frames to decode.\n\n    Returns:\n        Number of photons decoded.\n\n    Examples:\n        >>> import numpy, math\n        >>> from lfdfiles._lfdfiles import sflim_decode_photons\n        >>> data = numpy.fromfile(\n        ...     '20210123488_100x_NSC_166_TMRM_4_zoom4000_L115.bin',\n        ...      dtype=numpy.uint32\n        ... )\n        >>> frequency = 78e6\n        >>> frequency_factor = 0.9976\n        >>> dwelltime = 16e-6\n        >>> pixeltime = math.ceil(\n        ...     dwelltime * 256 / 255 * frequency_factor * frequency\n        ... )\n        >>> photons = numpy.zeros((2035488, 5), dtype=numpy.uint6)\n        >>> sflim_decode_photons(\n        ...     data, photons, (256, 342), pixeltime=pixeltime, maxframes=20\n        ... )\n        2035488\n        >>> photons[12345].tolist()\n        [205, 3, 2, 181, 51]\n\n    ";
+static PyMethodDef __pyx_mdef_8lfdfiles_9_lfdfiles_7sflim_decode_photons = {"sflim_decode_photons", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_8lfdfiles_9_lfdfiles_7sflim_decode_photons, METH_VARARGS|METH_KEYWORDS, __pyx_doc_8lfdfiles_9_lfdfiles_6sflim_decode_photons};
+static PyObject *__pyx_pw_8lfdfiles_9_lfdfiles_7sflim_decode_photons(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  __Pyx_memviewslice __pyx_v_data = { 0, 0, { 0 }, { 0 }, { 0 } };
+  __Pyx_memviewslice __pyx_v_photons = { 0, 0, { 0 }, { 0 }, { 0 } };
+  PyObject *__pyx_v_frameshape = 0;
+  uint64_t __pyx_v_pixeltime;
+  uint64_t __pyx_v_enabletime;
+  Py_ssize_t __pyx_v_maxframes;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("sflim_decode_photons (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_data,&__pyx_n_s_photons,&__pyx_n_s_frameshape,&__pyx_n_s_pixeltime,&__pyx_n_s_enabletime,&__pyx_n_s_maxframes,0};
+    PyObject* values[6] = {0,0,0,0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        CYTHON_FALLTHROUGH;
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_data)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_photons)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("sflim_decode_photons", 0, 4, 6, 1); __PYX_ERR(0, 460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_frameshape)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("sflim_decode_photons", 0, 4, 6, 2); __PYX_ERR(0, 460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  3:
+        if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pixeltime)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("sflim_decode_photons", 0, 4, 6, 3); __PYX_ERR(0, 460, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  4:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_enabletime);
+          if (value) { values[4] = value; kw_args--; }
+        }
+        CYTHON_FALLTHROUGH;
+        case  5:
+        if (kw_args > 0) {
+          PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_maxframes);
+          if (value) { values[5] = value; kw_args--; }
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "sflim_decode_photons") < 0)) __PYX_ERR(0, 460, __pyx_L3_error)
+      }
+    } else {
+      switch (PyTuple_GET_SIZE(__pyx_args)) {
+        case  6: values[5] = PyTuple_GET_ITEM(__pyx_args, 5);
+        CYTHON_FALLTHROUGH;
+        case  5: values[4] = PyTuple_GET_ITEM(__pyx_args, 4);
+        CYTHON_FALLTHROUGH;
+        case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
+        values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+    }
+    __pyx_v_data = __Pyx_PyObject_to_MemoryviewSlice_dc_nn_uint32_t__const__(values[0], 0); if (unlikely(!__pyx_v_data.memview)) __PYX_ERR(0, 461, __pyx_L3_error)
+    __pyx_v_photons = __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn_uint16_t(values[1], PyBUF_WRITABLE); if (unlikely(!__pyx_v_photons.memview)) __PYX_ERR(0, 462, __pyx_L3_error)
+    __pyx_v_frameshape = values[2];
+    __pyx_v_pixeltime = __Pyx_PyInt_As_uint64_t(values[3]); if (unlikely((__pyx_v_pixeltime == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 464, __pyx_L3_error)
+    if (values[4]) {
+      __pyx_v_enabletime = __Pyx_PyInt_As_uint64_t(values[4]); if (unlikely((__pyx_v_enabletime == ((uint64_t)-1)) && PyErr_Occurred())) __PYX_ERR(0, 465, __pyx_L3_error)
+    } else {
+      __pyx_v_enabletime = ((uint64_t)0);
+    }
+    if (values[5]) {
+      __pyx_v_maxframes = PyInt_AsSsize_t(values[5]); if (unlikely((__pyx_v_maxframes == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 466, __pyx_L3_error)
+    } else {
+      __pyx_v_maxframes = ((Py_ssize_t)-1L);
+    }
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("sflim_decode_photons", 0, 4, 6, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 460, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("lfdfiles._lfdfiles.sflim_decode_photons", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  __pyx_r = __pyx_pf_8lfdfiles_9_lfdfiles_6sflim_decode_photons(__pyx_self, __pyx_v_data, __pyx_v_photons, __pyx_v_frameshape, __pyx_v_pixeltime, __pyx_v_enabletime, __pyx_v_maxframes);
+
+  /* function exit code */
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_8lfdfiles_9_lfdfiles_6sflim_decode_photons(CYTHON_UNUSED PyObject *__pyx_self, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_photons, PyObject *__pyx_v_frameshape, uint64_t __pyx_v_pixeltime, uint64_t __pyx_v_enabletime, Py_ssize_t __pyx_v_maxframes) {
+  Py_ssize_t __pyx_v_size;
+  Py_ssize_t __pyx_v_ret;
+  Py_ssize_t __pyx_v_height;
+  Py_ssize_t __pyx_v_width;
+  Py_ssize_t __pyx_v_address;
+  Py_ssize_t __pyx_v_np;
+  Py_ssize_t __pyx_v_maxphotons;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  Py_ssize_t __pyx_t_3;
+  int __pyx_t_4;
+  Py_ssize_t __pyx_t_5;
+  Py_UCS4 __pyx_t_6;
+  PyObject *__pyx_t_7 = NULL;
+  int __pyx_t_8;
+  __Pyx_memviewslice __pyx_t_9 = { 0, 0, { 0 }, { 0 }, { 0 } };
+  int __pyx_t_10;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("sflim_decode_photons", 0);
+
+  /* "lfdfiles/_lfdfiles.pyx":516
+ *     """
+ *     cdef:
+ *         ssize_t size = data.size             # <<<<<<<<<<<<<<
+ *         ssize_t ret, height, width, address, np
+ *         ssize_t maxphotons = photons.shape[0]
+ */
+  __pyx_t_1 = __pyx_memoryview_fromslice(__pyx_v_data, 1, (PyObject *(*)(char *)) __pyx_memview_get_nn_uint32_t__const__, (int (*)(char *, PyObject *)) NULL, 0);; if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_size); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_3 = PyInt_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 516, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_size = __pyx_t_3;
+
+  /* "lfdfiles/_lfdfiles.pyx":518
+ *         ssize_t size = data.size
+ *         ssize_t ret, height, width, address, np
+ *         ssize_t maxphotons = photons.shape[0]             # <<<<<<<<<<<<<<
+ * 
+ *     if size == 0:
+ */
+  __pyx_v_maxphotons = (__pyx_v_photons.shape[0]);
+
+  /* "lfdfiles/_lfdfiles.pyx":520
+ *         ssize_t maxphotons = photons.shape[0]
+ * 
+ *     if size == 0:             # <<<<<<<<<<<<<<
+ *         return
+ *     if photons.shape[1] != 5:
+ */
+  __pyx_t_4 = ((__pyx_v_size == 0) != 0);
+  if (__pyx_t_4) {
+
+    /* "lfdfiles/_lfdfiles.pyx":521
+ * 
+ *     if size == 0:
+ *         return             # <<<<<<<<<<<<<<
+ *     if photons.shape[1] != 5:
+ *         raise ValueError(f'invalid photons shape {photons.shape} != (-1, 5)')
+ */
+    __Pyx_XDECREF(__pyx_r);
+    __pyx_r = Py_None; __Pyx_INCREF(Py_None);
+    goto __pyx_L0;
+
+    /* "lfdfiles/_lfdfiles.pyx":520
+ *         ssize_t maxphotons = photons.shape[0]
+ * 
+ *     if size == 0:             # <<<<<<<<<<<<<<
+ *         return
+ *     if photons.shape[1] != 5:
+ */
+  }
+
+  /* "lfdfiles/_lfdfiles.pyx":522
+ *     if size == 0:
+ *         return
+ *     if photons.shape[1] != 5:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'invalid photons shape {photons.shape} != (-1, 5)')
+ * 
+ */
+  __pyx_t_4 = (((__pyx_v_photons.shape[1]) != 5) != 0);
+  if (unlikely(__pyx_t_4)) {
+
+    /* "lfdfiles/_lfdfiles.pyx":523
+ *         return
+ *     if photons.shape[1] != 5:
+ *         raise ValueError(f'invalid photons shape {photons.shape} != (-1, 5)')             # <<<<<<<<<<<<<<
+ * 
+ *     if len(frameshape) != 2 or frameshape[0] < 1 or frameshape[1] < 1:
+ */
+    __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_5 = 0;
+    __pyx_t_6 = 127;
+    __Pyx_INCREF(__pyx_kp_u_invalid_photons_shape);
+    __pyx_t_5 += 22;
+    __Pyx_GIVEREF(__pyx_kp_u_invalid_photons_shape);
+    PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_kp_u_invalid_photons_shape);
+    __pyx_t_1 = __Pyx_carray_to_py_Py_ssize_t(__pyx_v_photons.shape, 8); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_7 = __Pyx_PyObject_FormatSimple(__pyx_t_1, __pyx_empty_unicode); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __pyx_t_6 = (__Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) > __pyx_t_6) ? __Pyx_PyUnicode_MAX_CHAR_VALUE(__pyx_t_7) : __pyx_t_6;
+    __pyx_t_5 += __Pyx_PyUnicode_GET_LENGTH(__pyx_t_7);
+    __Pyx_GIVEREF(__pyx_t_7);
+    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_t_7);
+    __pyx_t_7 = 0;
+    __Pyx_INCREF(__pyx_kp_u_1_5);
+    __pyx_t_5 += 11;
+    __Pyx_GIVEREF(__pyx_kp_u_1_5);
+    PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_kp_u_1_5);
+    __pyx_t_7 = __Pyx_PyUnicode_Join(__pyx_t_2, 3, __pyx_t_5, __pyx_t_6); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 523, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 523, __pyx_L1_error)
+
+    /* "lfdfiles/_lfdfiles.pyx":522
+ *     if size == 0:
+ *         return
+ *     if photons.shape[1] != 5:             # <<<<<<<<<<<<<<
+ *         raise ValueError(f'invalid photons shape {photons.shape} != (-1, 5)')
+ * 
+ */
+  }
+
+  /* "lfdfiles/_lfdfiles.pyx":525
+ *         raise ValueError(f'invalid photons shape {photons.shape} != (-1, 5)')
+ * 
+ *     if len(frameshape) != 2 or frameshape[0] < 1 or frameshape[1] < 1:             # <<<<<<<<<<<<<<
+ *         raise ValueError('invalid frameshape')
+ * 
+ */
+  __pyx_t_5 = PyObject_Length(__pyx_v_frameshape); if (unlikely(__pyx_t_5 == ((Py_ssize_t)-1))) __PYX_ERR(0, 525, __pyx_L1_error)
+  __pyx_t_8 = ((__pyx_t_5 != 2) != 0);
+  if (!__pyx_t_8) {
+  } else {
+    __pyx_t_4 = __pyx_t_8;
+    goto __pyx_L6_bool_binop_done;
+  }
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_frameshape, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_7 = PyObject_RichCompare(__pyx_t_2, __pyx_int_1, Py_LT); __Pyx_XGOTREF(__pyx_t_7); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_7); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (!__pyx_t_8) {
+  } else {
+    __pyx_t_4 = __pyx_t_8;
+    goto __pyx_L6_bool_binop_done;
+  }
+  __pyx_t_7 = __Pyx_GetItemInt(__pyx_v_frameshape, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_7);
+  __pyx_t_2 = PyObject_RichCompare(__pyx_t_7, __pyx_int_1, Py_LT); __Pyx_XGOTREF(__pyx_t_2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+  __pyx_t_8 = __Pyx_PyObject_IsTrue(__pyx_t_2); if (unlikely(__pyx_t_8 < 0)) __PYX_ERR(0, 525, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_4 = __pyx_t_8;
+  __pyx_L6_bool_binop_done:;
+  if (unlikely(__pyx_t_4)) {
+
+    /* "lfdfiles/_lfdfiles.pyx":526
+ * 
+ *     if len(frameshape) != 2 or frameshape[0] < 1 or frameshape[1] < 1:
+ *         raise ValueError('invalid frameshape')             # <<<<<<<<<<<<<<
+ * 
+ *     height = frameshape[0]
+ */
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 526, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __PYX_ERR(0, 526, __pyx_L1_error)
+
+    /* "lfdfiles/_lfdfiles.pyx":525
+ *         raise ValueError(f'invalid photons shape {photons.shape} != (-1, 5)')
+ * 
+ *     if len(frameshape) != 2 or frameshape[0] < 1 or frameshape[1] < 1:             # <<<<<<<<<<<<<<
+ *         raise ValueError('invalid frameshape')
+ * 
+ */
+  }
+
+  /* "lfdfiles/_lfdfiles.pyx":528
+ *         raise ValueError('invalid frameshape')
+ * 
+ *     height = frameshape[0]             # <<<<<<<<<<<<<<
+ *     width = frameshape[1]
+ * 
+ */
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_frameshape, 0, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 528, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyInt_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 528, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_height = __pyx_t_3;
+
+  /* "lfdfiles/_lfdfiles.pyx":529
+ * 
+ *     height = frameshape[0]
+ *     width = frameshape[1]             # <<<<<<<<<<<<<<
+ * 
+ *     if enabletime == 0:
+ */
+  __pyx_t_2 = __Pyx_GetItemInt(__pyx_v_frameshape, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 529, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_3 = PyInt_AsSsize_t(__pyx_t_2); if (unlikely((__pyx_t_3 == (Py_ssize_t)-1) && PyErr_Occurred())) __PYX_ERR(0, 529, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_width = __pyx_t_3;
+
+  /* "lfdfiles/_lfdfiles.pyx":531
+ *     width = frameshape[1]
+ * 
+ *     if enabletime == 0:             # <<<<<<<<<<<<<<
+ *         enabletime = pixeltime * width
+ * 
+ */
+  __pyx_t_4 = ((__pyx_v_enabletime == 0) != 0);
+  if (__pyx_t_4) {
+
+    /* "lfdfiles/_lfdfiles.pyx":532
+ * 
+ *     if enabletime == 0:
+ *         enabletime = pixeltime * width             # <<<<<<<<<<<<<<
+ * 
+ *     with nogil:
+ */
+    __pyx_v_enabletime = (__pyx_v_pixeltime * __pyx_v_width);
+
+    /* "lfdfiles/_lfdfiles.pyx":531
+ *     width = frameshape[1]
+ * 
+ *     if enabletime == 0:             # <<<<<<<<<<<<<<
+ *         enabletime = pixeltime * width
+ * 
+ */
+  }
+
+  /* "lfdfiles/_lfdfiles.pyx":534
+ *         enabletime = pixeltime * width
+ * 
+ *     with nogil:             # <<<<<<<<<<<<<<
+ *         np = 0
+ *         for address in range(8):
+ */
+  {
+      #ifdef WITH_THREAD
+      PyThreadState *_save;
+      Py_UNBLOCK_THREADS
+      __Pyx_FastGIL_Remember();
+      #endif
+      /*try:*/ {
+
+        /* "lfdfiles/_lfdfiles.pyx":535
+ * 
+ *     with nogil:
+ *         np = 0             # <<<<<<<<<<<<<<
+ *         for address in range(8):
+ *             ret = _decode_address_photons(
+ */
+        __pyx_v_np = 0;
+
+        /* "lfdfiles/_lfdfiles.pyx":536
+ *     with nogil:
+ *         np = 0
+ *         for address in range(8):             # <<<<<<<<<<<<<<
+ *             ret = _decode_address_photons(
+ *                 address,
+ */
+        for (__pyx_t_3 = 0; __pyx_t_3 < 8; __pyx_t_3+=1) {
+          __pyx_v_address = __pyx_t_3;
+
+          /* "lfdfiles/_lfdfiles.pyx":540
+ *                 address,
+ *                 data,
+ *                 photons[np:],             # <<<<<<<<<<<<<<
+ *                 size,
+ *                 height,
+ */
+          __pyx_t_9.data = __pyx_v_photons.data;
+          __pyx_t_9.memview = __pyx_v_photons.memview;
+          __PYX_INC_MEMVIEW(&__pyx_t_9, 0);
+          __pyx_t_10 = -1;
+          if (unlikely(__pyx_memoryview_slice_memviewslice(
+    &__pyx_t_9,
+    __pyx_v_photons.shape[0], __pyx_v_photons.strides[0], __pyx_v_photons.suboffsets[0],
+    0,
+    0,
+    &__pyx_t_10,
+    __pyx_v_np,
+    0,
+    0,
+    1,
+    0,
+    0,
+    1) < 0))
+{
+    __PYX_ERR(0, 540, __pyx_L11_error)
+}
+
+__pyx_t_9.shape[1] = __pyx_v_photons.shape[1];
+__pyx_t_9.strides[1] = __pyx_v_photons.strides[1];
+    __pyx_t_9.suboffsets[1] = -1;
+
+__pyx_v_ret = __pyx_f_8lfdfiles_9_lfdfiles__decode_address_photons(__pyx_v_address, __pyx_v_data, __pyx_t_9, __pyx_v_size, __pyx_v_height, __pyx_v_width, __pyx_v_pixeltime, __pyx_v_enabletime, __pyx_v_maxframes);
+
+          /* "lfdfiles/_lfdfiles.pyx":537
+ *         np = 0
+ *         for address in range(8):
+ *             ret = _decode_address_photons(             # <<<<<<<<<<<<<<
+ *                 address,
+ *                 data,
+ */
+          __PYX_XDEC_MEMVIEW(&__pyx_t_9, 0);
+          __pyx_t_9.memview = NULL;
+          __pyx_t_9.data = NULL;
+
+          /* "lfdfiles/_lfdfiles.pyx":548
+ *                 maxframes,
+ *             )
+ *             if ret < 0:             # <<<<<<<<<<<<<<
+ *                 raise ValueError(
+ *                     f'no start of frame found for address {address}'
+ */
+          __pyx_t_4 = ((__pyx_v_ret < 0) != 0);
+          if (__pyx_t_4) {
+
+            /* "lfdfiles/_lfdfiles.pyx":549
+ *             )
+ *             if ret < 0:
+ *                 raise ValueError(             # <<<<<<<<<<<<<<
+ *                     f'no start of frame found for address {address}'
+ *                 )
+ */
+            {
+                #ifdef WITH_THREAD
+                PyGILState_STATE __pyx_gilstate_save = __Pyx_PyGILState_Ensure();
+                #endif
+                /*try:*/ {
+
+                  /* "lfdfiles/_lfdfiles.pyx":550
+ *             if ret < 0:
+ *                 raise ValueError(
+ *                     f'no start of frame found for address {address}'             # <<<<<<<<<<<<<<
+ *                 )
+ *             np += ret
+ */
+                  __pyx_t_2 = __Pyx_PyUnicode_From_Py_ssize_t(__pyx_v_address, 0, ' ', 'd'); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 550, __pyx_L19_error)
+                  __Pyx_GOTREF(__pyx_t_2);
+                  __pyx_t_7 = __Pyx_PyUnicode_Concat(__pyx_kp_u_no_start_of_frame_found_for_addr, __pyx_t_2); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 550, __pyx_L19_error)
+                  __Pyx_GOTREF(__pyx_t_7);
+                  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+                  /* "lfdfiles/_lfdfiles.pyx":549
+ *             )
+ *             if ret < 0:
+ *                 raise ValueError(             # <<<<<<<<<<<<<<
+ *                     f'no start of frame found for address {address}'
+ *                 )
+ */
+                  __pyx_t_2 = __Pyx_PyObject_CallOneArg(__pyx_builtin_ValueError, __pyx_t_7); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 549, __pyx_L19_error)
+                  __Pyx_GOTREF(__pyx_t_2);
+                  __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+                  __Pyx_Raise(__pyx_t_2, 0, 0, 0);
+                  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+                  __PYX_ERR(0, 549, __pyx_L19_error)
+                }
+                /*finally:*/ {
+                  __pyx_L19_error: {
+                    #ifdef WITH_THREAD
+                    __Pyx_PyGILState_Release(__pyx_gilstate_save);
+                    #endif
+                    goto __pyx_L11_error;
+                  }
+                }
+            }
+
+            /* "lfdfiles/_lfdfiles.pyx":548
+ *                 maxframes,
+ *             )
+ *             if ret < 0:             # <<<<<<<<<<<<<<
+ *                 raise ValueError(
+ *                     f'no start of frame found for address {address}'
+ */
+          }
+
+          /* "lfdfiles/_lfdfiles.pyx":552
+ *                     f'no start of frame found for address {address}'
+ *                 )
+ *             np += ret             # <<<<<<<<<<<<<<
+ *             if np >= maxphotons:
+ *                 break
+ */
+          __pyx_v_np = (__pyx_v_np + __pyx_v_ret);
+
+          /* "lfdfiles/_lfdfiles.pyx":553
+ *                 )
+ *             np += ret
+ *             if np >= maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+          __pyx_t_4 = ((__pyx_v_np >= __pyx_v_maxphotons) != 0);
+          if (__pyx_t_4) {
+
+            /* "lfdfiles/_lfdfiles.pyx":554
+ *             np += ret
+ *             if np >= maxphotons:
+ *                 break             # <<<<<<<<<<<<<<
+ * 
+ *     return np
+ */
+            goto __pyx_L14_break;
+
+            /* "lfdfiles/_lfdfiles.pyx":553
+ *                 )
+ *             np += ret
+ *             if np >= maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+          }
+        }
+        __pyx_L14_break:;
+      }
+
+      /* "lfdfiles/_lfdfiles.pyx":534
+ *         enabletime = pixeltime * width
+ * 
+ *     with nogil:             # <<<<<<<<<<<<<<
+ *         np = 0
+ *         for address in range(8):
+ */
+      /*finally:*/ {
+        /*normal exit:*/{
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L12;
+        }
+        __pyx_L11_error: {
+          #ifdef WITH_THREAD
+          __Pyx_FastGIL_Forget();
+          Py_BLOCK_THREADS
+          #endif
+          goto __pyx_L1_error;
+        }
+        __pyx_L12:;
+      }
+  }
+
+  /* "lfdfiles/_lfdfiles.pyx":556
+ *                 break
+ * 
+ *     return np             # <<<<<<<<<<<<<<
+ * 
+ * 
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_2 = PyInt_FromSsize_t(__pyx_v_np); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 556, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_r = __pyx_t_2;
+  __pyx_t_2 = 0;
+  goto __pyx_L0;
+
+  /* "lfdfiles/_lfdfiles.pyx":460
+ * 
+ * 
+ * def sflim_decode_photons(             # <<<<<<<<<<<<<<
+ *     const uint32_t[::1] data,
+ *     uint16_t[:, ::1] photons,
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_7);
+  __PYX_XDEC_MEMVIEW(&__pyx_t_9, 1);
+  __Pyx_AddTraceback("lfdfiles._lfdfiles.sflim_decode_photons", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __PYX_XDEC_MEMVIEW(&__pyx_v_data, 1);
+  __PYX_XDEC_MEMVIEW(&__pyx_v_photons, 1);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "lfdfiles/_lfdfiles.pyx":559
+ * 
+ * 
+ * cdef ssize_t _decode_address_photons(             # <<<<<<<<<<<<<<
+ *     const ssize_t address,
+ *     const uint32_t[::1] data,
+ */
+
+static Py_ssize_t __pyx_f_8lfdfiles_9_lfdfiles__decode_address_photons(Py_ssize_t const __pyx_v_address, __Pyx_memviewslice __pyx_v_data, __Pyx_memviewslice __pyx_v_photons, Py_ssize_t const __pyx_v_size, Py_ssize_t const __pyx_v_height, Py_ssize_t const __pyx_v_width, uint64_t const __pyx_v_pixeltime, uint64_t const __pyx_v_enabletime, Py_ssize_t const __pyx_v_maxframes) {
+  Py_ssize_t __pyx_v_maxphotons;
+  Py_ssize_t __pyx_v_framesize;
+  Py_ssize_t __pyx_v_i;
+  Py_ssize_t __pyx_v_y;
+  Py_ssize_t __pyx_v_x;
+  Py_ssize_t __pyx_v_start;
+  Py_ssize_t __pyx_v_frames;
+  Py_ssize_t __pyx_v_pixelindex;
+  Py_ssize_t __pyx_v_np;
+  uint64_t __pyx_v_macrotime;
+  uint64_t __pyx_v_macrotime0;
+  uint32_t __pyx_v_d;
+  uint32_t __pyx_v_pcc;
+  uint32_t __pyx_v_tcc;
+  uint32_t __pyx_v_tcc0;
+  uint32_t __pyx_v_enable;
+  uint32_t __pyx_v_ph;
+  Py_ssize_t __pyx_r;
+  Py_ssize_t __pyx_t_1;
+  Py_ssize_t __pyx_t_2;
+  Py_ssize_t __pyx_t_3;
+  Py_ssize_t __pyx_t_4;
+  int __pyx_t_5;
+  int __pyx_t_6;
+  Py_ssize_t __pyx_t_7;
+
+  /* "lfdfiles/_lfdfiles.pyx":572
+ *     """Decode photons' time, channel, and pixel. Return number of photons."""
+ *     cdef:
+ *         ssize_t maxphotons = photons.shape[0]             # <<<<<<<<<<<<<<
+ *         ssize_t framesize = width * height
+ *         ssize_t i, y, x, start, frames, pixelindex, np
+ */
+  __pyx_v_maxphotons = (__pyx_v_photons.shape[0]);
+
+  /* "lfdfiles/_lfdfiles.pyx":573
+ *     cdef:
+ *         ssize_t maxphotons = photons.shape[0]
+ *         ssize_t framesize = width * height             # <<<<<<<<<<<<<<
+ *         ssize_t i, y, x, start, frames, pixelindex, np
+ *         uint64_t macrotime, macrotime0
+ */
+  __pyx_v_framesize = (__pyx_v_width * __pyx_v_height);
+
+  /* "lfdfiles/_lfdfiles.pyx":579
+ * 
+ *     # seek to first frame
+ *     start = 0             # <<<<<<<<<<<<<<
+ *     for i in range(size):
+ *         if (data[i] & <uint32_t> MASK_ENA) >> SHR_ENA:
+ */
+  __pyx_v_start = 0;
+
+  /* "lfdfiles/_lfdfiles.pyx":580
+ *     # seek to first frame
+ *     start = 0
+ *     for i in range(size):             # <<<<<<<<<<<<<<
+ *         if (data[i] & <uint32_t> MASK_ENA) >> SHR_ENA:
+ *             start = i
+ */
+  __pyx_t_1 = __pyx_v_size;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = 0; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_i = __pyx_t_3;
+
+    /* "lfdfiles/_lfdfiles.pyx":581
+ *     start = 0
+ *     for i in range(size):
+ *         if (data[i] & <uint32_t> MASK_ENA) >> SHR_ENA:             # <<<<<<<<<<<<<<
+ *             start = i
+ *             break
+ */
+    __pyx_t_4 = __pyx_v_i;
+    __pyx_t_5 = ((((*((uint32_t const  *) ( /* dim=0 */ ((char *) (((uint32_t const  *) __pyx_v_data.data) + __pyx_t_4)) ))) & ((uint32_t)0x1000)) >> 12) != 0);
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":582
+ *     for i in range(size):
+ *         if (data[i] & <uint32_t> MASK_ENA) >> SHR_ENA:
+ *             start = i             # <<<<<<<<<<<<<<
+ *             break
+ *     else:
+ */
+      __pyx_v_start = __pyx_v_i;
+
+      /* "lfdfiles/_lfdfiles.pyx":583
+ *         if (data[i] & <uint32_t> MASK_ENA) >> SHR_ENA:
+ *             start = i
+ *             break             # <<<<<<<<<<<<<<
+ *     else:
+ *         return -1
+ */
+      goto __pyx_L4_break;
+
+      /* "lfdfiles/_lfdfiles.pyx":581
+ *     start = 0
+ *     for i in range(size):
+ *         if (data[i] & <uint32_t> MASK_ENA) >> SHR_ENA:             # <<<<<<<<<<<<<<
+ *             start = i
+ *             break
+ */
+    }
+  }
+  /*else*/ {
+
+    /* "lfdfiles/_lfdfiles.pyx":585
+ *             break
+ *     else:
+ *         return -1             # <<<<<<<<<<<<<<
+ * 
+ *     tcc0 = data[start] & <uint32_t> MASK_TCC
+ */
+    __pyx_r = -1L;
+    goto __pyx_L0;
+  }
+  __pyx_L4_break:;
+
+  /* "lfdfiles/_lfdfiles.pyx":587
+ *         return -1
+ * 
+ *     tcc0 = data[start] & <uint32_t> MASK_TCC             # <<<<<<<<<<<<<<
+ *     macrotime = tcc0
+ *     macrotime0 = tcc0
+ */
+  __pyx_t_1 = __pyx_v_start;
+  __pyx_v_tcc0 = ((*((uint32_t const  *) ( /* dim=0 */ ((char *) (((uint32_t const  *) __pyx_v_data.data) + __pyx_t_1)) ))) & ((uint32_t)0xFFF));
+
+  /* "lfdfiles/_lfdfiles.pyx":588
+ * 
+ *     tcc0 = data[start] & <uint32_t> MASK_TCC
+ *     macrotime = tcc0             # <<<<<<<<<<<<<<
+ *     macrotime0 = tcc0
+ *     frames = 0
+ */
+  __pyx_v_macrotime = __pyx_v_tcc0;
+
+  /* "lfdfiles/_lfdfiles.pyx":589
+ *     tcc0 = data[start] & <uint32_t> MASK_TCC
+ *     macrotime = tcc0
+ *     macrotime0 = tcc0             # <<<<<<<<<<<<<<
+ *     frames = 0
+ *     np = 0
+ */
+  __pyx_v_macrotime0 = __pyx_v_tcc0;
+
+  /* "lfdfiles/_lfdfiles.pyx":590
+ *     macrotime = tcc0
+ *     macrotime0 = tcc0
+ *     frames = 0             # <<<<<<<<<<<<<<
+ *     np = 0
+ * 
+ */
+  __pyx_v_frames = 0;
+
+  /* "lfdfiles/_lfdfiles.pyx":591
+ *     macrotime0 = tcc0
+ *     frames = 0
+ *     np = 0             # <<<<<<<<<<<<<<
+ * 
+ *     # loop over all data items
+ */
+  __pyx_v_np = 0;
+
+  /* "lfdfiles/_lfdfiles.pyx":594
+ * 
+ *     # loop over all data items
+ *     for i in range(start, size):             # <<<<<<<<<<<<<<
+ * 
+ *         d = data[i]
+ */
+  __pyx_t_1 = __pyx_v_size;
+  __pyx_t_2 = __pyx_t_1;
+  for (__pyx_t_3 = __pyx_v_start; __pyx_t_3 < __pyx_t_2; __pyx_t_3+=1) {
+    __pyx_v_i = __pyx_t_3;
+
+    /* "lfdfiles/_lfdfiles.pyx":596
+ *     for i in range(start, size):
+ * 
+ *         d = data[i]             # <<<<<<<<<<<<<<
+ * 
+ *         if <uint32_t> address != (d & <uint32_t> MASK_ADR) >> SHR_ADR:
+ */
+    __pyx_t_4 = __pyx_v_i;
+    __pyx_v_d = (*((uint32_t const  *) ( /* dim=0 */ ((char *) (((uint32_t const  *) __pyx_v_data.data) + __pyx_t_4)) )));
+
+    /* "lfdfiles/_lfdfiles.pyx":598
+ *         d = data[i]
+ * 
+ *         if <uint32_t> address != (d & <uint32_t> MASK_ADR) >> SHR_ADR:             # <<<<<<<<<<<<<<
+ *             continue
+ * 
+ */
+    __pyx_t_5 = ((((uint32_t)__pyx_v_address) != ((__pyx_v_d & ((uint32_t)0xE0000000)) >> 29)) != 0);
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":599
+ * 
+ *         if <uint32_t> address != (d & <uint32_t> MASK_ADR) >> SHR_ADR:
+ *             continue             # <<<<<<<<<<<<<<
+ * 
+ *         pcc = d & <uint32_t> MASK_PCC
+ */
+      goto __pyx_L6_continue;
+
+      /* "lfdfiles/_lfdfiles.pyx":598
+ *         d = data[i]
+ * 
+ *         if <uint32_t> address != (d & <uint32_t> MASK_ADR) >> SHR_ADR:             # <<<<<<<<<<<<<<
+ *             continue
+ * 
+ */
+    }
+
+    /* "lfdfiles/_lfdfiles.pyx":601
+ *             continue
+ * 
+ *         pcc = d & <uint32_t> MASK_PCC             # <<<<<<<<<<<<<<
+ *         tcc = d & <uint32_t> MASK_TCC
+ *         enable = (d & <uint32_t> MASK_ENA) >> SHR_ENA
+ */
+    __pyx_v_pcc = (__pyx_v_d & ((uint32_t)0xFF));
+
+    /* "lfdfiles/_lfdfiles.pyx":602
+ * 
+ *         pcc = d & <uint32_t> MASK_PCC
+ *         tcc = d & <uint32_t> MASK_TCC             # <<<<<<<<<<<<<<
+ *         enable = (d & <uint32_t> MASK_ENA) >> SHR_ENA
+ * 
+ */
+    __pyx_v_tcc = (__pyx_v_d & ((uint32_t)0xFFF));
+
+    /* "lfdfiles/_lfdfiles.pyx":603
+ *         pcc = d & <uint32_t> MASK_PCC
+ *         tcc = d & <uint32_t> MASK_TCC
+ *         enable = (d & <uint32_t> MASK_ENA) >> SHR_ENA             # <<<<<<<<<<<<<<
+ * 
+ *         if tcc < tcc0:
+ */
+    __pyx_v_enable = ((__pyx_v_d & ((uint32_t)0x1000)) >> 12);
+
+    /* "lfdfiles/_lfdfiles.pyx":605
+ *         enable = (d & <uint32_t> MASK_ENA) >> SHR_ENA
+ * 
+ *         if tcc < tcc0:             # <<<<<<<<<<<<<<
+ *             macrotime += 4096
+ *         tcc0 = tcc
+ */
+    __pyx_t_5 = ((__pyx_v_tcc < __pyx_v_tcc0) != 0);
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":606
+ * 
+ *         if tcc < tcc0:
+ *             macrotime += 4096             # <<<<<<<<<<<<<<
+ *         tcc0 = tcc
+ * 
+ */
+      __pyx_v_macrotime = (__pyx_v_macrotime + 0x1000);
+
+      /* "lfdfiles/_lfdfiles.pyx":605
+ *         enable = (d & <uint32_t> MASK_ENA) >> SHR_ENA
+ * 
+ *         if tcc < tcc0:             # <<<<<<<<<<<<<<
+ *             macrotime += 4096
+ *         tcc0 = tcc
+ */
+    }
+
+    /* "lfdfiles/_lfdfiles.pyx":607
+ *         if tcc < tcc0:
+ *             macrotime += 4096
+ *         tcc0 = tcc             # <<<<<<<<<<<<<<
+ * 
+ *         if enable and (macrotime - macrotime0 + tcc) > enabletime:
+ */
+    __pyx_v_tcc0 = __pyx_v_tcc;
+
+    /* "lfdfiles/_lfdfiles.pyx":609
+ *         tcc0 = tcc
+ * 
+ *         if enable and (macrotime - macrotime0 + tcc) > enabletime:             # <<<<<<<<<<<<<<
+ *             if frames == maxframes:
+ *                 break
+ */
+    __pyx_t_6 = (__pyx_v_enable != 0);
+    if (__pyx_t_6) {
+    } else {
+      __pyx_t_5 = __pyx_t_6;
+      goto __pyx_L11_bool_binop_done;
+    }
+    __pyx_t_6 = ((((__pyx_v_macrotime - __pyx_v_macrotime0) + __pyx_v_tcc) > __pyx_v_enabletime) != 0);
+    __pyx_t_5 = __pyx_t_6;
+    __pyx_L11_bool_binop_done:;
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":610
+ * 
+ *         if enable and (macrotime - macrotime0 + tcc) > enabletime:
+ *             if frames == maxframes:             # <<<<<<<<<<<<<<
+ *                 break
+ *             frames += 1
+ */
+      __pyx_t_5 = ((__pyx_v_frames == __pyx_v_maxframes) != 0);
+      if (__pyx_t_5) {
+
+        /* "lfdfiles/_lfdfiles.pyx":611
+ *         if enable and (macrotime - macrotime0 + tcc) > enabletime:
+ *             if frames == maxframes:
+ *                 break             # <<<<<<<<<<<<<<
+ *             frames += 1
+ *             macrotime0 = macrotime
+ */
+        goto __pyx_L7_break;
+
+        /* "lfdfiles/_lfdfiles.pyx":610
+ * 
+ *         if enable and (macrotime - macrotime0 + tcc) > enabletime:
+ *             if frames == maxframes:             # <<<<<<<<<<<<<<
+ *                 break
+ *             frames += 1
+ */
+      }
+
+      /* "lfdfiles/_lfdfiles.pyx":612
+ *             if frames == maxframes:
+ *                 break
+ *             frames += 1             # <<<<<<<<<<<<<<
+ *             macrotime0 = macrotime
+ * 
+ */
+      __pyx_v_frames = (__pyx_v_frames + 1);
+
+      /* "lfdfiles/_lfdfiles.pyx":613
+ *                 break
+ *             frames += 1
+ *             macrotime0 = macrotime             # <<<<<<<<<<<<<<
+ * 
+ *         pixelindex = <ssize_t> ((macrotime - macrotime0 + tcc) // pixeltime)
+ */
+      __pyx_v_macrotime0 = __pyx_v_macrotime;
+
+      /* "lfdfiles/_lfdfiles.pyx":609
+ *         tcc0 = tcc
+ * 
+ *         if enable and (macrotime - macrotime0 + tcc) > enabletime:             # <<<<<<<<<<<<<<
+ *             if frames == maxframes:
+ *                 break
+ */
+    }
+
+    /* "lfdfiles/_lfdfiles.pyx":615
+ *             macrotime0 = macrotime
+ * 
+ *         pixelindex = <ssize_t> ((macrotime - macrotime0 + tcc) // pixeltime)             # <<<<<<<<<<<<<<
+ *         if pixelindex >= framesize:
+ *             # skipped += 1
+ */
+    __pyx_v_pixelindex = ((Py_ssize_t)(((__pyx_v_macrotime - __pyx_v_macrotime0) + __pyx_v_tcc) / __pyx_v_pixeltime));
+
+    /* "lfdfiles/_lfdfiles.pyx":616
+ * 
+ *         pixelindex = <ssize_t> ((macrotime - macrotime0 + tcc) // pixeltime)
+ *         if pixelindex >= framesize:             # <<<<<<<<<<<<<<
+ *             # skipped += 1
+ *             continue
+ */
+    __pyx_t_5 = ((__pyx_v_pixelindex >= __pyx_v_framesize) != 0);
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":618
+ *         if pixelindex >= framesize:
+ *             # skipped += 1
+ *             continue             # <<<<<<<<<<<<<<
+ * 
+ *         x = pixelindex % width
+ */
+      goto __pyx_L6_continue;
+
+      /* "lfdfiles/_lfdfiles.pyx":616
+ * 
+ *         pixelindex = <ssize_t> ((macrotime - macrotime0 + tcc) // pixeltime)
+ *         if pixelindex >= framesize:             # <<<<<<<<<<<<<<
+ *             # skipped += 1
+ *             continue
+ */
+    }
+
+    /* "lfdfiles/_lfdfiles.pyx":620
+ *             continue
+ * 
+ *         x = pixelindex % width             # <<<<<<<<<<<<<<
+ *         y = pixelindex // width
+ * 
+ */
+    __pyx_v_x = (__pyx_v_pixelindex % __pyx_v_width);
+
+    /* "lfdfiles/_lfdfiles.pyx":621
+ * 
+ *         x = pixelindex % width
+ *         y = pixelindex // width             # <<<<<<<<<<<<<<
+ * 
+ *         ph = (d & <uint32_t> MASK_PH0) >> SHR_PH0
+ */
+    __pyx_v_y = (__pyx_v_pixelindex / __pyx_v_width);
+
+    /* "lfdfiles/_lfdfiles.pyx":623
+ *         y = pixelindex // width
+ * 
+ *         ph = (d & <uint32_t> MASK_PH0) >> SHR_PH0             # <<<<<<<<<<<<<<
+ *         if ph:
+ *             photons[np, 0] = (
+ */
+    __pyx_v_ph = ((__pyx_v_d & ((uint32_t)0x10000)) >> 16);
+
+    /* "lfdfiles/_lfdfiles.pyx":624
+ * 
+ *         ph = (d & <uint32_t> MASK_PH0) >> SHR_PH0
+ *         if ph:             # <<<<<<<<<<<<<<
+ *             photons[np, 0] = (
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN0) >> SHR_WN0)) % 256
+ */
+    __pyx_t_5 = (__pyx_v_ph != 0);
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":625
+ *         ph = (d & <uint32_t> MASK_PH0) >> SHR_PH0
+ *         if ph:
+ *             photons[np, 0] = (             # <<<<<<<<<<<<<<
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN0) >> SHR_WN0)) % 256
+ *             )
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 0;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = ((__pyx_v_pcc + (32 * ((__pyx_v_d & ((uint32_t)0xE000)) >> 13))) % 0x100);
+
+      /* "lfdfiles/_lfdfiles.pyx":628
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN0) >> SHR_WN0)) % 256
+ *             )
+ *             photons[np, 1] = <uint16_t> frames             # <<<<<<<<<<<<<<
+ *             photons[np, 2] = address * 4
+ *             photons[np, 3] = y
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 1;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = ((uint16_t)__pyx_v_frames);
+
+      /* "lfdfiles/_lfdfiles.pyx":629
+ *             )
+ *             photons[np, 1] = <uint16_t> frames
+ *             photons[np, 2] = address * 4             # <<<<<<<<<<<<<<
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 2;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = (__pyx_v_address * 4);
+
+      /* "lfdfiles/_lfdfiles.pyx":630
+ *             photons[np, 1] = <uint16_t> frames
+ *             photons[np, 2] = address * 4
+ *             photons[np, 3] = y             # <<<<<<<<<<<<<<
+ *             photons[np, 4] = x
+ *             np += 1
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 3;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = __pyx_v_y;
+
+      /* "lfdfiles/_lfdfiles.pyx":631
+ *             photons[np, 2] = address * 4
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x             # <<<<<<<<<<<<<<
+ *             np += 1
+ *             if np == maxphotons:
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 4;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = __pyx_v_x;
+
+      /* "lfdfiles/_lfdfiles.pyx":632
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x
+ *             np += 1             # <<<<<<<<<<<<<<
+ *             if np == maxphotons:
+ *                 break
+ */
+      __pyx_v_np = (__pyx_v_np + 1);
+
+      /* "lfdfiles/_lfdfiles.pyx":633
+ *             photons[np, 4] = x
+ *             np += 1
+ *             if np == maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+      __pyx_t_5 = ((__pyx_v_np == __pyx_v_maxphotons) != 0);
+      if (__pyx_t_5) {
+
+        /* "lfdfiles/_lfdfiles.pyx":634
+ *             np += 1
+ *             if np == maxphotons:
+ *                 break             # <<<<<<<<<<<<<<
+ * 
+ *         ph = (d & <uint32_t> MASK_PH1) >> SHR_PH1
+ */
+        goto __pyx_L7_break;
+
+        /* "lfdfiles/_lfdfiles.pyx":633
+ *             photons[np, 4] = x
+ *             np += 1
+ *             if np == maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+      }
+
+      /* "lfdfiles/_lfdfiles.pyx":624
+ * 
+ *         ph = (d & <uint32_t> MASK_PH0) >> SHR_PH0
+ *         if ph:             # <<<<<<<<<<<<<<
+ *             photons[np, 0] = (
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN0) >> SHR_WN0)) % 256
+ */
+    }
+
+    /* "lfdfiles/_lfdfiles.pyx":636
+ *                 break
+ * 
+ *         ph = (d & <uint32_t> MASK_PH1) >> SHR_PH1             # <<<<<<<<<<<<<<
+ *         if ph:
+ *             photons[np, 0] = (
+ */
+    __pyx_v_ph = ((__pyx_v_d & ((uint32_t)0x20000)) >> 17);
+
+    /* "lfdfiles/_lfdfiles.pyx":637
+ * 
+ *         ph = (d & <uint32_t> MASK_PH1) >> SHR_PH1
+ *         if ph:             # <<<<<<<<<<<<<<
+ *             photons[np, 0] = (
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN1) >> SHR_WN1)) % 256
+ */
+    __pyx_t_5 = (__pyx_v_ph != 0);
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":638
+ *         ph = (d & <uint32_t> MASK_PH1) >> SHR_PH1
+ *         if ph:
+ *             photons[np, 0] = (             # <<<<<<<<<<<<<<
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN1) >> SHR_WN1)) % 256
+ *             )
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 0;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = ((__pyx_v_pcc + (32 * ((__pyx_v_d & ((uint32_t)0x1C0000)) >> 18))) % 0x100);
+
+      /* "lfdfiles/_lfdfiles.pyx":641
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN1) >> SHR_WN1)) % 256
+ *             )
+ *             photons[np, 1] = <uint16_t> frames             # <<<<<<<<<<<<<<
+ *             photons[np, 2] = address * 4 + 1
+ *             photons[np, 3] = y
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 1;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = ((uint16_t)__pyx_v_frames);
+
+      /* "lfdfiles/_lfdfiles.pyx":642
+ *             )
+ *             photons[np, 1] = <uint16_t> frames
+ *             photons[np, 2] = address * 4 + 1             # <<<<<<<<<<<<<<
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 2;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = ((__pyx_v_address * 4) + 1);
+
+      /* "lfdfiles/_lfdfiles.pyx":643
+ *             photons[np, 1] = <uint16_t> frames
+ *             photons[np, 2] = address * 4 + 1
+ *             photons[np, 3] = y             # <<<<<<<<<<<<<<
+ *             photons[np, 4] = x
+ *             np += 1
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 3;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = __pyx_v_y;
+
+      /* "lfdfiles/_lfdfiles.pyx":644
+ *             photons[np, 2] = address * 4 + 1
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x             # <<<<<<<<<<<<<<
+ *             np += 1
+ *             if np == maxphotons:
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 4;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = __pyx_v_x;
+
+      /* "lfdfiles/_lfdfiles.pyx":645
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x
+ *             np += 1             # <<<<<<<<<<<<<<
+ *             if np == maxphotons:
+ *                 break
+ */
+      __pyx_v_np = (__pyx_v_np + 1);
+
+      /* "lfdfiles/_lfdfiles.pyx":646
+ *             photons[np, 4] = x
+ *             np += 1
+ *             if np == maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+      __pyx_t_5 = ((__pyx_v_np == __pyx_v_maxphotons) != 0);
+      if (__pyx_t_5) {
+
+        /* "lfdfiles/_lfdfiles.pyx":647
+ *             np += 1
+ *             if np == maxphotons:
+ *                 break             # <<<<<<<<<<<<<<
+ * 
+ *         ph = (d & <uint32_t> MASK_PH2) >> SHR_PH2
+ */
+        goto __pyx_L7_break;
+
+        /* "lfdfiles/_lfdfiles.pyx":646
+ *             photons[np, 4] = x
+ *             np += 1
+ *             if np == maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+      }
+
+      /* "lfdfiles/_lfdfiles.pyx":637
+ * 
+ *         ph = (d & <uint32_t> MASK_PH1) >> SHR_PH1
+ *         if ph:             # <<<<<<<<<<<<<<
+ *             photons[np, 0] = (
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN1) >> SHR_WN1)) % 256
+ */
+    }
+
+    /* "lfdfiles/_lfdfiles.pyx":649
+ *                 break
+ * 
+ *         ph = (d & <uint32_t> MASK_PH2) >> SHR_PH2             # <<<<<<<<<<<<<<
+ *         if ph:
+ *             photons[np, 0] = (
+ */
+    __pyx_v_ph = ((__pyx_v_d & ((uint32_t)0x1000000)) >> 24);
+
+    /* "lfdfiles/_lfdfiles.pyx":650
+ * 
+ *         ph = (d & <uint32_t> MASK_PH2) >> SHR_PH2
+ *         if ph:             # <<<<<<<<<<<<<<
+ *             photons[np, 0] = (
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN2) >> SHR_WN2)) % 256
+ */
+    __pyx_t_5 = (__pyx_v_ph != 0);
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":651
+ *         ph = (d & <uint32_t> MASK_PH2) >> SHR_PH2
+ *         if ph:
+ *             photons[np, 0] = (             # <<<<<<<<<<<<<<
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN2) >> SHR_WN2)) % 256
+ *             )
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 0;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = ((__pyx_v_pcc + (32 * ((__pyx_v_d & ((uint32_t)0xE00000)) >> 21))) % 0x100);
+
+      /* "lfdfiles/_lfdfiles.pyx":654
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN2) >> SHR_WN2)) % 256
+ *             )
+ *             photons[np, 1] = <uint16_t> frames             # <<<<<<<<<<<<<<
+ *             photons[np, 2] = address * 4 + 2
+ *             photons[np, 3] = y
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 1;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = ((uint16_t)__pyx_v_frames);
+
+      /* "lfdfiles/_lfdfiles.pyx":655
+ *             )
+ *             photons[np, 1] = <uint16_t> frames
+ *             photons[np, 2] = address * 4 + 2             # <<<<<<<<<<<<<<
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 2;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = ((__pyx_v_address * 4) + 2);
+
+      /* "lfdfiles/_lfdfiles.pyx":656
+ *             photons[np, 1] = <uint16_t> frames
+ *             photons[np, 2] = address * 4 + 2
+ *             photons[np, 3] = y             # <<<<<<<<<<<<<<
+ *             photons[np, 4] = x
+ *             np += 1
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 3;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = __pyx_v_y;
+
+      /* "lfdfiles/_lfdfiles.pyx":657
+ *             photons[np, 2] = address * 4 + 2
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x             # <<<<<<<<<<<<<<
+ *             np += 1
+ *             if np == maxphotons:
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 4;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = __pyx_v_x;
+
+      /* "lfdfiles/_lfdfiles.pyx":658
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x
+ *             np += 1             # <<<<<<<<<<<<<<
+ *             if np == maxphotons:
+ *                 break
+ */
+      __pyx_v_np = (__pyx_v_np + 1);
+
+      /* "lfdfiles/_lfdfiles.pyx":659
+ *             photons[np, 4] = x
+ *             np += 1
+ *             if np == maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+      __pyx_t_5 = ((__pyx_v_np == __pyx_v_maxphotons) != 0);
+      if (__pyx_t_5) {
+
+        /* "lfdfiles/_lfdfiles.pyx":660
+ *             np += 1
+ *             if np == maxphotons:
+ *                 break             # <<<<<<<<<<<<<<
+ * 
+ *         ph = (d & <uint32_t> MASK_PH3) >> SHR_PH3
+ */
+        goto __pyx_L7_break;
+
+        /* "lfdfiles/_lfdfiles.pyx":659
+ *             photons[np, 4] = x
+ *             np += 1
+ *             if np == maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+      }
+
+      /* "lfdfiles/_lfdfiles.pyx":650
+ * 
+ *         ph = (d & <uint32_t> MASK_PH2) >> SHR_PH2
+ *         if ph:             # <<<<<<<<<<<<<<
+ *             photons[np, 0] = (
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN2) >> SHR_WN2)) % 256
+ */
+    }
+
+    /* "lfdfiles/_lfdfiles.pyx":662
+ *                 break
+ * 
+ *         ph = (d & <uint32_t> MASK_PH3) >> SHR_PH3             # <<<<<<<<<<<<<<
+ *         if ph:
+ *             photons[np, 0] = (
+ */
+    __pyx_v_ph = ((__pyx_v_d & ((uint32_t)0x2000000)) >> 25);
+
+    /* "lfdfiles/_lfdfiles.pyx":663
+ * 
+ *         ph = (d & <uint32_t> MASK_PH3) >> SHR_PH3
+ *         if ph:             # <<<<<<<<<<<<<<
+ *             photons[np, 0] = (
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN3) >> SHR_WN3)) % 256
+ */
+    __pyx_t_5 = (__pyx_v_ph != 0);
+    if (__pyx_t_5) {
+
+      /* "lfdfiles/_lfdfiles.pyx":664
+ *         ph = (d & <uint32_t> MASK_PH3) >> SHR_PH3
+ *         if ph:
+ *             photons[np, 0] = (             # <<<<<<<<<<<<<<
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN3) >> SHR_WN3)) % 256
+ *             )
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 0;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = ((__pyx_v_pcc + (32 * ((__pyx_v_d & ((uint32_t)0x1C000000)) >> 26))) % 0x100);
+
+      /* "lfdfiles/_lfdfiles.pyx":667
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN3) >> SHR_WN3)) % 256
+ *             )
+ *             photons[np, 1] = <uint16_t> frames             # <<<<<<<<<<<<<<
+ *             photons[np, 2] = address * 4 + 3
+ *             photons[np, 3] = y
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 1;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = ((uint16_t)__pyx_v_frames);
+
+      /* "lfdfiles/_lfdfiles.pyx":668
+ *             )
+ *             photons[np, 1] = <uint16_t> frames
+ *             photons[np, 2] = address * 4 + 3             # <<<<<<<<<<<<<<
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 2;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = ((__pyx_v_address * 4) + 3);
+
+      /* "lfdfiles/_lfdfiles.pyx":669
+ *             photons[np, 1] = <uint16_t> frames
+ *             photons[np, 2] = address * 4 + 3
+ *             photons[np, 3] = y             # <<<<<<<<<<<<<<
+ *             photons[np, 4] = x
+ *             np += 1
+ */
+      __pyx_t_4 = __pyx_v_np;
+      __pyx_t_7 = 3;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_4 * __pyx_v_photons.strides[0]) )) + __pyx_t_7)) )) = __pyx_v_y;
+
+      /* "lfdfiles/_lfdfiles.pyx":670
+ *             photons[np, 2] = address * 4 + 3
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x             # <<<<<<<<<<<<<<
+ *             np += 1
+ *             if np == maxphotons:
+ */
+      __pyx_t_7 = __pyx_v_np;
+      __pyx_t_4 = 4;
+      *((uint16_t *) ( /* dim=1 */ ((char *) (((uint16_t *) ( /* dim=0 */ (__pyx_v_photons.data + __pyx_t_7 * __pyx_v_photons.strides[0]) )) + __pyx_t_4)) )) = __pyx_v_x;
+
+      /* "lfdfiles/_lfdfiles.pyx":671
+ *             photons[np, 3] = y
+ *             photons[np, 4] = x
+ *             np += 1             # <<<<<<<<<<<<<<
+ *             if np == maxphotons:
+ *                 break
+ */
+      __pyx_v_np = (__pyx_v_np + 1);
+
+      /* "lfdfiles/_lfdfiles.pyx":672
+ *             photons[np, 4] = x
+ *             np += 1
+ *             if np == maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+      __pyx_t_5 = ((__pyx_v_np == __pyx_v_maxphotons) != 0);
+      if (__pyx_t_5) {
+
+        /* "lfdfiles/_lfdfiles.pyx":673
+ *             np += 1
+ *             if np == maxphotons:
+ *                 break             # <<<<<<<<<<<<<<
+ * 
+ *     return np
+ */
+        goto __pyx_L7_break;
+
+        /* "lfdfiles/_lfdfiles.pyx":672
+ *             photons[np, 4] = x
+ *             np += 1
+ *             if np == maxphotons:             # <<<<<<<<<<<<<<
+ *                 break
+ * 
+ */
+      }
+
+      /* "lfdfiles/_lfdfiles.pyx":663
+ * 
+ *         ph = (d & <uint32_t> MASK_PH3) >> SHR_PH3
+ *         if ph:             # <<<<<<<<<<<<<<
+ *             photons[np, 0] = (
+ *                 (pcc + 32 * ((d & <uint32_t> MASK_WN3) >> SHR_WN3)) % 256
+ */
+    }
+    __pyx_L6_continue:;
+  }
+  __pyx_L7_break:;
+
+  /* "lfdfiles/_lfdfiles.pyx":675
+ *                 break
+ * 
+ *     return np             # <<<<<<<<<<<<<<
+ */
+  __pyx_r = __pyx_v_np;
+  goto __pyx_L0;
+
+  /* "lfdfiles/_lfdfiles.pyx":559
+ * 
+ * 
+ * cdef ssize_t _decode_address_photons(             # <<<<<<<<<<<<<<
  *     const ssize_t address,
  *     const uint32_t[::1] data,
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -12808,15 +14416,15 @@
     /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__11, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 134, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 134, __pyx_L1_error)
 
     /* "View.MemoryView":133
  *         self.itemsize = itemsize
@@ -12840,15 +14448,15 @@
     /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__12, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 137, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 137, __pyx_L1_error)
 
     /* "View.MemoryView":136
  *             raise ValueError("Empty shape tuple for cython.array")
@@ -12967,15 +14575,15 @@
     /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__13, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 149, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 149, __pyx_L1_error)
 
     /* "View.MemoryView":148
  *         self._strides = self._shape + self.ndim
@@ -13241,15 +14849,15 @@
       /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__14, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
+      __pyx_t_10 = __Pyx_PyObject_Call(__pyx_builtin_MemoryError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_10)) __PYX_ERR(1, 177, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_10);
       __Pyx_Raise(__pyx_t_10, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_10); __pyx_t_10 = 0;
       __PYX_ERR(1, 177, __pyx_L1_error)
 
       /* "View.MemoryView":176
  * 
@@ -13485,15 +15093,15 @@
     /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__15, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 193, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 193, __pyx_L1_error)
 
     /* "View.MemoryView":192
  *         elif self.mode == u"fortran":
@@ -14219,15 +15827,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__16, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -14275,15 +15883,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__17, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -16004,15 +17612,15 @@
     /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__18, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 420, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 420, __pyx_L1_error)
 
     /* "View.MemoryView":419
  * 
@@ -17052,15 +18660,15 @@
       /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__19, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
+      __pyx_t_6 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 497, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_Raise(__pyx_t_6, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
       __PYX_ERR(1, 497, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
@@ -17414,15 +19022,15 @@
     /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__20, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
+    __pyx_t_3 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 522, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __PYX_ERR(1, 522, __pyx_L1_error)
 
     /* "View.MemoryView":521
  *     @cname('getbuffer')
@@ -17963,15 +19571,15 @@
     /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__21, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__22, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 572, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_Raise(__pyx_t_2, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __PYX_ERR(1, 572, __pyx_L1_error)
 
     /* "View.MemoryView":570
  *     @property
@@ -18080,15 +19688,15 @@
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_t_2 = __Pyx_PyInt_From_int(__pyx_v_self->view.ndim); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__22, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
+    __pyx_t_3 = PyNumber_Multiply(__pyx_tuple__23, __pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 579, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __pyx_r = __pyx_t_3;
     __pyx_t_3 = 0;
     goto __pyx_L0;
 
     /* "View.MemoryView":578
@@ -19118,15 +20726,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__23, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -19174,15 +20782,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__24, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__25, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -19531,17 +21139,17 @@
  *             else:
  */
         __pyx_t_8 = PyObject_Length(__pyx_v_tup); if (unlikely(__pyx_t_8 == ((Py_ssize_t)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __pyx_t_7 = PyList_New(1 * ((((__pyx_v_ndim - __pyx_t_8) + 1)<0) ? 0:((__pyx_v_ndim - __pyx_t_8) + 1))); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_7);
         { Py_ssize_t __pyx_temp;
           for (__pyx_temp=0; __pyx_temp < ((__pyx_v_ndim - __pyx_t_8) + 1); __pyx_temp++) {
-            __Pyx_INCREF(__pyx_slice__25);
-            __Pyx_GIVEREF(__pyx_slice__25);
-            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__25);
+            __Pyx_INCREF(__pyx_slice__26);
+            __Pyx_GIVEREF(__pyx_slice__26);
+            PyList_SET_ITEM(__pyx_t_7, __pyx_temp, __pyx_slice__26);
           }
         }
         __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_7); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 684, __pyx_L1_error)
         __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
 
         /* "View.MemoryView":685
  *             if not seen_ellipsis:
@@ -19566,15 +21174,15 @@
  *                 seen_ellipsis = True
  *             else:
  *                 result.append(slice(None))             # <<<<<<<<<<<<<<
  *             have_slices = True
  *         else:
  */
       /*else*/ {
-        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__25); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
+        __pyx_t_9 = __Pyx_PyList_Append(__pyx_v_result, __pyx_slice__26); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 687, __pyx_L1_error)
       }
       __pyx_L7:;
 
       /* "View.MemoryView":688
  *             else:
  *                 result.append(slice(None))
  *             have_slices = True             # <<<<<<<<<<<<<<
@@ -19706,17 +21314,17 @@
  * 
  *     return have_slices or nslices, tuple(result)
  */
     __pyx_t_3 = PyList_New(1 * ((__pyx_v_nslices<0) ? 0:__pyx_v_nslices)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     { Py_ssize_t __pyx_temp;
       for (__pyx_temp=0; __pyx_temp < __pyx_v_nslices; __pyx_temp++) {
-        __Pyx_INCREF(__pyx_slice__25);
-        __Pyx_GIVEREF(__pyx_slice__25);
-        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__25);
+        __Pyx_INCREF(__pyx_slice__26);
+        __Pyx_GIVEREF(__pyx_slice__26);
+        PyList_SET_ITEM(__pyx_t_3, __pyx_temp, __pyx_slice__26);
       }
     }
     __pyx_t_9 = __Pyx_PyList_Extend(__pyx_v_result, __pyx_t_3); if (unlikely(__pyx_t_9 == ((int)-1))) __PYX_ERR(1, 698, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "View.MemoryView":697
  * 
@@ -19835,15 +21443,15 @@
       /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__26, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
+      __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_ValueError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 705, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_Raise(__pyx_t_5, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
       __PYX_ERR(1, 705, __pyx_L1_error)
 
       /* "View.MemoryView":704
  * cdef assert_direct_dimensions(Py_ssize_t *suboffsets, int ndim):
@@ -19943,15 +21551,15 @@
  *     cdef _memoryviewslice memviewsliceobj
  * 
  *     assert memview.view.ndim > 0             # <<<<<<<<<<<<<<
  * 
  *     if isinstance(memview, _memoryviewslice):
  */
   #ifndef CYTHON_WITHOUT_ASSERTIONS
-  if (unlikely(!Py_OptimizeFlag)) {
+  if (unlikely(__pyx_assertions_enabled())) {
     if (unlikely(!((__pyx_v_memview->view.ndim > 0) != 0))) {
       PyErr_SetNone(PyExc_AssertionError);
       __PYX_ERR(1, 724, __pyx_L1_error)
     }
   }
   #endif
 
@@ -22019,15 +23627,15 @@
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__27, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 2, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
@@ -22075,15 +23683,15 @@
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__28, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_builtin_TypeError, __pyx_tuple__29, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_Raise(__pyx_t_1, 0, 0, 0);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __PYX_ERR(1, 4, __pyx_L1_error)
 
   /* "(tree fragment)":3
  * def __reduce_cython__(self):
@@ -25352,15 +26960,15 @@
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError("Incompatible checksums (0x%x vs (0xb068931, 0x82a3537, 0x6ae9995) = (name))" % __pyx_checksum)
  */
   __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__29, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple__30, Py_NE)); if (unlikely(__pyx_t_2 < 0)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_3 = (__pyx_t_2 != 0);
   if (__pyx_t_3) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
  *     if __pyx_checksum not in (0xb068931, 0x82a3537, 0x6ae9995):
@@ -25670,15 +27278,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_array(PyObject *o) {
   struct __pyx_array_obj *p = (struct __pyx_array_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
     __Pyx_SET_REFCNT(o, Py_REFCNT(o) + 1);
@@ -25833,15 +27441,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyObject *__pyx_tp_new_Enum(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
   struct __pyx_MemviewEnum_obj *p;
   PyObject *o;
@@ -25855,15 +27463,15 @@
   p->name = Py_None; Py_INCREF(Py_None);
   return o;
 }
 
 static void __pyx_tp_dealloc_Enum(PyObject *o) {
   struct __pyx_MemviewEnum_obj *p = (struct __pyx_MemviewEnum_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   Py_CLEAR(p->name);
   (*Py_TYPE(o)->tp_free)(o);
 }
@@ -25955,15 +27563,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct_memoryview __pyx_vtable_memoryview;
 
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryview_obj *p;
@@ -25986,15 +27594,15 @@
   Py_DECREF(o); o = 0;
   return NULL;
 }
 
 static void __pyx_tp_dealloc_memoryview(PyObject *o) {
   struct __pyx_memoryview_obj *p = (struct __pyx_memoryview_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -26219,15 +27827,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 static struct __pyx_vtabstruct__memoryviewslice __pyx_vtable__memoryviewslice;
 
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k) {
   struct __pyx_memoryviewslice_obj *p;
@@ -26239,15 +27847,15 @@
   p->from_slice.memview = NULL;
   return o;
 }
 
 static void __pyx_tp_dealloc__memoryviewslice(PyObject *o) {
   struct __pyx_memoryviewslice_obj *p = (struct __pyx_memoryviewslice_obj *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !_PyGC_FINALIZED(o)) {
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && !__Pyx_PyObject_GC_IsFinalized(o)) {
     if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   PyObject_GC_UnTrack(o);
   {
     PyObject *etype, *eval, *etb;
     PyErr_Fetch(&etype, &eval, &etb);
@@ -26368,15 +27976,15 @@
   #endif
   #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
   0, /*tp_vectorcall*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
   0, /*tp_pypy_flags*/
   #endif
 };
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
@@ -26420,23 +28028,25 @@
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
   {&__pyx_kp_s_, __pyx_k_, sizeof(__pyx_k_), 0, 0, 1, 0},
-  {&__pyx_kp_u_2023_4_20, __pyx_k_2023_4_20, sizeof(__pyx_k_2023_4_20), 0, 1, 0, 0},
+  {&__pyx_kp_u_1_5, __pyx_k_1_5, sizeof(__pyx_k_1_5), 0, 1, 0, 0},
+  {&__pyx_kp_u_2023_8_1, __pyx_k_2023_8_1, sizeof(__pyx_k_2023_8_1), 0, 1, 0, 0},
   {&__pyx_kp_u_32_256_height_width, __pyx_k_32_256_height_width, sizeof(__pyx_k_32_256_height_width), 0, 1, 0, 0},
   {&__pyx_n_s_ASCII, __pyx_k_ASCII, sizeof(__pyx_k_ASCII), 0, 0, 1, 1},
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
   {&__pyx_kp_u_Decode_Kintex_FLIMbox_data_to_SL, __pyx_k_Decode_Kintex_FLIMbox_data_to_SL, sizeof(__pyx_k_Decode_Kintex_FLIMbox_data_to_SL), 0, 1, 0, 0},
+  {&__pyx_kp_u_Decode_Kintex_FLIMbox_data_to_SL_2, __pyx_k_Decode_Kintex_FLIMbox_data_to_SL_2, sizeof(__pyx_k_Decode_Kintex_FLIMbox_data_to_SL_2), 0, 1, 0, 0},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
   {&__pyx_kp_s_Expected_at_least_d_argument_s_g, __pyx_k_Expected_at_least_d_argument_s_g, sizeof(__pyx_k_Expected_at_least_d_argument_s_g), 0, 0, 1, 0},
   {&__pyx_kp_s_Function_call_with_ambiguous_arg, __pyx_k_Function_call_with_ambiguous_arg, sizeof(__pyx_k_Function_call_with_ambiguous_arg), 0, 0, 1, 0},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
@@ -26481,23 +28091,27 @@
   {&__pyx_n_s_f, __pyx_k_f, sizeof(__pyx_k_f), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
   {&__pyx_n_s_frame_markers, __pyx_k_frame_markers, sizeof(__pyx_k_frame_markers), 0, 0, 1, 1},
   {&__pyx_n_s_framelen, __pyx_k_framelen, sizeof(__pyx_k_framelen), 0, 0, 1, 1},
+  {&__pyx_n_s_frameshape, __pyx_k_frameshape, sizeof(__pyx_k_frameshape), 0, 0, 1, 1},
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_s_harmonics, __pyx_k_harmonics, sizeof(__pyx_k_harmonics), 0, 0, 1, 1},
+  {&__pyx_n_s_height, __pyx_k_height, sizeof(__pyx_k_height), 0, 0, 1, 1},
   {&__pyx_n_s_hist_out, __pyx_k_hist_out, sizeof(__pyx_k_hist_out), 0, 0, 1, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_idx, __pyx_k_idx, sizeof(__pyx_k_idx), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+  {&__pyx_kp_u_invalid_frameshape, __pyx_k_invalid_frameshape, sizeof(__pyx_k_invalid_frameshape), 0, 1, 0, 0},
   {&__pyx_kp_u_invalid_parameters, __pyx_k_invalid_parameters, sizeof(__pyx_k_invalid_parameters), 0, 1, 0, 0},
+  {&__pyx_kp_u_invalid_photons_shape, __pyx_k_invalid_photons_shape, sizeof(__pyx_k_invalid_photons_shape), 0, 1, 0, 0},
   {&__pyx_kp_u_invalid_sflim_shape, __pyx_k_invalid_sflim_shape, sizeof(__pyx_k_invalid_sflim_shape), 0, 1, 0, 0},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_j, __pyx_k_j, sizeof(__pyx_k_j), 0, 0, 1, 1},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {&__pyx_n_s_kind, __pyx_k_kind, sizeof(__pyx_k_kind), 0, 0, 1, 1},
   {&__pyx_n_s_kwargs, __pyx_k_kwargs, sizeof(__pyx_k_kwargs), 0, 0, 1, 1},
@@ -26508,35 +28122,38 @@
   {&__pyx_n_s_m1, __pyx_k_m1, sizeof(__pyx_k_m1), 0, 0, 1, 1},
   {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
   {&__pyx_n_s_marker_mask, __pyx_k_marker_mask, sizeof(__pyx_k_marker_mask), 0, 0, 1, 1},
   {&__pyx_n_s_marker_shr, __pyx_k_marker_shr, sizeof(__pyx_k_marker_shr), 0, 0, 1, 1},
   {&__pyx_n_s_markers_out, __pyx_k_markers_out, sizeof(__pyx_k_markers_out), 0, 0, 1, 1},
   {&__pyx_n_s_maxframes, __pyx_k_maxframes, sizeof(__pyx_k_maxframes), 0, 0, 1, 1},
   {&__pyx_n_s_maxmarker, __pyx_k_maxmarker, sizeof(__pyx_k_maxmarker), 0, 0, 1, 1},
+  {&__pyx_n_s_maxphotons, __pyx_k_maxphotons, sizeof(__pyx_k_maxphotons), 0, 0, 1, 1},
   {&__pyx_n_s_maxwindex, __pyx_k_maxwindex, sizeof(__pyx_k_maxwindex), 0, 0, 1, 1},
   {&__pyx_n_s_memview, __pyx_k_memview, sizeof(__pyx_k_memview), 0, 0, 1, 1},
   {&__pyx_n_s_mode, __pyx_k_mode, sizeof(__pyx_k_mode), 0, 0, 1, 1},
   {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
   {&__pyx_n_s_name_2, __pyx_k_name_2, sizeof(__pyx_k_name_2), 0, 0, 1, 1},
   {&__pyx_n_s_nchannel, __pyx_k_nchannel, sizeof(__pyx_k_nchannel), 0, 0, 1, 1},
   {&__pyx_n_s_nchannels, __pyx_k_nchannels, sizeof(__pyx_k_nchannels), 0, 0, 1, 1},
   {&__pyx_n_s_ndim, __pyx_k_ndim, sizeof(__pyx_k_ndim), 0, 0, 1, 1},
   {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
   {&__pyx_n_s_nframes, __pyx_k_nframes, sizeof(__pyx_k_nframes), 0, 0, 1, 1},
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_kp_u_no_start_of_frame_found_for_addr, __pyx_k_no_start_of_frame_found_for_addr, sizeof(__pyx_k_no_start_of_frame_found_for_addr), 0, 1, 0, 0},
+  {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_n_s_numthreads, __pyx_k_numthreads, sizeof(__pyx_k_numthreads), 0, 0, 1, 1},
   {&__pyx_n_s_nwindows, __pyx_k_nwindows, sizeof(__pyx_k_nwindows), 0, 0, 1, 1},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
   {&__pyx_n_s_pcc, __pyx_k_pcc, sizeof(__pyx_k_pcc), 0, 0, 1, 1},
   {&__pyx_n_s_pcc_mask, __pyx_k_pcc_mask, sizeof(__pyx_k_pcc_mask), 0, 0, 1, 1},
   {&__pyx_n_s_pcc_shr, __pyx_k_pcc_shr, sizeof(__pyx_k_pcc_shr), 0, 0, 1, 1},
   {&__pyx_n_s_pdiv, __pyx_k_pdiv, sizeof(__pyx_k_pdiv), 0, 0, 1, 1},
+  {&__pyx_n_s_photons, __pyx_k_photons, sizeof(__pyx_k_photons), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_pixeltime, __pyx_k_pixeltime, sizeof(__pyx_k_pixeltime), 0, 0, 1, 1},
   {&__pyx_n_s_pmax, __pyx_k_pmax, sizeof(__pyx_k_pmax), 0, 0, 1, 1},
   {&__pyx_n_s_pmax_win, __pyx_k_pmax_win, sizeof(__pyx_k_pmax_win), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
@@ -26553,14 +28170,16 @@
   {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
   {&__pyx_n_s_scanner_frame_start, __pyx_k_scanner_frame_start, sizeof(__pyx_k_scanner_frame_start), 0, 0, 1, 1},
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_sflim, __pyx_k_sflim, sizeof(__pyx_k_sflim), 0, 0, 1, 1},
   {&__pyx_n_s_sflim_decode, __pyx_k_sflim_decode, sizeof(__pyx_k_sflim_decode), 0, 0, 1, 1},
   {&__pyx_kp_u_sflim_decode_line_274, __pyx_k_sflim_decode_line_274, sizeof(__pyx_k_sflim_decode_line_274), 0, 1, 0, 0},
+  {&__pyx_n_s_sflim_decode_photons, __pyx_k_sflim_decode_photons, sizeof(__pyx_k_sflim_decode_photons), 0, 0, 1, 1},
+  {&__pyx_kp_u_sflim_decode_photons_line_460, __pyx_k_sflim_decode_photons_line_460, sizeof(__pyx_k_sflim_decode_photons_line_460), 0, 1, 0, 0},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_kp_u_shape_mismatch_between_bins_and, __pyx_k_shape_mismatch_between_bins_and, sizeof(__pyx_k_shape_mismatch_between_bins_and), 0, 1, 0, 0},
   {&__pyx_kp_u_shape_mismatch_between_bins_and_2, __pyx_k_shape_mismatch_between_bins_and_2, sizeof(__pyx_k_shape_mismatch_between_bins_and_2), 0, 1, 0, 0},
   {&__pyx_kp_u_shape_mismatch_between_bins_and_3, __pyx_k_shape_mismatch_between_bins_and_3, sizeof(__pyx_k_shape_mismatch_between_bins_and_3), 0, 1, 0, 0},
   {&__pyx_kp_u_shape_mismatch_between_bins_and_4, __pyx_k_shape_mismatch_between_bins_and_4, sizeof(__pyx_k_shape_mismatch_between_bins_and_4), 0, 1, 0, 0},
   {&__pyx_n_s_signatures, __pyx_k_signatures, sizeof(__pyx_k_signatures), 0, 0, 1, 1},
   {&__pyx_n_s_simfcsfbd_decode, __pyx_k_simfcsfbd_decode, sizeof(__pyx_k_simfcsfbd_decode), 0, 0, 1, 1},
@@ -26595,14 +28214,15 @@
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_units_per_sample, __pyx_k_units_per_sample, sizeof(__pyx_k_units_per_sample), 0, 0, 1, 1},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_version, __pyx_k_version, sizeof(__pyx_k_version), 0, 0, 1, 1},
   {&__pyx_n_s_w, __pyx_k_w, sizeof(__pyx_k_w), 0, 0, 1, 1},
+  {&__pyx_n_s_width, __pyx_k_width, sizeof(__pyx_k_width), 0, 0, 1, 1},
   {&__pyx_n_s_win, __pyx_k_win, sizeof(__pyx_k_win), 0, 0, 1, 1},
   {&__pyx_n_s_win_mask, __pyx_k_win_mask, sizeof(__pyx_k_win_mask), 0, 0, 1, 1},
   {&__pyx_n_s_win_shr, __pyx_k_win_shr, sizeof(__pyx_k_win_shr), 0, 0, 1, 1},
   {&__pyx_n_s_windows, __pyx_k_windows, sizeof(__pyx_k_windows), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
@@ -26688,317 +28308,345 @@
  * 
  *     units_per_sample = 1.0 / units_per_sample
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_shape_mismatch_between_bins_and_4); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(0, 233, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
+  /* "lfdfiles/_lfdfiles.pyx":526
+ * 
+ *     if len(frameshape) != 2 or frameshape[0] < 1 or frameshape[1] < 1:
+ *         raise ValueError('invalid frameshape')             # <<<<<<<<<<<<<<
+ * 
+ *     height = frameshape[0]
+ */
+  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_u_invalid_frameshape); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(0, 526, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__11);
+  __Pyx_GIVEREF(__pyx_tuple__11);
+
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if itemsize <= 0:
  */
-  __pyx_tuple__11 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__11)) __PYX_ERR(1, 134, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__11);
-  __Pyx_GIVEREF(__pyx_tuple__11);
+  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_Empty_shape_tuple_for_cython_arr); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 134, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__12);
+  __Pyx_GIVEREF(__pyx_tuple__12);
 
   /* "View.MemoryView":137
  * 
  *         if itemsize <= 0:
  *             raise ValueError("itemsize <= 0 for cython.array")             # <<<<<<<<<<<<<<
  * 
  *         if not isinstance(format, bytes):
  */
-  __pyx_tuple__12 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__12)) __PYX_ERR(1, 137, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__12);
-  __Pyx_GIVEREF(__pyx_tuple__12);
+  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_itemsize_0_for_cython_array); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 137, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__13);
+  __Pyx_GIVEREF(__pyx_tuple__13);
 
   /* "View.MemoryView":149
  * 
  *         if not self._shape:
  *             raise MemoryError("unable to allocate shape and strides.")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__13 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__13)) __PYX_ERR(1, 149, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__13);
-  __Pyx_GIVEREF(__pyx_tuple__13);
+  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_shape_and_str); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 149, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__14);
+  __Pyx_GIVEREF(__pyx_tuple__14);
 
   /* "View.MemoryView":177
  *             self.data = <char *>malloc(self.len)
  *             if not self.data:
  *                 raise MemoryError("unable to allocate array data.")             # <<<<<<<<<<<<<<
  * 
  *             if self.dtype_is_object:
  */
-  __pyx_tuple__14 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__14)) __PYX_ERR(1, 177, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__14);
-  __Pyx_GIVEREF(__pyx_tuple__14);
+  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_unable_to_allocate_array_data); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 177, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__15);
+  __Pyx_GIVEREF(__pyx_tuple__15);
 
   /* "View.MemoryView":193
  *             bufmode = PyBUF_F_CONTIGUOUS | PyBUF_ANY_CONTIGUOUS
  *         if not (flags & bufmode):
  *             raise ValueError("Can only create a buffer that is contiguous in memory.")             # <<<<<<<<<<<<<<
  *         info.buf = self.data
  *         info.len = self.len
  */
-  __pyx_tuple__15 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__15)) __PYX_ERR(1, 193, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__15);
-  __Pyx_GIVEREF(__pyx_tuple__15);
+  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_Can_only_create_a_buffer_that_is); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 193, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__16);
+  __Pyx_GIVEREF(__pyx_tuple__16);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__16 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__16)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__16);
-  __Pyx_GIVEREF(__pyx_tuple__16);
+  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__17);
+  __Pyx_GIVEREF(__pyx_tuple__17);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__17 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__17)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__17);
-  __Pyx_GIVEREF(__pyx_tuple__17);
+  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__18);
+  __Pyx_GIVEREF(__pyx_tuple__18);
 
   /* "View.MemoryView":420
  *     def __setitem__(memoryview self, object index, object value):
  *         if self.view.readonly:
  *             raise TypeError("Cannot assign to read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         have_slices, index = _unellipsify(index, self.view.ndim)
  */
-  __pyx_tuple__18 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__18)) __PYX_ERR(1, 420, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__18);
-  __Pyx_GIVEREF(__pyx_tuple__18);
+  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Cannot_assign_to_read_only_memor); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 420, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__19);
+  __Pyx_GIVEREF(__pyx_tuple__19);
 
   /* "View.MemoryView":497
  *             result = struct.unpack(self.view.format, bytesitem)
  *         except struct.error:
  *             raise ValueError("Unable to convert item to object")             # <<<<<<<<<<<<<<
  *         else:
  *             if len(self.view.format) == 1:
  */
-  __pyx_tuple__19 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__19)) __PYX_ERR(1, 497, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__19);
-  __Pyx_GIVEREF(__pyx_tuple__19);
+  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Unable_to_convert_item_to_object); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 497, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__20);
+  __Pyx_GIVEREF(__pyx_tuple__20);
 
   /* "View.MemoryView":522
  *     def __getbuffer__(self, Py_buffer *info, int flags):
  *         if flags & PyBUF_WRITABLE and self.view.readonly:
  *             raise ValueError("Cannot create writable memory view from read-only memoryview")             # <<<<<<<<<<<<<<
  * 
  *         if flags & PyBUF_ND:
  */
-  __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(1, 522, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__20);
-  __Pyx_GIVEREF(__pyx_tuple__20);
+  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Cannot_create_writable_memory_vi); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 522, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__21);
+  __Pyx_GIVEREF(__pyx_tuple__21);
 
   /* "View.MemoryView":572
  *         if self.view.strides == NULL:
  * 
  *             raise ValueError("Buffer view does not expose strides")             # <<<<<<<<<<<<<<
  * 
  *         return tuple([stride for stride in self.view.strides[:self.view.ndim]])
  */
-  __pyx_tuple__21 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(1, 572, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__21);
-  __Pyx_GIVEREF(__pyx_tuple__21);
+  __pyx_tuple__22 = PyTuple_Pack(1, __pyx_kp_s_Buffer_view_does_not_expose_stri); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 572, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__22);
+  __Pyx_GIVEREF(__pyx_tuple__22);
 
   /* "View.MemoryView":579
  *     def suboffsets(self):
  *         if self.view.suboffsets == NULL:
  *             return (-1,) * self.view.ndim             # <<<<<<<<<<<<<<
  * 
  *         return tuple([suboffset for suboffset in self.view.suboffsets[:self.view.ndim]])
  */
-  __pyx_tuple__22 = PyTuple_New(1); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(1, 579, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__22);
+  __pyx_tuple__23 = PyTuple_New(1); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 579, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__23);
   __Pyx_INCREF(__pyx_int_neg_1);
   __Pyx_GIVEREF(__pyx_int_neg_1);
-  PyTuple_SET_ITEM(__pyx_tuple__22, 0, __pyx_int_neg_1);
-  __Pyx_GIVEREF(__pyx_tuple__22);
+  PyTuple_SET_ITEM(__pyx_tuple__23, 0, __pyx_int_neg_1);
+  __Pyx_GIVEREF(__pyx_tuple__23);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__23 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__23)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__23);
-  __Pyx_GIVEREF(__pyx_tuple__23);
+  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__24);
+  __Pyx_GIVEREF(__pyx_tuple__24);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__24 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__24);
-  __Pyx_GIVEREF(__pyx_tuple__24);
+  __pyx_tuple__25 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__25)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__25);
+  __Pyx_GIVEREF(__pyx_tuple__25);
 
   /* "View.MemoryView":684
  *         if item is Ellipsis:
  *             if not seen_ellipsis:
  *                 result.extend([slice(None)] * (ndim - len(tup) + 1))             # <<<<<<<<<<<<<<
  *                 seen_ellipsis = True
  *             else:
  */
-  __pyx_slice__25 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__25)) __PYX_ERR(1, 684, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_slice__25);
-  __Pyx_GIVEREF(__pyx_slice__25);
+  __pyx_slice__26 = PySlice_New(Py_None, Py_None, Py_None); if (unlikely(!__pyx_slice__26)) __PYX_ERR(1, 684, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_slice__26);
+  __Pyx_GIVEREF(__pyx_slice__26);
 
   /* "View.MemoryView":705
  *     for suboffset in suboffsets[:ndim]:
  *         if suboffset >= 0:
  *             raise ValueError("Indirect dimensions not supported")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__26 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(1, 705, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__26);
-  __Pyx_GIVEREF(__pyx_tuple__26);
+  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_Indirect_dimensions_not_supporte); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 705, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__27);
+  __Pyx_GIVEREF(__pyx_tuple__27);
 
   /* "(tree fragment)":2
  * def __reduce_cython__(self):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  */
-  __pyx_tuple__27 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__27)) __PYX_ERR(1, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__27);
-  __Pyx_GIVEREF(__pyx_tuple__27);
+  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__28);
+  __Pyx_GIVEREF(__pyx_tuple__28);
 
   /* "(tree fragment)":4
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")
  * def __setstate_cython__(self, __pyx_state):
  *     raise TypeError("no default __reduce__ due to non-trivial __cinit__")             # <<<<<<<<<<<<<<
  */
-  __pyx_tuple__28 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__28);
-  __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_tuple__29 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __pyx_tuple__29 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__29)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__29);
   __Pyx_GIVEREF(__pyx_tuple__29);
+  __pyx_tuple__30 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(1, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
 
   /* "lfdfiles/_lfdfiles.pyx":67
  * 
  * 
  * def simfcsfbd_decode(             # <<<<<<<<<<<<<<
  *     data_t[::] data,
  *     int8_t[:, ::1] bins_out,
  */
-  __pyx_tuple__30 = PyTuple_Pack(33, __pyx_n_s_data, __pyx_n_s_bins_out, __pyx_n_s_times_out, __pyx_n_s_markers_out, __pyx_n_s_windows, __pyx_n_s_pdiv, __pyx_n_s_harmonics, __pyx_n_s_decoder_table, __pyx_n_s_tcc_mask, __pyx_n_s_tcc_shr, __pyx_n_s_pcc_mask, __pyx_n_s_pcc_shr, __pyx_n_s_marker_mask, __pyx_n_s_marker_shr, __pyx_n_s_win_mask, __pyx_n_s_win_shr, __pyx_n_s_maxwindex, __pyx_n_s_maxmarker, __pyx_n_s_nchannel, __pyx_n_s_datasize, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_c, __pyx_n_s_d, __pyx_n_s_tcc_max, __pyx_n_s_t0, __pyx_n_s_t1, __pyx_n_s_m0, __pyx_n_s_m1, __pyx_n_s_pcc, __pyx_n_s_win, __pyx_n_s_pmax, __pyx_n_s_pmax_win); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 67, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
-  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(16, 0, 33, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_simfcsfbd_decode, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_tuple__31 = PyTuple_Pack(33, __pyx_n_s_data, __pyx_n_s_bins_out, __pyx_n_s_times_out, __pyx_n_s_markers_out, __pyx_n_s_windows, __pyx_n_s_pdiv, __pyx_n_s_harmonics, __pyx_n_s_decoder_table, __pyx_n_s_tcc_mask, __pyx_n_s_tcc_shr, __pyx_n_s_pcc_mask, __pyx_n_s_pcc_shr, __pyx_n_s_marker_mask, __pyx_n_s_marker_shr, __pyx_n_s_win_mask, __pyx_n_s_win_shr, __pyx_n_s_maxwindex, __pyx_n_s_maxmarker, __pyx_n_s_nchannel, __pyx_n_s_datasize, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_c, __pyx_n_s_d, __pyx_n_s_tcc_max, __pyx_n_s_t0, __pyx_n_s_t1, __pyx_n_s_m0, __pyx_n_s_m1, __pyx_n_s_pcc, __pyx_n_s_win, __pyx_n_s_pmax, __pyx_n_s_pmax_win); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__31);
+  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_codeobj__32 = (PyObject*)__Pyx_PyCode_New(16, 0, 33, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__31, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_simfcsfbd_decode, 67, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__32)) __PYX_ERR(0, 67, __pyx_L1_error)
 
   /* "lfdfiles/_lfdfiles.pyx":191
  * 
  * 
  * def simfcsfbd_histogram(             # <<<<<<<<<<<<<<
  *     int8_t[:, ::1] bins,
  *     times_t[::1] times,
  */
-  __pyx_tuple__32 = PyTuple_Pack(18, __pyx_n_s_bins, __pyx_n_s_times, __pyx_n_s_frame_markers, __pyx_n_s_units_per_sample, __pyx_n_s_scanner_frame_start, __pyx_n_s_hist_out, __pyx_n_s_nframes, __pyx_n_s_nchannels, __pyx_n_s_framelen, __pyx_n_s_nwindows, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_f, __pyx_n_s_c, __pyx_n_s_idx, __pyx_n_s_t0, __pyx_n_s_w); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(0, 191, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
-  __pyx_codeobj__33 = (PyObject*)__Pyx_PyCode_New(6, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__32, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_simfcsfbd_histogram, 191, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__33)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_tuple__33 = PyTuple_Pack(18, __pyx_n_s_bins, __pyx_n_s_times, __pyx_n_s_frame_markers, __pyx_n_s_units_per_sample, __pyx_n_s_scanner_frame_start, __pyx_n_s_hist_out, __pyx_n_s_nframes, __pyx_n_s_nchannels, __pyx_n_s_framelen, __pyx_n_s_nwindows, __pyx_n_s_i, __pyx_n_s_j, __pyx_n_s_k, __pyx_n_s_f, __pyx_n_s_c, __pyx_n_s_idx, __pyx_n_s_t0, __pyx_n_s_w); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_codeobj__34 = (PyObject*)__Pyx_PyCode_New(6, 0, 18, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__33, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_simfcsfbd_histogram, 191, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__34)) __PYX_ERR(0, 191, __pyx_L1_error)
 
   /* "lfdfiles/_lfdfiles.pyx":274
  * 
  * 
  * def sflim_decode(             # <<<<<<<<<<<<<<
  *     const uint32_t[::1] data,
  *     sflim_t[:, :, :, ::1] sflim,
  */
-  __pyx_tuple__34 = PyTuple_Pack(10, __pyx_n_s_data, __pyx_n_s_sflim, __pyx_n_s_pixeltime, __pyx_n_s_enabletime, __pyx_n_s_maxframes, __pyx_n_s_numthreads, __pyx_n_s_size, __pyx_n_s_address, __pyx_n_s_lock, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(0, 274, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
-  __pyx_codeobj__35 = (PyObject*)__Pyx_PyCode_New(6, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__34, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_sflim_decode, 274, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__35)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_tuple__35 = PyTuple_Pack(10, __pyx_n_s_data, __pyx_n_s_sflim, __pyx_n_s_pixeltime, __pyx_n_s_enabletime, __pyx_n_s_maxframes, __pyx_n_s_numthreads, __pyx_n_s_size, __pyx_n_s_address, __pyx_n_s_lock, __pyx_n_s_ret); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
+  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(6, 0, 10, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_sflim_decode, 274, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(0, 274, __pyx_L1_error)
+
+  /* "lfdfiles/_lfdfiles.pyx":460
+ * 
+ * 
+ * def sflim_decode_photons(             # <<<<<<<<<<<<<<
+ *     const uint32_t[::1] data,
+ *     uint16_t[:, ::1] photons,
+ */
+  __pyx_tuple__37 = PyTuple_Pack(13, __pyx_n_s_data, __pyx_n_s_photons, __pyx_n_s_frameshape, __pyx_n_s_pixeltime, __pyx_n_s_enabletime, __pyx_n_s_maxframes, __pyx_n_s_size, __pyx_n_s_ret, __pyx_n_s_height, __pyx_n_s_width, __pyx_n_s_address, __pyx_n_s_np, __pyx_n_s_maxphotons); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(6, 0, 13, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_lfdfiles__lfdfiles_pyx, __pyx_n_s_sflim_decode_photons, 460, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(0, 460, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(1, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__36);
-  __Pyx_GIVEREF(__pyx_tuple__36);
+  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__39);
+  __Pyx_GIVEREF(__pyx_tuple__39);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__37 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(1, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__37);
-  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__40);
+  __Pyx_GIVEREF(__pyx_tuple__40);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__38 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__38)) __PYX_ERR(1, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__38);
-  __Pyx_GIVEREF(__pyx_tuple__38);
+  __pyx_tuple__41 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__41);
+  __Pyx_GIVEREF(__pyx_tuple__41);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__39 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__39)) __PYX_ERR(1, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__39);
-  __Pyx_GIVEREF(__pyx_tuple__39);
+  __pyx_tuple__42 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__42)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__42);
+  __Pyx_GIVEREF(__pyx_tuple__42);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__40 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__40)) __PYX_ERR(1, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__40);
-  __Pyx_GIVEREF(__pyx_tuple__40);
+  __pyx_tuple__43 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__43)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__43);
+  __Pyx_GIVEREF(__pyx_tuple__43);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__41 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__41)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__41);
-  __Pyx_GIVEREF(__pyx_tuple__41);
-  __pyx_codeobj__42 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__41, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__42)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__44 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__44)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__44);
+  __Pyx_GIVEREF(__pyx_tuple__44);
+  __pyx_codeobj__45 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__44, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__45)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  /* AssertionsEnabled.init */
+  __Pyx_init_assertions_enabled();
+
+if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
+
   /* InitThreads.init */
   #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0
 PyEval_InitThreads();
 #endif
 
 if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 1, __pyx_L1_error)
 
@@ -27346,50 +28994,50 @@
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "lfdfiles/_lfdfiles.pyx":45
  * """
  * 
- * __version__ = '2023.4.20'             # <<<<<<<<<<<<<<
+ * __version__ = '2023.8.1'             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_2023_4_20) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_version, __pyx_kp_u_2023_8_1) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
 
   /* "lfdfiles/_lfdfiles.pyx":67
  * 
  * 
  * def simfcsfbd_decode(             # <<<<<<<<<<<<<<
  *     data_t[::] data,
  *     int8_t[:, ::1] bins_out,
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(4); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0_0__pyx_mdef_8lfdfiles_9_lfdfiles_7simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0_0__pyx_mdef_8lfdfiles_9_lfdfiles_9simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_uint16_t_uint32_t, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0_1__pyx_mdef_8lfdfiles_9_lfdfiles_9simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0_1__pyx_mdef_8lfdfiles_9_lfdfiles_11simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_uint16_t_uint64_t, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1_0__pyx_mdef_8lfdfiles_9_lfdfiles_11simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1_0__pyx_mdef_8lfdfiles_9_lfdfiles_13simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_uint32_t_uint32_t, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1_1__pyx_mdef_8lfdfiles_9_lfdfiles_13simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1_1__pyx_mdef_8lfdfiles_9_lfdfiles_15simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_1, __pyx_kp_s_uint32_t_uint64_t, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_8lfdfiles_9_lfdfiles_1simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__31)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_8lfdfiles_9_lfdfiles_1simfcsfbd_decode, 0, __pyx_n_s_simfcsfbd_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__32)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_empty_tuple);
   ((__pyx_FusedFunctionObject *) __pyx_t_2)->__signatures__ = __pyx_t_1;
   __Pyx_GIVEREF(__pyx_t_1);
   __pyx_t_1 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_simfcsfbd_decode, __pyx_t_2) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -27399,25 +29047,25 @@
  * 
  * def simfcsfbd_histogram(             # <<<<<<<<<<<<<<
  *     int8_t[:, ::1] bins,
  *     times_t[::1] times,
  */
   __pyx_t_2 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_8lfdfiles_9_lfdfiles_17simfcsfbd_histogram, 0, __pyx_n_s_simfcsfbd_histogram, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram, 0, __pyx_n_s_simfcsfbd_histogram, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint32_t, __pyx_t_1) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_8lfdfiles_9_lfdfiles_19simfcsfbd_histogram, 0, __pyx_n_s_simfcsfbd_histogram, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_8lfdfiles_9_lfdfiles_21simfcsfbd_histogram, 0, __pyx_n_s_simfcsfbd_histogram, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_uint64_t, __pyx_t_1) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_8lfdfiles_9_lfdfiles_3simfcsfbd_histogram, 0, __pyx_n_s_simfcsfbd_histogram, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__33)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+  __pyx_t_1 = __pyx_FusedFunction_New(&__pyx_mdef_8lfdfiles_9_lfdfiles_3simfcsfbd_histogram, 0, __pyx_n_s_simfcsfbd_histogram, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__34)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_1, __pyx_empty_tuple);
   ((__pyx_FusedFunctionObject *) __pyx_t_1)->__signatures__ = __pyx_t_2;
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_simfcsfbd_histogram, __pyx_t_1) < 0) __PYX_ERR(0, 191, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
@@ -27489,52 +29137,65 @@
  * 
  * def sflim_decode(             # <<<<<<<<<<<<<<
  *     const uint32_t[::1] data,
  *     sflim_t[:, :, :, ::1] sflim,
  */
   __pyx_t_3 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_8lfdfiles_9_lfdfiles_23sflim_decode, 0, __pyx_n_s_sflim_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_0__pyx_mdef_8lfdfiles_9_lfdfiles_25sflim_decode, 0, __pyx_n_s_sflim_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults2), 0)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_2)->__pyx_arg_enabletime = 0;
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_2)->__pyx_arg_maxframes = -1L;
   __Pyx_CyFunction_Defaults(__pyx_defaults2, __pyx_t_2)->__pyx_arg_numthreads = 1;
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_8lfdfiles_9_lfdfiles_32__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_8lfdfiles_9_lfdfiles_34__defaults__);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_uint8_t, __pyx_t_2) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_8lfdfiles_9_lfdfiles_25sflim_decode, 0, __pyx_n_s_sflim_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_fuse_1__pyx_mdef_8lfdfiles_9_lfdfiles_27sflim_decode, 0, __pyx_n_s_sflim_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   if (!__Pyx_CyFunction_InitDefaults(__pyx_t_2, sizeof(__pyx_defaults3), 0)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_t_2)->__pyx_arg_enabletime = 0;
   __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_t_2)->__pyx_arg_maxframes = -1L;
   __Pyx_CyFunction_Defaults(__pyx_defaults3, __pyx_t_2)->__pyx_arg_numthreads = 1;
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_t_4);
-  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_8lfdfiles_9_lfdfiles_34__defaults__);
+  __Pyx_CyFunction_SetDefaultsGetter(__pyx_t_2, __pyx_pf_8lfdfiles_9_lfdfiles_36__defaults__);
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_uint16_t, __pyx_t_2) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_8lfdfiles_9_lfdfiles_5sflim_decode, 0, __pyx_n_s_sflim_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__35)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_2 = __pyx_FusedFunction_New(&__pyx_mdef_8lfdfiles_9_lfdfiles_5sflim_decode, 0, __pyx_n_s_sflim_decode, NULL, __pyx_n_s_lfdfiles__lfdfiles, __pyx_d, ((PyObject *)__pyx_codeobj__36)); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_CyFunction_SetDefaultsTuple(__pyx_t_2, __pyx_t_4);
   ((__pyx_FusedFunctionObject *) __pyx_t_2)->__signatures__ = __pyx_t_3;
   __Pyx_GIVEREF(__pyx_t_3);
   __pyx_t_3 = 0;
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_sflim_decode, __pyx_t_2) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
+  /* "lfdfiles/_lfdfiles.pyx":460
+ * 
+ * 
+ * def sflim_decode_photons(             # <<<<<<<<<<<<<<
+ *     const uint32_t[::1] data,
+ *     uint16_t[:, ::1] photons,
+ */
+  __pyx_t_4 = PyCFunction_NewEx(&__pyx_mdef_8lfdfiles_9_lfdfiles_7sflim_decode_photons, NULL, __pyx_n_s_lfdfiles__lfdfiles); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 460, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sflim_decode_photons, __pyx_t_4) < 0) __PYX_ERR(0, 460, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+
   /* "lfdfiles/_lfdfiles.pyx":1
  * # _lfdfiles.pyx             # <<<<<<<<<<<<<<
  * # distutils: language = c
  * # cython: language_level = 3
  */
-  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   if (PyDict_SetItem(__pyx_t_4, __pyx_kp_u_sflim_decode_line_274, __pyx_kp_u_Decode_Kintex_FLIMbox_data_to_SL) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_4, __pyx_kp_u_sflim_decode_photons_line_460, __pyx_kp_u_Decode_Kintex_FLIMbox_data_to_SL_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_4) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
   /* "View.MemoryView":210
  *         info.obj = self
  * 
  *     __pyx_getbuffer = capsule(<void *> &__pyx_array_getbuffer, "getbuffer(obj, view, flags)")             # <<<<<<<<<<<<<<
@@ -27550,71 +29211,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 287, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__37, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 288, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__38, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 289, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__41, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__39, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 292, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__42, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__40, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 293, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__43, NULL); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_4);
   __pyx_t_4 = 0;
 
   /* "View.MemoryView":317
@@ -30958,15 +32619,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_CyFunction_init(void) {
     __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
     if (unlikely(__pyx_CyFunctionType == NULL)) {
         return -1;
@@ -31341,15 +33005,18 @@
 #endif
 #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
     0,
 #endif
 #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
     0,
 #endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000
+#if PY_VERSION_HEX >= 0x030C0000
+    0,
+#endif
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
     0,
 #endif
 };
 static int __pyx_FusedFunction_init(void) {
     __pyx_FusedFunctionType_type.tp_base = __pyx_CyFunctionType;
     __pyx_FusedFunctionType = __Pyx_FetchCommonType(&__pyx_FusedFunctionType_type);
     if (__pyx_FusedFunctionType == NULL) {
@@ -32663,14 +34330,37 @@
     return result;
 __pyx_fail:
     result.memview = NULL;
     result.data = NULL;
     return result;
 }
 
+/* ObjectToMemviewSlice */
+  static CYTHON_INLINE __Pyx_memviewslice __Pyx_PyObject_to_MemoryviewSlice_d_dc_nn_uint16_t(PyObject *obj, int writable_flag) {
+    __Pyx_memviewslice result = { 0, 0, { 0 }, { 0 }, { 0 } };
+    __Pyx_BufFmt_StackElem stack[1];
+    int axes_specs[] = { (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_FOLLOW), (__Pyx_MEMVIEW_DIRECT | __Pyx_MEMVIEW_CONTIG) };
+    int retcode;
+    if (obj == Py_None) {
+        result.memview = (struct __pyx_memoryview_obj *) Py_None;
+        return result;
+    }
+    retcode = __Pyx_ValidateAndInit_memviewslice(axes_specs, __Pyx_IS_C_CONTIG,
+                                                 (PyBUF_C_CONTIGUOUS | PyBUF_FORMAT) | writable_flag, 2,
+                                                 &__Pyx_TypeInfo_nn_uint16_t, stack,
+                                                 &result, obj);
+    if (unlikely(retcode == -1))
+        goto __pyx_fail;
+    return result;
+__pyx_fail:
+    result.memview = NULL;
+    result.data = NULL;
+    return result;
+}
+
 /* MemviewDtypeToObject */
   static CYTHON_INLINE PyObject *__pyx_memview_get_Py_ssize_t(const char *itemp) {
     return (PyObject *) PyInt_FromSsize_t(*(Py_ssize_t *) itemp);
 }
 static CYTHON_INLINE int __pyx_memview_set_Py_ssize_t(const char *itemp, PyObject *obj) {
     Py_ssize_t value = PyInt_AsSsize_t(obj);
     if ((value == (Py_ssize_t)-1) && PyErr_Occurred())
@@ -32831,15 +34521,15 @@
                         } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
                             return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -33027,15 +34717,15 @@
                         } else if (8 * sizeof(uint16_t) >= 4 * PyLong_SHIFT) {
                             return (uint16_t) (((((((((uint16_t)digits[3]) << PyLong_SHIFT) | (uint16_t)digits[2]) << PyLong_SHIFT) | (uint16_t)digits[1]) << PyLong_SHIFT) | (uint16_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -33223,15 +34913,15 @@
                         } else if (8 * sizeof(uint32_t) >= 4 * PyLong_SHIFT) {
                             return (uint32_t) (((((((((uint32_t)digits[3]) << PyLong_SHIFT) | (uint32_t)digits[2]) << PyLong_SHIFT) | (uint32_t)digits[1]) << PyLong_SHIFT) | (uint32_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -33457,15 +35147,15 @@
                         } else if (8 * sizeof(uint64_t) >= 4 * PyLong_SHIFT) {
                             return (uint64_t) (((((((((uint64_t)digits[3]) << PyLong_SHIFT) | (uint64_t)digits[2]) << PyLong_SHIFT) | (uint64_t)digits[1]) << PyLong_SHIFT) | (uint64_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -33800,15 +35490,15 @@
                         } else if (8 * sizeof(size_t) >= 4 * PyLong_SHIFT) {
                             return (size_t) (((((((((size_t)digits[3]) << PyLong_SHIFT) | (size_t)digits[2]) << PyLong_SHIFT) | (size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -33996,15 +35686,15 @@
                         } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
                             return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
@@ -34192,15 +35882,15 @@
                         } else if (8 * sizeof(char) >= 4 * PyLong_SHIFT) {
                             return (char) (((((((((char)digits[3]) << PyLong_SHIFT) | (char)digits[2]) << PyLong_SHIFT) | (char)digits[1]) << PyLong_SHIFT) | (char)digits[0]));
                         }
                     }
                     break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
```

### Comparing `lfdfiles-2023.4.20/lfdfiles/_lfdfiles.pyx` & `lfdfiles-2023.8.1/lfdfiles/_lfdfiles.pyx`

 * *Files 20% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 """Fast implementations for the lfdfiles module.
 
 :Author: Christoph Gohlke
 :License: BSD 3-Clause
 
 """
 
-__version__ = '2023.4.20'
+__version__ = '2023.8.1'
 
 
 from cython.parallel import parallel, prange
 
 from libc.stdint cimport int8_t, int16_t, uint8_t, uint16_t, uint32_t, uint64_t
 
 cimport openmp
@@ -319,15 +319,15 @@
         (24, 178, 132, 248)
 
     """
     cdef:
         ssize_t size = data.size
         ssize_t address
         openmp.omp_lock_t lock
-        int ret
+        ssize_t ret
 
     if size == 0:
         return
     if sflim.shape[0] != 32 or sflim.shape[1] != 256:
         raise ValueError(
             f'invalid sflim shape {sflim.shape} != (32, 256, height, width)'
         )
@@ -355,15 +355,15 @@
                         raise ValueError(
                             f'no start of frame found for address {address}'
                         )
     finally:
         openmp.omp_destroy_lock(&lock)
 
 
-cdef int _decode_address(
+cdef ssize_t _decode_address(
     const ssize_t address,
     const uint32_t[::1] data,
     sflim_t[:, :, :, ::1] sflim,
     const ssize_t size,
     const uint64_t pixeltime,
     const uint64_t enabletime,
     const ssize_t maxframes,
@@ -450,8 +450,226 @@
         if ph:
             c = address * 4 + 3
             h = (pcc + 32 * ((d & <uint32_t> MASK_WN3) >> SHR_WN3)) % 256
             openmp.omp_set_lock(&lock)
             sflim[c, h, y, x] += 1
             openmp.omp_unset_lock(&lock)
 
-    return <int> frames
+    return frames
+
+
+def sflim_decode_photons(
+    const uint32_t[::1] data,
+    uint16_t[:, ::1] photons,
+    frameshape,
+    const uint64_t pixeltime,
+    uint64_t enabletime=0,
+    const ssize_t maxframes=-1,
+):
+    """Decode Kintex FLIMbox data to SLIM photon array.
+
+    This function is private and may change or be removed in future versions.
+
+    Parameters:
+        data (numpy.ndarray):
+            Data stream from Kintex FLIMbox. A `uint32` array.
+        photons (numpy.ndarray):
+            `uint16` array of shape `(number of photons, 5)`,
+            where arrival time, frame, channel, y and x position are stored for
+            each photon.
+        frameshape (tuple):
+            Shape of image frame.
+        pixeltime (int):
+            Pixel dwell time in FLIMbox units.
+            ``math.ceil(dwelltime * 256 / 255 * frequency_factor * frequency)``
+        enabletime (int):
+            Time in FLIMbox units to wait after detecting enable bit before
+            detecting next enable bit.
+        maxframes (int):
+            Maximum number of image frames to decode.
+
+    Returns:
+        Number of photons decoded.
+
+    Examples:
+        >>> import numpy, math
+        >>> from lfdfiles._lfdfiles import sflim_decode_photons
+        >>> data = numpy.fromfile(
+        ...     '20210123488_100x_NSC_166_TMRM_4_zoom4000_L115.bin',
+        ...      dtype=numpy.uint32
+        ... )
+        >>> frequency = 78e6
+        >>> frequency_factor = 0.9976
+        >>> dwelltime = 16e-6
+        >>> pixeltime = math.ceil(
+        ...     dwelltime * 256 / 255 * frequency_factor * frequency
+        ... )
+        >>> photons = numpy.zeros((2035488, 5), dtype=numpy.uint6)
+        >>> sflim_decode_photons(
+        ...     data, photons, (256, 342), pixeltime=pixeltime, maxframes=20
+        ... )
+        2035488
+        >>> photons[12345].tolist()
+        [205, 3, 2, 181, 51]
+
+    """
+    cdef:
+        ssize_t size = data.size
+        ssize_t ret, height, width, address, np
+        ssize_t maxphotons = photons.shape[0]
+
+    if size == 0:
+        return
+    if photons.shape[1] != 5:
+        raise ValueError(f'invalid photons shape {photons.shape} != (-1, 5)')
+
+    if len(frameshape) != 2 or frameshape[0] < 1 or frameshape[1] < 1:
+        raise ValueError('invalid frameshape')
+
+    height = frameshape[0]
+    width = frameshape[1]
+
+    if enabletime == 0:
+        enabletime = pixeltime * width
+
+    with nogil:
+        np = 0
+        for address in range(8):
+            ret = _decode_address_photons(
+                address,
+                data,
+                photons[np:],
+                size,
+                height,
+                width,
+                pixeltime,
+                enabletime,
+                maxframes,
+            )
+            if ret < 0:
+                raise ValueError(
+                    f'no start of frame found for address {address}'
+                )
+            np += ret
+            if np >= maxphotons:
+                break
+
+    return np
+
+
+cdef ssize_t _decode_address_photons(
+    const ssize_t address,
+    const uint32_t[::1] data,
+    uint16_t[:, ::1] photons,
+    const ssize_t size,
+    const ssize_t height,
+    const ssize_t width,
+    const uint64_t pixeltime,
+    const uint64_t enabletime,
+    const ssize_t maxframes,
+) nogil:
+    """Decode photons' time, channel, and pixel. Return number of photons."""
+    cdef:
+        ssize_t maxphotons = photons.shape[0]
+        ssize_t framesize = width * height
+        ssize_t i, y, x, start, frames, pixelindex, np
+        uint64_t macrotime, macrotime0
+        uint32_t d, pcc, tcc, tcc0, enable, ph
+
+    # seek to first frame
+    start = 0
+    for i in range(size):
+        if (data[i] & <uint32_t> MASK_ENA) >> SHR_ENA:
+            start = i
+            break
+    else:
+        return -1
+
+    tcc0 = data[start] & <uint32_t> MASK_TCC
+    macrotime = tcc0
+    macrotime0 = tcc0
+    frames = 0
+    np = 0
+
+    # loop over all data items
+    for i in range(start, size):
+
+        d = data[i]
+
+        if <uint32_t> address != (d & <uint32_t> MASK_ADR) >> SHR_ADR:
+            continue
+
+        pcc = d & <uint32_t> MASK_PCC
+        tcc = d & <uint32_t> MASK_TCC
+        enable = (d & <uint32_t> MASK_ENA) >> SHR_ENA
+
+        if tcc < tcc0:
+            macrotime += 4096
+        tcc0 = tcc
+
+        if enable and (macrotime - macrotime0 + tcc) > enabletime:
+            if frames == maxframes:
+                break
+            frames += 1
+            macrotime0 = macrotime
+
+        pixelindex = <ssize_t> ((macrotime - macrotime0 + tcc) // pixeltime)
+        if pixelindex >= framesize:
+            # skipped += 1
+            continue
+
+        x = pixelindex % width
+        y = pixelindex // width
+
+        ph = (d & <uint32_t> MASK_PH0) >> SHR_PH0
+        if ph:
+            photons[np, 0] = (
+                (pcc + 32 * ((d & <uint32_t> MASK_WN0) >> SHR_WN0)) % 256
+            )
+            photons[np, 1] = <uint16_t> frames
+            photons[np, 2] = address * 4
+            photons[np, 3] = y
+            photons[np, 4] = x
+            np += 1
+            if np == maxphotons:
+                break
+
+        ph = (d & <uint32_t> MASK_PH1) >> SHR_PH1
+        if ph:
+            photons[np, 0] = (
+                (pcc + 32 * ((d & <uint32_t> MASK_WN1) >> SHR_WN1)) % 256
+            )
+            photons[np, 1] = <uint16_t> frames
+            photons[np, 2] = address * 4 + 1
+            photons[np, 3] = y
+            photons[np, 4] = x
+            np += 1
+            if np == maxphotons:
+                break
+
+        ph = (d & <uint32_t> MASK_PH2) >> SHR_PH2
+        if ph:
+            photons[np, 0] = (
+                (pcc + 32 * ((d & <uint32_t> MASK_WN2) >> SHR_WN2)) % 256
+            )
+            photons[np, 1] = <uint16_t> frames
+            photons[np, 2] = address * 4 + 2
+            photons[np, 3] = y
+            photons[np, 4] = x
+            np += 1
+            if np == maxphotons:
+                break
+
+        ph = (d & <uint32_t> MASK_PH3) >> SHR_PH3
+        if ph:
+            photons[np, 0] = (
+                (pcc + 32 * ((d & <uint32_t> MASK_WN3) >> SHR_WN3)) % 256
+            )
+            photons[np, 1] = <uint16_t> frames
+            photons[np, 2] = address * 4 + 3
+            photons[np, 3] = y
+            photons[np, 4] = x
+            np += 1
+            if np == maxphotons:
+                break
+
+    return np
```

### Comparing `lfdfiles-2023.4.20/lfdfiles/fbd2b64.py` & `lfdfiles-2023.8.1/lfdfiles/fbd2b64.py`

 * *Files identical despite different names*

### Comparing `lfdfiles-2023.4.20/lfdfiles/lfdfiles.py` & `lfdfiles-2023.8.1/lfdfiles/lfdfiles.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,54 +44,61 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.20
+:Version: 2023.8.1
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
 
     python -m pip install -U lfdfiles[all]
 
 Print the console script usage::
 
     python -m lfdfiles --help
 
+The lfdfiles library is type annotated and documented via docstrings.
+
 See `Examples`_ for using the programming interface.
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/lfdfiles>`_.
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
-- `Cython <https://pypi.org/project/cython/>`_ 0.29.34 (build)
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12(optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b4
+- `Cython <https://pypi.org/project/cython/>`_ 0.29.36 (build)
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.1
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.7.18 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile />`_ 2022.9.29 (optional)
-- `Netpbmfile <https://pypi.org/project/netpbmfile />`_ 2023.1.1 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+- `Netpbmfile <https://pypi.org/project/netpbmfile />`_ 2023.6.15 (optional)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
   (optional, for plotting)
-- `Click <https://pypi.python.org/pypi/click>`_ 8.1.3
+- `Click <https://pypi.python.org/pypi/click>`_ 8.1.6
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2023.8.1
+
+- Specify encoding of text files.
+- Fix linting issues.
+
 2023.4.20
 
 - Improve type hints.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2022.9.29
 
@@ -215,15 +222,15 @@
 >>> with BioradPic('_biorad.pic') as f:
 ...     f.totiff('_biorad.tif', compression='zlib')
 
 """
 
 from __future__ import annotations
 
-__version__ = '2023.4.20'
+__version__ = '2023.8.1'
 
 __all__ = [
     'LfdFile',
     'LfdFileSequence',
     'LfdFileError',
     'RawPal',
     'SimfcsVpl',
@@ -357,16 +364,16 @@
 
 class LfdFileRegistry(type):
     """Metaclass to register classes derived from LfdFile."""
 
     classes: list[type[LfdFile]] = []
     """Registered LfdFile classes."""
 
-    def __new__(cls, name, bases, dct):
-        klass = type.__new__(cls, name, bases, dct)
+    def __new__(mcs, name, bases, dct):
+        klass = type.__new__(mcs, name, bases, dct)
         if klass.__name__[:7] != 'LfdFile':
             LfdFileRegistry.classes.append(klass)  # type: ignore
         return klass
 
     @staticmethod
     def sort() -> None:
         """Move SimfcsBin class to end of list.
@@ -410,14 +417,22 @@
 
     _filemode: ClassVar[str] = 'rb'
     """File open mode.
 
     :meta public:
 
     """
+
+    _fileencoding: str | None = None
+    """Text file encoding mode.
+
+    :meta public:
+
+    """
+
     _filepattern: ClassVar[str] = r'.*'
     """Regular expression pattern matching valid file names.
 
     :meta public:
 
     """
     _filesizemin: ClassVar[int] = 16
@@ -551,27 +566,29 @@
                 raise LfdFileError(self, 'no shape')
             self.shape = (len(component_list), *lfdfile.shape)
             self.dtype = lfdfile.dtype
             if component_list[0][1].axes is not None:
                 self.axes = 'S' + component_list[0][1].axes
         else:
             self.components = []
-            self._fh = open(filename, self._filemode)
+            self._fh = open(
+                filename, self._filemode, encoding=self._fileencoding
+            )
             self._fh.seek(_offset)
             try:
                 if self._filesizemin != len(self._fh.read(self._filesizemin)):
                     raise LfdFileError(self, 'file is too small')
             except LfdFileError:
                 self._fh.close()
                 self._fh = None
                 raise
-            except Exception:
+            except Exception as exc:
                 self._fh.close()
                 self._fh = None
-                raise LfdFileError(self, 'not a text file')
+                raise LfdFileError(self, 'not a text file') from exc
 
             self._fh.seek(_offset)
             try:
                 self._init(**kwargs)
             except Exception:
                 if self._fh:
                     self._fh.close()
@@ -950,15 +967,15 @@
     """
 
     _filepattern = r'.*\.(pal|raw|bin|lut)$'
     _figureargs = {'figsize': (6, 1)}
 
     def _init(self, **kwargs) -> None:
         """Verify file size is 768 or 1024."""
-        if self._filesize not in (768, 1024):
+        if self._filesize not in {768, 1024}:
             raise LfdFileError(self)
         self.shape = 256, -1
         self.dtype = numpy.dtype('u1')
         self.axes = 'XS'
 
     def _asarray(
         self, order: Literal['C', 'F'] | None = None, **kwargs
@@ -1223,14 +1240,15 @@
         >>> with SimfcsJrn('simfcs.jrn', lower=True) as f:
         ...     f[1]['paramters for tracking']['samplimg frequency']
         15625
 
     """
 
     _filemode = 'r'
+    _fileencoding = 'cp1252'
     _filepattern = r'.*\.jrn$'
     _noplot = True
 
     # regular expressions of all keys found in journal files
     _keys_ = r"""
         Image experiment
         Correlation expt
@@ -1344,15 +1362,19 @@
                 record[0], self._keys, result=recdict, lower=lower_
             )
             self._records.append(recdict)
         self.close()
 
     def _asarray(self, **kwargs) -> numpy.ndarray:
         """Raise ValueError."""
-        raise ValueError('file does not contain array data')
+        raise ValueError('SimfcsJrn file does not contain array data')
+
+    def _totiff(self, tif: TiffFile, **kwargs) -> None:
+        """Write image data to TIFF file."""
+        raise ValueError('SimfcsJrn file does not contain image data')
 
     @staticmethod
     def _parse_journal(
         journal: str,
         repattern: re.Pattern[str],
         result: dict[str, Any],
         lower: Callable[[str], str],
@@ -1885,15 +1907,15 @@
     SimFCS B&H files contain time-domain fluorescence lifetime histogram data,
     acquired from Becker and Hickl(r) TCSPC cards, or converted from other
     data sources.
     The data are stored consecutively as 256 bins of 256x256 float32 images.
     SimFCS BHZ files are zipped B&H files: a Zip archive containing a single
     B&H file.
     BHZ files are occasionally used to store consecutive 256x256 float32
-    images, e.g., volume data.
+    images, for example, volume data.
 
     Parameters:
         filename: Name of file to open.
 
     Examples:
         >>> with SimfcsBh('simfcs.b&h') as f:
         ...     data = f.asarray()
@@ -2515,14 +2537,18 @@
             raise LfdFileError(self)
 
     def _asarray(self, **kwargs) -> numpy.ndarray:
         """Return firmware as binary string."""
         assert self._fh is not None
         return self._fh.read()
 
+    def _totiff(self, tif: TiffFile, **kwargs) -> None:
+        """Write image data to TIFF file."""
+        raise ValueError('SimfcsFbf file does not contain image data')
+
     def _str(self) -> str | None:
         """Return string with header settings."""
         return format_dict(self._settings)
 
     def __getitem__(self, key: str) -> Any:
         return self._settings[key]
 
@@ -2547,16 +2573,16 @@
     windows, and scanner type are encoded in the last four letters of the
     file name.
     Newer FBD files, where the 3rd character in the file name tag is `0`,
     start with the first 1kB of the firmware file used for the measurement,
     followed by 31kB containing a binary record with measurement settings.
 
     It depends on the application and its setting how to interpret the
-    decoded data, e.g. as time series, line scans, or image frames of FCS
-    or digital frequency domain fluorescence lifetime measurements.
+    decoded data, for example, as time series, line scans, or image frames
+    of FCS or digital frequency domain fluorescence lifetime measurements.
 
     The data word format depends on the device's firmware.
     A common layout is::
 
         |F|E|D|C|B|A|9|8|7|6|5|4|3|2|1|0|  data word bits
                             |-----------|  pcc (cross correlation phase)
                         |---------------|  tcc (cross correlation time)
@@ -2565,15 +2591,15 @@
 
     The data word can be decoded into a cross correlation phase histogram
     index (shown for the 1st harmonics)::
 
         bin = (pmax-1 - (pcc + win * (pmax//windows)) % pmax) // pdiv
 
     - ``bin``, cross correlation phase index (phase histogram bin number).
-    - ``pcc``, ross correlation phase (counter).
+    - ``pcc``, cross correlation phase (counter).
     - ``pmax``, number of entries in cross correlation phase histogram.
     - ``pdiv``, divisor to reduce number of entries in phase histogram.
     - ``win``, arrival window.
     - ``windows``, number of sampling windows.
 
     Parameters:
         filename:
@@ -2933,16 +2959,16 @@
               shift to extract index into lookup table from data word.
 
         """
         bytes_ = 4 if self.is_32bit else 2
         decoder = f'_b{bytes_}w{self.windows}c{self.channels}'
         try:
             return getattr(self, decoder)()
-        except Exception:
-            raise ValueError(f'Decoder{decoder} not implemented')
+        except Exception as exc:
+            raise ValueError(f'Decoder{decoder} not implemented') from exc
 
     @staticmethod
     def _b4w8c4():
         # return parameters to decode 32-bit, 8 windows, 4 channels (Spartan-6)
         # 0b00000000000000000000000000000001 ch0 photon
         # 0b00000000000000000000000000001110 ch0 window
         # 0b00000000000000000000000000010000 ch1 photon
@@ -3303,16 +3329,15 @@
             self.laser_frequency = float(hdr['laser_frequency'])
         if self.laser_factor < 0:
             self.laser_factor = float(hdr['laser_factor'])
         if self.scanner_line_length < 0:
             self.scanner_line_length = int(hdr['line_length'])
         if self.scanner_line_start < 0:
             self.scanner_line_start = int(hdr['x_starting_pixel'])
-        if self.scanner_frame_start < 0:
-            self.scanner_frame_start = 0
+        self.scanner_frame_start = max(self.scanner_frame_start, 0)
 
         if hdr['frame_time'] >= hdr['line_time'] > 1.0:
             if self.frame_size < 0:
                 self.frame_size = round(hdr['frame_time'] / hdr['line_time'])
                 for frame_size in self._header_frame_size:
                     if abs(self.frame_size - frame_size) < 3:
                         self.frame_size = frame_size
@@ -3339,16 +3364,15 @@
                 except (IndexError, KeyError, TypeError):
                     try:
                         dwt = self._header_pixel_dwell_time[
                             hdr['pixel_dwell_time_index']
                         ]
                     except IndexError:
                         dwt = 1.0
-                finally:
-                    self.pixel_dwell_time = dwt
+                self.pixel_dwell_time = dwt
 
         self._data_offset = 65536  # start of encoded data; contains 2 headers
 
     @property
     def pmax(self):
         """Number of entries in cross correlation phase histogram."""
         d = self.decoder_settings
@@ -3488,16 +3512,15 @@
                 aspect = self.frame_size / lines
                 if aspect_range[0] < aspect < aspect_range[1]:
                     frame_markers.append(
                         (int(markers[i]), int(markers[i + 1]) - 1)
                     )
                 else:
                     continue
-                if line_num > lines:
-                    line_num = lines
+                line_num = min(line_num, lines)
             line_num = int(round(line_num))
 
         if not frame_markers:
             # calculate frame duration clusters, assuming few clusters that
             # are narrower and more separated than cluster_size.
             cluster_size = 1024
             clusters: list[list[int]] = []
@@ -3867,15 +3890,15 @@
         if self._filesize % 472 or self._filesize // 472 > 1024:
             raise LfdFileError(self)
         records = []
         for rec in numpy.rec.fromfile(self._fh, self._record_t):
             number = int(rec['number'])
             if number == 0:
                 continue
-            elif number > 25:
+            if number > 25:
                 warnings.warn('corrupted record')
                 continue
             record = self.Record()
             record['number'] = number
             record['title'] = bytes2str(rec['title'][: rec['_title_len']])
             record['nanal'] = int(rec['nanal'])
             record['date'] = '{}.{}.{}'.format(*rec['date'])
@@ -3930,14 +3953,18 @@
         ax.set_ylabel('Delta Phase and Modulation')
         ax.set_xlabel('Frequency (MHz)')
         ax.set_prop_cycle(colors)
         for rec in self._records[:maxplots]:
             ax.semilogx(rec['frequency'], rec['deltap'], '+-')
             ax.semilogx(rec['frequency'], rec['deltam'], '.-')
 
+    def _totiff(self, tif: TiffFile, **kwargs) -> None:
+        """Write image data to TIFF file."""
+        raise ValueError('GlobalsLif file does not contain image data')
+
     def _str(self) -> str | None:
         """Return string with information about file."""
         return f'records: {len(self._records)}'
         # return '\n '.join(f'Record {i}\n{format_dict(r, "  ", trim=0)}'
         #                   for i, r in enumerate(self._records))
 
     def __getitem__(self, key: int) -> Record:
@@ -3971,14 +3998,15 @@
         >>> with GlobalsAscii('FLOP.001') as f:
         ...    print(f['experiment'], f.asarray().shape)
         LIFETIME (5, 20)
 
     """
 
     _filemode = 'r'
+    _fileencoding = 'cp1252'
     _filepattern = r'.*\.(\d){3}$'
     _figureargs = {'figsize': (6, 5)}
 
     _record: dict[str, Any]
 
     def _init(self, **kwargs) -> None:
         """Read file and parse into dictionary and data array."""
@@ -4057,14 +4085,18 @@
         # delta
         ax = pyplot.subplot2grid((3, 1), (2, 0), sharex=ax)
         ax.set_xlim([data[0][0], data[0][-1]])
         ax.semilogx(data[0], data[2], 'bx-')
         ax.semilogx(data[0], data[4] * 100, 'gx-')
         ax.set_xlabel('Frequency (MHz)')
 
+    def _totiff(self, tif: TiffFile, **kwargs) -> None:
+        """Write image data to TIFF file."""
+        raise ValueError('GlobalsAscii file does not contain image data')
+
     def _str(self) -> str:
         """Return string with information about file."""
         return format_dict(self._record)
 
     def __getitem__(self, key: str) -> Any:
         """Return value of key in record."""
         return self._record[key]
@@ -4118,15 +4150,15 @@
         """Read header and metadata from file."""
         assert self._fh is not None
         self.header = h = numpy.rec.fromfile(
             self._fh, self._header_t, shape=1, byteorder='<'  # type: ignore
         )[0]
         if h['signature'] != b'VISTAIMAGE':
             raise LfdFileError(self)
-        if h['version'] not in (4,):
+        if h['version'] != 4:
             log_warning(f'unrecognized VistaIfi file version {h["version"]}')
         self.shape = tuple(int(i) for i in reversed(h['dimensions']))
         if self.shape[0] == 1:
             self.shape = self.shape[1:]
             self.axes = 'YX'
         else:
             self.axes = 'ZYX'
@@ -4248,15 +4280,15 @@
         self._fh.seek(0)
         self.header = h = numpy.rec.fromfile(
             self._fh,  # type: ignore
             self._header_t(numfreq),
             shape=1,
             byteorder='<',
         )[0]
-        if h['version'] not in (1, 13):
+        if h['version'] not in {1, 13}:
             log_warning(f'unrecognized VistaIfli file version {h["version"]}')
         if h['compression'] != 0:
             raise NotImplementedError(
                 f'VistaIfli compression {h["compression"]} not supported'
             )
         shape = tuple(int(i) for i in reversed(h['dimensions'])) + (numfreq,)
         self.shape = shape  # type: ignore
@@ -4475,15 +4507,15 @@
         dtypes = {
             'f': float,
             'i': int,
             'u': int,
             'S': lambda x: str(x, 'latin-1'),
         }
         for name, dtype in self.header.dtype.fields.items():
-            if name not in ('_', 'magic'):
+            if name not in {'_', 'magic'}:
                 dtype = dtypes[dtype[0].kind]
                 metadata[name] = dtype(self.header[name])
         for name, dtype in self.records.dtype.fields.items():
             dtype = dtypes[dtype[0].kind]
             metadata[name] = list(dtype(i) for i in self.records[name])
         update_kwargs(kwargs, contiguous=True, metadata=metadata)
         for data in self.asarray():
@@ -4835,15 +4867,15 @@
         self.origin = ()
         if notes != 0:
             try:
                 self.notes, self.spacing, self.origin = self._notes()
             except Exception as exc:
                 warnings.warn(f'failed to read PIC notes: {exc}')
         ndims = len(self.spacing)
-        if npic > 1 and ndims in (2, 3):
+        if npic > 1 and ndims in {2, 3}:
             self.axes = 'ZYX' if ndims == 3 else 'CYX'
 
     def _notes(
         self,
     ) -> tuple[
         list[tuple[str, int, int, int, int]],
         tuple[float, ...],
@@ -4953,15 +4985,15 @@
         >>> data = numpy.arange(1000000).reshape(100, 100, 100).astype('u1')
         >>> bioradpic_write('_test.pic', data)
         >>> with BioradPic('_test.pic') as f:
         ...     assert_array_equal(f.asarray(), data)
 
     """
     data = numpy.asarray(data)
-    if data.ndim not in (2, 3):
+    if data.ndim not in {2, 3}:
         raise ValueError('data must be 2 or 3 dimensional')
     if data.dtype not in ('uint8', 'uint16'):
         raise ValueError('data type must be uint18 or uint16')
     if data.ndim == 2:
         data.shape = 1, data.shape[0], data.shape[1]
     if name is None:
         name = os.path.split(filename)[-1]
@@ -5094,15 +5126,15 @@
 
     _dtypes: dict[int, str] = {0: 'i1', 1: 'i2', 2: 'f4', 4: 'q8', 5: 'i1'}
 
     def _init(self, **kwargs) -> None:
         """Read CCP4 file header and symboltable."""
         assert self._fh is not None
         header = self._fh.read(1024)
-        if header[208:212] not in (b'MAP ', b'PAM\x00', b'MAP\x00'):
+        if header[208:212] not in {b'MAP ', b'PAM\x00', b'MAP\x00'}:
             raise LfdFileError(self, f' {header[:32]}')
         try:
             (
                 nc,
                 nr,
                 ns,
                 mode,  # data type
@@ -5501,14 +5533,15 @@
         (256, 3) [255 227 155 237]
         >>> with TiffFile('_voxx.map.tif') as f:
         ...     assert_array_equal(f.asarray()[0], data)
 
     """
 
     _filemode = 'r'
+    _fileencoding = 'latin-1'
     _filepattern = r'.*\.map$'
     _figureargs = {'figsize': (6, 1)}
 
     def _init(self, **kwargs) -> None:
         """Verify file starts with numbers."""
         assert self._fh is not None
         try:
@@ -5602,25 +5635,25 @@
     _figureargs = {'figsize': (8, 6)}
 
     # _netpbm: netpbmfile.NetpbmFile
 
     def _init(self, **kwargs) -> None:
         """Validate file is a Netpbm file."""
         assert self._fh is not None
-        if self._fh.read(2) not in (
+        if self._fh.read(2) not in {
             b'P1',
             b'P2',
             b'P3',
             b'P4',
             b'P5',
             b'P6',
             b'P7',
             b'PF',
             b'Pf',
-        ):
+        }:
             raise LfdFileError(self)
         self._fh.seek(0)
 
         import netpbmfile
 
         try:
             self._netpbm = netpbmfile.NetpbmFile(self._fh, **kwargs)
@@ -5639,15 +5672,15 @@
         """Display images stored in file."""
         imshow(self.asarray(**kwargs), figure=figure, title=self._filename)
 
     def _totiff(self, tif: TiffFile, **kwargs) -> None:
         """Write image data to TIFF file."""
         kwargs.update(metadata=None)
         data = self.asarray()
-        if data.ndim > 2 and data.shape[-1] in (3, 4):
+        if data.ndim > 2 and data.shape[-1] in {3, 4}:
             kwargs.update(photometric='rgb', planarconfig='contig')
         tif.write(data, **kwargs)
 
     def _str(self) -> str | None:
         """Return info about Netpbm file as string."""
         # return str(self._netpbm)
 
@@ -5714,15 +5747,15 @@
     def _plot(self, figure, **kwargs) -> None:
         """Display images stored in file."""
         imshow(self.asarray(**kwargs), figure=figure, title=self._filename)
 
     def _totiff(self, tif: TiffFile, **kwargs) -> None:
         """Write image data to TIFF file."""
         data = self.asarray()
-        if data.ndim > 2 and data.shape[-1] in (3, 4):
+        if data.ndim > 2 and data.shape[-1] in {3, 4}:
             kwargs.update(photometric='rgb', planarconfig='contig')
         tif.write(data, **kwargs)
 
     def _str(self) -> str | None:
         """Return info about OIF as string."""
         # return str(self._oif).split('\n', 2)[-1]
 
@@ -5835,20 +5868,20 @@
     _figureargs = {'figsize': (8, 6)}
 
     _series: tifffile.TiffPageSeries
 
     def _init(self, series: int = 0, **kwargs) -> None:
         """Validate file is a TIFF file."""
         assert self._fh is not None
-        if self._fh.read(4) not in (
+        if self._fh.read(4) not in {
             b'MM\x00*',
             b'II*\x00',
             b'MM\x00+',
             b'II+\x00',
-        ):
+        }:
             raise LfdFileError(self)
         self._fh.seek(0)
 
         try:
             self._tif = tifffile.TiffFile(self._fh, **kwargs)
         except Exception as exc:
             raise LfdFileError(self) from exc
@@ -5878,15 +5911,15 @@
             photometric=page.photometric,
             bitspersample=page.bitspersample,
         )
 
     def _totiff(self, tif: TiffFile, **kwargs) -> None:
         """Write image data to TIFF file."""
         data = self.asarray()
-        if data.ndim > 2 and data.shape[-1] in (3, 4):
+        if data.ndim > 2 and data.shape[-1] in {3, 4}:
             kwargs.update(photometric='rgb', planarconfig='contig')
         tif.write(data, **kwargs)
 
     def _str(self) -> str | None:
         """Return TIFF info as string."""
         # return str(self._tif)
 
@@ -6076,14 +6109,15 @@
                 pass
             except Exception as exc:
                 if verbose:
                     print(exc, end=' - ')
         else:
             if verbose:
                 print('failed')
+            continue
         registry.remove(cls)
         registry.insert(0, cls)
 
 
 def determine_shape(
     shape: tuple[int, ...],
     dtype: numpy.dtype[Any] | str,
```

### Comparing `lfdfiles-2023.4.20/lfdfiles.egg-info/PKG-INFO` & `lfdfiles-2023.8.1/lfdfiles.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lfdfiles
-Version: 2023.4.20
+Version: 2023.8.1
 Summary: Laboratory for Fluorescence Dynamics (LFD) file formats
 Home-page: https://www.cgohlke.com
 Author: Christoph Gohlke
 Author-email: cgohlke@cgohlke.com
 License: BSD
 Project-URL: Bug Tracker, https://github.com/cgohlke/lfdfiles/issues
 Project-URL: Source Code, https://github.com/cgohlke/lfdfiles
@@ -15,15 +15,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Cython
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
+Description-Content-Type: text/x-rst
 Provides-Extra: all
 License-File: LICENSE
 
 Laboratory for Fluorescence Dynamics (LFD) file formats
 =======================================================
 
 Lfdfiles is a Python library and console script for reading, writing,
@@ -39,54 +41,61 @@
 - Vaa3D RAW
 - Bio-Rad(r) PIC
 - ISS Vista IFLI, IFI
 - FlimFast FLIF
 
 :Author: `Christoph Gohlke <https://www.cgohlke.com>`_
 :License: BSD 3-Clause
-:Version: 2023.4.20
+:Version: 2023.8.1
 
 Quickstart
 ----------
 
 Install the lfdfiles package and all dependencies from the
 `Python Package Index <https://pypi.org/project/lfdfiles/>`_::
 
     python -m pip install -U lfdfiles[all]
 
 Print the console script usage::
 
     python -m lfdfiles --help
 
+The lfdfiles library is type annotated and documented via docstrings.
+
 See `Examples`_ for using the programming interface.
 
 Source code and support are available on
 `GitHub <https://github.com/cgohlke/lfdfiles>`_.
 
 Requirements
 ------------
 
 This revision was tested with the following requirements and dependencies
 (other versions may work):
 
-- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.3
-- `Cython <https://pypi.org/project/cython/>`_ 0.29.34 (build)
-- `NumPy <https://pypi.org/project/numpy/>`_ 1.23.5
-- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.4.12(optional)
+- `CPython <https://www.python.org>`_ 3.9.13, 3.10.11, 3.11.4, 3.12.0b4
+- `Cython <https://pypi.org/project/cython/>`_ 0.29.36 (build)
+- `NumPy <https://pypi.org/project/numpy/>`_ 1.25.1
+- `Tifffile <https://pypi.org/project/tifffile/>`_ 2023.7.18 (optional)
 - `Czifile <https://pypi.org/project/czifile/>`_ 2019.7.2 (optional)
 - `Oiffile <https://pypi.org/project/oiffile />`_ 2022.9.29 (optional)
-- `Netpbmfile <https://pypi.org/project/netpbmfile />`_ 2023.1.1 (optional)
-- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.1
+- `Netpbmfile <https://pypi.org/project/netpbmfile />`_ 2023.6.15 (optional)
+- `Matplotlib <https://pypi.org/project/matplotlib/>`_ 3.7.2
   (optional, for plotting)
-- `Click <https://pypi.python.org/pypi/click>`_ 8.1.3
+- `Click <https://pypi.python.org/pypi/click>`_ 8.1.6
   (optional, for command line apps)
 
 Revisions
 ---------
 
+2023.8.1
+
+- Specify encoding of text files.
+- Fix linting issues.
+
 2023.4.20
 
 - Improve type hints.
 - Drop support for Python 3.8 and numpy < 1.21 (NEP29).
 
 2022.9.29
```

### Comparing `lfdfiles-2023.4.20/setup.py` & `lfdfiles-2023.8.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,18 +15,18 @@
     # return first match for pattern in code
     match = re.search(pattern, code, flags)
     if match is None:
         raise ValueError(f'{pattern!r} not found')
     return match.groups()[0]
 
 
-with open('lfdfiles/lfdfiles.py') as fh:
+with open('lfdfiles/lfdfiles.py', encoding='utf-8') as fh:
     code = fh.read()
 
-version = search(r"__version__ = '(.*?)'", code)
+version = search(r"__version__ = '(.*?)'", code).replace('.x.x', '.dev0')
 version += ('.' + buildnumber) if buildnumber else ''
 
 description = search(r'"""(.*)\.(?:\r\n|\r|\n)', code)
 
 readme = search(
     r'(?:\r\n|\r|\n){2}"""(.*)"""(?:\r\n|\r|\n){2}from __future__',
     code,
@@ -35,40 +35,40 @@
 readme = '\n'.join(
     [description, '=' * len(description)] + readme.splitlines()[1:]
 )
 
 if 'sdist' in sys.argv:
     # update README, LICENSE, and CHANGES files
 
-    with open('README.rst', 'w') as fh:
+    with open('README.rst', 'w', encoding='utf-8') as fh:
         fh.write(readme)
 
     license = search(
         r'(# Copyright.*?(?:\r\n|\r|\n))(?:\r\n|\r|\n)+""',
         code,
         re.MULTILINE | re.DOTALL,
     )
     license = license.replace('# ', '').replace('#', '')
 
-    with open('LICENSE', 'w') as fh:
+    with open('LICENSE', 'w', encoding='utf-8') as fh:
         fh.write('BSD 3-Clause License\n\n')
         fh.write(license)
 
     revisions = search(
         r'(?:\r\n|\r|\n){2}(Revisions.*)- \.\.\.',
         readme,
         re.MULTILINE | re.DOTALL,
     ).strip()
 
-    with open('CHANGES.rst') as fh:
+    with open('CHANGES.rst', encoding='utf-8') as fh:
         old = fh.read()
 
     d = revisions.splitlines()[-1]
     old = old.split(d)[-1]
-    with open('CHANGES.rst', 'w') as fh:
+    with open('CHANGES.rst', 'w', encoding='utf-8') as fh:
         fh.write(revisions.strip())
         fh.write(old)
 
 
 class build_ext(_build_ext):
     """Delay import numpy until build."""
 
@@ -90,15 +90,15 @@
 
     ext = '.pyx'
 except ImportError:
     ext = '.c'
 
 if sys.platform == 'win32':
     extra_compile_args = ['/openmp']
-    extra_link_args = []
+    extra_link_args: list[str] = []
 elif sys.platform == 'darwin':
     # https://mac.r-project.org/openmp/
     extra_compile_args = ['-Xclang', '-fopenmp']
     extra_link_args = ['-lomp']
 else:
     extra_compile_args = ['-fopenmp']
     extra_link_args = ['-fopenmp']
@@ -114,14 +114,15 @@
 
 setup(
     name='lfdfiles',
     version=version,
     license='BSD',
     description=description,
     long_description=readme,
+    long_description_content_type='text/x-rst',
     author='Christoph Gohlke',
     author_email='cgohlke@cgohlke.com',
     url='https://www.cgohlke.com',
     project_urls={
         'Bug Tracker': 'https://github.com/cgohlke/lfdfiles/issues',
         'Source Code': 'https://github.com/cgohlke/lfdfiles',
         # 'Documentation': 'https://',
@@ -157,9 +158,10 @@
         'Intended Audience :: Developers',
         'Operating System :: OS Independent',
         'Programming Language :: Cython',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

