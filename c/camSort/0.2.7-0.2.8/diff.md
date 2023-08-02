# Comparing `tmp/camSort-0.2.7.tar.gz` & `tmp/camSort-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/macbook/Desktop/camSort-project/dist/.tmp-fb4qa7gn/camSort-0.2.7.tar", last modified: Tue Aug  1 10:25:52 2023, max compression
+gzip compressed data, was "dist/camSort-0.2.8.tar", last modified: Wed Aug  2 09:35:50 2023, max compression
```

## Comparing `camSort-0.2.7.tar` & `camSort-0.2.8.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 10:25:52.000000 camSort-0.2.7/
--rw-r--r--   0 macbook    (501) staff       (20)     2049 2023-08-01 10:25:52.000000 camSort-0.2.7/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)     1529 2023-08-01 07:52:20.000000 camSort-0.2.7/README.md
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 10:25:52.000000 camSort-0.2.7/camSort/
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-01 10:25:41.000000 camSort-0.2.7/camSort/__init__.py
--rw-r--r--   0 macbook    (501) staff       (20)   381141 2023-08-01 10:25:11.000000 camSort-0.2.7/camSort/camSort.c
--rw-r--r--   0 macbook    (501) staff       (20)      655 2023-08-01 09:32:11.000000 camSort-0.2.7/camSort/camSort.pyx
-drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-01 10:25:52.000000 camSort-0.2.7/camSort.egg-info/
--rw-r--r--   0 macbook    (501) staff       (20)     2049 2023-08-01 10:25:52.000000 camSort-0.2.7/camSort.egg-info/PKG-INFO
--rw-r--r--   0 macbook    (501) staff       (20)      245 2023-08-01 10:25:52.000000 camSort-0.2.7/camSort.egg-info/SOURCES.txt
--rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-01 10:25:52.000000 camSort-0.2.7/camSort.egg-info/dependency_links.txt
--rw-r--r--   0 macbook    (501) staff       (20)       24 2023-08-01 10:25:52.000000 camSort-0.2.7/camSort.egg-info/requires.txt
--rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-01 10:25:52.000000 camSort-0.2.7/camSort.egg-info/top_level.txt
--rw-r--r--   0 macbook    (501) staff       (20)       99 2023-08-01 09:18:16.000000 camSort-0.2.7/pyproject.toml
--rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-01 10:25:52.000000 camSort-0.2.7/setup.cfg
--rw-r--r--   0 macbook    (501) staff       (20)     1094 2023-08-01 10:25:43.000000 camSort-0.2.7/setup.py
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-02 09:35:50.000000 camSort-0.2.8/
+-rw-r--r--   0 macbook    (501) staff       (20)     2435 2023-08-02 09:35:50.000000 camSort-0.2.8/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)     1529 2023-08-01 07:52:20.000000 camSort-0.2.8/README.md
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort/
+-rw-r--r--   0 macbook    (501) staff       (20)   235338 2023-08-02 09:34:25.000000 camSort-0.2.8/camSort/stringSort.c
+drwxr-xr-x   0 macbook    (501) staff       (20)        0 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/
+-rw-r--r--   0 macbook    (501) staff       (20)     2435 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/PKG-INFO
+-rw-r--r--   0 macbook    (501) staff       (20)      208 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/SOURCES.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        1 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/dependency_links.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       24 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/requires.txt
+-rw-r--r--   0 macbook    (501) staff       (20)        8 2023-08-02 09:35:50.000000 camSort-0.2.8/camSort.egg-info/top_level.txt
+-rw-r--r--   0 macbook    (501) staff       (20)       99 2023-08-02 08:57:15.000000 camSort-0.2.8/pyproject.toml
+-rw-r--r--   0 macbook    (501) staff       (20)       38 2023-08-02 09:35:50.000000 camSort-0.2.8/setup.cfg
+-rw-r--r--   0 macbook    (501) staff       (20)     1043 2023-08-02 09:34:18.000000 camSort-0.2.8/setup.py
```

### Comparing `camSort-0.2.7/PKG-INFO` & `camSort-0.2.8/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.2.7
+Version: 0.2.8
 Summary: make sorted() fast for strings
+Home-page: UNKNOWN
 Author: ['cameronbae / cameron jay']
 Author-email: <contact@camjay.io>
+License: UNKNOWN
+Description: 
+        # camSort
+        
+        Working on `python 3.7.1`!
+        
+        `camSort` is a Python library that makes sorted() look slow while also using sorted(). It's built on Cython, and provides preallocation to string sorting by using a custom key calculation for each string. Normal key calculation and object creation are often computationally expensive—but here we optimize that with Cython >:)!
+        
+        ## Overview
+        
+        The `camSort` library sorts a list of strings by creating a custom object for each string. This custom object, `StringWithKey`, holds the string and a unique key calculated from it. The key is a long integer derived from the sum of Unicode code points of the characters in the string, and the string's length.
+        
+        The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
+        
+        The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
+        
+        ## Installation
+        
+        ```pip install camSort``` or compile locally :)
+        
+        ## Usage
+        
+        ```python
+        import camSort
+        # or
+        from camSort import sortStrings
+        
+        myList = ['your', 'list', 'of', 'strings', ':)!']
+        
+        sortedStrings = camSort.sortStrings(myList)
+        # or
+        sortedStrings = sortStrings(myList)
+        
+        ```
+        
+        ## Performance
+        
+        Average output on my 2017 macbook pro:
+            (1 million strings, with a random legnth of 1 to 1000 chararacters)
+        
+        Time taken by Python sorted(): 56.08621883392334 seconds
+        Time taken by camSort: 6.356221914291382 seconds
 Keywords: python,sorted,sort,camSort
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-
-
-# camSort
-
-Working on `python 3.7.1`!
-
-`camSort` is a Python library that makes sorted() look slow while also using sorted(). It's built on Cython, and provides preallocation to string sorting by using a custom key calculation for each string. Normal key calculation and object creation are often computationally expensive—but here we optimize that with Cython >:)!
-
-## Overview
-
-The `camSort` library sorts a list of strings by creating a custom object for each string. This custom object, `StringWithKey`, holds the string and a unique key calculated from it. The key is a long integer derived from the sum of Unicode code points of the characters in the string, and the string's length.
-
-The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
-
-The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
-
-## Installation
-
-```pip install camSort``` or compile locally :)
-
-## Usage
-
-```python
-import camSort
-# or
-from camSort import sortStrings
-
-myList = ['your', 'list', 'of', 'strings', ':)!']
-
-sortedStrings = camSort.sortStrings(myList)
-# or
-sortedStrings = sortStrings(myList)
-
-```
-
-## Performance
-
-Average output on my 2017 macbook pro:
-    (1 million strings, with a random legnth of 1 to 1000 chararacters)
-
-Time taken by Python sorted(): 56.08621883392334 seconds
-Time taken by camSort: 6.356221914291382 seconds
```

### Comparing `camSort-0.2.7/README.md` & `camSort-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `camSort-0.2.7/camSort/camSort.c` & `camSort-0.2.8/camSort/stringSort.c`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,36 @@
-/* Generated by Cython 3.0.0 */
+/* Generated by Cython 0.29.21 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
-        "name": "camSort.camSort",
+        "name": "camSort.stringSort",
         "sources": [
-            "camSort/camSort.pyx"
+            "camSort/stringSort.pyx"
         ]
     },
-    "module_name": "camSort.camSort"
+    "module_name": "camSort.stringSort"
 }
 END: Cython Metadata */
 
-#ifndef PY_SSIZE_T_CLEAN
 #define PY_SSIZE_T_CLEAN
-#endif /* PY_SSIZE_T_CLEAN */
-#if defined(CYTHON_LIMITED_API) && 0
-  #ifndef Py_LIMITED_API
-    #if CYTHON_LIMITED_API+0 > 0x03030000
-      #define Py_LIMITED_API CYTHON_LIMITED_API
-    #else
-      #define Py_LIMITED_API 0x03030000
-    #endif
-  #endif
-#endif
-
 #include "Python.h"
 #ifndef Py_PYTHON_H
     #error Python headers needed to compile C extensions, please install development version of Python.
-#elif PY_VERSION_HEX < 0x02070000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
-    #error Cython requires Python 2.7+ or Python 3.3+.
+#elif PY_VERSION_HEX < 0x02060000 || (0x03000000 <= PY_VERSION_HEX && PY_VERSION_HEX < 0x03030000)
+    #error Cython requires Python 2.6+ or Python 3.3+.
 #else
-#define CYTHON_ABI "3_0_0"
-#define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
-#define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030000F0
+#define CYTHON_ABI "0_29_21"
+#define CYTHON_HEX_VERSION 0x001D15F0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
-#if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
+#if !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
     #define __stdcall
   #endif
   #ifndef __cdecl
     #define __cdecl
   #endif
   #ifndef __fastcall
@@ -55,90 +41,30 @@
   #define DL_IMPORT(t) t
 #endif
 #ifndef DL_EXPORT
   #define DL_EXPORT(t) t
 #endif
 #define __PYX_COMMA ,
 #ifndef HAVE_LONG_LONG
-  #define HAVE_LONG_LONG
+  #if PY_VERSION_HEX >= 0x02070000
+    #define HAVE_LONG_LONG
+  #endif
 #endif
 #ifndef PY_LONG_LONG
   #define PY_LONG_LONG LONG_LONG
 #endif
 #ifndef Py_HUGE_VAL
   #define Py_HUGE_VAL HUGE_VAL
 #endif
-#if defined(GRAALVM_PYTHON)
-  /* For very preliminary testing purposes. Most variables are set the same as PyPy.
-     The existence of this section does not imply that anything works or is even tested */
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_LIMITED_API 0
-  #define CYTHON_COMPILING_IN_GRAAL 1
-  #define CYTHON_COMPILING_IN_NOGIL 0
-  #undef CYTHON_USE_TYPE_SLOTS
-  #define CYTHON_USE_TYPE_SLOTS 0
-  #undef CYTHON_USE_TYPE_SPECS
-  #define CYTHON_USE_TYPE_SPECS 0
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #if PY_VERSION_HEX < 0x03050000
-    #undef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 0
-  #elif !defined(CYTHON_USE_ASYNC_SLOTS)
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #undef CYTHON_USE_UNICODE_INTERNALS
-  #define CYTHON_USE_UNICODE_INTERNALS 0
-  #undef CYTHON_USE_UNICODE_WRITER
-  #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #undef CYTHON_AVOID_BORROWED_REFS
-  #define CYTHON_AVOID_BORROWED_REFS 1
-  #undef CYTHON_ASSUME_SAFE_MACROS
-  #define CYTHON_ASSUME_SAFE_MACROS 0
-  #undef CYTHON_UNPACK_METHODS
-  #define CYTHON_UNPACK_METHODS 0
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_GIL
-  #define CYTHON_FAST_GIL 0
-  #undef CYTHON_METH_FASTCALL
-  #define CYTHON_METH_FASTCALL 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP487_INIT_SUBCLASS
-    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
-  #endif
-  #undef CYTHON_PEP489_MULTI_PHASE_INIT
-  #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #undef CYTHON_USE_MODULE_STATE
-  #define CYTHON_USE_MODULE_STATE 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE 0
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PYPY_VERSION)
+#ifdef PYPY_VERSION
   #define CYTHON_COMPILING_IN_PYPY 1
+  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_LIMITED_API 0
-  #define CYTHON_COMPILING_IN_GRAAL 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
   #define CYTHON_USE_TYPE_SLOTS 0
-  #undef CYTHON_USE_TYPE_SPECS
-  #define CYTHON_USE_TYPE_SPECS 0
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #if PY_VERSION_HEX < 0x03050000
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
@@ -155,111 +81,35 @@
   #define CYTHON_AVOID_BORROWED_REFS 1
   #undef CYTHON_ASSUME_SAFE_MACROS
   #define CYTHON_ASSUME_SAFE_MACROS 0
   #undef CYTHON_UNPACK_METHODS
   #define CYTHON_UNPACK_METHODS 0
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_GIL
-  #define CYTHON_FAST_GIL 0
-  #undef CYTHON_METH_FASTCALL
-  #define CYTHON_METH_FASTCALL 0
-  #undef CYTHON_FAST_PYCALL
-  #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP487_INIT_SUBCLASS
-    #define CYTHON_PEP487_INIT_SUBCLASS (PY_MAJOR_VERSION >= 3)
-  #endif
-  #if PY_VERSION_HEX < 0x03090000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #undef CYTHON_USE_MODULE_STATE
-  #define CYTHON_USE_MODULE_STATE 0
-  #undef CYTHON_USE_TP_FINALIZE
-  #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1 && PYPY_VERSION_NUM >= 0x07030C00)
-  #undef CYTHON_USE_DICT_VERSIONS
-  #define CYTHON_USE_DICT_VERSIONS 0
-  #undef CYTHON_USE_EXC_INFO_STACK
-  #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(CYTHON_LIMITED_API)
-  #define CYTHON_COMPILING_IN_PYPY 0
-  #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_LIMITED_API 1
-  #define CYTHON_COMPILING_IN_GRAAL 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
-  #undef CYTHON_CLINE_IN_TRACEBACK
-  #define CYTHON_CLINE_IN_TRACEBACK 0
-  #undef CYTHON_USE_TYPE_SLOTS
-  #define CYTHON_USE_TYPE_SLOTS 0
-  #undef CYTHON_USE_TYPE_SPECS
-  #define CYTHON_USE_TYPE_SPECS 1
-  #undef CYTHON_USE_PYTYPE_LOOKUP
-  #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #undef CYTHON_USE_ASYNC_SLOTS
-  #define CYTHON_USE_ASYNC_SLOTS 0
-  #undef CYTHON_USE_PYLIST_INTERNALS
-  #define CYTHON_USE_PYLIST_INTERNALS 0
-  #undef CYTHON_USE_UNICODE_INTERNALS
-  #define CYTHON_USE_UNICODE_INTERNALS 0
-  #ifndef CYTHON_USE_UNICODE_WRITER
-    #define CYTHON_USE_UNICODE_WRITER 0
-  #endif
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
-  #ifndef CYTHON_AVOID_BORROWED_REFS
-    #define CYTHON_AVOID_BORROWED_REFS 0
-  #endif
-  #undef CYTHON_ASSUME_SAFE_MACROS
-  #define CYTHON_ASSUME_SAFE_MACROS 0
-  #undef CYTHON_UNPACK_METHODS
-  #define CYTHON_UNPACK_METHODS 0
-  #undef CYTHON_FAST_THREAD_STATE
-  #define CYTHON_FAST_THREAD_STATE 0
-  #undef CYTHON_FAST_GIL
-  #define CYTHON_FAST_GIL 0
-  #undef CYTHON_METH_FASTCALL
-  #define CYTHON_METH_FASTCALL 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP487_INIT_SUBCLASS
-    #define CYTHON_PEP487_INIT_SUBCLASS 1
-  #endif
   #undef CYTHON_PEP489_MULTI_PHASE_INIT
   #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #undef CYTHON_USE_MODULE_STATE
-  #define CYTHON_USE_MODULE_STATE 1
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
-  #endif
-#elif defined(PY_NOGIL)
+#elif defined(PYSTON_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
-  #define CYTHON_COMPILING_IN_LIMITED_API 0
-  #define CYTHON_COMPILING_IN_GRAAL 0
-  #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
-  #ifndef CYTHON_USE_ASYNC_SLOTS
-    #define CYTHON_USE_ASYNC_SLOTS 1
-  #endif
+  #undef CYTHON_USE_ASYNC_SLOTS
+  #define CYTHON_USE_ASYNC_SLOTS 0
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
@@ -274,55 +124,54 @@
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
-  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
+  #undef CYTHON_PEP489_MULTI_PHASE_INIT
+  #define CYTHON_PEP489_MULTI_PHASE_INIT 0
+  #undef CYTHON_USE_TP_FINALIZE
+  #define CYTHON_USE_TP_FINALIZE 0
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
+  #define CYTHON_COMPILING_IN_PYSTON 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
-  #define CYTHON_COMPILING_IN_LIMITED_API 0
-  #define CYTHON_COMPILING_IN_GRAAL 0
-  #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
-  #ifndef CYTHON_USE_TYPE_SPECS
-    #define CYTHON_USE_TYPE_SPECS 0
-  #endif
-  #ifndef CYTHON_USE_PYTYPE_LOOKUP
+  #if PY_VERSION_HEX < 0x02070000
+    #undef CYTHON_USE_PYTYPE_LOOKUP
+    #define CYTHON_USE_PYTYPE_LOOKUP 0
+  #elif !defined(CYTHON_USE_PYTYPE_LOOKUP)
     #define CYTHON_USE_PYTYPE_LOOKUP 1
   #endif
   #if PY_MAJOR_VERSION < 3
     #undef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 0
   #elif !defined(CYTHON_USE_ASYNC_SLOTS)
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
-  #ifndef CYTHON_USE_PYLONG_INTERNALS
+  #if PY_VERSION_HEX < 0x02070000
+    #undef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #elif !defined(CYTHON_USE_PYLONG_INTERNALS)
     #define CYTHON_USE_PYLONG_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_PYLIST_INTERNALS
     #define CYTHON_USE_PYLIST_INTERNALS 1
   #endif
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
-  #if PY_VERSION_HEX < 0x030300F0 || PY_VERSION_HEX >= 0x030B00A2
+  #if PY_VERSION_HEX < 0x030300F0
     #undef CYTHON_USE_UNICODE_WRITER
     #define CYTHON_USE_UNICODE_WRITER 0
   #elif !defined(CYTHON_USE_UNICODE_WRITER)
     #define CYTHON_USE_UNICODE_WRITER 1
   #endif
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
@@ -332,68 +181,35 @@
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #ifndef CYTHON_FAST_THREAD_STATE
     #define CYTHON_FAST_THREAD_STATE 1
   #endif
-  #ifndef CYTHON_FAST_GIL
-    #define CYTHON_FAST_GIL (PY_MAJOR_VERSION < 3 || PY_VERSION_HEX >= 0x03060000 && PY_VERSION_HEX < 0x030C00A6)
-  #endif
-  #ifndef CYTHON_METH_FASTCALL
-    #define CYTHON_METH_FASTCALL (PY_VERSION_HEX >= 0x030700A1)
-  #endif
   #ifndef CYTHON_FAST_PYCALL
     #define CYTHON_FAST_PYCALL 1
   #endif
-  #ifndef CYTHON_PEP487_INIT_SUBCLASS
-    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
+    #define CYTHON_PEP489_MULTI_PHASE_INIT (PY_VERSION_HEX >= 0x03050000)
   #endif
-  #if PY_VERSION_HEX < 0x03050000
-    #undef CYTHON_PEP489_MULTI_PHASE_INIT
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 0
-  #elif !defined(CYTHON_PEP489_MULTI_PHASE_INIT)
-    #define CYTHON_PEP489_MULTI_PHASE_INIT 1
-  #endif
-  #ifndef CYTHON_USE_MODULE_STATE
-    #define CYTHON_USE_MODULE_STATE 0
-  #endif
-  #if PY_VERSION_HEX < 0x030400a1
-    #undef CYTHON_USE_TP_FINALIZE
-    #define CYTHON_USE_TP_FINALIZE 0
-  #elif !defined(CYTHON_USE_TP_FINALIZE)
-    #define CYTHON_USE_TP_FINALIZE 1
-  #endif
-  #if PY_VERSION_HEX < 0x030600B1
-    #undef CYTHON_USE_DICT_VERSIONS
-    #define CYTHON_USE_DICT_VERSIONS 0
-  #elif !defined(CYTHON_USE_DICT_VERSIONS)
-    #define CYTHON_USE_DICT_VERSIONS  (PY_VERSION_HEX < 0x030C00A5)
-  #endif
-  #if PY_VERSION_HEX < 0x030700A3
-    #undef CYTHON_USE_EXC_INFO_STACK
-    #define CYTHON_USE_EXC_INFO_STACK 0
-  #elif !defined(CYTHON_USE_EXC_INFO_STACK)
-    #define CYTHON_USE_EXC_INFO_STACK 1
+  #ifndef CYTHON_USE_TP_FINALIZE
+    #define CYTHON_USE_TP_FINALIZE (PY_VERSION_HEX >= 0x030400a1)
   #endif
-  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
-    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #ifndef CYTHON_USE_DICT_VERSIONS
+    #define CYTHON_USE_DICT_VERSIONS (PY_VERSION_HEX >= 0x030600B1)
+  #endif
+  #ifndef CYTHON_USE_EXC_INFO_STACK
+    #define CYTHON_USE_EXC_INFO_STACK (PY_VERSION_HEX >= 0x030700A3)
   #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
-#if !defined(CYTHON_VECTORCALL)
-#define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
-#endif
-#define CYTHON_BACKPORT_VECTORCALL (CYTHON_METH_FASTCALL && PY_VERSION_HEX < 0x030800B1)
 #if CYTHON_USE_PYLONG_INTERNALS
-  #if PY_MAJOR_VERSION < 3
-    #include "longintrepr.h"
-  #endif
+  #include "longintrepr.h"
   #undef SHIFT
   #undef BASE
   #undef MASK
   #ifdef SIZEOF_VOID_P
     enum { __pyx_check_sizeof_voidp = 1 / (int)(SIZEOF_VOID_P == sizeof(void*)) };
   #endif
 #endif
@@ -411,128 +227,78 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_RESTRICT restrict
   #else
     #define CYTHON_RESTRICT
   #endif
 #endif
 #ifndef CYTHON_UNUSED
-  #if defined(__cplusplus)
-    /* for clang __has_cpp_attribute(maybe_unused) is true even before C++17
-     * but leads to warnings with -pedantic, since it is a C++17 feature */
-    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
-      #if __has_cpp_attribute(maybe_unused)
-        #define CYTHON_UNUSED [[maybe_unused]]
-      #endif
-    #endif
-  #endif
-#endif
-#ifndef CYTHON_UNUSED
 # if defined(__GNUC__)
 #   if !(defined(__cplusplus)) || (__GNUC__ > 3 || (__GNUC__ == 3 && __GNUC_MINOR__ >= 4))
 #     define CYTHON_UNUSED __attribute__ ((__unused__))
 #   else
 #     define CYTHON_UNUSED
 #   endif
 # elif defined(__ICC) || (defined(__INTEL_COMPILER) && !defined(_MSC_VER))
 #   define CYTHON_UNUSED __attribute__ ((__unused__))
 # else
 #   define CYTHON_UNUSED
 # endif
 #endif
-#ifndef CYTHON_UNUSED_VAR
+#ifndef CYTHON_MAYBE_UNUSED_VAR
 #  if defined(__cplusplus)
-     template<class T> void CYTHON_UNUSED_VAR( const T& ) { }
+     template<class T> void CYTHON_MAYBE_UNUSED_VAR( const T& ) { }
 #  else
-#    define CYTHON_UNUSED_VAR(x) (void)(x)
+#    define CYTHON_MAYBE_UNUSED_VAR(x) (void)(x)
 #  endif
 #endif
-#ifndef CYTHON_MAYBE_UNUSED_VAR
-  #define CYTHON_MAYBE_UNUSED_VAR(x) CYTHON_UNUSED_VAR(x)
-#endif
 #ifndef CYTHON_NCP_UNUSED
 # if CYTHON_COMPILING_IN_CPYTHON
 #  define CYTHON_NCP_UNUSED
 # else
 #  define CYTHON_NCP_UNUSED CYTHON_UNUSED
 # endif
 #endif
 #define __Pyx_void_to_None(void_result) ((void)(void_result), Py_INCREF(Py_None), Py_None)
 #ifdef _MSC_VER
     #ifndef _MSC_STDINT_H_
         #if _MSC_VER < 1300
-            typedef unsigned char     uint8_t;
-            typedef unsigned short    uint16_t;
-            typedef unsigned int      uint32_t;
-        #else
-            typedef unsigned __int8   uint8_t;
-            typedef unsigned __int16  uint16_t;
-            typedef unsigned __int32  uint32_t;
-        #endif
-    #endif
-    #if _MSC_VER < 1300
-        #ifdef _WIN64
-            typedef unsigned long long  __pyx_uintptr_t;
+           typedef unsigned char     uint8_t;
+           typedef unsigned int      uint32_t;
         #else
-            typedef unsigned int        __pyx_uintptr_t;
-        #endif
-    #else
-        #ifdef _WIN64
-            typedef unsigned __int64    __pyx_uintptr_t;
-        #else
-            typedef unsigned __int32    __pyx_uintptr_t;
+           typedef unsigned __int8   uint8_t;
+           typedef unsigned __int32  uint32_t;
         #endif
     #endif
 #else
-    #include <stdint.h>
-    typedef uintptr_t  __pyx_uintptr_t;
+   #include <stdint.h>
 #endif
 #ifndef CYTHON_FALLTHROUGH
-  #if defined(__cplusplus)
-    /* for clang __has_cpp_attribute(fallthrough) is true even before C++17
-     * but leads to warnings with -pedantic, since it is a C++17 feature */
-    #if ((defined(_MSVC_LANG) && _MSVC_LANG >= 201703L) || __cplusplus >= 201703L)
-      #if __has_cpp_attribute(fallthrough)
-        #define CYTHON_FALLTHROUGH [[fallthrough]]
-      #endif
-    #endif
-    #ifndef CYTHON_FALLTHROUGH
-      #if __has_cpp_attribute(clang::fallthrough)
-        #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
-      #elif __has_cpp_attribute(gnu::fallthrough)
-        #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
-      #endif
+  #if defined(__cplusplus) && __cplusplus >= 201103L
+    #if __has_cpp_attribute(fallthrough)
+      #define CYTHON_FALLTHROUGH [[fallthrough]]
+    #elif __has_cpp_attribute(clang::fallthrough)
+      #define CYTHON_FALLTHROUGH [[clang::fallthrough]]
+    #elif __has_cpp_attribute(gnu::fallthrough)
+      #define CYTHON_FALLTHROUGH [[gnu::fallthrough]]
     #endif
   #endif
   #ifndef CYTHON_FALLTHROUGH
     #if __has_attribute(fallthrough)
       #define CYTHON_FALLTHROUGH __attribute__((fallthrough))
     #else
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
-  #if defined(__clang__) && defined(__apple_build_version__)
+  #if defined(__clang__ ) && defined(__apple_build_version__)
     #if __apple_build_version__ < 7000000
       #undef  CYTHON_FALLTHROUGH
       #define CYTHON_FALLTHROUGH
     #endif
   #endif
 #endif
-#ifdef __cplusplus
-  template <typename T>
-  struct __PYX_IS_UNSIGNED_IMPL {static const bool value = T(0) < T(-1);};
-  #define __PYX_IS_UNSIGNED(type) (__PYX_IS_UNSIGNED_IMPL<type>::value)
-#else
-  #define __PYX_IS_UNSIGNED(type) (((type)-1) > 0)
-#endif
-#if CYTHON_COMPILING_IN_PYPY == 1
-  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x030A0000)
-#else
-  #define __PYX_NEED_TP_PRINT_SLOT  (PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000)
-#endif
-#define __PYX_REINTERPRET_FUNCION(func_pointer, other_pointer) ((func_pointer)(void(*)(void))(other_pointer))
 
 #ifndef CYTHON_INLINE
   #if defined(__clang__)
     #define CYTHON_INLINE __inline__ __attribute__ ((__unused__))
   #elif defined(__GNUC__)
     #define CYTHON_INLINE __inline__
   #elif defined(_MSC_VER)
@@ -540,225 +306,93 @@
   #elif defined (__STDC_VERSION__) && __STDC_VERSION__ >= 199901L
     #define CYTHON_INLINE inline
   #else
     #define CYTHON_INLINE
   #endif
 #endif
 
+#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX < 0x02070600 && !defined(Py_OptimizeFlag)
+  #define Py_OptimizeFlag 0
+#endif
 #define __PYX_BUILD_PY_SSIZE_T "n"
 #define CYTHON_FORMAT_SSIZE_T "z"
 #if PY_MAJOR_VERSION < 3
   #define __Pyx_BUILTIN_MODULE_NAME "__builtin__"
-  #define __Pyx_DefaultClassType PyClass_Type
-  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a+k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+  #define __Pyx_DefaultClassType PyClass_Type
 #else
   #define __Pyx_BUILTIN_MODULE_NAME "builtins"
-  #define __Pyx_DefaultClassType PyType_Type
-#if PY_VERSION_HEX >= 0x030B00A1
-    static CYTHON_INLINE PyCodeObject* __Pyx_PyCode_New(int a, int p, int k, int l, int s, int f,
-                                                    PyObject *code, PyObject *c, PyObject* n, PyObject *v,
-                                                    PyObject *fv, PyObject *cell, PyObject* fn,
-                                                    PyObject *name, int fline, PyObject *lnos) {
-        PyObject *kwds=NULL, *argcount=NULL, *posonlyargcount=NULL, *kwonlyargcount=NULL;
-        PyObject *nlocals=NULL, *stacksize=NULL, *flags=NULL, *replace=NULL, *empty=NULL;
-        const char *fn_cstr=NULL;
-        const char *name_cstr=NULL;
-        PyCodeObject *co=NULL, *result=NULL;
-        PyObject *type, *value, *traceback;
-        PyErr_Fetch(&type, &value, &traceback);
-        if (!(kwds=PyDict_New())) goto end;
-        if (!(argcount=PyLong_FromLong(a))) goto end;
-        if (PyDict_SetItemString(kwds, "co_argcount", argcount) != 0) goto end;
-        if (!(posonlyargcount=PyLong_FromLong(p))) goto end;
-        if (PyDict_SetItemString(kwds, "co_posonlyargcount", posonlyargcount) != 0) goto end;
-        if (!(kwonlyargcount=PyLong_FromLong(k))) goto end;
-        if (PyDict_SetItemString(kwds, "co_kwonlyargcount", kwonlyargcount) != 0) goto end;
-        if (!(nlocals=PyLong_FromLong(l))) goto end;
-        if (PyDict_SetItemString(kwds, "co_nlocals", nlocals) != 0) goto end;
-        if (!(stacksize=PyLong_FromLong(s))) goto end;
-        if (PyDict_SetItemString(kwds, "co_stacksize", stacksize) != 0) goto end;
-        if (!(flags=PyLong_FromLong(f))) goto end;
-        if (PyDict_SetItemString(kwds, "co_flags", flags) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_code", code) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_consts", c) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_names", n) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_varnames", v) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_freevars", fv) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_cellvars", cell) != 0) goto end;
-        if (PyDict_SetItemString(kwds, "co_linetable", lnos) != 0) goto end;
-        if (!(fn_cstr=PyUnicode_AsUTF8AndSize(fn, NULL))) goto end;
-        if (!(name_cstr=PyUnicode_AsUTF8AndSize(name, NULL))) goto end;
-        if (!(co = PyCode_NewEmpty(fn_cstr, name_cstr, fline))) goto end;
-        if (!(replace = PyObject_GetAttrString((PyObject*)co, "replace"))) goto end;
-        if (!(empty = PyTuple_New(0))) goto end;
-        result = (PyCodeObject*) PyObject_Call(replace, empty, kwds);
-    end:
-        Py_XDECREF((PyObject*) co);
-        Py_XDECREF(kwds);
-        Py_XDECREF(argcount);
-        Py_XDECREF(posonlyargcount);
-        Py_XDECREF(kwonlyargcount);
-        Py_XDECREF(nlocals);
-        Py_XDECREF(stacksize);
-        Py_XDECREF(replace);
-        Py_XDECREF(empty);
-        if (type) {
-            PyErr_Restore(type, value, traceback);
-        }
-        return result;
-    }
-#elif PY_VERSION_HEX >= 0x030800B2 && !CYTHON_COMPILING_IN_PYPY
-  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
-          PyCode_NewWithPosOnlyArgs(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
+#if PY_VERSION_HEX >= 0x030800A4 && PY_VERSION_HEX < 0x030800B2
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+          PyCode_New(a, 0, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #else
-  #define __Pyx_PyCode_New(a, p, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
+  #define __Pyx_PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)\
           PyCode_New(a, k, l, s, f, code, c, n, v, fv, cell, fn, name, fline, lnos)
 #endif
-#endif
-#if PY_VERSION_HEX >= 0x030900A4 || defined(Py_IS_TYPE)
-  #define __Pyx_IS_TYPE(ob, type) Py_IS_TYPE(ob, type)
-#else
-  #define __Pyx_IS_TYPE(ob, type) (((const PyObject*)ob)->ob_type == (type))
-#endif
-#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_Is)
-  #define __Pyx_Py_Is(x, y)  Py_Is(x, y)
-#else
-  #define __Pyx_Py_Is(x, y) ((x) == (y))
-#endif
-#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsNone)
-  #define __Pyx_Py_IsNone(ob) Py_IsNone(ob)
-#else
-  #define __Pyx_Py_IsNone(ob) __Pyx_Py_Is((ob), Py_None)
-#endif
-#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsTrue)
-  #define __Pyx_Py_IsTrue(ob) Py_IsTrue(ob)
-#else
-  #define __Pyx_Py_IsTrue(ob) __Pyx_Py_Is((ob), Py_True)
-#endif
-#if PY_VERSION_HEX >= 0x030A00B1 || defined(Py_IsFalse)
-  #define __Pyx_Py_IsFalse(ob) Py_IsFalse(ob)
-#else
-  #define __Pyx_Py_IsFalse(ob) __Pyx_Py_Is((ob), Py_False)
-#endif
-#define __Pyx_NoneAsNull(obj)  (__Pyx_Py_IsNone(obj) ? NULL : (obj))
-#if PY_VERSION_HEX >= 0x030900F0 && !CYTHON_COMPILING_IN_PYPY
-  #define __Pyx_PyObject_GC_IsFinalized(o) PyObject_GC_IsFinalized(o)
-#else
-  #define __Pyx_PyObject_GC_IsFinalized(o) _PyGC_FINALIZED(o)
-#endif
-#ifndef CO_COROUTINE
-  #define CO_COROUTINE 0x80
-#endif
-#ifndef CO_ASYNC_GENERATOR
-  #define CO_ASYNC_GENERATOR 0x200
+  #define __Pyx_DefaultClassType PyType_Type
 #endif
 #ifndef Py_TPFLAGS_CHECKTYPES
   #define Py_TPFLAGS_CHECKTYPES 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_INDEX
   #define Py_TPFLAGS_HAVE_INDEX 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_NEWBUFFER
   #define Py_TPFLAGS_HAVE_NEWBUFFER 0
 #endif
 #ifndef Py_TPFLAGS_HAVE_FINALIZE
   #define Py_TPFLAGS_HAVE_FINALIZE 0
 #endif
-#ifndef Py_TPFLAGS_SEQUENCE
-  #define Py_TPFLAGS_SEQUENCE 0
-#endif
-#ifndef Py_TPFLAGS_MAPPING
-  #define Py_TPFLAGS_MAPPING 0
-#endif
 #ifndef METH_STACKLESS
   #define METH_STACKLESS 0
 #endif
 #if PY_VERSION_HEX <= 0x030700A3 || !defined(METH_FASTCALL)
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
   #define __Pyx_PyCFunctionFast _PyCFunctionFast
   #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
 #endif
-#if CYTHON_METH_FASTCALL
-  #define __Pyx_METH_FASTCALL METH_FASTCALL
-  #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
-  #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
-#else
-  #define __Pyx_METH_FASTCALL METH_VARARGS
-  #define __Pyx_PyCFunction_FastCall PyCFunction
-  #define __Pyx_PyCFunction_FastCallWithKeywords PyCFunctionWithKeywords
-#endif
-#if CYTHON_VECTORCALL
-  #define __pyx_vectorcallfunc vectorcallfunc
-  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  PY_VECTORCALL_ARGUMENTS_OFFSET
-  #define __Pyx_PyVectorcall_NARGS(n)  PyVectorcall_NARGS((size_t)(n))
-#elif CYTHON_BACKPORT_VECTORCALL
-  typedef PyObject *(*__pyx_vectorcallfunc)(PyObject *callable, PyObject *const *args,
-                                            size_t nargsf, PyObject *kwnames);
-  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  ((size_t)1 << (8 * sizeof(size_t) - 1))
-  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(((size_t)(n)) & ~__Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET))
-#else
-  #define __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET  0
-  #define __Pyx_PyVectorcall_NARGS(n)  ((Py_ssize_t)(n))
-#endif
-#if PY_VERSION_HEX < 0x030900B1
-  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  ((void)m, PyType_FromSpecWithBases(s, b))
-  typedef PyObject *(*__Pyx_PyCMethod)(PyObject *, PyTypeObject *, PyObject *const *, size_t, PyObject *);
+#if CYTHON_FAST_PYCCALL
+#define __Pyx_PyFastCFunction_Check(func)\
+    ((PyCFunction_Check(func) && (METH_FASTCALL == (PyCFunction_GET_FLAGS(func) & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)))))
 #else
-  #define __Pyx_PyType_FromModuleAndSpec(m, s, b)  PyType_FromModuleAndSpec(m, s, b)
-  #define __Pyx_PyCMethod  PyCMethod
-#endif
-#ifndef METH_METHOD
-  #define METH_METHOD 0x200
+#define __Pyx_PyFastCFunction_Check(func) 0
 #endif
 #if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Malloc)
   #define PyObject_Malloc(s)   PyMem_Malloc(s)
   #define PyObject_Free(p)     PyMem_Free(p)
   #define PyObject_Realloc(p)  PyMem_Realloc(p)
 #endif
-#if CYTHON_COMPILING_IN_LIMITED_API
-  #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
-  #define __Pyx_PyFrame_SetLineNumber(frame, lineno)
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030400A1
+  #define PyMem_RawMalloc(n)           PyMem_Malloc(n)
+  #define PyMem_RawRealloc(p, n)       PyMem_Realloc(p, n)
+  #define PyMem_RawFree(p)             PyMem_Free(p)
+#endif
+#if CYTHON_COMPILING_IN_PYSTON
+  #define __Pyx_PyCode_HasFreeVars(co)  PyCode_HasFreeVars(co)
+  #define __Pyx_PyFrame_SetLineNumber(frame, lineno) PyFrame_SetLineNumber(frame, lineno)
 #else
   #define __Pyx_PyCode_HasFreeVars(co)  (PyCode_GetNumFree(co) > 0)
   #define __Pyx_PyFrame_SetLineNumber(frame, lineno)  (frame)->f_lineno = (lineno)
 #endif
-#if CYTHON_COMPILING_IN_LIMITED_API
-  #define __Pyx_PyThreadState_Current PyThreadState_Get()
-#elif !CYTHON_FAST_THREAD_STATE
+#if !CYTHON_FAST_THREAD_STATE || PY_VERSION_HEX < 0x02070000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #elif PY_VERSION_HEX >= 0x03060000
   #define __Pyx_PyThreadState_Current _PyThreadState_UncheckedGet()
 #elif PY_VERSION_HEX >= 0x03000000
   #define __Pyx_PyThreadState_Current PyThreadState_GET()
 #else
   #define __Pyx_PyThreadState_Current _PyThreadState_Current
 #endif
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE void *__Pyx_PyModule_GetState(PyObject *op)
-{
-    void *result;
-    result = PyModule_GetState(op);
-    if (!result)
-        Py_FatalError("Couldn't find the module state");
-    return result;
-}
-#endif
-#define __Pyx_PyObject_GetSlot(obj, name, func_ctype)  __Pyx_PyType_GetSlot(Py_TYPE(obj), name, func_ctype)
-#if CYTHON_COMPILING_IN_LIMITED_API
-  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((func_ctype) PyType_GetSlot((type), Py_##name))
-#else
-  #define __Pyx_PyType_GetSlot(type, name, func_ctype)  ((type)->name)
-#endif
 #if PY_VERSION_HEX < 0x030700A2 && !defined(PyThread_tss_create) && !defined(Py_tss_NEEDS_INIT)
 #include "pythread.h"
 #define Py_tss_NEEDS_INIT 0
 typedef int Py_tss_t;
 static CYTHON_INLINE int PyThread_tss_create(Py_tss_t *key) {
   *key = PyThread_create_key();
   return 0;
@@ -781,166 +415,78 @@
 static CYTHON_INLINE int PyThread_tss_set(Py_tss_t *key, void *value) {
   return PyThread_set_key_value(*key, value);
 }
 static CYTHON_INLINE void * PyThread_tss_get(Py_tss_t *key) {
   return PyThread_get_key_value(*key);
 }
 #endif
-#if PY_MAJOR_VERSION < 3
-    #if CYTHON_COMPILING_IN_PYPY
-        #if PYPY_VERSION_NUM < 0x07030600
-            #if defined(__cplusplus) && __cplusplus >= 201402L
-                [[deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")]]
-            #elif defined(__GNUC__) || defined(__clang__)
-                __attribute__ ((__deprecated__("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6")))
-            #elif defined(_MSC_VER)
-                __declspec(deprecated("`with nogil:` inside a nogil function will not release the GIL in PyPy2 < 7.3.6"))
-            #endif
-            static CYTHON_INLINE int PyGILState_Check(void) {
-                return 0;
-            }
-        #else  // PYPY_VERSION_NUM < 0x07030600
-        #endif  // PYPY_VERSION_NUM < 0x07030600
-    #else
-        static CYTHON_INLINE int PyGILState_Check(void) {
-            PyThreadState * tstate = _PyThreadState_Current;
-            return tstate && (tstate == PyGILState_GetThisThreadState());
-        }
-    #endif
-#endif
 #if CYTHON_COMPILING_IN_CPYTHON || defined(_PyDict_NewPresized)
 #define __Pyx_PyDict_NewPresized(n)  ((n <= 8) ? PyDict_New() : _PyDict_NewPresized(n))
 #else
 #define __Pyx_PyDict_NewPresized(n)  PyDict_New()
 #endif
 #if PY_MAJOR_VERSION >= 3 || CYTHON_FUTURE_DIVISION
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_TrueDivide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceTrueDivide(x,y)
 #else
   #define __Pyx_PyNumber_Divide(x,y)         PyNumber_Divide(x,y)
   #define __Pyx_PyNumber_InPlaceDivide(x,y)  PyNumber_InPlaceDivide(x,y)
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX > 0x030600B4 && CYTHON_USE_UNICODE_INTERNALS
-#define __Pyx_PyDict_GetItemStrWithError(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
-static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStr(PyObject *dict, PyObject *name) {
-    PyObject *res = __Pyx_PyDict_GetItemStrWithError(dict, name);
-    if (res == NULL) PyErr_Clear();
-    return res;
-}
-#elif PY_MAJOR_VERSION >= 3 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07020000)
-#define __Pyx_PyDict_GetItemStrWithError  PyDict_GetItemWithError
-#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
+#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x030500A1 && CYTHON_USE_UNICODE_INTERNALS
+#define __Pyx_PyDict_GetItemStr(dict, name)  _PyDict_GetItem_KnownHash(dict, name, ((PyASCIIObject *) name)->hash)
 #else
-static CYTHON_INLINE PyObject * __Pyx_PyDict_GetItemStrWithError(PyObject *dict, PyObject *name) {
-#if CYTHON_COMPILING_IN_PYPY
-    return PyDict_GetItem(dict, name);
-#else
-    PyDictEntry *ep;
-    PyDictObject *mp = (PyDictObject*) dict;
-    long hash = ((PyStringObject *) name)->ob_shash;
-    assert(hash != -1);
-    ep = (mp->ma_lookup)(mp, name, hash);
-    if (ep == NULL) {
-        return NULL;
-    }
-    return ep->me_value;
-#endif
-}
-#define __Pyx_PyDict_GetItemStr           PyDict_GetItem
-#endif
-#if CYTHON_USE_TYPE_SLOTS
-  #define __Pyx_PyType_GetFlags(tp)   (((PyTypeObject *)tp)->tp_flags)
-  #define __Pyx_PyType_HasFeature(type, feature)  ((__Pyx_PyType_GetFlags(type) & (feature)) != 0)
-  #define __Pyx_PyObject_GetIterNextFunc(obj)  (Py_TYPE(obj)->tp_iternext)
-#else
-  #define __Pyx_PyType_GetFlags(tp)   (PyType_GetFlags((PyTypeObject *)tp))
-  #define __Pyx_PyType_HasFeature(type, feature)  PyType_HasFeature(type, feature)
-  #define __Pyx_PyObject_GetIterNextFunc(obj)  PyIter_Next
-#endif
-#if CYTHON_USE_TYPE_SPECS && PY_VERSION_HEX >= 0x03080000
-#define __Pyx_PyHeapTypeObject_GC_Del(obj)  {\
-    PyTypeObject *type = Py_TYPE(obj);\
-    assert(__Pyx_PyType_HasFeature(type, Py_TPFLAGS_HEAPTYPE));\
-    PyObject_GC_Del(obj);\
-    Py_DECREF(type);\
-}
-#else
-#define __Pyx_PyHeapTypeObject_GC_Del(obj)  PyObject_GC_Del(obj)
+#define __Pyx_PyDict_GetItemStr(dict, name)  PyDict_GetItem(dict, name)
 #endif
-#if CYTHON_COMPILING_IN_LIMITED_API
-  #define CYTHON_PEP393_ENABLED 1
-  #define __Pyx_PyUnicode_READY(op)       (0)
-  #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GetLength(u)
-  #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_ReadChar(u, i)
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((void)u, 1114111U)
-  #define __Pyx_PyUnicode_KIND(u)         ((void)u, (0))
-  #define __Pyx_PyUnicode_DATA(u)         ((void*)u)
-  #define __Pyx_PyUnicode_READ(k, d, i)   ((void)k, PyUnicode_ReadChar((PyObject*)(d), i))
-  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GetLength(u))
-#elif PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
+#if PY_VERSION_HEX > 0x03030000 && defined(PyUnicode_KIND)
   #define CYTHON_PEP393_ENABLED 1
-  #if PY_VERSION_HEX >= 0x030C0000
-    #define __Pyx_PyUnicode_READY(op)       (0)
-  #else
-    #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
-                                                0 : _PyUnicode_Ready((PyObject *)(op)))
-  #endif
+  #define __Pyx_PyUnicode_READY(op)       (likely(PyUnicode_IS_READY(op)) ?\
+                                              0 : _PyUnicode_Ready((PyObject *)(op)))
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_LENGTH(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) PyUnicode_READ_CHAR(u, i)
   #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   PyUnicode_MAX_CHAR_VALUE(u)
-  #define __Pyx_PyUnicode_KIND(u)         ((int)PyUnicode_KIND(u))
+  #define __Pyx_PyUnicode_KIND(u)         PyUnicode_KIND(u)
   #define __Pyx_PyUnicode_DATA(u)         PyUnicode_DATA(u)
   #define __Pyx_PyUnicode_READ(k, d, i)   PyUnicode_READ(k, d, i)
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, (Py_UCS4) ch)
-  #if PY_VERSION_HEX >= 0x030C0000
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  PyUnicode_WRITE(k, d, i, ch)
+  #if defined(PyUnicode_IS_READY) && defined(PyUnicode_GET_SIZE)
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
   #else
-    #if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX >= 0x03090000
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : ((PyCompactUnicodeObject *)(u))->wstr_length))
-    #else
-    #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != (likely(PyUnicode_IS_READY(u)) ? PyUnicode_GET_LENGTH(u) : PyUnicode_GET_SIZE(u)))
-    #endif
+  #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_LENGTH(u))
   #endif
 #else
   #define CYTHON_PEP393_ENABLED 0
   #define PyUnicode_1BYTE_KIND  1
   #define PyUnicode_2BYTE_KIND  2
   #define PyUnicode_4BYTE_KIND  4
   #define __Pyx_PyUnicode_READY(op)       (0)
   #define __Pyx_PyUnicode_GET_LENGTH(u)   PyUnicode_GET_SIZE(u)
   #define __Pyx_PyUnicode_READ_CHAR(u, i) ((Py_UCS4)(PyUnicode_AS_UNICODE(u)[i]))
-  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535U : 1114111U)
-  #define __Pyx_PyUnicode_KIND(u)         ((int)sizeof(Py_UNICODE))
+  #define __Pyx_PyUnicode_MAX_CHAR_VALUE(u)   ((sizeof(Py_UNICODE) == 2) ? 65535 : 1114111)
+  #define __Pyx_PyUnicode_KIND(u)         (sizeof(Py_UNICODE))
   #define __Pyx_PyUnicode_DATA(u)         ((void*)PyUnicode_AS_UNICODE(u))
   #define __Pyx_PyUnicode_READ(k, d, i)   ((void)(k), (Py_UCS4)(((Py_UNICODE*)d)[i]))
-  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = (Py_UNICODE) ch)
+  #define __Pyx_PyUnicode_WRITE(k, d, i, ch)  (((void)(k)), ((Py_UNICODE*)d)[i] = ch)
   #define __Pyx_PyUnicode_IS_TRUE(u)      (0 != PyUnicode_GET_SIZE(u))
 #endif
 #if CYTHON_COMPILING_IN_PYPY
   #define __Pyx_PyUnicode_Concat(a, b)      PyNumber_Add(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  PyNumber_Add(a, b)
 #else
   #define __Pyx_PyUnicode_Concat(a, b)      PyUnicode_Concat(a, b)
   #define __Pyx_PyUnicode_ConcatSafe(a, b)  ((unlikely((a) == Py_None) || unlikely((b) == Py_None)) ?\
       PyNumber_Add(a, b) : __Pyx_PyUnicode_Concat(a, b))
 #endif
-#if CYTHON_COMPILING_IN_PYPY
-  #if !defined(PyUnicode_DecodeUnicodeEscape)
-    #define PyUnicode_DecodeUnicodeEscape(s, size, errors)  PyUnicode_Decode(s, size, "unicode_escape", errors)
-  #endif
-  #if !defined(PyUnicode_Contains) || (PY_MAJOR_VERSION == 2 && PYPY_VERSION_NUM < 0x07030500)
-    #undef PyUnicode_Contains
-    #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
-  #endif
-  #if !defined(PyByteArray_Check)
-    #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
-  #endif
-  #if !defined(PyObject_Format)
-    #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
-  #endif
+#if CYTHON_COMPILING_IN_PYPY && !defined(PyUnicode_Contains)
+  #define PyUnicode_Contains(u, s)  PySequence_Contains(u, s)
+#endif
+#if CYTHON_COMPILING_IN_PYPY && !defined(PyByteArray_Check)
+  #define PyByteArray_Check(obj)  PyObject_TypeCheck(obj, &PyByteArray_Type)
+#endif
+#if CYTHON_COMPILING_IN_PYPY && !defined(PyObject_Format)
+  #define PyObject_Format(obj, fmt)  PyObject_CallMethod(obj, "__format__", "O", fmt)
 #endif
 #define __Pyx_PyString_FormatSafe(a, b)   ((unlikely((a) == Py_None || (PyString_Check(b) && !PyString_CheckExact(b)))) ? PyNumber_Remainder(a, b) : __Pyx_PyString_Format(a, b))
 #define __Pyx_PyUnicode_FormatSafe(a, b)  ((unlikely((a) == Py_None || (PyUnicode_Check(b) && !PyUnicode_CheckExact(b)))) ? PyNumber_Remainder(a, b) : PyUnicode_Format(a, b))
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyString_Format(a, b)  PyUnicode_Format(a, b)
 #else
   #define __Pyx_PyString_Format(a, b)  PyString_Format(a, b)
@@ -961,22 +507,16 @@
 #if PY_MAJOR_VERSION >= 3
   #define __Pyx_PyBaseString_Check(obj) PyUnicode_Check(obj)
   #define __Pyx_PyBaseString_CheckExact(obj) PyUnicode_CheckExact(obj)
 #else
   #define __Pyx_PyBaseString_Check(obj) (PyString_Check(obj) || PyUnicode_Check(obj))
   #define __Pyx_PyBaseString_CheckExact(obj) (PyString_CheckExact(obj) || PyUnicode_CheckExact(obj))
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON
-  #define __Pyx_PySequence_ListKeepNew(obj)\
-    (likely(PyList_CheckExact(obj) && Py_REFCNT(obj) == 1) ? __Pyx_NewRef(obj) : PySequence_List(obj))
-#else
-  #define __Pyx_PySequence_ListKeepNew(obj)  PySequence_List(obj)
-#endif
 #ifndef PySet_CheckExact
-  #define PySet_CheckExact(obj)        __Pyx_IS_TYPE(obj, &PySet_Type)
+  #define PySet_CheckExact(obj)        (Py_TYPE(obj) == &PySet_Type)
 #endif
 #if PY_VERSION_HEX >= 0x030900A4
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_SET_REFCNT(obj, refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SET_SIZE(obj, size)
 #else
   #define __Pyx_SET_REFCNT(obj, refcnt) Py_REFCNT(obj) = (refcnt)
   #define __Pyx_SET_SIZE(obj, size) Py_SIZE(obj) = (size)
@@ -987,46 +527,46 @@
   #define __Pyx_PySequence_SIZE(seq)  PySequence_Size(seq)
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyIntObject                  PyLongObject
   #define PyInt_Type                   PyLong_Type
   #define PyInt_Check(op)              PyLong_Check(op)
   #define PyInt_CheckExact(op)         PyLong_CheckExact(op)
-  #define __Pyx_Py3Int_Check(op)       PyLong_Check(op)
-  #define __Pyx_Py3Int_CheckExact(op)  PyLong_CheckExact(op)
   #define PyInt_FromString             PyLong_FromString
   #define PyInt_FromUnicode            PyLong_FromUnicode
   #define PyInt_FromLong               PyLong_FromLong
   #define PyInt_FromSize_t             PyLong_FromSize_t
   #define PyInt_FromSsize_t            PyLong_FromSsize_t
   #define PyInt_AsLong                 PyLong_AsLong
   #define PyInt_AS_LONG                PyLong_AS_LONG
   #define PyInt_AsSsize_t              PyLong_AsSsize_t
   #define PyInt_AsUnsignedLongMask     PyLong_AsUnsignedLongMask
   #define PyInt_AsUnsignedLongLongMask PyLong_AsUnsignedLongLongMask
   #define PyNumber_Int                 PyNumber_Long
-#else
-  #define __Pyx_Py3Int_Check(op)       (PyLong_Check(op) || PyInt_Check(op))
-  #define __Pyx_Py3Int_CheckExact(op)  (PyLong_CheckExact(op) || PyInt_CheckExact(op))
 #endif
 #if PY_MAJOR_VERSION >= 3
   #define PyBoolObject                 PyLongObject
 #endif
 #if PY_MAJOR_VERSION >= 3 && CYTHON_COMPILING_IN_PYPY
   #ifndef PyUnicode_InternFromString
     #define PyUnicode_InternFromString(s) PyUnicode_FromString(s)
   #endif
 #endif
 #if PY_VERSION_HEX < 0x030200A4
   typedef long Py_hash_t;
   #define __Pyx_PyInt_FromHash_t PyInt_FromLong
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsHash_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsLong
 #else
   #define __Pyx_PyInt_FromHash_t PyInt_FromSsize_t
-  #define __Pyx_PyInt_AsHash_t   __Pyx_PyIndex_AsSsize_t
+  #define __Pyx_PyInt_AsHash_t   PyInt_AsSsize_t
+#endif
+#if PY_MAJOR_VERSION >= 3
+  #define __Pyx_PyMethod_New(func, self, klass) ((self) ? ((void)(klass), PyMethod_New(func, self)) : __Pyx_NewRef(func))
+#else
+  #define __Pyx_PyMethod_New(func, self, klass) PyMethod_New(func, self, klass)
 #endif
 #if CYTHON_USE_ASYNC_SLOTS
   #if PY_VERSION_HEX >= 0x030500B1
     #define __Pyx_PyAsyncMethodsStruct PyAsyncMethods
     #define __Pyx_PyType_AsAsync(obj) (Py_TYPE(obj)->tp_as_async)
   #else
     #define __Pyx_PyType_AsAsync(obj) ((__Pyx_PyAsyncMethodsStruct*) (Py_TYPE(obj)->tp_reserved))
@@ -1038,18 +578,16 @@
     typedef struct {
         unaryfunc am_await;
         unaryfunc am_aiter;
         unaryfunc am_anext;
     } __Pyx_PyAsyncMethodsStruct;
 #endif
 
-#if defined(_WIN32) || defined(WIN32) || defined(MS_WINDOWS)
-  #if !defined(_USE_MATH_DEFINES)
-    #define _USE_MATH_DEFINES
-  #endif
+#if defined(WIN32) || defined(MS_WINDOWS)
+  #define _USE_MATH_DEFINES
 #endif
 #include <math.h>
 #ifdef NAN
 #define __PYX_NAN() ((float) NAN)
 #else
 static CYTHON_INLINE float __PYX_NAN() {
   float value;
@@ -1064,33 +602,24 @@
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
     { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
-#ifdef CYTHON_EXTERN_C
-    #undef __PYX_EXTERN_C
-    #define __PYX_EXTERN_C CYTHON_EXTERN_C
-#elif defined(__PYX_EXTERN_C)
-    #ifdef _MSC_VER
-    #pragma message ("Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.")
-    #else
-    #warning Please do not define the '__PYX_EXTERN_C' macro externally. Use 'CYTHON_EXTERN_C' instead.
-    #endif
-#else
+#ifndef __PYX_EXTERN_C
   #ifdef __cplusplus
     #define __PYX_EXTERN_C extern "C"
   #else
     #define __PYX_EXTERN_C extern
   #endif
 #endif
 
-#define __PYX_HAVE__camSort__camSort
-#define __PYX_HAVE_API__camSort__camSort
+#define __PYX_HAVE__camSort__stringSort
+#define __PYX_HAVE_API__camSort__stringSort
 /* Early includes */
 #ifdef _OPENMP
 #include <omp.h>
 #endif /* _OPENMP */
 
 #if defined(PYREX_WITHOUT_ASSERTIONS) && !defined(CYTHON_WITHOUT_ASSERTIONS)
 #define CYTHON_WITHOUT_ASSERTIONS
@@ -1152,111 +681,54 @@
 #endif
 #define __Pyx_PyBytes_AsWritableString(s)     ((char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableSString(s)    ((signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsWritableUString(s)    ((unsigned char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsString(s)     ((const char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsSString(s)    ((const signed char*) PyBytes_AS_STRING(s))
 #define __Pyx_PyBytes_AsUString(s)    ((const unsigned char*) PyBytes_AS_STRING(s))
-#define __Pyx_PyObject_AsWritableString(s)    ((char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
-#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*)(__pyx_uintptr_t) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableString(s)    ((char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableSString(s)    ((signed char*) __Pyx_PyObject_AsString(s))
+#define __Pyx_PyObject_AsWritableUString(s)    ((unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
+static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u) {
     const Py_UNICODE *u_end = u;
     while (*u_end++) ;
     return (size_t)(u_end - u - 1);
 }
-#endif
-#define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
 #define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
 #define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
 #define __Pyx_PySequence_Tuple(obj)\
     (likely(PyTuple_CheckExact(obj)) ? __Pyx_NewRef(obj) : PySequence_Tuple(obj))
 static CYTHON_INLINE Py_ssize_t __Pyx_PyIndex_AsSsize_t(PyObject*);
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t);
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject*);
 #if CYTHON_ASSUME_SAFE_MACROS
 #define __pyx_PyFloat_AsDouble(x) (PyFloat_CheckExact(x) ? PyFloat_AS_DOUBLE(x) : PyFloat_AsDouble(x))
 #else
 #define __pyx_PyFloat_AsDouble(x) PyFloat_AsDouble(x)
 #endif
 #define __pyx_PyFloat_AsFloat(x) ((float) __pyx_PyFloat_AsDouble(x))
 #if PY_MAJOR_VERSION >= 3
 #define __Pyx_PyNumber_Int(x) (PyLong_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Long(x))
 #else
 #define __Pyx_PyNumber_Int(x) (PyInt_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Int(x))
 #endif
-#if CYTHON_USE_PYLONG_INTERNALS
-  #if PY_VERSION_HEX >= 0x030C00A7
-  #ifndef _PyLong_SIGN_MASK
-    #define _PyLong_SIGN_MASK 3
-  #endif
-  #ifndef _PyLong_NON_SIZE_BITS
-    #define _PyLong_NON_SIZE_BITS 3
-  #endif
-  #define __Pyx_PyLong_Sign(x)  (((PyLongObject*)x)->long_value.lv_tag & _PyLong_SIGN_MASK)
-  #define __Pyx_PyLong_IsNeg(x)  ((__Pyx_PyLong_Sign(x) & 2) != 0)
-  #define __Pyx_PyLong_IsNonNeg(x)  (!__Pyx_PyLong_IsNeg(x))
-  #define __Pyx_PyLong_IsZero(x)  (__Pyx_PyLong_Sign(x) & 1)
-  #define __Pyx_PyLong_IsPos(x)  (__Pyx_PyLong_Sign(x) == 0)
-  #define __Pyx_PyLong_CompactValueUnsigned(x)  (__Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  ((Py_ssize_t) (((PyLongObject*)x)->long_value.lv_tag >> _PyLong_NON_SIZE_BITS))
-  #define __Pyx_PyLong_SignedDigitCount(x)\
-        ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * __Pyx_PyLong_DigitCount(x))
-  #if defined(PyUnstable_Long_IsCompact) && defined(PyUnstable_Long_CompactValue)
-    #define __Pyx_PyLong_IsCompact(x)     PyUnstable_Long_IsCompact((PyLongObject*) x)
-    #define __Pyx_PyLong_CompactValue(x)  PyUnstable_Long_CompactValue((PyLongObject*) x)
-  #else
-    #define __Pyx_PyLong_IsCompact(x)     (((PyLongObject*)x)->long_value.lv_tag < (2 << _PyLong_NON_SIZE_BITS))
-    #define __Pyx_PyLong_CompactValue(x)  ((1 - (Py_ssize_t) __Pyx_PyLong_Sign(x)) * (Py_ssize_t) __Pyx_PyLong_Digits(x)[0])
-  #endif
-  typedef Py_ssize_t  __Pyx_compact_pylong;
-  typedef size_t  __Pyx_compact_upylong;
-  #else  // Py < 3.12
-  #define __Pyx_PyLong_IsNeg(x)  (Py_SIZE(x) < 0)
-  #define __Pyx_PyLong_IsNonNeg(x)  (Py_SIZE(x) >= 0)
-  #define __Pyx_PyLong_IsZero(x)  (Py_SIZE(x) == 0)
-  #define __Pyx_PyLong_IsPos(x)  (Py_SIZE(x) > 0)
-  #define __Pyx_PyLong_CompactValueUnsigned(x)  ((Py_SIZE(x) == 0) ? 0 : __Pyx_PyLong_Digits(x)[0])
-  #define __Pyx_PyLong_DigitCount(x)  __Pyx_sst_abs(Py_SIZE(x))
-  #define __Pyx_PyLong_SignedDigitCount(x)  Py_SIZE(x)
-  #define __Pyx_PyLong_IsCompact(x)  (Py_SIZE(x) == 0 || Py_SIZE(x) == 1 || Py_SIZE(x) == -1)
-  #define __Pyx_PyLong_CompactValue(x)\
-        ((Py_SIZE(x) == 0) ? (sdigit) 0 : ((Py_SIZE(x) < 0) ? -(sdigit)__Pyx_PyLong_Digits(x)[0] : (sdigit)__Pyx_PyLong_Digits(x)[0]))
-  typedef sdigit  __Pyx_compact_pylong;
-  typedef digit  __Pyx_compact_upylong;
-  #endif
-  #if PY_VERSION_HEX >= 0x030C00A5
-  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->long_value.ob_digit)
-  #else
-  #define __Pyx_PyLong_Digits(x)  (((PyLongObject*)x)->ob_digit)
-  #endif
-#endif
+#define __Pyx_PyNumber_Float(x) (PyFloat_CheckExact(x) ? __Pyx_NewRef(x) : PyNumber_Float(x))
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
 static int __Pyx_sys_getdefaultencoding_not_ascii;
 static int __Pyx_init_sys_getdefaultencoding_params(void) {
     PyObject* sys;
     PyObject* default_encoding = NULL;
     PyObject* ascii_chars_u = NULL;
     PyObject* ascii_chars_b = NULL;
@@ -1270,15 +742,15 @@
     if (!default_encoding_c) goto bad;
     if (strcmp(default_encoding_c, "ascii") == 0) {
         __Pyx_sys_getdefaultencoding_not_ascii = 0;
     } else {
         char ascii_chars[128];
         int c;
         for (c = 0; c < 128; c++) {
-            ascii_chars[c] = (char) c;
+            ascii_chars[c] = c;
         }
         __Pyx_sys_getdefaultencoding_not_ascii = 1;
         ascii_chars_u = PyUnicode_DecodeASCII(ascii_chars, 128, NULL);
         if (!ascii_chars_u) goto bad;
         ascii_chars_b = PyUnicode_AsEncodedString(ascii_chars_u, default_encoding_c, NULL);
         if (!ascii_chars_b || !PyBytes_Check(ascii_chars_b) || memcmp(ascii_chars, PyBytes_AS_STRING(ascii_chars_b), 128) != 0) {
             PyErr_Format(
@@ -1335,174 +807,175 @@
   #define unlikely(x) __builtin_expect(!!(x), 0)
 #else /* !__GNUC__ or GCC < 2.95 */
   #define likely(x)   (x)
   #define unlikely(x) (x)
 #endif /* __GNUC__ */
 static CYTHON_INLINE void __Pyx_pretend_to_initialize(void* ptr) { (void)ptr; }
 
-#if !CYTHON_USE_MODULE_STATE
 static PyObject *__pyx_m = NULL;
-#endif
+static PyObject *__pyx_d;
+static PyObject *__pyx_b;
+static PyObject *__pyx_cython_runtime = NULL;
+static PyObject *__pyx_empty_tuple;
+static PyObject *__pyx_empty_bytes;
+static PyObject *__pyx_empty_unicode;
 static int __pyx_lineno;
 static int __pyx_clineno = 0;
-static const char * __pyx_cfilenm = __FILE__;
+static const char * __pyx_cfilenm= __FILE__;
 static const char *__pyx_filename;
 
-/* #### Code section: filename_table ### */
 
 static const char *__pyx_f[] = {
-  "camSort/camSort.pyx",
-  "<stringsource>",
+  "camSort/stringSort.pyx",
+  "stringsource",
 };
-/* #### Code section: utility_code_proto_before_types ### */
-/* #### Code section: numeric_typedefs ### */
-/* #### Code section: complex_type_declarations ### */
-/* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
-struct __pyx_obj_7camSort_7camSort_StringWithKey;
+struct __pyx_obj_7camSort_10stringSort_StringWithKey;
 
-/* "camSort/camSort.pyx":4
+/* "camSort/stringSort.pyx":4
  * from operator import attrgetter
  * 
  * cdef class StringWithKey:             # <<<<<<<<<<<<<<
  *     cdef public:
  *         str str
  */
-struct __pyx_obj_7camSort_7camSort_StringWithKey {
+struct __pyx_obj_7camSort_10stringSort_StringWithKey {
   PyObject_HEAD
-  struct __pyx_vtabstruct_7camSort_7camSort_StringWithKey *__pyx_vtab;
+  struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *__pyx_vtab;
   PyObject *str;
   PY_LONG_LONG key;
 };
 
 
 
-struct __pyx_vtabstruct_7camSort_7camSort_StringWithKey {
-  PY_LONG_LONG (*calculate_key)(struct __pyx_obj_7camSort_7camSort_StringWithKey *, PyObject *);
+struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey {
+  PY_LONG_LONG (*calculate_key)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *);
 };
-static struct __pyx_vtabstruct_7camSort_7camSort_StringWithKey *__pyx_vtabptr_7camSort_7camSort_StringWithKey;
-/* #### Code section: utility_code_proto ### */
+static struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *__pyx_vtabptr_7camSort_10stringSort_StringWithKey;
 
 /* --- Runtime support code (head) --- */
 /* Refnanny.proto */
 #ifndef CYTHON_REFNANNY
   #define CYTHON_REFNANNY 0
 #endif
 #if CYTHON_REFNANNY
   typedef struct {
-    void (*INCREF)(void*, PyObject*, Py_ssize_t);
-    void (*DECREF)(void*, PyObject*, Py_ssize_t);
-    void (*GOTREF)(void*, PyObject*, Py_ssize_t);
-    void (*GIVEREF)(void*, PyObject*, Py_ssize_t);
-    void* (*SetupContext)(const char*, Py_ssize_t, const char*);
+    void (*INCREF)(void*, PyObject*, int);
+    void (*DECREF)(void*, PyObject*, int);
+    void (*GOTREF)(void*, PyObject*, int);
+    void (*GIVEREF)(void*, PyObject*, int);
+    void* (*SetupContext)(const char*, int, const char*);
     void (*FinishContext)(void**);
   } __Pyx_RefNannyAPIStruct;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNanny = NULL;
   static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname);
   #define __Pyx_RefNannyDeclarations void *__pyx_refnanny = NULL;
 #ifdef WITH_THREAD
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
           if (acquire_gil) {\
               PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
               PyGILState_Release(__pyx_gilstate_save);\
           } else {\
-              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__));\
-          }
-  #define __Pyx_RefNannyFinishContextNogil() {\
-              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __Pyx_RefNannyFinishContext();\
-              PyGILState_Release(__pyx_gilstate_save);\
+              __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__);\
           }
 #else
   #define __Pyx_RefNannySetupContext(name, acquire_gil)\
-          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), (__LINE__), (__FILE__))
-  #define __Pyx_RefNannyFinishContextNogil() __Pyx_RefNannyFinishContext()
+          __pyx_refnanny = __Pyx_RefNanny->SetupContext((name), __LINE__, __FILE__)
 #endif
-  #define __Pyx_RefNannyFinishContextNogil() {\
-              PyGILState_STATE __pyx_gilstate_save = PyGILState_Ensure();\
-              __Pyx_RefNannyFinishContext();\
-              PyGILState_Release(__pyx_gilstate_save);\
-          }
   #define __Pyx_RefNannyFinishContext()\
           __Pyx_RefNanny->FinishContext(&__pyx_refnanny)
-  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
-  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
-  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
-  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), (__LINE__))
-  #define __Pyx_XINCREF(r)  do { if((r) == NULL); else {__Pyx_INCREF(r); }} while(0)
-  #define __Pyx_XDECREF(r)  do { if((r) == NULL); else {__Pyx_DECREF(r); }} while(0)
-  #define __Pyx_XGOTREF(r)  do { if((r) == NULL); else {__Pyx_GOTREF(r); }} while(0)
-  #define __Pyx_XGIVEREF(r) do { if((r) == NULL); else {__Pyx_GIVEREF(r);}} while(0)
+  #define __Pyx_INCREF(r)  __Pyx_RefNanny->INCREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
+  #define __Pyx_DECREF(r)  __Pyx_RefNanny->DECREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
+  #define __Pyx_GOTREF(r)  __Pyx_RefNanny->GOTREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
+  #define __Pyx_GIVEREF(r) __Pyx_RefNanny->GIVEREF(__pyx_refnanny, (PyObject *)(r), __LINE__)
+  #define __Pyx_XINCREF(r)  do { if((r) != NULL) {__Pyx_INCREF(r); }} while(0)
+  #define __Pyx_XDECREF(r)  do { if((r) != NULL) {__Pyx_DECREF(r); }} while(0)
+  #define __Pyx_XGOTREF(r)  do { if((r) != NULL) {__Pyx_GOTREF(r); }} while(0)
+  #define __Pyx_XGIVEREF(r) do { if((r) != NULL) {__Pyx_GIVEREF(r);}} while(0)
 #else
   #define __Pyx_RefNannyDeclarations
   #define __Pyx_RefNannySetupContext(name, acquire_gil)
-  #define __Pyx_RefNannyFinishContextNogil()
   #define __Pyx_RefNannyFinishContext()
   #define __Pyx_INCREF(r) Py_INCREF(r)
   #define __Pyx_DECREF(r) Py_DECREF(r)
   #define __Pyx_GOTREF(r)
   #define __Pyx_GIVEREF(r)
   #define __Pyx_XINCREF(r) Py_XINCREF(r)
   #define __Pyx_XDECREF(r) Py_XDECREF(r)
   #define __Pyx_XGOTREF(r)
   #define __Pyx_XGIVEREF(r)
 #endif
-#define __Pyx_Py_XDECREF_SET(r, v) do {\
-        PyObject *tmp = (PyObject *) r;\
-        r = v; Py_XDECREF(tmp);\
-    } while (0)
 #define __Pyx_XDECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_XDECREF(tmp);\
     } while (0)
 #define __Pyx_DECREF_SET(r, v) do {\
         PyObject *tmp = (PyObject *) r;\
         r = v; __Pyx_DECREF(tmp);\
     } while (0)
 #define __Pyx_CLEAR(r)    do { PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);} while(0)
 #define __Pyx_XCLEAR(r)   do { if((r) != NULL) {PyObject* tmp = ((PyObject*)(r)); r = NULL; __Pyx_DECREF(tmp);}} while(0)
 
-/* PyErrExceptionMatches.proto */
-#if CYTHON_FAST_THREAD_STATE
-#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
+/* PyObjectGetAttrStr.proto */
+#if CYTHON_USE_TYPE_SLOTS
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
 #else
-#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
+#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
 #endif
 
+/* GetBuiltinName.proto */
+static PyObject *__Pyx_GetBuiltinName(PyObject *name);
+
+/* RaiseDoubleKeywords.proto */
+static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
+
+/* ParseKeywords.proto */
+static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject **argnames[],\
+    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,\
+    const char* function_name);
+
+/* RaiseArgTupleInvalid.proto */
+static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
+    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
+
+/* UnicodeAsUCS4.proto */
+static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject*);
+
+/* object_ord.proto */
+#if PY_MAJOR_VERSION >= 3
+#define __Pyx_PyObject_Ord(c)\
+    (likely(PyUnicode_Check(c)) ? (long)__Pyx_PyUnicode_AsPy_UCS4(c) : __Pyx__PyObject_Ord(c))
+#else
+#define __Pyx_PyObject_Ord(c) __Pyx__PyObject_Ord(c)
+#endif
+static long __Pyx__PyObject_Ord(PyObject* c);
+
 /* PyThreadStateGet.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyThreadState_declare  PyThreadState *__pyx_tstate;
 #define __Pyx_PyThreadState_assign  __pyx_tstate = __Pyx_PyThreadState_Current;
-#if PY_VERSION_HEX >= 0x030C00A6
-#define __Pyx_PyErr_Occurred()  (__pyx_tstate->current_exception != NULL)
-#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->current_exception ? (PyObject*) Py_TYPE(__pyx_tstate->current_exception) : (PyObject*) NULL)
-#else
-#define __Pyx_PyErr_Occurred()  (__pyx_tstate->curexc_type != NULL)
-#define __Pyx_PyErr_CurrentExceptionType()  (__pyx_tstate->curexc_type)
-#endif
+#define __Pyx_PyErr_Occurred()  __pyx_tstate->curexc_type
 #else
 #define __Pyx_PyThreadState_declare
 #define __Pyx_PyThreadState_assign
-#define __Pyx_PyErr_Occurred()  (PyErr_Occurred() != NULL)
-#define __Pyx_PyErr_CurrentExceptionType()  PyErr_Occurred()
+#define __Pyx_PyErr_Occurred()  PyErr_Occurred()
 #endif
 
 /* PyErrFetchRestore.proto */
 #if CYTHON_FAST_THREAD_STATE
 #define __Pyx_PyErr_Clear() __Pyx_ErrRestore(NULL, NULL, NULL)
 #define __Pyx_ErrRestoreWithState(type, value, tb)  __Pyx_ErrRestoreInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrFetchWithState(type, value, tb)    __Pyx_ErrFetchInState(PyThreadState_GET(), type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  __Pyx_ErrRestoreInState(__pyx_tstate, type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)    __Pyx_ErrFetchInState(__pyx_tstate, type, value, tb)
 static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb);
 static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb);
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A6
+#if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_PyErr_SetNone(exc) (Py_INCREF(exc), __Pyx_ErrRestore((exc), NULL, NULL))
 #else
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
 #endif
 #else
 #define __Pyx_PyErr_Clear() PyErr_Clear()
 #define __Pyx_PyErr_SetNone(exc) PyErr_SetNone(exc)
@@ -1510,99 +983,29 @@
 #define __Pyx_ErrFetchWithState(type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestoreInState(tstate, type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetchInState(tstate, type, value, tb)  PyErr_Fetch(type, value, tb)
 #define __Pyx_ErrRestore(type, value, tb)  PyErr_Restore(type, value, tb)
 #define __Pyx_ErrFetch(type, value, tb)  PyErr_Fetch(type, value, tb)
 #endif
 
-/* PyObjectGetAttrStr.proto */
-#if CYTHON_USE_TYPE_SLOTS
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name);
-#else
-#define __Pyx_PyObject_GetAttrStr(o,n) PyObject_GetAttr(o,n)
-#endif
-
-/* PyObjectGetAttrStrNoError.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
-
-/* GetBuiltinName.proto */
-static PyObject *__Pyx_GetBuiltinName(PyObject *name);
-
-/* TupleAndListFromArray.proto */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE PyObject* __Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n);
-static CYTHON_INLINE PyObject* __Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n);
-#endif
-
-/* IncludeStringH.proto */
-#include <string.h>
+/* WriteUnraisableException.proto */
+static void __Pyx_WriteUnraisable(const char *name, int clineno,
+                                  int lineno, const char *filename,
+                                  int full_traceback, int nogil);
 
-/* BytesEquals.proto */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* UnicodeEquals.proto */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals);
-
-/* fastcall.proto */
-#define __Pyx_Arg_VARARGS(args, i) PyTuple_GET_ITEM(args, i)
-#define __Pyx_NumKwargs_VARARGS(kwds) PyDict_Size(kwds)
-#define __Pyx_KwValues_VARARGS(args, nargs) NULL
-#define __Pyx_GetKwValue_VARARGS(kw, kwvalues, s) __Pyx_PyDict_GetItemStrWithError(kw, s)
-#define __Pyx_KwargsAsDict_VARARGS(kw, kwvalues) PyDict_Copy(kw)
-#if CYTHON_METH_FASTCALL
-    #define __Pyx_Arg_FASTCALL(args, i) args[i]
-    #define __Pyx_NumKwargs_FASTCALL(kwds) PyTuple_GET_SIZE(kwds)
-    #define __Pyx_KwValues_FASTCALL(args, nargs) ((args) + (nargs))
-    static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s);
-    #define __Pyx_KwargsAsDict_FASTCALL(kw, kwvalues) _PyStack_AsDict(kwvalues, kw)
-#else
-    #define __Pyx_Arg_FASTCALL __Pyx_Arg_VARARGS
-    #define __Pyx_NumKwargs_FASTCALL __Pyx_NumKwargs_VARARGS
-    #define __Pyx_KwValues_FASTCALL __Pyx_KwValues_VARARGS
-    #define __Pyx_GetKwValue_FASTCALL __Pyx_GetKwValue_VARARGS
-    #define __Pyx_KwargsAsDict_FASTCALL __Pyx_KwargsAsDict_VARARGS
-#endif
-#if CYTHON_COMPILING_IN_CPYTHON
-#define __Pyx_ArgsSlice_VARARGS(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_VARARGS(args, start), stop - start)
-#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) __Pyx_PyTuple_FromArray(&__Pyx_Arg_FASTCALL(args, start), stop - start)
-#else
-#define __Pyx_ArgsSlice_VARARGS(args, start, stop) PyTuple_GetSlice(args, start, stop)
-#define __Pyx_ArgsSlice_FASTCALL(args, start, stop) PyTuple_GetSlice(args, start, stop)
-#endif
-
-/* RaiseDoubleKeywords.proto */
-static void __Pyx_RaiseDoubleKeywordsError(const char* func_name, PyObject* kw_name);
-
-/* ParseKeywords.proto */
-static int __Pyx_ParseOptionalKeywords(PyObject *kwds, PyObject *const *kwvalues,
-    PyObject **argnames[],
-    PyObject *kwds2, PyObject *values[], Py_ssize_t num_pos_args,
-    const char* function_name);
-
-/* RaiseArgTupleInvalid.proto */
-static void __Pyx_RaiseArgtupleInvalid(const char* func_name, int exact,
-    Py_ssize_t num_min, Py_ssize_t num_max, Py_ssize_t num_found);
-
-/* RaiseUnexpectedTypeError.proto */
-static int __Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj);
-
-/* UnicodeAsUCS4.proto */
-static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject*);
-
-/* object_ord.proto */
-#if PY_MAJOR_VERSION >= 3
-#define __Pyx_PyObject_Ord(c)\
-    (likely(PyUnicode_Check(c)) ? (long)__Pyx_PyUnicode_AsPy_UCS4(c) : __Pyx__PyObject_Ord(c))
+/* PyErrExceptionMatches.proto */
+#if CYTHON_FAST_THREAD_STATE
+#define __Pyx_PyErr_ExceptionMatches(err) __Pyx_PyErr_ExceptionMatchesInState(__pyx_tstate, err)
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err);
 #else
-#define __Pyx_PyObject_Ord(c) __Pyx__PyObject_Ord(c)
+#define __Pyx_PyErr_ExceptionMatches(err)  PyErr_ExceptionMatches(err)
 #endif
-static long __Pyx__PyObject_Ord(PyObject* c);
 
-/* KeywordStringCheck.proto */
-static int __Pyx_CheckKeywordStrings(PyObject *kw, const char* function_name, int kw_allowed);
+/* GetAttr.proto */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
 
 /* GetAttr3.proto */
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *, PyObject *, PyObject *);
 
 /* PyDictVersioning.proto */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 #define __PYX_DICT_VERSION_INIT  ((PY_UINT64_T) -1)
@@ -1627,26 +1030,26 @@
 #define __PYX_GET_DICT_VERSION(dict)  (0)
 #define __PYX_UPDATE_DICT_CACHE(dict, value, cache_var, version_var)
 #define __PYX_PY_DICT_LOOKUP_IF_MODIFIED(VAR, DICT, LOOKUP)  (VAR) = (LOOKUP);
 #endif
 
 /* GetModuleGlobalName.proto */
 #if CYTHON_USE_DICT_VERSIONS
-#define __Pyx_GetModuleGlobalName(var, name)  do {\
+#define __Pyx_GetModuleGlobalName(var, name)  {\
     static PY_UINT64_T __pyx_dict_version = 0;\
     static PyObject *__pyx_dict_cached_value = NULL;\
     (var) = (likely(__pyx_dict_version == __PYX_GET_DICT_VERSION(__pyx_d))) ?\
         (likely(__pyx_dict_cached_value) ? __Pyx_NewRef(__pyx_dict_cached_value) : __Pyx_GetBuiltinName(name)) :\
         __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
-#define __Pyx_GetModuleGlobalNameUncached(var, name)  do {\
+}
+#define __Pyx_GetModuleGlobalNameUncached(var, name)  {\
     PY_UINT64_T __pyx_dict_version;\
     PyObject *__pyx_dict_cached_value;\
     (var) = __Pyx__GetModuleGlobalName(name, &__pyx_dict_version, &__pyx_dict_cached_value);\
-} while(0)
+}
 static PyObject *__Pyx__GetModuleGlobalName(PyObject *name, PY_UINT64_T *dict_version, PyObject **dict_cached_value);
 #else
 #define __Pyx_GetModuleGlobalName(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 #define __Pyx_GetModuleGlobalNameUncached(var, name)  (var) = __Pyx__GetModuleGlobalName(name)
 static CYTHON_INLINE PyObject *__Pyx__GetModuleGlobalName(PyObject *name);
 #endif
 
@@ -1663,73 +1066,61 @@
     }
     return PyList_Append(list, x);
 }
 #else
 #define __Pyx_ListComp_Append(L,x) PyList_Append(L,x)
 #endif
 
+/* PyCFunctionFastCall.proto */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject *__Pyx_PyCFunction_FastCall(PyObject *func, PyObject **args, Py_ssize_t nargs);
+#else
+#define __Pyx_PyCFunction_FastCall(func, args, nargs)  (assert(0), NULL)
+#endif
+
 /* PyFunctionFastCall.proto */
 #if CYTHON_FAST_PYCALL
-#if !CYTHON_VECTORCALL
 #define __Pyx_PyFunction_FastCall(func, args, nargs)\
     __Pyx_PyFunction_FastCallDict((func), (args), (nargs), NULL)
+#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs);
+#else
+#define __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs) _PyFunction_FastCallDict(func, args, nargs, kwargs)
 #endif
 #define __Pyx_BUILD_ASSERT_EXPR(cond)\
     (sizeof(char [1 - 2*!(cond)]) - 1)
 #ifndef Py_MEMBER_SIZE
 #define Py_MEMBER_SIZE(type, member) sizeof(((type *)0)->member)
 #endif
-#if !CYTHON_VECTORCALL
-#if PY_VERSION_HEX >= 0x03080000
-  #include "frameobject.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-  #define __Pxy_PyFrame_Initialize_Offsets()
-  #define __Pyx_PyFrame_GetLocalsplus(frame)  ((frame)->f_localsplus)
-#else
   static size_t __pyx_pyframe_localsplus_offset = 0;
   #include "frameobject.h"
   #define __Pxy_PyFrame_Initialize_Offsets()\
     ((void)__Pyx_BUILD_ASSERT_EXPR(sizeof(PyFrameObject) == offsetof(PyFrameObject, f_localsplus) + Py_MEMBER_SIZE(PyFrameObject, f_localsplus)),\
      (void)(__pyx_pyframe_localsplus_offset = ((size_t)PyFrame_Type.tp_basicsize) - Py_MEMBER_SIZE(PyFrameObject, f_localsplus)))
   #define __Pyx_PyFrame_GetLocalsplus(frame)\
     (assert(__pyx_pyframe_localsplus_offset), (PyObject **)(((char *)(frame)) + __pyx_pyframe_localsplus_offset))
 #endif
-#endif
-#endif
 
 /* PyObjectCall.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw);
 #else
 #define __Pyx_PyObject_Call(func, arg, kw) PyObject_Call(func, arg, kw)
 #endif
 
 /* PyObjectCallMethO.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallMethO(PyObject *func, PyObject *arg);
 #endif
 
-/* PyObjectFastCall.proto */
-#define __Pyx_PyObject_FastCall(func, args, nargs)  __Pyx_PyObject_FastCallDict(func, args, (size_t)(nargs), NULL)
-static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs);
-
 /* PyObjectCallOneArg.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg);
 
-/* PySequenceContains.proto */
-static CYTHON_INLINE int __Pyx_PySequence_ContainsTF(PyObject* item, PyObject* seq, int eq) {
-    int result = PySequence_Contains(seq, item);
-    return unlikely(result < 0) ? result : (result == (eq == Py_EQ));
-}
+/* PyObjectCall2Args.proto */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2);
 
 /* Import.proto */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level);
 
 /* ImportFrom.proto */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name);
 
@@ -1754,45 +1145,17 @@
     (PyErr_SetString(PyExc_IndexError, "tuple index out of range"), (PyObject*)NULL))
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Tuple_Fast(PyObject *o, Py_ssize_t i,
                                                               int wraparound, int boundscheck);
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j);
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_Fast(PyObject *o, Py_ssize_t i,
                                                      int is_list, int wraparound, int boundscheck);
 
-/* GetAttr.proto */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *, PyObject *);
-
 /* HasAttr.proto */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *, PyObject *);
 
-/* IncludeStructmemberH.proto */
-#include <structmember.h>
-
-/* FixUpExtensionType.proto */
-#if CYTHON_USE_TYPE_SPECS
-static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type);
-#endif
-
-/* PyObjectCallNoArg.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func);
-
-/* PyObjectGetMethod.proto */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method);
-
-/* PyObjectCallMethod0.proto */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name);
-
-/* ValidateBasesTuple.proto */
-#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
-static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases);
-#endif
-
-/* PyType_Ready.proto */
-CYTHON_UNUSED static int __Pyx_PyType_Ready(PyTypeObject *t);
-
 /* PyObject_GenericGetAttrNoDict.proto */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttrNoDict PyObject_GenericGetAttr
 #endif
 
@@ -1800,835 +1163,314 @@
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject* __Pyx_PyObject_GenericGetAttr(PyObject* obj, PyObject* attr_name);
 #else
 #define __Pyx_PyObject_GenericGetAttr PyObject_GenericGetAttr
 #endif
 
 /* SetVTable.proto */
-static int __Pyx_SetVtable(PyTypeObject* typeptr , void* vtable);
-
-/* GetVTable.proto */
-static void* __Pyx_GetVtable(PyTypeObject *type);
+static int __Pyx_SetVtable(PyObject *dict, void *vtable);
 
-/* MergeVTables.proto */
-#if !CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_MergeVtables(PyTypeObject *type);
-#endif
+/* PyObjectGetAttrStrNoError.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name);
 
 /* SetupReduce.proto */
-#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
-#endif
-
-/* FetchSharedCythonModule.proto */
-static PyObject *__Pyx_FetchSharedCythonABIModule(void);
-
-/* FetchCommonType.proto */
-#if !CYTHON_USE_TYPE_SPECS
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type);
-#else
-static PyTypeObject* __Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases);
-#endif
-
-/* PyMethodNew.proto */
-#if PY_MAJOR_VERSION >= 3
-static PyObject *__Pyx_PyMethod_New(PyObject *func, PyObject *self, PyObject *typ) {
-    CYTHON_UNUSED_VAR(typ);
-    if (!self)
-        return __Pyx_NewRef(func);
-    return PyMethod_New(func, self);
-}
-#else
-    #define __Pyx_PyMethod_New PyMethod_New
-#endif
-
-/* PyVectorcallFastCallDict.proto */
-#if CYTHON_METH_FASTCALL
-static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw);
-#endif
-
-/* CythonFunctionShared.proto */
-#define __Pyx_CyFunction_USED
-#define __Pyx_CYFUNCTION_STATICMETHOD  0x01
-#define __Pyx_CYFUNCTION_CLASSMETHOD   0x02
-#define __Pyx_CYFUNCTION_CCLASS        0x04
-#define __Pyx_CYFUNCTION_COROUTINE     0x08
-#define __Pyx_CyFunction_GetClosure(f)\
-    (((__pyx_CyFunctionObject *) (f))->func_closure)
-#if PY_VERSION_HEX < 0x030900B1
-  #define __Pyx_CyFunction_GetClassObj(f)\
-      (((__pyx_CyFunctionObject *) (f))->func_classobj)
-#else
-  #define __Pyx_CyFunction_GetClassObj(f)\
-      ((PyObject*) ((PyCMethodObject *) (f))->mm_class)
-#endif
-#define __Pyx_CyFunction_SetClassObj(f, classobj)\
-    __Pyx__CyFunction_SetClassObj((__pyx_CyFunctionObject *) (f), (classobj))
-#define __Pyx_CyFunction_Defaults(type, f)\
-    ((type *)(((__pyx_CyFunctionObject *) (f))->defaults))
-#define __Pyx_CyFunction_SetDefaultsGetter(f, g)\
-    ((__pyx_CyFunctionObject *) (f))->defaults_getter = (g)
-typedef struct {
-#if PY_VERSION_HEX < 0x030900B1
-    PyCFunctionObject func;
-#else
-    PyCMethodObject func;
-#endif
-#if CYTHON_BACKPORT_VECTORCALL
-    __pyx_vectorcallfunc func_vectorcall;
-#endif
-#if PY_VERSION_HEX < 0x030500A0
-    PyObject *func_weakreflist;
-#endif
-    PyObject *func_dict;
-    PyObject *func_name;
-    PyObject *func_qualname;
-    PyObject *func_doc;
-    PyObject *func_globals;
-    PyObject *func_code;
-    PyObject *func_closure;
-#if PY_VERSION_HEX < 0x030900B1
-    PyObject *func_classobj;
-#endif
-    void *defaults;
-    int defaults_pyobjects;
-    size_t defaults_size;  // used by FusedFunction for copying defaults
-    int flags;
-    PyObject *defaults_tuple;
-    PyObject *defaults_kwdict;
-    PyObject *(*defaults_getter)(PyObject *);
-    PyObject *func_annotations;
-    PyObject *func_is_coroutine;
-} __pyx_CyFunctionObject;
-#define __Pyx_CyFunction_Check(obj)  __Pyx_TypeCheck(obj, __pyx_CyFunctionType)
-#define __Pyx_IsCyOrPyCFunction(obj)  __Pyx_TypeCheck2(obj, __pyx_CyFunctionType, &PyCFunction_Type)
-#define __Pyx_CyFunction_CheckExact(obj)  __Pyx_IS_TYPE(obj, __pyx_CyFunctionType)
-static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject* op, PyMethodDef *ml,
-                                      int flags, PyObject* qualname,
-                                      PyObject *closure,
-                                      PyObject *module, PyObject *globals,
-                                      PyObject* code);
-static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj);
-static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *m,
-                                                         size_t size,
-                                                         int pyobjects);
-static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *m,
-                                                            PyObject *tuple);
-static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *m,
-                                                             PyObject *dict);
-static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *m,
-                                                              PyObject *dict);
-static int __pyx_CyFunction_init(PyObject *module);
-#if CYTHON_METH_FASTCALL
-static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
-static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
-static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
-static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames);
-#if CYTHON_BACKPORT_VECTORCALL
-#define __Pyx_CyFunction_func_vectorcall(f) (((__pyx_CyFunctionObject*)f)->func_vectorcall)
-#else
-#define __Pyx_CyFunction_func_vectorcall(f) (((PyCFunctionObject*)f)->vectorcall)
-#endif
-#endif
-
-/* CythonFunction.proto */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml,
-                                      int flags, PyObject* qualname,
-                                      PyObject *closure,
-                                      PyObject *module, PyObject *globals,
-                                      PyObject* code);
 
 /* CLineInTraceback.proto */
 #ifdef CYTHON_CLINE_IN_TRACEBACK
 #define __Pyx_CLineForTraceback(tstate, c_line)  (((CYTHON_CLINE_IN_TRACEBACK)) ? c_line : 0)
 #else
 static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line);
 #endif
 
 /* CodeObjectCache.proto */
-#if !CYTHON_COMPILING_IN_LIMITED_API
 typedef struct {
     PyCodeObject* code_object;
     int code_line;
 } __Pyx_CodeObjectCacheEntry;
 struct __Pyx_CodeObjectCache {
     int count;
     int max_count;
     __Pyx_CodeObjectCacheEntry* entries;
 };
 static struct __Pyx_CodeObjectCache __pyx_code_cache = {0,0,NULL};
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line);
 static PyCodeObject *__pyx_find_code_object(int code_line);
 static void __pyx_insert_code_object(int code_line, PyCodeObject* code_object);
-#endif
 
 /* AddTraceback.proto */
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename);
 
-/* GCCDiagnostics.proto */
-#if !defined(__INTEL_COMPILER) && defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 6))
-#define __Pyx_HAS_GCC_DIAGNOSTIC
-#endif
-
 /* CIntToPy.proto */
 static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value);
 
+/* CIntToPy.proto */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
+
 /* CIntFromPy.proto */
 static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *);
 
 /* CIntFromPy.proto */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *);
 
-/* CIntToPy.proto */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value);
-
-/* FormatTypeName.proto */
-#if CYTHON_COMPILING_IN_LIMITED_API
-typedef PyObject *__Pyx_TypeName;
-#define __Pyx_FMT_TYPENAME "%U"
-static __Pyx_TypeName __Pyx_PyType_GetName(PyTypeObject* tp);
-#define __Pyx_DECREF_TypeName(obj) Py_XDECREF(obj)
-#else
-typedef const char *__Pyx_TypeName;
-#define __Pyx_FMT_TYPENAME "%.200s"
-#define __Pyx_PyType_GetName(tp) ((tp)->tp_name)
-#define __Pyx_DECREF_TypeName(obj)
-#endif
-
 /* CIntFromPy.proto */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *);
 
 /* FastTypeChecks.proto */
 #if CYTHON_COMPILING_IN_CPYTHON
 #define __Pyx_TypeCheck(obj, type) __Pyx_IsSubtype(Py_TYPE(obj), (PyTypeObject *)type)
-#define __Pyx_TypeCheck2(obj, type1, type2) __Pyx_IsAnySubtype2(Py_TYPE(obj), (PyTypeObject *)type1, (PyTypeObject *)type2)
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b);
-static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches(PyObject *err, PyObject *type);
 static CYTHON_INLINE int __Pyx_PyErr_GivenExceptionMatches2(PyObject *err, PyObject *type1, PyObject *type2);
 #else
 #define __Pyx_TypeCheck(obj, type) PyObject_TypeCheck(obj, (PyTypeObject *)type)
-#define __Pyx_TypeCheck2(obj, type1, type2) (PyObject_TypeCheck(obj, (PyTypeObject *)type1) || PyObject_TypeCheck(obj, (PyTypeObject *)type2))
 #define __Pyx_PyErr_GivenExceptionMatches(err, type) PyErr_GivenExceptionMatches(err, type)
 #define __Pyx_PyErr_GivenExceptionMatches2(err, type1, type2) (PyErr_GivenExceptionMatches(err, type1) || PyErr_GivenExceptionMatches(err, type2))
 #endif
-#define __Pyx_PyErr_ExceptionMatches2(err1, err2)  __Pyx_PyErr_GivenExceptionMatches2(__Pyx_PyErr_CurrentExceptionType(), err1, err2)
 #define __Pyx_PyException_Check(obj) __Pyx_TypeCheck(obj, PyExc_Exception)
 
 /* CheckBinaryVersion.proto */
 static int __Pyx_check_binary_version(void);
 
 /* InitStrings.proto */
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t);
 
-/* #### Code section: module_declarations ### */
-static PY_LONG_LONG __pyx_f_7camSort_7camSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
+static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto*/
 
-/* Module declarations from "camSort.camSort" */
-static PyObject *__pyx_f_7camSort_7camSort___pyx_unpickle_StringWithKey__set_state(struct __pyx_obj_7camSort_7camSort_StringWithKey *, PyObject *); /*proto*/
-/* #### Code section: typeinfo ### */
-/* #### Code section: before_global_var ### */
-#define __Pyx_MODULE_NAME "camSort.camSort"
-extern int __pyx_module_is_main_camSort__camSort;
-int __pyx_module_is_main_camSort__camSort = 0;
+/* Module declarations from 'camSort.stringSort' */
+static PyTypeObject *__pyx_ptype_7camSort_10stringSort_StringWithKey = 0;
+static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_StringWithKey__set_state(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *); /*proto*/
+#define __Pyx_MODULE_NAME "camSort.stringSort"
+extern int __pyx_module_is_main_camSort__stringSort;
+int __pyx_module_is_main_camSort__stringSort = 0;
 
-/* Implementation of "camSort.camSort" */
-/* #### Code section: global_var ### */
+/* Implementation of 'camSort.stringSort' */
 static PyObject *__pyx_builtin_sorted;
-/* #### Code section: string_decls ### */
 static const char __pyx_k_n[] = "n";
 static const char __pyx_k_s[] = "s";
-static const char __pyx_k__2[] = ".";
-static const char __pyx_k_gc[] = "gc";
-static const char __pyx_k__11[] = "?";
 static const char __pyx_k_key[] = "key";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_str[] = "str";
 static const char __pyx_k_dict[] = "__dict__";
 static const char __pyx_k_main[] = "__main__";
 static const char __pyx_k_name[] = "__name__";
-static const char __pyx_k_self[] = "self";
 static const char __pyx_k_test[] = "__test__";
 static const char __pyx_k_array[] = "array";
-static const char __pyx_k_state[] = "state";
-static const char __pyx_k_dict_2[] = "_dict";
-static const char __pyx_k_enable[] = "enable";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_sorted[] = "sorted";
 static const char __pyx_k_update[] = "update";
-static const char __pyx_k_disable[] = "disable";
+static const char __pyx_k_byLength[] = "byLength";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_operator[] = "operator";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
-static const char __pyx_k_isenabled[] = "isenabled";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_attrgetter[] = "attrgetter";
 static const char __pyx_k_input_list[] = "input_list";
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_PickleError[] = "PickleError";
-static const char __pyx_k_sortStrings[] = "sortStrings";
-static const char __pyx_k_is_coroutine[] = "_is_coroutine";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_sorted_array[] = "sorted_array";
-static const char __pyx_k_stringsource[] = "<stringsource>";
-static const char __pyx_k_use_setstate[] = "use_setstate";
+static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_StringWithKey[] = "StringWithKey";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
-static const char __pyx_k_camSort_camSort[] = "camSort.camSort";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
-static const char __pyx_k_asyncio_coroutines[] = "asyncio.coroutines";
+static const char __pyx_k_camSort_stringSort[] = "camSort.stringSort";
 static const char __pyx_k_cline_in_traceback[] = "cline_in_traceback";
-static const char __pyx_k_camSort_camSort_pyx[] = "camSort/camSort.pyx";
+static const char __pyx_k_camSort_stringSort_pyx[] = "camSort/stringSort.pyx";
 static const char __pyx_k_pyx_unpickle_StringWithKey[] = "__pyx_unpickle_StringWithKey";
-static const char __pyx_k_StringWithKey___reduce_cython[] = "StringWithKey.__reduce_cython__";
-static const char __pyx_k_StringWithKey___setstate_cython[] = "StringWithKey.__setstate_cython__";
-static const char __pyx_k_Incompatible_checksums_0x_x_vs_0[] = "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))";
-/* #### Code section: decls ### */
-static int __pyx_pf_7camSort_7camSort_13StringWithKey___init__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto */
-static PyObject *__pyx_pf_7camSort_7camSort_13StringWithKey_3str___get__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self); /* proto */
-static int __pyx_pf_7camSort_7camSort_13StringWithKey_3str_2__set__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static int __pyx_pf_7camSort_7camSort_13StringWithKey_3str_4__del__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7camSort_7camSort_13StringWithKey_3key___get__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self); /* proto */
-static int __pyx_pf_7camSort_7camSort_13StringWithKey_3key_2__set__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
-static PyObject *__pyx_pf_7camSort_7camSort_13StringWithKey_2__reduce_cython__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self); /* proto */
-static PyObject *__pyx_pf_7camSort_7camSort_13StringWithKey_4__setstate_cython__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_pf_7camSort_7camSort_sortStrings(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
-static PyObject *__pyx_pf_7camSort_7camSort_2__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
-static PyObject *__pyx_tp_new_7camSort_7camSort_StringWithKey(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
-/* #### Code section: late_includes ### */
-/* #### Code section: module_state ### */
-typedef struct {
-  PyObject *__pyx_d;
-  PyObject *__pyx_b;
-  PyObject *__pyx_cython_runtime;
-  PyObject *__pyx_empty_tuple;
-  PyObject *__pyx_empty_bytes;
-  PyObject *__pyx_empty_unicode;
-  #ifdef __Pyx_CyFunction_USED
-  PyTypeObject *__pyx_CyFunctionType;
-  #endif
-  #ifdef __Pyx_FusedFunction_USED
-  PyTypeObject *__pyx_FusedFunctionType;
-  #endif
-  #ifdef __Pyx_Generator_USED
-  PyTypeObject *__pyx_GeneratorType;
-  #endif
-  #ifdef __Pyx_IterableCoroutine_USED
-  PyTypeObject *__pyx_IterableCoroutineType;
-  #endif
-  #ifdef __Pyx_Coroutine_USED
-  PyTypeObject *__pyx_CoroutineAwaitType;
-  #endif
-  #ifdef __Pyx_Coroutine_USED
-  PyTypeObject *__pyx_CoroutineType;
-  #endif
-  #if CYTHON_USE_MODULE_STATE
-  PyObject *__pyx_type_7camSort_7camSort_StringWithKey;
-  #endif
-  PyTypeObject *__pyx_ptype_7camSort_7camSort_StringWithKey;
-  PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
-  PyObject *__pyx_n_s_PickleError;
-  PyObject *__pyx_n_s_StringWithKey;
-  PyObject *__pyx_n_s_StringWithKey___reduce_cython;
-  PyObject *__pyx_n_s_StringWithKey___setstate_cython;
-  PyObject *__pyx_n_s__11;
-  PyObject *__pyx_kp_u__2;
-  PyObject *__pyx_n_s_array;
-  PyObject *__pyx_n_s_asyncio_coroutines;
-  PyObject *__pyx_n_s_attrgetter;
-  PyObject *__pyx_n_s_camSort_camSort;
-  PyObject *__pyx_kp_s_camSort_camSort_pyx;
-  PyObject *__pyx_n_s_cline_in_traceback;
-  PyObject *__pyx_n_s_dict;
-  PyObject *__pyx_n_s_dict_2;
-  PyObject *__pyx_kp_u_disable;
-  PyObject *__pyx_kp_u_enable;
-  PyObject *__pyx_kp_u_gc;
-  PyObject *__pyx_n_s_getstate;
-  PyObject *__pyx_n_s_import;
-  PyObject *__pyx_n_s_input_list;
-  PyObject *__pyx_n_s_is_coroutine;
-  PyObject *__pyx_kp_u_isenabled;
-  PyObject *__pyx_n_s_key;
-  PyObject *__pyx_n_u_key;
-  PyObject *__pyx_n_s_main;
-  PyObject *__pyx_n_s_n;
-  PyObject *__pyx_n_s_name;
-  PyObject *__pyx_n_s_new;
-  PyObject *__pyx_n_s_operator;
-  PyObject *__pyx_n_s_pickle;
-  PyObject *__pyx_n_s_pyx_PickleError;
-  PyObject *__pyx_n_s_pyx_checksum;
-  PyObject *__pyx_n_s_pyx_result;
-  PyObject *__pyx_n_s_pyx_state;
-  PyObject *__pyx_n_s_pyx_type;
-  PyObject *__pyx_n_s_pyx_unpickle_StringWithKey;
-  PyObject *__pyx_n_s_pyx_vtable;
-  PyObject *__pyx_n_s_reduce;
-  PyObject *__pyx_n_s_reduce_cython;
-  PyObject *__pyx_n_s_reduce_ex;
-  PyObject *__pyx_n_s_s;
-  PyObject *__pyx_n_s_self;
-  PyObject *__pyx_n_s_setstate;
-  PyObject *__pyx_n_s_setstate_cython;
-  PyObject *__pyx_n_s_sortStrings;
-  PyObject *__pyx_n_s_sorted;
-  PyObject *__pyx_n_s_sorted_array;
-  PyObject *__pyx_n_s_state;
-  PyObject *__pyx_n_s_str;
-  PyObject *__pyx_kp_s_stringsource;
-  PyObject *__pyx_n_s_test;
-  PyObject *__pyx_n_s_update;
-  PyObject *__pyx_n_s_use_setstate;
-  PyObject *__pyx_int_163061131;
-  PyObject *__pyx_int_179973907;
-  PyObject *__pyx_int_250931038;
-  PyObject *__pyx_tuple_;
-  PyObject *__pyx_tuple__3;
-  PyObject *__pyx_tuple__5;
-  PyObject *__pyx_tuple__7;
-  PyObject *__pyx_tuple__9;
-  PyObject *__pyx_codeobj__4;
-  PyObject *__pyx_codeobj__6;
-  PyObject *__pyx_codeobj__8;
-  PyObject *__pyx_codeobj__10;
-} __pyx_mstate;
-
-#if CYTHON_USE_MODULE_STATE
-#ifdef __cplusplus
-namespace {
-  extern struct PyModuleDef __pyx_moduledef;
-} /* anonymous namespace */
-#else
-static struct PyModuleDef __pyx_moduledef;
-#endif
-
-#define __pyx_mstate(o) ((__pyx_mstate *)__Pyx_PyModule_GetState(o))
+static const char __pyx_k_Incompatible_checksums_s_vs_0xef[] = "Incompatible checksums (%s vs 0xef4e75e = (key, str))";
+static PyObject *__pyx_kp_s_Incompatible_checksums_s_vs_0xef;
+static PyObject *__pyx_n_s_PickleError;
+static PyObject *__pyx_n_s_StringWithKey;
+static PyObject *__pyx_n_s_array;
+static PyObject *__pyx_n_s_attrgetter;
+static PyObject *__pyx_n_s_byLength;
+static PyObject *__pyx_n_s_camSort_stringSort;
+static PyObject *__pyx_kp_s_camSort_stringSort_pyx;
+static PyObject *__pyx_n_s_cline_in_traceback;
+static PyObject *__pyx_n_s_dict;
+static PyObject *__pyx_n_s_getstate;
+static PyObject *__pyx_n_s_import;
+static PyObject *__pyx_n_s_input_list;
+static PyObject *__pyx_n_s_key;
+static PyObject *__pyx_n_u_key;
+static PyObject *__pyx_n_s_main;
+static PyObject *__pyx_n_s_n;
+static PyObject *__pyx_n_s_name;
+static PyObject *__pyx_n_s_new;
+static PyObject *__pyx_n_s_operator;
+static PyObject *__pyx_n_s_pickle;
+static PyObject *__pyx_n_s_pyx_PickleError;
+static PyObject *__pyx_n_s_pyx_checksum;
+static PyObject *__pyx_n_s_pyx_result;
+static PyObject *__pyx_n_s_pyx_state;
+static PyObject *__pyx_n_s_pyx_type;
+static PyObject *__pyx_n_s_pyx_unpickle_StringWithKey;
+static PyObject *__pyx_n_s_pyx_vtable;
+static PyObject *__pyx_n_s_reduce;
+static PyObject *__pyx_n_s_reduce_cython;
+static PyObject *__pyx_n_s_reduce_ex;
+static PyObject *__pyx_n_s_s;
+static PyObject *__pyx_n_s_setstate;
+static PyObject *__pyx_n_s_setstate_cython;
+static PyObject *__pyx_n_s_sorted;
+static PyObject *__pyx_n_s_sorted_array;
+static PyObject *__pyx_n_s_str;
+static PyObject *__pyx_kp_s_stringsource;
+static PyObject *__pyx_n_s_test;
+static PyObject *__pyx_n_s_update;
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3str___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3key___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_2__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_4__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_byLength(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list); /* proto */
+static PyObject *__pyx_pf_7camSort_10stringSort_2__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state); /* proto */
+static PyObject *__pyx_tp_new_7camSort_10stringSort_StringWithKey(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
+static PyObject *__pyx_int_250931038;
+static PyObject *__pyx_tuple_;
+static PyObject *__pyx_tuple__3;
+static PyObject *__pyx_codeobj__2;
+static PyObject *__pyx_codeobj__4;
+/* Late includes */
 
-#define __pyx_mstate_global (__pyx_mstate(PyState_FindModule(&__pyx_moduledef)))
-
-#define __pyx_m (PyState_FindModule(&__pyx_moduledef))
-#else
-static __pyx_mstate __pyx_mstate_global_static =
-#ifdef __cplusplus
-    {};
-#else
-    {0};
-#endif
-static __pyx_mstate *__pyx_mstate_global = &__pyx_mstate_global_static;
-#endif
-/* #### Code section: module_state_clear ### */
-#if CYTHON_USE_MODULE_STATE
-static int __pyx_m_clear(PyObject *m) {
-  __pyx_mstate *clear_module_state = __pyx_mstate(m);
-  if (!clear_module_state) return 0;
-  Py_CLEAR(clear_module_state->__pyx_d);
-  Py_CLEAR(clear_module_state->__pyx_b);
-  Py_CLEAR(clear_module_state->__pyx_cython_runtime);
-  Py_CLEAR(clear_module_state->__pyx_empty_tuple);
-  Py_CLEAR(clear_module_state->__pyx_empty_bytes);
-  Py_CLEAR(clear_module_state->__pyx_empty_unicode);
-  #ifdef __Pyx_CyFunction_USED
-  Py_CLEAR(clear_module_state->__pyx_CyFunctionType);
-  #endif
-  #ifdef __Pyx_FusedFunction_USED
-  Py_CLEAR(clear_module_state->__pyx_FusedFunctionType);
-  #endif
-  Py_CLEAR(clear_module_state->__pyx_ptype_7camSort_7camSort_StringWithKey);
-  Py_CLEAR(clear_module_state->__pyx_type_7camSort_7camSort_StringWithKey);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
-  Py_CLEAR(clear_module_state->__pyx_n_s_PickleError);
-  Py_CLEAR(clear_module_state->__pyx_n_s_StringWithKey);
-  Py_CLEAR(clear_module_state->__pyx_n_s_StringWithKey___reduce_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_StringWithKey___setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s__11);
-  Py_CLEAR(clear_module_state->__pyx_kp_u__2);
-  Py_CLEAR(clear_module_state->__pyx_n_s_array);
-  Py_CLEAR(clear_module_state->__pyx_n_s_asyncio_coroutines);
-  Py_CLEAR(clear_module_state->__pyx_n_s_attrgetter);
-  Py_CLEAR(clear_module_state->__pyx_n_s_camSort_camSort);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_camSort_camSort_pyx);
-  Py_CLEAR(clear_module_state->__pyx_n_s_cline_in_traceback);
-  Py_CLEAR(clear_module_state->__pyx_n_s_dict);
-  Py_CLEAR(clear_module_state->__pyx_n_s_dict_2);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_disable);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_enable);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_gc);
-  Py_CLEAR(clear_module_state->__pyx_n_s_getstate);
-  Py_CLEAR(clear_module_state->__pyx_n_s_import);
-  Py_CLEAR(clear_module_state->__pyx_n_s_input_list);
-  Py_CLEAR(clear_module_state->__pyx_n_s_is_coroutine);
-  Py_CLEAR(clear_module_state->__pyx_kp_u_isenabled);
-  Py_CLEAR(clear_module_state->__pyx_n_s_key);
-  Py_CLEAR(clear_module_state->__pyx_n_u_key);
-  Py_CLEAR(clear_module_state->__pyx_n_s_main);
-  Py_CLEAR(clear_module_state->__pyx_n_s_n);
-  Py_CLEAR(clear_module_state->__pyx_n_s_name);
-  Py_CLEAR(clear_module_state->__pyx_n_s_new);
-  Py_CLEAR(clear_module_state->__pyx_n_s_operator);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pickle);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_PickleError);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_checksum);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_result);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_state);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_type);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_unpickle_StringWithKey);
-  Py_CLEAR(clear_module_state->__pyx_n_s_pyx_vtable);
-  Py_CLEAR(clear_module_state->__pyx_n_s_reduce);
-  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_reduce_ex);
-  Py_CLEAR(clear_module_state->__pyx_n_s_s);
-  Py_CLEAR(clear_module_state->__pyx_n_s_self);
-  Py_CLEAR(clear_module_state->__pyx_n_s_setstate);
-  Py_CLEAR(clear_module_state->__pyx_n_s_setstate_cython);
-  Py_CLEAR(clear_module_state->__pyx_n_s_sortStrings);
-  Py_CLEAR(clear_module_state->__pyx_n_s_sorted);
-  Py_CLEAR(clear_module_state->__pyx_n_s_sorted_array);
-  Py_CLEAR(clear_module_state->__pyx_n_s_state);
-  Py_CLEAR(clear_module_state->__pyx_n_s_str);
-  Py_CLEAR(clear_module_state->__pyx_kp_s_stringsource);
-  Py_CLEAR(clear_module_state->__pyx_n_s_test);
-  Py_CLEAR(clear_module_state->__pyx_n_s_update);
-  Py_CLEAR(clear_module_state->__pyx_n_s_use_setstate);
-  Py_CLEAR(clear_module_state->__pyx_int_163061131);
-  Py_CLEAR(clear_module_state->__pyx_int_179973907);
-  Py_CLEAR(clear_module_state->__pyx_int_250931038);
-  Py_CLEAR(clear_module_state->__pyx_tuple_);
-  Py_CLEAR(clear_module_state->__pyx_tuple__3);
-  Py_CLEAR(clear_module_state->__pyx_tuple__5);
-  Py_CLEAR(clear_module_state->__pyx_tuple__7);
-  Py_CLEAR(clear_module_state->__pyx_tuple__9);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__4);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__6);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__8);
-  Py_CLEAR(clear_module_state->__pyx_codeobj__10);
-  return 0;
-}
-#endif
-/* #### Code section: module_state_traverse ### */
-#if CYTHON_USE_MODULE_STATE
-static int __pyx_m_traverse(PyObject *m, visitproc visit, void *arg) {
-  __pyx_mstate *traverse_module_state = __pyx_mstate(m);
-  if (!traverse_module_state) return 0;
-  Py_VISIT(traverse_module_state->__pyx_d);
-  Py_VISIT(traverse_module_state->__pyx_b);
-  Py_VISIT(traverse_module_state->__pyx_cython_runtime);
-  Py_VISIT(traverse_module_state->__pyx_empty_tuple);
-  Py_VISIT(traverse_module_state->__pyx_empty_bytes);
-  Py_VISIT(traverse_module_state->__pyx_empty_unicode);
-  #ifdef __Pyx_CyFunction_USED
-  Py_VISIT(traverse_module_state->__pyx_CyFunctionType);
-  #endif
-  #ifdef __Pyx_FusedFunction_USED
-  Py_VISIT(traverse_module_state->__pyx_FusedFunctionType);
-  #endif
-  Py_VISIT(traverse_module_state->__pyx_ptype_7camSort_7camSort_StringWithKey);
-  Py_VISIT(traverse_module_state->__pyx_type_7camSort_7camSort_StringWithKey);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0);
-  Py_VISIT(traverse_module_state->__pyx_n_s_PickleError);
-  Py_VISIT(traverse_module_state->__pyx_n_s_StringWithKey);
-  Py_VISIT(traverse_module_state->__pyx_n_s_StringWithKey___reduce_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_StringWithKey___setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s__11);
-  Py_VISIT(traverse_module_state->__pyx_kp_u__2);
-  Py_VISIT(traverse_module_state->__pyx_n_s_array);
-  Py_VISIT(traverse_module_state->__pyx_n_s_asyncio_coroutines);
-  Py_VISIT(traverse_module_state->__pyx_n_s_attrgetter);
-  Py_VISIT(traverse_module_state->__pyx_n_s_camSort_camSort);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_camSort_camSort_pyx);
-  Py_VISIT(traverse_module_state->__pyx_n_s_cline_in_traceback);
-  Py_VISIT(traverse_module_state->__pyx_n_s_dict);
-  Py_VISIT(traverse_module_state->__pyx_n_s_dict_2);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_disable);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_enable);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_gc);
-  Py_VISIT(traverse_module_state->__pyx_n_s_getstate);
-  Py_VISIT(traverse_module_state->__pyx_n_s_import);
-  Py_VISIT(traverse_module_state->__pyx_n_s_input_list);
-  Py_VISIT(traverse_module_state->__pyx_n_s_is_coroutine);
-  Py_VISIT(traverse_module_state->__pyx_kp_u_isenabled);
-  Py_VISIT(traverse_module_state->__pyx_n_s_key);
-  Py_VISIT(traverse_module_state->__pyx_n_u_key);
-  Py_VISIT(traverse_module_state->__pyx_n_s_main);
-  Py_VISIT(traverse_module_state->__pyx_n_s_n);
-  Py_VISIT(traverse_module_state->__pyx_n_s_name);
-  Py_VISIT(traverse_module_state->__pyx_n_s_new);
-  Py_VISIT(traverse_module_state->__pyx_n_s_operator);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pickle);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_PickleError);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_checksum);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_result);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_state);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_type);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_unpickle_StringWithKey);
-  Py_VISIT(traverse_module_state->__pyx_n_s_pyx_vtable);
-  Py_VISIT(traverse_module_state->__pyx_n_s_reduce);
-  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_reduce_ex);
-  Py_VISIT(traverse_module_state->__pyx_n_s_s);
-  Py_VISIT(traverse_module_state->__pyx_n_s_self);
-  Py_VISIT(traverse_module_state->__pyx_n_s_setstate);
-  Py_VISIT(traverse_module_state->__pyx_n_s_setstate_cython);
-  Py_VISIT(traverse_module_state->__pyx_n_s_sortStrings);
-  Py_VISIT(traverse_module_state->__pyx_n_s_sorted);
-  Py_VISIT(traverse_module_state->__pyx_n_s_sorted_array);
-  Py_VISIT(traverse_module_state->__pyx_n_s_state);
-  Py_VISIT(traverse_module_state->__pyx_n_s_str);
-  Py_VISIT(traverse_module_state->__pyx_kp_s_stringsource);
-  Py_VISIT(traverse_module_state->__pyx_n_s_test);
-  Py_VISIT(traverse_module_state->__pyx_n_s_update);
-  Py_VISIT(traverse_module_state->__pyx_n_s_use_setstate);
-  Py_VISIT(traverse_module_state->__pyx_int_163061131);
-  Py_VISIT(traverse_module_state->__pyx_int_179973907);
-  Py_VISIT(traverse_module_state->__pyx_int_250931038);
-  Py_VISIT(traverse_module_state->__pyx_tuple_);
-  Py_VISIT(traverse_module_state->__pyx_tuple__3);
-  Py_VISIT(traverse_module_state->__pyx_tuple__5);
-  Py_VISIT(traverse_module_state->__pyx_tuple__7);
-  Py_VISIT(traverse_module_state->__pyx_tuple__9);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__4);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__6);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__8);
-  Py_VISIT(traverse_module_state->__pyx_codeobj__10);
-  return 0;
-}
-#endif
-/* #### Code section: module_state_defines ### */
-#define __pyx_d __pyx_mstate_global->__pyx_d
-#define __pyx_b __pyx_mstate_global->__pyx_b
-#define __pyx_cython_runtime __pyx_mstate_global->__pyx_cython_runtime
-#define __pyx_empty_tuple __pyx_mstate_global->__pyx_empty_tuple
-#define __pyx_empty_bytes __pyx_mstate_global->__pyx_empty_bytes
-#define __pyx_empty_unicode __pyx_mstate_global->__pyx_empty_unicode
-#ifdef __Pyx_CyFunction_USED
-#define __pyx_CyFunctionType __pyx_mstate_global->__pyx_CyFunctionType
-#endif
-#ifdef __Pyx_FusedFunction_USED
-#define __pyx_FusedFunctionType __pyx_mstate_global->__pyx_FusedFunctionType
-#endif
-#ifdef __Pyx_Generator_USED
-#define __pyx_GeneratorType __pyx_mstate_global->__pyx_GeneratorType
-#endif
-#ifdef __Pyx_IterableCoroutine_USED
-#define __pyx_IterableCoroutineType __pyx_mstate_global->__pyx_IterableCoroutineType
-#endif
-#ifdef __Pyx_Coroutine_USED
-#define __pyx_CoroutineAwaitType __pyx_mstate_global->__pyx_CoroutineAwaitType
-#endif
-#ifdef __Pyx_Coroutine_USED
-#define __pyx_CoroutineType __pyx_mstate_global->__pyx_CoroutineType
-#endif
-#if CYTHON_USE_MODULE_STATE
-#define __pyx_type_7camSort_7camSort_StringWithKey __pyx_mstate_global->__pyx_type_7camSort_7camSort_StringWithKey
-#endif
-#define __pyx_ptype_7camSort_7camSort_StringWithKey __pyx_mstate_global->__pyx_ptype_7camSort_7camSort_StringWithKey
-#define __pyx_kp_s_Incompatible_checksums_0x_x_vs_0 __pyx_mstate_global->__pyx_kp_s_Incompatible_checksums_0x_x_vs_0
-#define __pyx_n_s_PickleError __pyx_mstate_global->__pyx_n_s_PickleError
-#define __pyx_n_s_StringWithKey __pyx_mstate_global->__pyx_n_s_StringWithKey
-#define __pyx_n_s_StringWithKey___reduce_cython __pyx_mstate_global->__pyx_n_s_StringWithKey___reduce_cython
-#define __pyx_n_s_StringWithKey___setstate_cython __pyx_mstate_global->__pyx_n_s_StringWithKey___setstate_cython
-#define __pyx_n_s__11 __pyx_mstate_global->__pyx_n_s__11
-#define __pyx_kp_u__2 __pyx_mstate_global->__pyx_kp_u__2
-#define __pyx_n_s_array __pyx_mstate_global->__pyx_n_s_array
-#define __pyx_n_s_asyncio_coroutines __pyx_mstate_global->__pyx_n_s_asyncio_coroutines
-#define __pyx_n_s_attrgetter __pyx_mstate_global->__pyx_n_s_attrgetter
-#define __pyx_n_s_camSort_camSort __pyx_mstate_global->__pyx_n_s_camSort_camSort
-#define __pyx_kp_s_camSort_camSort_pyx __pyx_mstate_global->__pyx_kp_s_camSort_camSort_pyx
-#define __pyx_n_s_cline_in_traceback __pyx_mstate_global->__pyx_n_s_cline_in_traceback
-#define __pyx_n_s_dict __pyx_mstate_global->__pyx_n_s_dict
-#define __pyx_n_s_dict_2 __pyx_mstate_global->__pyx_n_s_dict_2
-#define __pyx_kp_u_disable __pyx_mstate_global->__pyx_kp_u_disable
-#define __pyx_kp_u_enable __pyx_mstate_global->__pyx_kp_u_enable
-#define __pyx_kp_u_gc __pyx_mstate_global->__pyx_kp_u_gc
-#define __pyx_n_s_getstate __pyx_mstate_global->__pyx_n_s_getstate
-#define __pyx_n_s_import __pyx_mstate_global->__pyx_n_s_import
-#define __pyx_n_s_input_list __pyx_mstate_global->__pyx_n_s_input_list
-#define __pyx_n_s_is_coroutine __pyx_mstate_global->__pyx_n_s_is_coroutine
-#define __pyx_kp_u_isenabled __pyx_mstate_global->__pyx_kp_u_isenabled
-#define __pyx_n_s_key __pyx_mstate_global->__pyx_n_s_key
-#define __pyx_n_u_key __pyx_mstate_global->__pyx_n_u_key
-#define __pyx_n_s_main __pyx_mstate_global->__pyx_n_s_main
-#define __pyx_n_s_n __pyx_mstate_global->__pyx_n_s_n
-#define __pyx_n_s_name __pyx_mstate_global->__pyx_n_s_name
-#define __pyx_n_s_new __pyx_mstate_global->__pyx_n_s_new
-#define __pyx_n_s_operator __pyx_mstate_global->__pyx_n_s_operator
-#define __pyx_n_s_pickle __pyx_mstate_global->__pyx_n_s_pickle
-#define __pyx_n_s_pyx_PickleError __pyx_mstate_global->__pyx_n_s_pyx_PickleError
-#define __pyx_n_s_pyx_checksum __pyx_mstate_global->__pyx_n_s_pyx_checksum
-#define __pyx_n_s_pyx_result __pyx_mstate_global->__pyx_n_s_pyx_result
-#define __pyx_n_s_pyx_state __pyx_mstate_global->__pyx_n_s_pyx_state
-#define __pyx_n_s_pyx_type __pyx_mstate_global->__pyx_n_s_pyx_type
-#define __pyx_n_s_pyx_unpickle_StringWithKey __pyx_mstate_global->__pyx_n_s_pyx_unpickle_StringWithKey
-#define __pyx_n_s_pyx_vtable __pyx_mstate_global->__pyx_n_s_pyx_vtable
-#define __pyx_n_s_reduce __pyx_mstate_global->__pyx_n_s_reduce
-#define __pyx_n_s_reduce_cython __pyx_mstate_global->__pyx_n_s_reduce_cython
-#define __pyx_n_s_reduce_ex __pyx_mstate_global->__pyx_n_s_reduce_ex
-#define __pyx_n_s_s __pyx_mstate_global->__pyx_n_s_s
-#define __pyx_n_s_self __pyx_mstate_global->__pyx_n_s_self
-#define __pyx_n_s_setstate __pyx_mstate_global->__pyx_n_s_setstate
-#define __pyx_n_s_setstate_cython __pyx_mstate_global->__pyx_n_s_setstate_cython
-#define __pyx_n_s_sortStrings __pyx_mstate_global->__pyx_n_s_sortStrings
-#define __pyx_n_s_sorted __pyx_mstate_global->__pyx_n_s_sorted
-#define __pyx_n_s_sorted_array __pyx_mstate_global->__pyx_n_s_sorted_array
-#define __pyx_n_s_state __pyx_mstate_global->__pyx_n_s_state
-#define __pyx_n_s_str __pyx_mstate_global->__pyx_n_s_str
-#define __pyx_kp_s_stringsource __pyx_mstate_global->__pyx_kp_s_stringsource
-#define __pyx_n_s_test __pyx_mstate_global->__pyx_n_s_test
-#define __pyx_n_s_update __pyx_mstate_global->__pyx_n_s_update
-#define __pyx_n_s_use_setstate __pyx_mstate_global->__pyx_n_s_use_setstate
-#define __pyx_int_163061131 __pyx_mstate_global->__pyx_int_163061131
-#define __pyx_int_179973907 __pyx_mstate_global->__pyx_int_179973907
-#define __pyx_int_250931038 __pyx_mstate_global->__pyx_int_250931038
-#define __pyx_tuple_ __pyx_mstate_global->__pyx_tuple_
-#define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
-#define __pyx_tuple__5 __pyx_mstate_global->__pyx_tuple__5
-#define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
-#define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
-#define __pyx_codeobj__4 __pyx_mstate_global->__pyx_codeobj__4
-#define __pyx_codeobj__6 __pyx_mstate_global->__pyx_codeobj__6
-#define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
-#define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
-/* #### Code section: module_code ### */
-
-/* "camSort/camSort.pyx":9
+/* "camSort/stringSort.pyx":9
  *         long long key
  * 
  *     def __init__(self, str):             # <<<<<<<<<<<<<<
  *         self.str = str
  *         self.key = self.calculate_key(str)
  */
 
 /* Python wrapper */
-static int __pyx_pw_7camSort_7camSort_13StringWithKey_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
-static int __pyx_pw_7camSort_7camSort_13StringWithKey_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_1__init__(PyObject *__pyx_v_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v_str = 0;
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__init__ (wrapper)", 0);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_str,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_str,0};
     PyObject* values[1] = {0};
-    if (__pyx_kwds) {
+    if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = __Pyx_NumKwargs_VARARGS(__pyx_kwds);
-      switch (__pyx_nargs) {
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_VARARGS(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_str)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 9, __pyx_L3_error)
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_str)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
       }
       if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__init__") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__init__") < 0)) __PYX_ERR(0, 9, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 1)) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 1) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = __Pyx_Arg_VARARGS(__pyx_args, 0);
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
     }
     __pyx_v_str = values[0];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 9, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__init__", 1, 1, 1, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 9, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return -1;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7camSort_7camSort_13StringWithKey___init__(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v_self), __pyx_v_str);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self), __pyx_v_str);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7camSort_7camSort_13StringWithKey___init__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey___init__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
-  PY_LONG_LONG __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__init__", 0);
 
-  /* "camSort/camSort.pyx":10
+  /* "camSort/stringSort.pyx":10
  * 
  *     def __init__(self, str):
  *         self.str = str             # <<<<<<<<<<<<<<
  *         self.key = self.calculate_key(str)
  * 
  */
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_str))||((__pyx_v_str) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_str))) __PYX_ERR(0, 10, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_str))||((__pyx_v_str) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_str)->tp_name), 0))) __PYX_ERR(0, 10, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_str;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->str);
   __Pyx_DECREF(__pyx_v_self->str);
   __pyx_v_self->str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "camSort/camSort.pyx":11
+  /* "camSort/stringSort.pyx":11
  *     def __init__(self, str):
  *         self.str = str
  *         self.key = self.calculate_key(str)             # <<<<<<<<<<<<<<
  * 
  *     cdef long long calculate_key(self, str):
  */
-  __pyx_t_2 = ((struct __pyx_vtabstruct_7camSort_7camSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str); if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 11, __pyx_L1_error)
-  __pyx_v_self->key = __pyx_t_2;
+  __pyx_v_self->key = ((struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey *)__pyx_v_self->__pyx_vtab)->calculate_key(__pyx_v_self, __pyx_v_str);
 
-  /* "camSort/camSort.pyx":9
+  /* "camSort/stringSort.pyx":9
  *         long long key
  * 
  *     def __init__(self, str):             # <<<<<<<<<<<<<<
  *         self.str = str
  *         self.key = self.calculate_key(str)
  */
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__init__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/camSort.pyx":13
+/* "camSort/stringSort.pyx":13
  *         self.key = self.calculate_key(str)
  * 
  *     cdef long long calculate_key(self, str):             # <<<<<<<<<<<<<<
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  */
 
-static PY_LONG_LONG __pyx_f_7camSort_7camSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
+static PY_LONG_LONG __pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key(CYTHON_UNUSED struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_str) {
   int __pyx_v_length;
   PY_LONG_LONG __pyx_v_sum;
   PyObject *__pyx_v_c = NULL;
   PY_LONG_LONG __pyx_r;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
@@ -2636,62 +1478,62 @@
   PyObject *__pyx_t_4 = NULL;
   long __pyx_t_5;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("calculate_key", 0);
 
-  /* "camSort/camSort.pyx":14
+  /* "camSort/stringSort.pyx":14
  * 
  *     cdef long long calculate_key(self, str):
  *         cdef int length = len(str)             # <<<<<<<<<<<<<<
  *         cdef long long sum = 0
  *         for c in str:
  */
   __pyx_t_1 = PyObject_Length(__pyx_v_str); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 14, __pyx_L1_error)
   __pyx_v_length = __pyx_t_1;
 
-  /* "camSort/camSort.pyx":15
+  /* "camSort/stringSort.pyx":15
  *     cdef long long calculate_key(self, str):
  *         cdef int length = len(str)
  *         cdef long long sum = 0             # <<<<<<<<<<<<<<
  *         for c in str:
  *             sum += ord(c)
  */
   __pyx_v_sum = 0;
 
-  /* "camSort/camSort.pyx":16
+  /* "camSort/stringSort.pyx":16
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  *         for c in str:             # <<<<<<<<<<<<<<
  *             sum += ord(c)
  *         return length * 10000 + sum
  */
   if (likely(PyList_CheckExact(__pyx_v_str)) || PyTuple_CheckExact(__pyx_v_str)) {
     __pyx_t_2 = __pyx_v_str; __Pyx_INCREF(__pyx_t_2); __pyx_t_1 = 0;
     __pyx_t_3 = NULL;
   } else {
     __pyx_t_1 = -1; __pyx_t_2 = PyObject_GetIter(__pyx_v_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 16, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_3 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
+    __pyx_t_3 = Py_TYPE(__pyx_t_2)->tp_iternext; if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 16, __pyx_L1_error)
   }
   for (;;) {
     if (likely(!__pyx_t_3)) {
       if (likely(PyList_CheckExact(__pyx_t_2))) {
         if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 16, __pyx_L1_error)
+        __pyx_t_4 = PyList_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 16, __pyx_L1_error)
         #else
         __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       } else {
         if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_2)) break;
         #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 16, __pyx_L1_error)
+        __pyx_t_4 = PyTuple_GET_ITEM(__pyx_t_2, __pyx_t_1); __Pyx_INCREF(__pyx_t_4); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 16, __pyx_L1_error)
         #else
         __pyx_t_4 = PySequence_ITEM(__pyx_t_2, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 16, __pyx_L1_error)
         __Pyx_GOTREF(__pyx_t_4);
         #endif
       }
     } else {
       __pyx_t_4 = __pyx_t_3(__pyx_t_2);
@@ -2704,87 +1546,86 @@
         break;
       }
       __Pyx_GOTREF(__pyx_t_4);
     }
     __Pyx_XDECREF_SET(__pyx_v_c, __pyx_t_4);
     __pyx_t_4 = 0;
 
-    /* "camSort/camSort.pyx":17
+    /* "camSort/stringSort.pyx":17
  *         cdef long long sum = 0
  *         for c in str:
  *             sum += ord(c)             # <<<<<<<<<<<<<<
  *         return length * 10000 + sum
  * 
  */
     __pyx_t_5 = __Pyx_PyObject_Ord(__pyx_v_c); if (unlikely(__pyx_t_5 == ((long)(long)(Py_UCS4)-1))) __PYX_ERR(0, 17, __pyx_L1_error)
     __pyx_v_sum = (__pyx_v_sum + __pyx_t_5);
 
-    /* "camSort/camSort.pyx":16
+    /* "camSort/stringSort.pyx":16
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  *         for c in str:             # <<<<<<<<<<<<<<
  *             sum += ord(c)
  *         return length * 10000 + sum
  */
   }
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/camSort.pyx":18
+  /* "camSort/stringSort.pyx":18
  *         for c in str:
  *             sum += ord(c)
  *         return length * 10000 + sum             # <<<<<<<<<<<<<<
  * 
- * def sortStrings(input_list):
+ * def byLength(input_list):
  */
   __pyx_r = ((__pyx_v_length * 0x2710) + __pyx_v_sum);
   goto __pyx_L0;
 
-  /* "camSort/camSort.pyx":13
+  /* "camSort/stringSort.pyx":13
  *         self.key = self.calculate_key(str)
  * 
  *     cdef long long calculate_key(self, str):             # <<<<<<<<<<<<<<
  *         cdef int length = len(str)
  *         cdef long long sum = 0
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.calculate_key", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_WriteUnraisable("camSort.stringSort.StringWithKey.calculate_key", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_c);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/camSort.pyx":6
+/* "camSort/stringSort.pyx":6
  * cdef class StringWithKey:
  *     cdef public:
  *         str str             # <<<<<<<<<<<<<<
  *         long long key
  * 
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_7camSort_13StringWithKey_3str_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7camSort_7camSort_13StringWithKey_3str_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3str_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3str_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_7camSort_13StringWithKey_3str___get__(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey_3str___get__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_7camSort_13StringWithKey_3str___get__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self) {
+static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3str___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__", 0);
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_self->str);
   __pyx_r = __pyx_v_self->str;
   goto __pyx_L0;
@@ -2793,71 +1634,69 @@
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static int __pyx_pw_7camSort_7camSort_13StringWithKey_3str_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static int __pyx_pw_7camSort_7camSort_13StringWithKey_3str_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_7camSort_13StringWithKey_3str_2__set__(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_2__set__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7camSort_7camSort_13StringWithKey_3str_2__set__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value) {
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
-  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_v_value))) __PYX_ERR(0, 6, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_v_value))||((__pyx_v_value) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_v_value)->tp_name), 0))) __PYX_ERR(0, 6, __pyx_L1_error)
   __pyx_t_1 = __pyx_v_value;
   __Pyx_INCREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v_self->str);
   __Pyx_DECREF(__pyx_v_self->str);
   __pyx_v_self->str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.str.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.str.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static int __pyx_pw_7camSort_7camSort_13StringWithKey_3str_5__del__(PyObject *__pyx_v_self); /*proto*/
-static int __pyx_pw_7camSort_7camSort_13StringWithKey_3str_5__del__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_5__del__(PyObject *__pyx_v_self); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_5__del__(PyObject *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__del__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_7camSort_13StringWithKey_3str_4__del__(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_4__del__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7camSort_7camSort_13StringWithKey_3str_4__del__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self) {
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3str_4__del__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__del__", 0);
   __Pyx_INCREF(Py_None);
   __Pyx_GIVEREF(Py_None);
   __Pyx_GOTREF(__pyx_v_self->str);
   __Pyx_DECREF(__pyx_v_self->str);
@@ -2865,37 +1704,36 @@
 
   /* function exit code */
   __pyx_r = 0;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/camSort.pyx":7
+/* "camSort/stringSort.pyx":7
  *     cdef public:
  *         str str
  *         long long key             # <<<<<<<<<<<<<<
  * 
  *     def __init__(self, str):
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_7camSort_13StringWithKey_3key_1__get__(PyObject *__pyx_v_self); /*proto*/
-static PyObject *__pyx_pw_7camSort_7camSort_13StringWithKey_3key_1__get__(PyObject *__pyx_v_self) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3key_1__get__(PyObject *__pyx_v_self); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3key_1__get__(PyObject *__pyx_v_self) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__get__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_7camSort_13StringWithKey_3key___get__(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey_3key___get__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_7camSort_13StringWithKey_3key___get__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self) {
+static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_3key___get__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__get__", 0);
@@ -2905,107 +1743,87 @@
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.key.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.key.__get__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* Python wrapper */
-static int __pyx_pw_7camSort_7camSort_13StringWithKey_3key_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
-static int __pyx_pw_7camSort_7camSort_13StringWithKey_3key_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_VARARGS(__pyx_args, __pyx_nargs);
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_3key_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value); /*proto*/
+static int __pyx_pw_7camSort_10stringSort_13StringWithKey_3key_3__set__(PyObject *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__set__ (wrapper)", 0);
-  __pyx_r = __pyx_pf_7camSort_7camSort_13StringWithKey_3key_2__set__(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v_self), ((PyObject *)__pyx_v_value));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_2__set__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self), ((PyObject *)__pyx_v_value));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static int __pyx_pf_7camSort_7camSort_13StringWithKey_3key_2__set__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value) {
+static int __pyx_pf_7camSort_10stringSort_13StringWithKey_3key_2__set__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v_value) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   PY_LONG_LONG __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__set__", 0);
   __pyx_t_1 = __Pyx_PyInt_As_PY_LONG_LONG(__pyx_v_value); if (unlikely((__pyx_t_1 == (PY_LONG_LONG)-1) && PyErr_Occurred())) __PYX_ERR(0, 7, __pyx_L1_error)
   __pyx_v_self->key = __pyx_t_1;
 
   /* function exit code */
   __pyx_r = 0;
   goto __pyx_L0;
   __pyx_L1_error:;
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.key.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.key.__set__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":1
  * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
  *     cdef tuple state
  *     cdef object _dict
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_7camSort_13StringWithKey_3__reduce_cython__(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_7camSort_13StringWithKey_3__reduce_cython__ = {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7camSort_7camSort_13StringWithKey_3__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7camSort_7camSort_13StringWithKey_3__reduce_cython__(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
+static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_3__reduce_cython__(PyObject *__pyx_v_self, CYTHON_UNUSED PyObject *unused) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__reduce_cython__ (wrapper)", 0);
-  if (unlikely(__pyx_nargs > 0)) {
-    __Pyx_RaiseArgtupleInvalid("__reduce_cython__", 1, 0, 0, __pyx_nargs); return NULL;}
-  if (unlikely(__pyx_kwds) && __Pyx_NumKwargs_FASTCALL(__pyx_kwds) && unlikely(!__Pyx_CheckKeywordStrings(__pyx_kwds, "__reduce_cython__", 0))) return NULL;
-  __pyx_r = __pyx_pf_7camSort_7camSort_13StringWithKey_2__reduce_cython__(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v_self));
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey_2__reduce_cython__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_7camSort_13StringWithKey_2__reduce_cython__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self) {
+static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_2__reduce_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self) {
   PyObject *__pyx_v_state = 0;
   PyObject *__pyx_v__dict = 0;
   int __pyx_v_use_setstate;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
   int __pyx_t_3;
-  PyObject *__pyx_t_4 = NULL;
+  int __pyx_t_4;
+  PyObject *__pyx_t_5 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__reduce_cython__", 0);
 
   /* "(tree fragment)":5
  *     cdef object _dict
@@ -3043,15 +1861,16 @@
  *     state = (self.key, self.str)
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:             # <<<<<<<<<<<<<<
  *         state += (_dict,)
  *         use_setstate = True
  */
   __pyx_t_3 = (__pyx_v__dict != Py_None);
-  if (__pyx_t_3) {
+  __pyx_t_4 = (__pyx_t_3 != 0);
+  if (__pyx_t_4) {
 
     /* "(tree fragment)":8
  *     _dict = getattr(self, '__dict__', None)
  *     if _dict is not None:
  *         state += (_dict,)             # <<<<<<<<<<<<<<
  *         use_setstate = True
  *     else:
@@ -3087,105 +1906,106 @@
   }
 
   /* "(tree fragment)":11
  *         use_setstate = True
  *     else:
  *         use_setstate = self.str is not None             # <<<<<<<<<<<<<<
  *     if use_setstate:
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, None), state
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state
  */
   /*else*/ {
-    __pyx_t_3 = (__pyx_v_self->str != ((PyObject*)Py_None));
-    __pyx_v_use_setstate = __pyx_t_3;
+    __pyx_t_4 = (__pyx_v_self->str != ((PyObject*)Py_None));
+    __pyx_v_use_setstate = __pyx_t_4;
   }
   __pyx_L3:;
 
   /* "(tree fragment)":12
  *     else:
  *         use_setstate = self.str is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, None), state
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state
  *     else:
  */
-  if (__pyx_v_use_setstate) {
+  __pyx_t_4 = (__pyx_v_use_setstate != 0);
+  if (__pyx_t_4) {
 
     /* "(tree fragment)":13
  *         use_setstate = self.str is not None
  *     if use_setstate:
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, None), state             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state             # <<<<<<<<<<<<<<
  *     else:
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, state)
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, state)
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_pyx_unpickle_StringWithKey); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 13, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_INCREF(__pyx_int_163061131);
-    __Pyx_GIVEREF(__pyx_int_163061131);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_163061131);
+    __Pyx_INCREF(__pyx_int_250931038);
+    __Pyx_GIVEREF(__pyx_int_250931038);
+    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_250931038);
     __Pyx_INCREF(Py_None);
     __Pyx_GIVEREF(Py_None);
     PyTuple_SET_ITEM(__pyx_t_2, 2, Py_None);
-    __pyx_t_4 = PyTuple_New(3); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 13, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_5 = PyTuple_New(3); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 13, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_1);
-    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_5, 0, __pyx_t_1);
     __Pyx_GIVEREF(__pyx_t_2);
-    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_2);
+    PyTuple_SET_ITEM(__pyx_t_5, 1, __pyx_t_2);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
-    PyTuple_SET_ITEM(__pyx_t_4, 2, __pyx_v_state);
+    PyTuple_SET_ITEM(__pyx_t_5, 2, __pyx_v_state);
     __pyx_t_1 = 0;
     __pyx_t_2 = 0;
-    __pyx_r = __pyx_t_4;
-    __pyx_t_4 = 0;
+    __pyx_r = __pyx_t_5;
+    __pyx_t_5 = 0;
     goto __pyx_L0;
 
     /* "(tree fragment)":12
  *     else:
  *         use_setstate = self.str is not None
  *     if use_setstate:             # <<<<<<<<<<<<<<
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, None), state
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state
  *     else:
  */
   }
 
   /* "(tree fragment)":15
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, None), state
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, None), state
  *     else:
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, state)             # <<<<<<<<<<<<<<
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, state)             # <<<<<<<<<<<<<<
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_StringWithKey__set_state(self, __pyx_state)
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
-    __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_pyx_unpickle_StringWithKey); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 15, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_GetModuleGlobalName(__pyx_t_5, __pyx_n_s_pyx_unpickle_StringWithKey); if (unlikely(!__pyx_t_5)) __PYX_ERR(1, 15, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_5);
     __pyx_t_2 = PyTuple_New(3); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     __Pyx_GIVEREF(((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
     PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)Py_TYPE(((PyObject *)__pyx_v_self))));
-    __Pyx_INCREF(__pyx_int_163061131);
-    __Pyx_GIVEREF(__pyx_int_163061131);
-    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_163061131);
+    __Pyx_INCREF(__pyx_int_250931038);
+    __Pyx_GIVEREF(__pyx_int_250931038);
+    PyTuple_SET_ITEM(__pyx_t_2, 1, __pyx_int_250931038);
     __Pyx_INCREF(__pyx_v_state);
     __Pyx_GIVEREF(__pyx_v_state);
     PyTuple_SET_ITEM(__pyx_t_2, 2, __pyx_v_state);
     __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 15, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_GIVEREF(__pyx_t_4);
-    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_4);
+    __Pyx_GIVEREF(__pyx_t_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_5);
     __Pyx_GIVEREF(__pyx_t_2);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_2);
-    __pyx_t_4 = 0;
+    __pyx_t_5 = 0;
     __pyx_t_2 = 0;
     __pyx_r = __pyx_t_1;
     __pyx_t_1 = 0;
     goto __pyx_L0;
   }
 
   /* "(tree fragment)":1
@@ -3194,284 +2014,168 @@
  *     cdef object _dict
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__reduce_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_state);
   __Pyx_XDECREF(__pyx_v__dict);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "(tree fragment)":16
  *     else:
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, state)
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_StringWithKey__set_state(self, __pyx_state)
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_7camSort_13StringWithKey_5__setstate_cython__(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_7camSort_13StringWithKey_5__setstate_cython__ = {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7camSort_7camSort_13StringWithKey_5__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7camSort_7camSort_13StringWithKey_5__setstate_cython__(PyObject *__pyx_v_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v___pyx_state = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state); /*proto*/
+static PyObject *__pyx_pw_7camSort_10stringSort_13StringWithKey_5__setstate_cython__(PyObject *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__setstate_cython__ (wrapper)", 0);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_state,0};
-    PyObject* values[1] = {0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 16, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__setstate_cython__") < 0)) __PYX_ERR(1, 16, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 1)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-    }
-    __pyx_v___pyx_state = values[0];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__setstate_cython__", 1, 1, 1, __pyx_nargs); __PYX_ERR(1, 16, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7camSort_7camSort_13StringWithKey_4__setstate_cython__(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v_self), __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_13StringWithKey_4__setstate_cython__(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v_self), ((PyObject *)__pyx_v___pyx_state));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_7camSort_13StringWithKey_4__setstate_cython__(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7camSort_10stringSort_13StringWithKey_4__setstate_cython__(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v_self, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__setstate_cython__", 0);
 
   /* "(tree fragment)":17
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, state)
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, state)
  * def __setstate_cython__(self, __pyx_state):
  *     __pyx_unpickle_StringWithKey__set_state(self, __pyx_state)             # <<<<<<<<<<<<<<
  */
-  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 17, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_7camSort_7camSort___pyx_unpickle_StringWithKey__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
+  if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 17, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_7camSort_10stringSort___pyx_unpickle_StringWithKey__set_state(__pyx_v_self, ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 17, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
   /* "(tree fragment)":16
  *     else:
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, state)
+ *         return __pyx_unpickle_StringWithKey, (type(self), 0xef4e75e, state)
  * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_unpickle_StringWithKey__set_state(self, __pyx_state)
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_AddTraceback("camSort.camSort.StringWithKey.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.StringWithKey.__setstate_cython__", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "camSort/camSort.pyx":20
+/* "camSort/stringSort.pyx":20
  *         return length * 10000 + sum
  * 
- * def sortStrings(input_list):             # <<<<<<<<<<<<<<
+ * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_7camSort_1sortStrings(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_7camSort_1sortStrings = {"sortStrings", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7camSort_7camSort_1sortStrings, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7camSort_7camSort_1sortStrings(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
-  PyObject *__pyx_v_input_list = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
+static PyObject *__pyx_pw_7camSort_10stringSort_1byLength(PyObject *__pyx_self, PyObject *__pyx_v_input_list); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_1byLength = {"byLength", (PyCFunction)__pyx_pw_7camSort_10stringSort_1byLength, METH_O, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_1byLength(PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
-  __Pyx_RefNannySetupContext("sortStrings (wrapper)", 0);
-  {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_input_list,0};
-    PyObject* values[1] = {0};
-    if (__pyx_kwds) {
-      Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-        CYTHON_FALLTHROUGH;
-        case  0: break;
-        default: goto __pyx_L5_argtuple_error;
-      }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
-        case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_input_list)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(0, 20, __pyx_L3_error)
-        else goto __pyx_L5_argtuple_error;
-      }
-      if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "sortStrings") < 0)) __PYX_ERR(0, 20, __pyx_L3_error)
-      }
-    } else if (unlikely(__pyx_nargs != 1)) {
-      goto __pyx_L5_argtuple_error;
-    } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-    }
-    __pyx_v_input_list = values[0];
-  }
-  goto __pyx_L4_argument_unpacking_done;
-  __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("sortStrings", 1, 1, 1, __pyx_nargs); __PYX_ERR(0, 20, __pyx_L3_error)
-  __pyx_L3_error:;
-  __Pyx_AddTraceback("camSort.camSort.sortStrings", __pyx_clineno, __pyx_lineno, __pyx_filename);
-  __Pyx_RefNannyFinishContext();
-  return NULL;
-  __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7camSort_7camSort_sortStrings(__pyx_self, __pyx_v_input_list);
+  __Pyx_RefNannySetupContext("byLength (wrapper)", 0);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_byLength(__pyx_self, ((PyObject *)__pyx_v_input_list));
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_7camSort_sortStrings(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
+static PyObject *__pyx_pf_7camSort_10stringSort_byLength(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_input_list) {
   CYTHON_UNUSED int __pyx_v_n;
   PyObject *__pyx_v_array = 0;
   PyObject *__pyx_v_sorted_array = NULL;
   PyObject *__pyx_7genexpr__pyx_v_s = NULL;
   PyObject *__pyx_8genexpr1__pyx_v_s = NULL;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   Py_ssize_t __pyx_t_1;
   PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *(*__pyx_t_4)(PyObject *);
   PyObject *__pyx_t_5 = NULL;
   PyObject *__pyx_t_6 = NULL;
   PyObject *__pyx_t_7 = NULL;
-  int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
-  __Pyx_RefNannySetupContext("sortStrings", 0);
+  __Pyx_RefNannySetupContext("byLength", 0);
 
-  /* "camSort/camSort.pyx":21
+  /* "camSort/stringSort.pyx":21
  * 
- * def sortStrings(input_list):
+ * def byLength(input_list):
  *     cdef int n = len(input_list)             # <<<<<<<<<<<<<<
  *     cdef list array = [StringWithKey(s) for s in input_list]
  * 
  */
   __pyx_t_1 = PyObject_Length(__pyx_v_input_list); if (unlikely(__pyx_t_1 == ((Py_ssize_t)-1))) __PYX_ERR(0, 21, __pyx_L1_error)
   __pyx_v_n = __pyx_t_1;
 
-  /* "camSort/camSort.pyx":22
- * def sortStrings(input_list):
+  /* "camSort/stringSort.pyx":22
+ * def byLength(input_list):
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]             # <<<<<<<<<<<<<<
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
  */
   { /* enter inner scope */
     __pyx_t_2 = PyList_New(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 22, __pyx_L5_error)
     __Pyx_GOTREF(__pyx_t_2);
     if (likely(PyList_CheckExact(__pyx_v_input_list)) || PyTuple_CheckExact(__pyx_v_input_list)) {
       __pyx_t_3 = __pyx_v_input_list; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
       __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_input_list); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 22, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 22, __pyx_L5_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 22, __pyx_L5_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 22, __pyx_L5_error)
+          __pyx_t_5 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 22, __pyx_L5_error)
           #else
           __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 22, __pyx_L5_error)
+          __pyx_t_5 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_5); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 22, __pyx_L5_error)
           #else
           __pyx_t_5 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L5_error)
           __Pyx_GOTREF(__pyx_t_5);
           #endif
         }
       } else {
         __pyx_t_5 = __pyx_t_4(__pyx_t_3);
@@ -3483,31 +2187,31 @@
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_5);
       }
       __Pyx_XDECREF_SET(__pyx_7genexpr__pyx_v_s, __pyx_t_5);
       __pyx_t_5 = 0;
-      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_7camSort_StringWithKey), __pyx_7genexpr__pyx_v_s); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L5_error)
+      __pyx_t_5 = __Pyx_PyObject_CallOneArg(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_7genexpr__pyx_v_s); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 22, __pyx_L5_error)
       __Pyx_GOTREF(__pyx_t_5);
       if (unlikely(__Pyx_ListComp_Append(__pyx_t_2, (PyObject*)__pyx_t_5))) __PYX_ERR(0, 22, __pyx_L5_error)
       __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s); __pyx_7genexpr__pyx_v_s = 0;
-    goto __pyx_L9_exit_scope;
+    goto __pyx_L8_exit_scope;
     __pyx_L5_error:;
     __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s); __pyx_7genexpr__pyx_v_s = 0;
     goto __pyx_L1_error;
-    __pyx_L9_exit_scope:;
+    __pyx_L8_exit_scope:;
   } /* exit inner scope */
   __pyx_v_array = ((PyObject*)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "camSort/camSort.pyx":24
+  /* "camSort/stringSort.pyx":24
  *     cdef list array = [StringWithKey(s) for s in input_list]
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))             # <<<<<<<<<<<<<<
  *     return [s.str for s in sorted_array]
  */
   __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -3515,125 +2219,120 @@
   __Pyx_GIVEREF(__pyx_v_array);
   PyTuple_SET_ITEM(__pyx_t_2, 0, __pyx_v_array);
   __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GetModuleGlobalName(__pyx_t_6, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_6);
   __pyx_t_7 = NULL;
-  __pyx_t_8 = 0;
   if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_6))) {
     __pyx_t_7 = PyMethod_GET_SELF(__pyx_t_6);
     if (likely(__pyx_t_7)) {
       PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_6);
       __Pyx_INCREF(__pyx_t_7);
       __Pyx_INCREF(function);
       __Pyx_DECREF_SET(__pyx_t_6, function);
-      __pyx_t_8 = 1;
     }
   }
-  {
-    PyObject *__pyx_callargs[2] = {__pyx_t_7, __pyx_n_u_key};
-    __pyx_t_5 = __Pyx_PyObject_FastCall(__pyx_t_6, __pyx_callargs+1-__pyx_t_8, 1+__pyx_t_8);
-    __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
-    if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_5);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-  }
+  __pyx_t_5 = (__pyx_t_7) ? __Pyx_PyObject_Call2Args(__pyx_t_6, __pyx_t_7, __pyx_n_u_key) : __Pyx_PyObject_CallOneArg(__pyx_t_6, __pyx_n_u_key);
+  __Pyx_XDECREF(__pyx_t_7); __pyx_t_7 = 0;
+  if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_5);
+  __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
   if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_key, __pyx_t_5) < 0) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
   __pyx_t_5 = __Pyx_PyObject_Call(__pyx_builtin_sorted, __pyx_t_2, __pyx_t_3); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 24, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __pyx_v_sorted_array = __pyx_t_5;
   __pyx_t_5 = 0;
 
-  /* "camSort/camSort.pyx":25
+  /* "camSort/stringSort.pyx":25
  * 
  *     sorted_array = sorted(array, key=attrgetter('key'))
  *     return [s.str for s in sorted_array]             # <<<<<<<<<<<<<<
  */
   __Pyx_XDECREF(__pyx_r);
   { /* enter inner scope */
-    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L12_error)
+    __pyx_t_5 = PyList_New(0); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 25, __pyx_L11_error)
     __Pyx_GOTREF(__pyx_t_5);
     if (likely(PyList_CheckExact(__pyx_v_sorted_array)) || PyTuple_CheckExact(__pyx_v_sorted_array)) {
       __pyx_t_3 = __pyx_v_sorted_array; __Pyx_INCREF(__pyx_t_3); __pyx_t_1 = 0;
       __pyx_t_4 = NULL;
     } else {
-      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L12_error)
+      __pyx_t_1 = -1; __pyx_t_3 = PyObject_GetIter(__pyx_v_sorted_array); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 25, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_3);
-      __pyx_t_4 = __Pyx_PyObject_GetIterNextFunc(__pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L12_error)
+      __pyx_t_4 = Py_TYPE(__pyx_t_3)->tp_iternext; if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 25, __pyx_L11_error)
     }
     for (;;) {
       if (likely(!__pyx_t_4)) {
         if (likely(PyList_CheckExact(__pyx_t_3))) {
           if (__pyx_t_1 >= PyList_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 25, __pyx_L12_error)
+          __pyx_t_2 = PyList_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 25, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L12_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         } else {
           if (__pyx_t_1 >= PyTuple_GET_SIZE(__pyx_t_3)) break;
           #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely((0 < 0))) __PYX_ERR(0, 25, __pyx_L12_error)
+          __pyx_t_2 = PyTuple_GET_ITEM(__pyx_t_3, __pyx_t_1); __Pyx_INCREF(__pyx_t_2); __pyx_t_1++; if (unlikely(0 < 0)) __PYX_ERR(0, 25, __pyx_L11_error)
           #else
-          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L12_error)
+          __pyx_t_2 = PySequence_ITEM(__pyx_t_3, __pyx_t_1); __pyx_t_1++; if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L11_error)
           __Pyx_GOTREF(__pyx_t_2);
           #endif
         }
       } else {
         __pyx_t_2 = __pyx_t_4(__pyx_t_3);
         if (unlikely(!__pyx_t_2)) {
           PyObject* exc_type = PyErr_Occurred();
           if (exc_type) {
             if (likely(__Pyx_PyErr_GivenExceptionMatches(exc_type, PyExc_StopIteration))) PyErr_Clear();
-            else __PYX_ERR(0, 25, __pyx_L12_error)
+            else __PYX_ERR(0, 25, __pyx_L11_error)
           }
           break;
         }
         __Pyx_GOTREF(__pyx_t_2);
       }
       __Pyx_XDECREF_SET(__pyx_8genexpr1__pyx_v_s, __pyx_t_2);
       __pyx_t_2 = 0;
-      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L12_error)
+      __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_8genexpr1__pyx_v_s, __pyx_n_s_str); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L11_error)
       __Pyx_GOTREF(__pyx_t_2);
-      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 25, __pyx_L12_error)
+      if (unlikely(__Pyx_ListComp_Append(__pyx_t_5, (PyObject*)__pyx_t_2))) __PYX_ERR(0, 25, __pyx_L11_error)
       __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     }
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s); __pyx_8genexpr1__pyx_v_s = 0;
-    goto __pyx_L16_exit_scope;
-    __pyx_L12_error:;
+    goto __pyx_L14_exit_scope;
+    __pyx_L11_error:;
     __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s); __pyx_8genexpr1__pyx_v_s = 0;
     goto __pyx_L1_error;
-    __pyx_L16_exit_scope:;
+    __pyx_L14_exit_scope:;
   } /* exit inner scope */
   __pyx_r = __pyx_t_5;
   __pyx_t_5 = 0;
   goto __pyx_L0;
 
-  /* "camSort/camSort.pyx":20
+  /* "camSort/stringSort.pyx":20
  *         return length * 10000 + sum
  * 
- * def sortStrings(input_list):             # <<<<<<<<<<<<<<
+ * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_5);
   __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
-  __Pyx_AddTraceback("camSort.camSort.sortStrings", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.byLength", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_array);
   __Pyx_XDECREF(__pyx_v_sorted_array);
   __Pyx_XDECREF(__pyx_7genexpr__pyx_v_s);
   __Pyx_XDECREF(__pyx_8genexpr1__pyx_v_s);
   __Pyx_XGIVEREF(__pyx_r);
@@ -3644,239 +2343,231 @@
 /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
 /* Python wrapper */
-static PyObject *__pyx_pw_7camSort_7camSort_3__pyx_unpickle_StringWithKey(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-); /*proto*/
-static PyMethodDef __pyx_mdef_7camSort_7camSort_3__pyx_unpickle_StringWithKey = {"__pyx_unpickle_StringWithKey", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7camSort_7camSort_3__pyx_unpickle_StringWithKey, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0};
-static PyObject *__pyx_pw_7camSort_7camSort_3__pyx_unpickle_StringWithKey(PyObject *__pyx_self, 
-#if CYTHON_METH_FASTCALL
-PyObject *const *__pyx_args, Py_ssize_t __pyx_nargs, PyObject *__pyx_kwds
-#else
-PyObject *__pyx_args, PyObject *__pyx_kwds
-#endif
-) {
+static PyObject *__pyx_pw_7camSort_10stringSort_3__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static PyMethodDef __pyx_mdef_7camSort_10stringSort_3__pyx_unpickle_StringWithKey = {"__pyx_unpickle_StringWithKey", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_7camSort_10stringSort_3__pyx_unpickle_StringWithKey, METH_VARARGS|METH_KEYWORDS, 0};
+static PyObject *__pyx_pw_7camSort_10stringSort_3__pyx_unpickle_StringWithKey(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
   PyObject *__pyx_v___pyx_type = 0;
   long __pyx_v___pyx_checksum;
   PyObject *__pyx_v___pyx_state = 0;
-  #if !CYTHON_METH_FASTCALL
-  CYTHON_UNUSED const Py_ssize_t __pyx_nargs = PyTuple_GET_SIZE(__pyx_args);
-  #endif
-  CYTHON_UNUSED PyObject *const *__pyx_kwvalues = __Pyx_KwValues_FASTCALL(__pyx_args, __pyx_nargs);
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   PyObject *__pyx_r = 0;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__pyx_unpickle_StringWithKey (wrapper)", 0);
   {
-    PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_pyx_type,&__pyx_n_s_pyx_checksum,&__pyx_n_s_pyx_state,0};
     PyObject* values[3] = {0,0,0};
-    if (__pyx_kwds) {
+    if (unlikely(__pyx_kwds)) {
       Py_ssize_t kw_args;
-      switch (__pyx_nargs) {
-        case  3: values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
-        case  2: values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         CYTHON_FALLTHROUGH;
-        case  1: values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         CYTHON_FALLTHROUGH;
         case  0: break;
         default: goto __pyx_L5_argtuple_error;
       }
-      kw_args = __Pyx_NumKwargs_FASTCALL(__pyx_kwds);
-      switch (__pyx_nargs) {
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
         case  0:
-        if (likely((values[0] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_type)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_type)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
-        if (likely((values[1] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_checksum)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_StringWithKey", 1, 3, 3, 1); __PYX_ERR(1, 1, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
-        if (likely((values[2] = __Pyx_GetKwValue_FASTCALL(__pyx_kwds, __pyx_kwvalues, __pyx_n_s_pyx_state)) != 0)) kw_args--;
-        else if (unlikely(PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_pyx_state)) != 0)) kw_args--;
         else {
           __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_StringWithKey", 1, 3, 3, 2); __PYX_ERR(1, 1, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        const Py_ssize_t kwd_pos_args = __pyx_nargs;
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_kwvalues, __pyx_pyargnames, 0, values + 0, kwd_pos_args, "__pyx_unpickle_StringWithKey") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "__pyx_unpickle_StringWithKey") < 0)) __PYX_ERR(1, 1, __pyx_L3_error)
       }
-    } else if (unlikely(__pyx_nargs != 3)) {
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
-      values[0] = __Pyx_Arg_FASTCALL(__pyx_args, 0);
-      values[1] = __Pyx_Arg_FASTCALL(__pyx_args, 1);
-      values[2] = __Pyx_Arg_FASTCALL(__pyx_args, 2);
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v___pyx_type = values[0];
     __pyx_v___pyx_checksum = __Pyx_PyInt_As_long(values[1]); if (unlikely((__pyx_v___pyx_checksum == (long)-1) && PyErr_Occurred())) __PYX_ERR(1, 1, __pyx_L3_error)
     __pyx_v___pyx_state = values[2];
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_StringWithKey", 1, 3, 3, __pyx_nargs); __PYX_ERR(1, 1, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("__pyx_unpickle_StringWithKey", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(1, 1, __pyx_L3_error)
   __pyx_L3_error:;
-  __Pyx_AddTraceback("camSort.camSort.__pyx_unpickle_StringWithKey", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_StringWithKey", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  __pyx_r = __pyx_pf_7camSort_7camSort_2__pyx_unpickle_StringWithKey(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
+  __pyx_r = __pyx_pf_7camSort_10stringSort_2__pyx_unpickle_StringWithKey(__pyx_self, __pyx_v___pyx_type, __pyx_v___pyx_checksum, __pyx_v___pyx_state);
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-static PyObject *__pyx_pf_7camSort_7camSort_2__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_pf_7camSort_10stringSort_2__pyx_unpickle_StringWithKey(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v___pyx_type, long __pyx_v___pyx_checksum, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_v___pyx_PickleError = 0;
   PyObject *__pyx_v___pyx_result = 0;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
-  PyObject *__pyx_t_1 = NULL;
-  int __pyx_t_2;
+  int __pyx_t_1;
+  PyObject *__pyx_t_2 = NULL;
   PyObject *__pyx_t_3 = NULL;
   PyObject *__pyx_t_4 = NULL;
-  int __pyx_t_5;
+  PyObject *__pyx_t_5 = NULL;
+  int __pyx_t_6;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_StringWithKey", 0);
 
   /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x9b81d8b, 0xaba2f13, 0xef4e75e):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum != 0xef4e75e:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))" % __pyx_checksum
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xef4e75e = (key, str))" % __pyx_checksum)
  */
-  __pyx_t_1 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = (__Pyx_PySequence_ContainsTF(__pyx_t_1, __pyx_tuple_, Py_NE)); if (unlikely((__pyx_t_2 < 0))) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (__pyx_t_2) {
+  __pyx_t_1 = ((__pyx_v___pyx_checksum != 0xef4e75e) != 0);
+  if (__pyx_t_1) {
 
     /* "(tree fragment)":5
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x9b81d8b, 0xaba2f13, 0xef4e75e):
+ *     if __pyx_checksum != 0xef4e75e:
  *         from pickle import PickleError as __pyx_PickleError             # <<<<<<<<<<<<<<
- *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))" % __pyx_checksum
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xef4e75e = (key, str))" % __pyx_checksum)
  *     __pyx_result = StringWithKey.__new__(__pyx_type)
  */
-    __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
     __Pyx_INCREF(__pyx_n_s_PickleError);
     __Pyx_GIVEREF(__pyx_n_s_PickleError);
-    PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_PickleError);
-    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_1, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
+    PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_PickleError);
+    __pyx_t_3 = __Pyx_Import(__pyx_n_s_pickle, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 5, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-    __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 5, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_INCREF(__pyx_t_1);
-    __pyx_v___pyx_PickleError = __pyx_t_1;
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_PickleError); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 5, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __Pyx_INCREF(__pyx_t_2);
+    __pyx_v___pyx_PickleError = __pyx_t_2;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":6
- *     if __pyx_checksum not in (0x9b81d8b, 0xaba2f13, 0xef4e75e):
+ *     if __pyx_checksum != 0xef4e75e:
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))" % __pyx_checksum             # <<<<<<<<<<<<<<
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xef4e75e = (key, str))" % __pyx_checksum)             # <<<<<<<<<<<<<<
  *     __pyx_result = StringWithKey.__new__(__pyx_type)
  *     if __pyx_state is not None:
  */
-    __pyx_t_3 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyInt_From_long(__pyx_v___pyx_checksum); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_s_vs_0xef, __pyx_t_2); if (unlikely(!__pyx_t_4)) __PYX_ERR(1, 6, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_INCREF(__pyx_v___pyx_PickleError);
+    __pyx_t_2 = __pyx_v___pyx_PickleError; __pyx_t_5 = NULL;
+    if (CYTHON_UNPACK_METHODS && unlikely(PyMethod_Check(__pyx_t_2))) {
+      __pyx_t_5 = PyMethod_GET_SELF(__pyx_t_2);
+      if (likely(__pyx_t_5)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
+        __Pyx_INCREF(__pyx_t_5);
+        __Pyx_INCREF(function);
+        __Pyx_DECREF_SET(__pyx_t_2, function);
+      }
+    }
+    __pyx_t_3 = (__pyx_t_5) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_5, __pyx_t_4) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_t_4);
+    __Pyx_XDECREF(__pyx_t_5); __pyx_t_5 = 0;
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 6, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
-    __pyx_t_1 = __Pyx_PyString_Format(__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_t_3); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 6, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+    __Pyx_Raise(__pyx_t_3, 0, 0, 0);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-    __Pyx_Raise(__pyx_v___pyx_PickleError, __pyx_t_1, 0, 0);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __PYX_ERR(1, 6, __pyx_L1_error)
 
     /* "(tree fragment)":4
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x9b81d8b, 0xaba2f13, 0xef4e75e):             # <<<<<<<<<<<<<<
+ *     if __pyx_checksum != 0xef4e75e:             # <<<<<<<<<<<<<<
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))" % __pyx_checksum
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xef4e75e = (key, str))" % __pyx_checksum)
  */
   }
 
   /* "(tree fragment)":7
  *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))" % __pyx_checksum
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xef4e75e = (key, str))" % __pyx_checksum)
  *     __pyx_result = StringWithKey.__new__(__pyx_type)             # <<<<<<<<<<<<<<
  *     if __pyx_state is not None:
  *         __pyx_unpickle_StringWithKey__set_state(<StringWithKey> __pyx_result, __pyx_state)
  */
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7camSort_7camSort_StringWithKey), __pyx_n_s_new); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_ptype_7camSort_10stringSort_StringWithKey), __pyx_n_s_new); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
   __pyx_t_4 = NULL;
-  __pyx_t_5 = 0;
-  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_3))) {
-    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_3);
+  if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_2))) {
+    __pyx_t_4 = PyMethod_GET_SELF(__pyx_t_2);
     if (likely(__pyx_t_4)) {
-      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_3);
+      PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_2);
       __Pyx_INCREF(__pyx_t_4);
       __Pyx_INCREF(function);
-      __Pyx_DECREF_SET(__pyx_t_3, function);
-      __pyx_t_5 = 1;
+      __Pyx_DECREF_SET(__pyx_t_2, function);
     }
   }
-  {
-    PyObject *__pyx_callargs[2] = {__pyx_t_4, __pyx_v___pyx_type};
-    __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_3, __pyx_callargs+1-__pyx_t_5, 1+__pyx_t_5);
-    __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
-    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 7, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  }
-  __pyx_v___pyx_result = __pyx_t_1;
-  __pyx_t_1 = 0;
+  __pyx_t_3 = (__pyx_t_4) ? __Pyx_PyObject_Call2Args(__pyx_t_2, __pyx_t_4, __pyx_v___pyx_type) : __Pyx_PyObject_CallOneArg(__pyx_t_2, __pyx_v___pyx_type);
+  __Pyx_XDECREF(__pyx_t_4); __pyx_t_4 = 0;
+  if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 7, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v___pyx_result = __pyx_t_3;
+  __pyx_t_3 = 0;
 
   /* "(tree fragment)":8
- *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))" % __pyx_checksum
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xef4e75e = (key, str))" % __pyx_checksum)
  *     __pyx_result = StringWithKey.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_StringWithKey__set_state(<StringWithKey> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
-  __pyx_t_2 = (__pyx_v___pyx_state != Py_None);
-  if (__pyx_t_2) {
+  __pyx_t_1 = (__pyx_v___pyx_state != Py_None);
+  __pyx_t_6 = (__pyx_t_1 != 0);
+  if (__pyx_t_6) {
 
     /* "(tree fragment)":9
  *     __pyx_result = StringWithKey.__new__(__pyx_type)
  *     if __pyx_state is not None:
  *         __pyx_unpickle_StringWithKey__set_state(<StringWithKey> __pyx_result, __pyx_state)             # <<<<<<<<<<<<<<
  *     return __pyx_result
  * cdef __pyx_unpickle_StringWithKey__set_state(StringWithKey __pyx_result, tuple __pyx_state):
  */
-    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None) || __Pyx_RaiseUnexpectedTypeError("tuple", __pyx_v___pyx_state))) __PYX_ERR(1, 9, __pyx_L1_error)
-    __pyx_t_1 = __pyx_f_7camSort_7camSort___pyx_unpickle_StringWithKey__set_state(((struct __pyx_obj_7camSort_7camSort_StringWithKey *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 9, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_1);
-    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    if (!(likely(PyTuple_CheckExact(__pyx_v___pyx_state))||((__pyx_v___pyx_state) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "tuple", Py_TYPE(__pyx_v___pyx_state)->tp_name), 0))) __PYX_ERR(1, 9, __pyx_L1_error)
+    __pyx_t_3 = __pyx_f_7camSort_10stringSort___pyx_unpickle_StringWithKey__set_state(((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)__pyx_v___pyx_result), ((PyObject*)__pyx_v___pyx_state)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 9, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_3);
+    __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
     /* "(tree fragment)":8
- *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))" % __pyx_checksum
+ *         raise __pyx_PickleError("Incompatible checksums (%s vs 0xef4e75e = (key, str))" % __pyx_checksum)
  *     __pyx_result = StringWithKey.__new__(__pyx_type)
  *     if __pyx_state is not None:             # <<<<<<<<<<<<<<
  *         __pyx_unpickle_StringWithKey__set_state(<StringWithKey> __pyx_result, __pyx_state)
  *     return __pyx_result
  */
   }
 
@@ -3896,18 +2587,19 @@
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
 
   /* function exit code */
   __pyx_L1_error:;
-  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
   __Pyx_XDECREF(__pyx_t_3);
   __Pyx_XDECREF(__pyx_t_4);
-  __Pyx_AddTraceback("camSort.camSort.__pyx_unpickle_StringWithKey", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_5);
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_StringWithKey", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v___pyx_PickleError);
   __Pyx_XDECREF(__pyx_v___pyx_result);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
@@ -3917,26 +2609,26 @@
  *         __pyx_unpickle_StringWithKey__set_state(<StringWithKey> __pyx_result, __pyx_state)
  *     return __pyx_result
  * cdef __pyx_unpickle_StringWithKey__set_state(StringWithKey __pyx_result, tuple __pyx_state):             # <<<<<<<<<<<<<<
  *     __pyx_result.key = __pyx_state[0]; __pyx_result.str = __pyx_state[1]
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):
  */
 
-static PyObject *__pyx_f_7camSort_7camSort___pyx_unpickle_StringWithKey__set_state(struct __pyx_obj_7camSort_7camSort_StringWithKey *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
+static PyObject *__pyx_f_7camSort_10stringSort___pyx_unpickle_StringWithKey__set_state(struct __pyx_obj_7camSort_10stringSort_StringWithKey *__pyx_v___pyx_result, PyObject *__pyx_v___pyx_state) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   PY_LONG_LONG __pyx_t_2;
   int __pyx_t_3;
   Py_ssize_t __pyx_t_4;
   int __pyx_t_5;
-  PyObject *__pyx_t_6 = NULL;
+  int __pyx_t_6;
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
-  int __pyx_t_9;
+  PyObject *__pyx_t_9 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__pyx_unpickle_StringWithKey__set_state", 0);
 
   /* "(tree fragment)":12
  *     return __pyx_result
@@ -3956,15 +2648,15 @@
   __pyx_v___pyx_result->key = __pyx_t_2;
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
     __PYX_ERR(1, 12, __pyx_L1_error)
   }
   __pyx_t_1 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 1, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None) || __Pyx_RaiseUnexpectedTypeError("unicode", __pyx_t_1))) __PYX_ERR(1, 12, __pyx_L1_error)
+  if (!(likely(PyUnicode_CheckExact(__pyx_t_1))||((__pyx_t_1) == Py_None)||(PyErr_Format(PyExc_TypeError, "Expected %.16s, got %.200s", "unicode", Py_TYPE(__pyx_t_1)->tp_name), 0))) __PYX_ERR(1, 12, __pyx_L1_error)
   __Pyx_GIVEREF(__pyx_t_1);
   __Pyx_GOTREF(__pyx_v___pyx_result->str);
   __Pyx_DECREF(__pyx_v___pyx_result->str);
   __pyx_v___pyx_result->str = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "(tree fragment)":13
@@ -3974,62 +2666,58 @@
  *         __pyx_result.__dict__.update(__pyx_state[2])
  */
   if (unlikely(__pyx_v___pyx_state == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "object of type 'NoneType' has no len()");
     __PYX_ERR(1, 13, __pyx_L1_error)
   }
   __pyx_t_4 = PyTuple_GET_SIZE(__pyx_v___pyx_state); if (unlikely(__pyx_t_4 == ((Py_ssize_t)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
-  __pyx_t_5 = (__pyx_t_4 > 2);
+  __pyx_t_5 = ((__pyx_t_4 > 2) != 0);
   if (__pyx_t_5) {
   } else {
     __pyx_t_3 = __pyx_t_5;
     goto __pyx_L4_bool_binop_done;
   }
   __pyx_t_5 = __Pyx_HasAttr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(__pyx_t_5 == ((int)-1))) __PYX_ERR(1, 13, __pyx_L1_error)
-  __pyx_t_3 = __pyx_t_5;
+  __pyx_t_6 = (__pyx_t_5 != 0);
+  __pyx_t_3 = __pyx_t_6;
   __pyx_L4_bool_binop_done:;
   if (__pyx_t_3) {
 
     /* "(tree fragment)":14
  *     __pyx_result.key = __pyx_state[0]; __pyx_result.str = __pyx_state[1]
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):
  *         __pyx_result.__dict__.update(__pyx_state[2])             # <<<<<<<<<<<<<<
  */
-    __pyx_t_6 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_6, __pyx_n_s_update); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __pyx_t_7 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v___pyx_result), __pyx_n_s_dict); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_7);
-    __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
+    __pyx_t_8 = __Pyx_PyObject_GetAttrStr(__pyx_t_7, __pyx_n_s_update); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_8);
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
     if (unlikely(__pyx_v___pyx_state == Py_None)) {
       PyErr_SetString(PyExc_TypeError, "'NoneType' object is not subscriptable");
       __PYX_ERR(1, 14, __pyx_L1_error)
     }
-    __pyx_t_6 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_6)) __PYX_ERR(1, 14, __pyx_L1_error)
-    __Pyx_GOTREF(__pyx_t_6);
-    __pyx_t_8 = NULL;
-    __pyx_t_9 = 0;
-    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_7))) {
-      __pyx_t_8 = PyMethod_GET_SELF(__pyx_t_7);
-      if (likely(__pyx_t_8)) {
-        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_7);
-        __Pyx_INCREF(__pyx_t_8);
+    __pyx_t_7 = __Pyx_GetItemInt_Tuple(__pyx_v___pyx_state, 2, long, 1, __Pyx_PyInt_From_long, 0, 0, 1); if (unlikely(!__pyx_t_7)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_7);
+    __pyx_t_9 = NULL;
+    if (CYTHON_UNPACK_METHODS && likely(PyMethod_Check(__pyx_t_8))) {
+      __pyx_t_9 = PyMethod_GET_SELF(__pyx_t_8);
+      if (likely(__pyx_t_9)) {
+        PyObject* function = PyMethod_GET_FUNCTION(__pyx_t_8);
+        __Pyx_INCREF(__pyx_t_9);
         __Pyx_INCREF(function);
-        __Pyx_DECREF_SET(__pyx_t_7, function);
-        __pyx_t_9 = 1;
+        __Pyx_DECREF_SET(__pyx_t_8, function);
       }
     }
-    {
-      PyObject *__pyx_callargs[2] = {__pyx_t_8, __pyx_t_6};
-      __pyx_t_1 = __Pyx_PyObject_FastCall(__pyx_t_7, __pyx_callargs+1-__pyx_t_9, 1+__pyx_t_9);
-      __Pyx_XDECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
-      if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
-      __Pyx_GOTREF(__pyx_t_1);
-      __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
-    }
+    __pyx_t_1 = (__pyx_t_9) ? __Pyx_PyObject_Call2Args(__pyx_t_8, __pyx_t_9, __pyx_t_7) : __Pyx_PyObject_CallOneArg(__pyx_t_8, __pyx_t_7);
+    __Pyx_XDECREF(__pyx_t_9); __pyx_t_9 = 0;
+    __Pyx_DECREF(__pyx_t_7); __pyx_t_7 = 0;
+    if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 14, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
     /* "(tree fragment)":13
  * cdef __pyx_unpickle_StringWithKey__set_state(StringWithKey __pyx_result, tuple __pyx_state):
  *     __pyx_result.key = __pyx_state[0]; __pyx_result.str = __pyx_state[1]
  *     if len(__pyx_state) > 2 and hasattr(__pyx_result, '__dict__'):             # <<<<<<<<<<<<<<
  *         __pyx_result.__dict__.update(__pyx_state[2])
@@ -4045,121 +2733,97 @@
  */
 
   /* function exit code */
   __pyx_r = Py_None; __Pyx_INCREF(Py_None);
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
-  __Pyx_XDECREF(__pyx_t_6);
   __Pyx_XDECREF(__pyx_t_7);
   __Pyx_XDECREF(__pyx_t_8);
-  __Pyx_AddTraceback("camSort.camSort.__pyx_unpickle_StringWithKey__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_XDECREF(__pyx_t_9);
+  __Pyx_AddTraceback("camSort.stringSort.__pyx_unpickle_StringWithKey__set_state", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
-static struct __pyx_vtabstruct_7camSort_7camSort_StringWithKey __pyx_vtable_7camSort_7camSort_StringWithKey;
+static struct __pyx_vtabstruct_7camSort_10stringSort_StringWithKey __pyx_vtable_7camSort_10stringSort_StringWithKey;
 
-static PyObject *__pyx_tp_new_7camSort_7camSort_StringWithKey(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
-  struct __pyx_obj_7camSort_7camSort_StringWithKey *p;
+static PyObject *__pyx_tp_new_7camSort_10stringSort_StringWithKey(PyTypeObject *t, CYTHON_UNUSED PyObject *a, CYTHON_UNUSED PyObject *k) {
+  struct __pyx_obj_7camSort_10stringSort_StringWithKey *p;
   PyObject *o;
-  #if CYTHON_COMPILING_IN_LIMITED_API
-  allocfunc alloc_func = (allocfunc)PyType_GetSlot(t, Py_tp_alloc);
-  o = alloc_func(t, 0);
-  #else
-  if (likely(!__Pyx_PyType_HasFeature(t, Py_TPFLAGS_IS_ABSTRACT))) {
+  if (likely((t->tp_flags & Py_TPFLAGS_IS_ABSTRACT) == 0)) {
     o = (*t->tp_alloc)(t, 0);
   } else {
     o = (PyObject *) PyBaseObject_Type.tp_new(t, __pyx_empty_tuple, 0);
   }
   if (unlikely(!o)) return 0;
-  #endif
-  p = ((struct __pyx_obj_7camSort_7camSort_StringWithKey *)o);
-  p->__pyx_vtab = __pyx_vtabptr_7camSort_7camSort_StringWithKey;
+  p = ((struct __pyx_obj_7camSort_10stringSort_StringWithKey *)o);
+  p->__pyx_vtab = __pyx_vtabptr_7camSort_10stringSort_StringWithKey;
   p->str = ((PyObject*)Py_None); Py_INCREF(Py_None);
   return o;
 }
 
-static void __pyx_tp_dealloc_7camSort_7camSort_StringWithKey(PyObject *o) {
-  struct __pyx_obj_7camSort_7camSort_StringWithKey *p = (struct __pyx_obj_7camSort_7camSort_StringWithKey *)o;
+static void __pyx_tp_dealloc_7camSort_10stringSort_StringWithKey(PyObject *o) {
+  struct __pyx_obj_7camSort_10stringSort_StringWithKey *p = (struct __pyx_obj_7camSort_10stringSort_StringWithKey *)o;
   #if CYTHON_USE_TP_FINALIZE
-  if (unlikely((PY_VERSION_HEX >= 0x03080000 || __Pyx_PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE)) && __Pyx_PyObject_GetSlot(o, tp_finalize, destructor)) && (!PyType_IS_GC(Py_TYPE(o)) || !__Pyx_PyObject_GC_IsFinalized(o))) {
-    if (__Pyx_PyObject_GetSlot(o, tp_dealloc, destructor) == __pyx_tp_dealloc_7camSort_7camSort_StringWithKey) {
-      if (PyObject_CallFinalizerFromDealloc(o)) return;
-    }
+  if (unlikely(PyType_HasFeature(Py_TYPE(o), Py_TPFLAGS_HAVE_FINALIZE) && Py_TYPE(o)->tp_finalize) && (!PyType_IS_GC(Py_TYPE(o)) || !_PyGC_FINALIZED(o))) {
+    if (PyObject_CallFinalizerFromDealloc(o)) return;
   }
   #endif
   Py_CLEAR(p->str);
   (*Py_TYPE(o)->tp_free)(o);
 }
 
-static PyObject *__pyx_getprop_7camSort_7camSort_13StringWithKey_str(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7camSort_7camSort_13StringWithKey_3str_1__get__(o);
+static PyObject *__pyx_getprop_7camSort_10stringSort_13StringWithKey_str(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_1__get__(o);
 }
 
-static int __pyx_setprop_7camSort_7camSort_13StringWithKey_str(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+static int __pyx_setprop_7camSort_10stringSort_13StringWithKey_str(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
   if (v) {
-    return __pyx_pw_7camSort_7camSort_13StringWithKey_3str_3__set__(o, v);
+    return __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_3__set__(o, v);
   }
   else {
-    return __pyx_pw_7camSort_7camSort_13StringWithKey_3str_5__del__(o);
+    return __pyx_pw_7camSort_10stringSort_13StringWithKey_3str_5__del__(o);
   }
 }
 
-static PyObject *__pyx_getprop_7camSort_7camSort_13StringWithKey_key(PyObject *o, CYTHON_UNUSED void *x) {
-  return __pyx_pw_7camSort_7camSort_13StringWithKey_3key_1__get__(o);
+static PyObject *__pyx_getprop_7camSort_10stringSort_13StringWithKey_key(PyObject *o, CYTHON_UNUSED void *x) {
+  return __pyx_pw_7camSort_10stringSort_13StringWithKey_3key_1__get__(o);
 }
 
-static int __pyx_setprop_7camSort_7camSort_13StringWithKey_key(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
+static int __pyx_setprop_7camSort_10stringSort_13StringWithKey_key(PyObject *o, PyObject *v, CYTHON_UNUSED void *x) {
   if (v) {
-    return __pyx_pw_7camSort_7camSort_13StringWithKey_3key_3__set__(o, v);
+    return __pyx_pw_7camSort_10stringSort_13StringWithKey_3key_3__set__(o, v);
   }
   else {
     PyErr_SetString(PyExc_NotImplementedError, "__del__");
     return -1;
   }
 }
 
-static PyMethodDef __pyx_methods_7camSort_7camSort_StringWithKey[] = {
-  {"__reduce_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7camSort_7camSort_13StringWithKey_3__reduce_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
-  {"__setstate_cython__", (PyCFunction)(void*)(__Pyx_PyCFunction_FastCallWithKeywords)__pyx_pw_7camSort_7camSort_13StringWithKey_5__setstate_cython__, __Pyx_METH_FASTCALL|METH_KEYWORDS, 0},
+static PyMethodDef __pyx_methods_7camSort_10stringSort_StringWithKey[] = {
+  {"__reduce_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_13StringWithKey_3__reduce_cython__, METH_NOARGS, 0},
+  {"__setstate_cython__", (PyCFunction)__pyx_pw_7camSort_10stringSort_13StringWithKey_5__setstate_cython__, METH_O, 0},
   {0, 0, 0, 0}
 };
 
-static struct PyGetSetDef __pyx_getsets_7camSort_7camSort_StringWithKey[] = {
-  {(char *)"str", __pyx_getprop_7camSort_7camSort_13StringWithKey_str, __pyx_setprop_7camSort_7camSort_13StringWithKey_str, (char *)0, 0},
-  {(char *)"key", __pyx_getprop_7camSort_7camSort_13StringWithKey_key, __pyx_setprop_7camSort_7camSort_13StringWithKey_key, (char *)0, 0},
+static struct PyGetSetDef __pyx_getsets_7camSort_10stringSort_StringWithKey[] = {
+  {(char *)"str", __pyx_getprop_7camSort_10stringSort_13StringWithKey_str, __pyx_setprop_7camSort_10stringSort_13StringWithKey_str, (char *)0, 0},
+  {(char *)"key", __pyx_getprop_7camSort_10stringSort_13StringWithKey_key, __pyx_setprop_7camSort_10stringSort_13StringWithKey_key, (char *)0, 0},
   {0, 0, 0, 0, 0}
 };
-#if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_type_7camSort_7camSort_StringWithKey_slots[] = {
-  {Py_tp_dealloc, (void *)__pyx_tp_dealloc_7camSort_7camSort_StringWithKey},
-  {Py_tp_methods, (void *)__pyx_methods_7camSort_7camSort_StringWithKey},
-  {Py_tp_getset, (void *)__pyx_getsets_7camSort_7camSort_StringWithKey},
-  {Py_tp_init, (void *)__pyx_pw_7camSort_7camSort_13StringWithKey_1__init__},
-  {Py_tp_new, (void *)__pyx_tp_new_7camSort_7camSort_StringWithKey},
-  {0, 0},
-};
-static PyType_Spec __pyx_type_7camSort_7camSort_StringWithKey_spec = {
-  "camSort.camSort.StringWithKey",
-  sizeof(struct __pyx_obj_7camSort_7camSort_StringWithKey),
-  0,
-  Py_TPFLAGS_DEFAULT|Py_TPFLAGS_HAVE_VERSION_TAG|Py_TPFLAGS_CHECKTYPES|Py_TPFLAGS_HAVE_NEWBUFFER|Py_TPFLAGS_BASETYPE,
-  __pyx_type_7camSort_7camSort_StringWithKey_slots,
-};
-#else
 
-static PyTypeObject __pyx_type_7camSort_7camSort_StringWithKey = {
+static PyTypeObject __pyx_type_7camSort_10stringSort_StringWithKey = {
   PyVarObject_HEAD_INIT(0, 0)
-  "camSort.camSort.""StringWithKey", /*tp_name*/
-  sizeof(struct __pyx_obj_7camSort_7camSort_StringWithKey), /*tp_basicsize*/
+  "camSort.stringSort.StringWithKey", /*tp_name*/
+  sizeof(struct __pyx_obj_7camSort_10stringSort_StringWithKey), /*tp_basicsize*/
   0, /*tp_itemsize*/
-  __pyx_tp_dealloc_7camSort_7camSort_StringWithKey, /*tp_dealloc*/
+  __pyx_tp_dealloc_7camSort_10stringSort_StringWithKey, /*tp_dealloc*/
   #if PY_VERSION_HEX < 0x030800b4
   0, /*tp_print*/
   #endif
   #if PY_VERSION_HEX >= 0x030800b4
   0, /*tp_vectorcall_offset*/
   #endif
   0, /*tp_getattr*/
@@ -4184,221 +2848,179 @@
   0, /*tp_doc*/
   0, /*tp_traverse*/
   0, /*tp_clear*/
   0, /*tp_richcompare*/
   0, /*tp_weaklistoffset*/
   0, /*tp_iter*/
   0, /*tp_iternext*/
-  __pyx_methods_7camSort_7camSort_StringWithKey, /*tp_methods*/
+  __pyx_methods_7camSort_10stringSort_StringWithKey, /*tp_methods*/
   0, /*tp_members*/
-  __pyx_getsets_7camSort_7camSort_StringWithKey, /*tp_getset*/
+  __pyx_getsets_7camSort_10stringSort_StringWithKey, /*tp_getset*/
   0, /*tp_base*/
   0, /*tp_dict*/
   0, /*tp_descr_get*/
   0, /*tp_descr_set*/
-  #if !CYTHON_USE_TYPE_SPECS
   0, /*tp_dictoffset*/
-  #endif
-  __pyx_pw_7camSort_7camSort_13StringWithKey_1__init__, /*tp_init*/
+  __pyx_pw_7camSort_10stringSort_13StringWithKey_1__init__, /*tp_init*/
   0, /*tp_alloc*/
-  __pyx_tp_new_7camSort_7camSort_StringWithKey, /*tp_new*/
+  __pyx_tp_new_7camSort_10stringSort_StringWithKey, /*tp_new*/
   0, /*tp_free*/
   0, /*tp_is_gc*/
   0, /*tp_bases*/
   0, /*tp_mro*/
   0, /*tp_cache*/
   0, /*tp_subclasses*/
   0, /*tp_weaklist*/
   0, /*tp_del*/
   0, /*tp_version_tag*/
   #if PY_VERSION_HEX >= 0x030400a1
-  #if CYTHON_USE_TP_FINALIZE
   0, /*tp_finalize*/
-  #else
-  NULL, /*tp_finalize*/
   #endif
-  #endif
-  #if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
+  #if PY_VERSION_HEX >= 0x030800b1
   0, /*tp_vectorcall*/
   #endif
-  #if __PYX_NEED_TP_PRINT_SLOT == 1
+  #if PY_VERSION_HEX >= 0x030800b4 && PY_VERSION_HEX < 0x03090000
   0, /*tp_print*/
   #endif
-  #if PY_VERSION_HEX >= 0x030C0000
-  0, /*tp_watched*/
-  #endif
-  #if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-  0, /*tp_pypy_flags*/
-  #endif
 };
-#endif
 
 static PyMethodDef __pyx_methods[] = {
   {0, 0, 0, 0}
 };
+
+#if PY_MAJOR_VERSION >= 3
+#if CYTHON_PEP489_MULTI_PHASE_INIT
+static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
+static int __pyx_pymod_exec_stringSort(PyObject* module); /*proto*/
+static PyModuleDef_Slot __pyx_moduledef_slots[] = {
+  {Py_mod_create, (void*)__pyx_pymod_create},
+  {Py_mod_exec, (void*)__pyx_pymod_exec_stringSort},
+  {0, NULL}
+};
+#endif
+
+static struct PyModuleDef __pyx_moduledef = {
+    PyModuleDef_HEAD_INIT,
+    "stringSort",
+    0, /* m_doc */
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+    0, /* m_size */
+  #else
+    -1, /* m_size */
+  #endif
+    __pyx_methods /* m_methods */,
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+    __pyx_moduledef_slots, /* m_slots */
+  #else
+    NULL, /* m_reload */
+  #endif
+    NULL, /* m_traverse */
+    NULL, /* m_clear */
+    NULL /* m_free */
+};
+#endif
 #ifndef CYTHON_SMALL_CODE
 #if defined(__clang__)
     #define CYTHON_SMALL_CODE
 #elif defined(__GNUC__) && (__GNUC__ > 4 || (__GNUC__ == 4 && __GNUC_MINOR__ >= 3))
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
-/* #### Code section: pystring_table ### */
 
-static int __Pyx_CreateStringTabAndInitStrings(void) {
-  __Pyx_StringTabEntry __pyx_string_tab[] = {
-    {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
-    {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
-    {&__pyx_n_s_StringWithKey, __pyx_k_StringWithKey, sizeof(__pyx_k_StringWithKey), 0, 0, 1, 1},
-    {&__pyx_n_s_StringWithKey___reduce_cython, __pyx_k_StringWithKey___reduce_cython, sizeof(__pyx_k_StringWithKey___reduce_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_StringWithKey___setstate_cython, __pyx_k_StringWithKey___setstate_cython, sizeof(__pyx_k_StringWithKey___setstate_cython), 0, 0, 1, 1},
-    {&__pyx_n_s__11, __pyx_k__11, sizeof(__pyx_k__11), 0, 0, 1, 1},
-    {&__pyx_kp_u__2, __pyx_k__2, sizeof(__pyx_k__2), 0, 1, 0, 0},
-    {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
-    {&__pyx_n_s_asyncio_coroutines, __pyx_k_asyncio_coroutines, sizeof(__pyx_k_asyncio_coroutines), 0, 0, 1, 1},
-    {&__pyx_n_s_attrgetter, __pyx_k_attrgetter, sizeof(__pyx_k_attrgetter), 0, 0, 1, 1},
-    {&__pyx_n_s_camSort_camSort, __pyx_k_camSort_camSort, sizeof(__pyx_k_camSort_camSort), 0, 0, 1, 1},
-    {&__pyx_kp_s_camSort_camSort_pyx, __pyx_k_camSort_camSort_pyx, sizeof(__pyx_k_camSort_camSort_pyx), 0, 0, 1, 0},
-    {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
-    {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
-    {&__pyx_n_s_dict_2, __pyx_k_dict_2, sizeof(__pyx_k_dict_2), 0, 0, 1, 1},
-    {&__pyx_kp_u_disable, __pyx_k_disable, sizeof(__pyx_k_disable), 0, 1, 0, 0},
-    {&__pyx_kp_u_enable, __pyx_k_enable, sizeof(__pyx_k_enable), 0, 1, 0, 0},
-    {&__pyx_kp_u_gc, __pyx_k_gc, sizeof(__pyx_k_gc), 0, 1, 0, 0},
-    {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
-    {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
-    {&__pyx_n_s_input_list, __pyx_k_input_list, sizeof(__pyx_k_input_list), 0, 0, 1, 1},
-    {&__pyx_n_s_is_coroutine, __pyx_k_is_coroutine, sizeof(__pyx_k_is_coroutine), 0, 0, 1, 1},
-    {&__pyx_kp_u_isenabled, __pyx_k_isenabled, sizeof(__pyx_k_isenabled), 0, 1, 0, 0},
-    {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
-    {&__pyx_n_u_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 1, 0, 1},
-    {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
-    {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
-    {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
-    {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
-    {&__pyx_n_s_operator, __pyx_k_operator, sizeof(__pyx_k_operator), 0, 0, 1, 1},
-    {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
-    {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
-    {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
-    {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
-    {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
-    {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
-    {&__pyx_n_s_pyx_unpickle_StringWithKey, __pyx_k_pyx_unpickle_StringWithKey, sizeof(__pyx_k_pyx_unpickle_StringWithKey), 0, 0, 1, 1},
-    {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
-    {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
-    {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
-    {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
-    {&__pyx_n_s_self, __pyx_k_self, sizeof(__pyx_k_self), 0, 0, 1, 1},
-    {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
-    {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
-    {&__pyx_n_s_sortStrings, __pyx_k_sortStrings, sizeof(__pyx_k_sortStrings), 0, 0, 1, 1},
-    {&__pyx_n_s_sorted, __pyx_k_sorted, sizeof(__pyx_k_sorted), 0, 0, 1, 1},
-    {&__pyx_n_s_sorted_array, __pyx_k_sorted_array, sizeof(__pyx_k_sorted_array), 0, 0, 1, 1},
-    {&__pyx_n_s_state, __pyx_k_state, sizeof(__pyx_k_state), 0, 0, 1, 1},
-    {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
-    {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
-    {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
-    {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
-    {&__pyx_n_s_use_setstate, __pyx_k_use_setstate, sizeof(__pyx_k_use_setstate), 0, 0, 1, 1},
-    {0, 0, 0, 0, 0, 0, 0}
-  };
-  return __Pyx_InitStrings(__pyx_string_tab);
-}
-/* #### Code section: cached_builtins ### */
+static __Pyx_StringTabEntry __pyx_string_tab[] = {
+  {&__pyx_kp_s_Incompatible_checksums_s_vs_0xef, __pyx_k_Incompatible_checksums_s_vs_0xef, sizeof(__pyx_k_Incompatible_checksums_s_vs_0xef), 0, 0, 1, 0},
+  {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
+  {&__pyx_n_s_StringWithKey, __pyx_k_StringWithKey, sizeof(__pyx_k_StringWithKey), 0, 0, 1, 1},
+  {&__pyx_n_s_array, __pyx_k_array, sizeof(__pyx_k_array), 0, 0, 1, 1},
+  {&__pyx_n_s_attrgetter, __pyx_k_attrgetter, sizeof(__pyx_k_attrgetter), 0, 0, 1, 1},
+  {&__pyx_n_s_byLength, __pyx_k_byLength, sizeof(__pyx_k_byLength), 0, 0, 1, 1},
+  {&__pyx_n_s_camSort_stringSort, __pyx_k_camSort_stringSort, sizeof(__pyx_k_camSort_stringSort), 0, 0, 1, 1},
+  {&__pyx_kp_s_camSort_stringSort_pyx, __pyx_k_camSort_stringSort_pyx, sizeof(__pyx_k_camSort_stringSort_pyx), 0, 0, 1, 0},
+  {&__pyx_n_s_cline_in_traceback, __pyx_k_cline_in_traceback, sizeof(__pyx_k_cline_in_traceback), 0, 0, 1, 1},
+  {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
+  {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
+  {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+  {&__pyx_n_s_input_list, __pyx_k_input_list, sizeof(__pyx_k_input_list), 0, 0, 1, 1},
+  {&__pyx_n_s_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 0, 1, 1},
+  {&__pyx_n_u_key, __pyx_k_key, sizeof(__pyx_k_key), 0, 1, 0, 1},
+  {&__pyx_n_s_main, __pyx_k_main, sizeof(__pyx_k_main), 0, 0, 1, 1},
+  {&__pyx_n_s_n, __pyx_k_n, sizeof(__pyx_k_n), 0, 0, 1, 1},
+  {&__pyx_n_s_name, __pyx_k_name, sizeof(__pyx_k_name), 0, 0, 1, 1},
+  {&__pyx_n_s_new, __pyx_k_new, sizeof(__pyx_k_new), 0, 0, 1, 1},
+  {&__pyx_n_s_operator, __pyx_k_operator, sizeof(__pyx_k_operator), 0, 0, 1, 1},
+  {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_unpickle_StringWithKey, __pyx_k_pyx_unpickle_StringWithKey, sizeof(__pyx_k_pyx_unpickle_StringWithKey), 0, 0, 1, 1},
+  {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
+  {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
+  {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
+  {&__pyx_n_s_s, __pyx_k_s, sizeof(__pyx_k_s), 0, 0, 1, 1},
+  {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
+  {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
+  {&__pyx_n_s_sorted, __pyx_k_sorted, sizeof(__pyx_k_sorted), 0, 0, 1, 1},
+  {&__pyx_n_s_sorted_array, __pyx_k_sorted_array, sizeof(__pyx_k_sorted_array), 0, 0, 1, 1},
+  {&__pyx_n_s_str, __pyx_k_str, sizeof(__pyx_k_str), 0, 0, 1, 1},
+  {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
+  {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+  {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
+  {0, 0, 0, 0, 0, 0, 0}
+};
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
   __pyx_builtin_sorted = __Pyx_GetBuiltinName(__pyx_n_s_sorted); if (!__pyx_builtin_sorted) __PYX_ERR(0, 24, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
-/* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "(tree fragment)":4
- *     cdef object __pyx_PickleError
- *     cdef object __pyx_result
- *     if __pyx_checksum not in (0x9b81d8b, 0xaba2f13, 0xef4e75e):             # <<<<<<<<<<<<<<
- *         from pickle import PickleError as __pyx_PickleError
- *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x9b81d8b, 0xaba2f13, 0xef4e75e) = (key, str))" % __pyx_checksum
- */
-  __pyx_tuple_ = PyTuple_Pack(3, __pyx_int_163061131, __pyx_int_179973907, __pyx_int_250931038); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 4, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple_);
-  __Pyx_GIVEREF(__pyx_tuple_);
-
-  /* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     cdef tuple state
- *     cdef object _dict
- */
-  __pyx_tuple__3 = PyTuple_Pack(4, __pyx_n_s_self, __pyx_n_s_state, __pyx_n_s_dict_2, __pyx_n_s_use_setstate); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__3);
-  __Pyx_GIVEREF(__pyx_tuple__3);
-  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 4, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_reduce_cython, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(1, 1, __pyx_L1_error)
-
-  /* "(tree fragment)":16
- *     else:
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, state)
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_unpickle_StringWithKey__set_state(self, __pyx_state)
- */
-  __pyx_tuple__5 = PyTuple_Pack(2, __pyx_n_s_self, __pyx_n_s_pyx_state); if (unlikely(!__pyx_tuple__5)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__5);
-  __Pyx_GIVEREF(__pyx_tuple__5);
-  __pyx_codeobj__6 = (PyObject*)__Pyx_PyCode_New(2, 0, 0, 2, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__5, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_setstate_cython, 16, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__6)) __PYX_ERR(1, 16, __pyx_L1_error)
-
-  /* "camSort/camSort.pyx":20
+  /* "camSort/stringSort.pyx":20
  *         return length * 10000 + sum
  * 
- * def sortStrings(input_list):             # <<<<<<<<<<<<<<
+ * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
-  __pyx_tuple__7 = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__7);
-  __Pyx_GIVEREF(__pyx_tuple__7);
-  __pyx_codeobj__8 = (PyObject*)__Pyx_PyCode_New(1, 0, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__7, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_camSort_pyx, __pyx_n_s_sortStrings, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__8)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(6, __pyx_n_s_input_list, __pyx_n_s_n, __pyx_n_s_array, __pyx_n_s_sorted_array, __pyx_n_s_s, __pyx_n_s_s); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple_);
+  __Pyx_GIVEREF(__pyx_tuple_);
+  __pyx_codeobj__2 = (PyObject*)__Pyx_PyCode_New(1, 0, 6, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple_, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_camSort_stringSort_pyx, __pyx_n_s_byLength, 20, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__2)) __PYX_ERR(0, 20, __pyx_L1_error)
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__9 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__9);
-  __Pyx_GIVEREF(__pyx_tuple__9);
-  __pyx_codeobj__10 = (PyObject*)__Pyx_PyCode_New(3, 0, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__9, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StringWithKey, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__10)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __pyx_tuple__3 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__3);
+  __Pyx_GIVEREF(__pyx_tuple__3);
+  __pyx_codeobj__4 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__3, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_StringWithKey, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__4)) __PYX_ERR(1, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
-/* #### Code section: init_constants ### */
 
-static CYTHON_SMALL_CODE int __Pyx_InitConstants(void) {
-  if (__Pyx_CreateStringTabAndInitStrings() < 0) __PYX_ERR(0, 1, __pyx_L1_error);
-  __pyx_int_163061131 = PyInt_FromLong(163061131L); if (unlikely(!__pyx_int_163061131)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __pyx_int_179973907 = PyInt_FromLong(179973907L); if (unlikely(!__pyx_int_179973907)) __PYX_ERR(0, 1, __pyx_L1_error)
+static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
+  if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   __pyx_int_250931038 = PyInt_FromLong(250931038L); if (unlikely(!__pyx_int_250931038)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
 }
-/* #### Code section: init_globals ### */
-
-static CYTHON_SMALL_CODE int __Pyx_InitGlobals(void) {
-  return 0;
-}
-/* #### Code section: init_module ### */
 
 static CYTHON_SMALL_CODE int __Pyx_modinit_global_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_function_export_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_init_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_type_import_code(void); /*proto*/
 static CYTHON_SMALL_CODE int __Pyx_modinit_variable_import_code(void); /*proto*/
@@ -4431,43 +3053,27 @@
 static int __Pyx_modinit_type_init_code(void) {
   __Pyx_RefNannyDeclarations
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_init_code", 0);
   /*--- Type init code ---*/
-  __pyx_vtabptr_7camSort_7camSort_StringWithKey = &__pyx_vtable_7camSort_7camSort_StringWithKey;
-  __pyx_vtable_7camSort_7camSort_StringWithKey.calculate_key = (PY_LONG_LONG (*)(struct __pyx_obj_7camSort_7camSort_StringWithKey *, PyObject *))__pyx_f_7camSort_7camSort_13StringWithKey_calculate_key;
-  #if CYTHON_USE_TYPE_SPECS
-  __pyx_ptype_7camSort_7camSort_StringWithKey = (PyTypeObject *) __Pyx_PyType_FromModuleAndSpec(__pyx_m, &__pyx_type_7camSort_7camSort_StringWithKey_spec, NULL); if (unlikely(!__pyx_ptype_7camSort_7camSort_StringWithKey)) __PYX_ERR(0, 4, __pyx_L1_error)
-  if (__Pyx_fix_up_extension_type_from_spec(&__pyx_type_7camSort_7camSort_StringWithKey_spec, __pyx_ptype_7camSort_7camSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  #else
-  __pyx_ptype_7camSort_7camSort_StringWithKey = &__pyx_type_7camSort_7camSort_StringWithKey;
-  #endif
-  #if !CYTHON_COMPILING_IN_LIMITED_API
-  #endif
-  #if !CYTHON_USE_TYPE_SPECS
-  if (__Pyx_PyType_Ready(__pyx_ptype_7camSort_7camSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  #endif
-  #if PY_MAJOR_VERSION < 3
-  __pyx_ptype_7camSort_7camSort_StringWithKey->tp_print = 0;
-  #endif
-  #if !CYTHON_COMPILING_IN_LIMITED_API
-  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_ptype_7camSort_7camSort_StringWithKey->tp_dictoffset && __pyx_ptype_7camSort_7camSort_StringWithKey->tp_getattro == PyObject_GenericGetAttr)) {
-    __pyx_ptype_7camSort_7camSort_StringWithKey->tp_getattro = __Pyx_PyObject_GenericGetAttr;
-  }
-  #endif
-  if (__Pyx_SetVtable(__pyx_ptype_7camSort_7camSort_StringWithKey, __pyx_vtabptr_7camSort_7camSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_MergeVtables(__pyx_ptype_7camSort_7camSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  #endif
-  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringWithKey, (PyObject *) __pyx_ptype_7camSort_7camSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  #if !CYTHON_COMPILING_IN_LIMITED_API
-  if (__Pyx_setup_reduce((PyObject *) __pyx_ptype_7camSort_7camSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
-  #endif
+  __pyx_vtabptr_7camSort_10stringSort_StringWithKey = &__pyx_vtable_7camSort_10stringSort_StringWithKey;
+  __pyx_vtable_7camSort_10stringSort_StringWithKey.calculate_key = (PY_LONG_LONG (*)(struct __pyx_obj_7camSort_10stringSort_StringWithKey *, PyObject *))__pyx_f_7camSort_10stringSort_13StringWithKey_calculate_key;
+  if (PyType_Ready(&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  #if PY_VERSION_HEX < 0x030800B1
+  __pyx_type_7camSort_10stringSort_StringWithKey.tp_print = 0;
+  #endif
+  if ((CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP) && likely(!__pyx_type_7camSort_10stringSort_StringWithKey.tp_dictoffset && __pyx_type_7camSort_10stringSort_StringWithKey.tp_getattro == PyObject_GenericGetAttr)) {
+    __pyx_type_7camSort_10stringSort_StringWithKey.tp_getattro = __Pyx_PyObject_GenericGetAttr;
+  }
+  if (__Pyx_SetVtable(__pyx_type_7camSort_10stringSort_StringWithKey.tp_dict, __pyx_vtabptr_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  if (PyObject_SetAttr(__pyx_m, __pyx_n_s_StringWithKey, (PyObject *)&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  if (__Pyx_setup_reduce((PyObject*)&__pyx_type_7camSort_10stringSort_StringWithKey) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_ptype_7camSort_10stringSort_StringWithKey = &__pyx_type_7camSort_10stringSort_StringWithKey;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -4492,63 +3098,14 @@
   __Pyx_RefNannySetupContext("__Pyx_modinit_function_import_code", 0);
   /*--- Function import code ---*/
   __Pyx_RefNannyFinishContext();
   return 0;
 }
 
 
-#if PY_MAJOR_VERSION >= 3
-#if CYTHON_PEP489_MULTI_PHASE_INIT
-static PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def); /*proto*/
-static int __pyx_pymod_exec_camSort(PyObject* module); /*proto*/
-static PyModuleDef_Slot __pyx_moduledef_slots[] = {
-  {Py_mod_create, (void*)__pyx_pymod_create},
-  {Py_mod_exec, (void*)__pyx_pymod_exec_camSort},
-  {0, NULL}
-};
-#endif
-
-#ifdef __cplusplus
-namespace {
-  struct PyModuleDef __pyx_moduledef =
-  #else
-  static struct PyModuleDef __pyx_moduledef =
-  #endif
-  {
-      PyModuleDef_HEAD_INIT,
-      "camSort",
-      0, /* m_doc */
-    #if CYTHON_PEP489_MULTI_PHASE_INIT
-      0, /* m_size */
-    #elif CYTHON_USE_MODULE_STATE
-      sizeof(__pyx_mstate), /* m_size */
-    #else
-      -1, /* m_size */
-    #endif
-      __pyx_methods /* m_methods */,
-    #if CYTHON_PEP489_MULTI_PHASE_INIT
-      __pyx_moduledef_slots, /* m_slots */
-    #else
-      NULL, /* m_reload */
-    #endif
-    #if CYTHON_USE_MODULE_STATE
-      __pyx_m_traverse, /* m_traverse */
-      __pyx_m_clear, /* m_clear */
-      NULL /* m_free */
-    #else
-      NULL, /* m_traverse */
-      NULL, /* m_clear */
-      NULL /* m_free */
-    #endif
-  };
-  #ifdef __cplusplus
-} /* anonymous namespace */
-#endif
-#endif
-
 #ifndef CYTHON_NO_PYINIT_EXPORT
 #define __Pyx_PyMODINIT_FUNC PyMODINIT_FUNC
 #elif PY_MAJOR_VERSION < 3
 #ifdef __cplusplus
 #define __Pyx_PyMODINIT_FUNC extern "C" void
 #else
 #define __Pyx_PyMODINIT_FUNC void
@@ -4559,19 +3116,19 @@
 #else
 #define __Pyx_PyMODINIT_FUNC PyObject *
 #endif
 #endif
 
 
 #if PY_MAJOR_VERSION < 3
-__Pyx_PyMODINIT_FUNC initcamSort(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC initcamSort(void)
+__Pyx_PyMODINIT_FUNC initstringSort(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC initstringSort(void)
 #else
-__Pyx_PyMODINIT_FUNC PyInit_camSort(void) CYTHON_SMALL_CODE; /*proto*/
-__Pyx_PyMODINIT_FUNC PyInit_camSort(void)
+__Pyx_PyMODINIT_FUNC PyInit_stringSort(void) CYTHON_SMALL_CODE; /*proto*/
+__Pyx_PyMODINIT_FUNC PyInit_stringSort(void)
 #if CYTHON_PEP489_MULTI_PHASE_INIT
 {
   return PyModuleDef_Init(&__pyx_moduledef);
 }
 static CYTHON_SMALL_CODE int __Pyx_check_single_interpreter(void) {
     #if PY_VERSION_HEX >= 0x030700A1
     static PY_INT64_T main_interpreter_id = -1;
@@ -4591,320 +3148,242 @@
         PyErr_SetString(
             PyExc_ImportError,
             "Interpreter change detected - this module can only be loaded into one interpreter per process.");
         return -1;
     }
     return 0;
 }
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *module, const char* from_name, const char* to_name, int allow_none)
-#else
-static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none)
-#endif
-{
+static CYTHON_SMALL_CODE int __Pyx_copy_spec_to_module(PyObject *spec, PyObject *moddict, const char* from_name, const char* to_name, int allow_none) {
     PyObject *value = PyObject_GetAttrString(spec, from_name);
     int result = 0;
     if (likely(value)) {
         if (allow_none || value != Py_None) {
-#if CYTHON_COMPILING_IN_LIMITED_API
-            result = PyModule_AddObject(module, to_name, value);
-#else
             result = PyDict_SetItemString(moddict, to_name, value);
-#endif
         }
         Py_DECREF(value);
     } else if (PyErr_ExceptionMatches(PyExc_AttributeError)) {
         PyErr_Clear();
     } else {
         result = -1;
     }
     return result;
 }
-static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, PyModuleDef *def) {
+static CYTHON_SMALL_CODE PyObject* __pyx_pymod_create(PyObject *spec, CYTHON_UNUSED PyModuleDef *def) {
     PyObject *module = NULL, *moddict, *modname;
-    CYTHON_UNUSED_VAR(def);
     if (__Pyx_check_single_interpreter())
         return NULL;
     if (__pyx_m)
         return __Pyx_NewRef(__pyx_m);
     modname = PyObject_GetAttrString(spec, "name");
     if (unlikely(!modname)) goto bad;
     module = PyModule_NewObject(modname);
     Py_DECREF(modname);
     if (unlikely(!module)) goto bad;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    moddict = module;
-#else
     moddict = PyModule_GetDict(module);
     if (unlikely(!moddict)) goto bad;
-#endif
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "loader", "__loader__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "origin", "__file__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "parent", "__package__", 1) < 0)) goto bad;
     if (unlikely(__Pyx_copy_spec_to_module(spec, moddict, "submodule_search_locations", "__path__", 0) < 0)) goto bad;
     return module;
 bad:
     Py_XDECREF(module);
     return NULL;
 }
 
 
-static CYTHON_SMALL_CODE int __pyx_pymod_exec_camSort(PyObject *__pyx_pyinit_module)
+static CYTHON_SMALL_CODE int __pyx_pymod_exec_stringSort(PyObject *__pyx_pyinit_module)
 #endif
 #endif
 {
-  int stringtab_initialized = 0;
-  #if CYTHON_USE_MODULE_STATE
-  int pystate_addmodule_run = 0;
-  #endif
   PyObject *__pyx_t_1 = NULL;
   PyObject *__pyx_t_2 = NULL;
-  PyObject *__pyx_t_3 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannyDeclarations
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   if (__pyx_m) {
     if (__pyx_m == __pyx_pyinit_module) return 0;
-    PyErr_SetString(PyExc_RuntimeError, "Module 'camSort' has already been imported. Re-initialisation is not supported.");
+    PyErr_SetString(PyExc_RuntimeError, "Module 'stringSort' has already been imported. Re-initialisation is not supported.");
     return -1;
   }
   #elif PY_MAJOR_VERSION >= 3
   if (__pyx_m) return __Pyx_NewRef(__pyx_m);
   #endif
-  /*--- Module creation code ---*/
-  #if CYTHON_PEP489_MULTI_PHASE_INIT
-  __pyx_m = __pyx_pyinit_module;
-  Py_INCREF(__pyx_m);
-  #else
-  #if PY_MAJOR_VERSION < 3
-  __pyx_m = Py_InitModule4("camSort", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #elif CYTHON_USE_MODULE_STATE
-  __pyx_t_1 = PyModule_Create(&__pyx_moduledef); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
-  {
-    int add_module_result = PyState_AddModule(__pyx_t_1, &__pyx_moduledef);
-    __pyx_t_1 = 0; /* transfer ownership from __pyx_t_1 to camSort pseudovariable */
-    if (unlikely((add_module_result < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
-    pystate_addmodule_run = 1;
-  }
-  #else
-  __pyx_m = PyModule_Create(&__pyx_moduledef);
-  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
-  #endif
-  #endif
-  CYTHON_UNUSED_VAR(__pyx_t_1);
-  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_d);
-  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_b);
-  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
-  Py_INCREF(__pyx_cython_runtime);
-  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if CYTHON_REFNANNY
 __Pyx_RefNanny = __Pyx_RefNannyImportAPI("refnanny");
 if (!__Pyx_RefNanny) {
   PyErr_Clear();
   __Pyx_RefNanny = __Pyx_RefNannyImportAPI("Cython.Runtime.refnanny");
   if (!__Pyx_RefNanny)
       Py_FatalError("failed to import 'refnanny' module");
 }
 #endif
-  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_camSort(void)", 0);
+  __Pyx_RefNannySetupContext("__Pyx_PyMODINIT_FUNC PyInit_stringSort(void)", 0);
   if (__Pyx_check_binary_version() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pxy_PyFrame_Initialize_Offsets
   __Pxy_PyFrame_Initialize_Offsets();
   #endif
   __pyx_empty_tuple = PyTuple_New(0); if (unlikely(!__pyx_empty_tuple)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_bytes = PyBytes_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_bytes)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_empty_unicode = PyUnicode_FromStringAndSize("", 0); if (unlikely(!__pyx_empty_unicode)) __PYX_ERR(0, 1, __pyx_L1_error)
   #ifdef __Pyx_CyFunction_USED
-  if (__pyx_CyFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_CyFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_FusedFunction_USED
-  if (__pyx_FusedFunction_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_FusedFunction_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Coroutine_USED
-  if (__pyx_Coroutine_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Coroutine_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_Generator_USED
-  if (__pyx_Generator_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_Generator_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_AsyncGen_USED
-  if (__pyx_AsyncGen_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_AsyncGen_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   #ifdef __Pyx_StopAsyncIteration_USED
-  if (__pyx_StopAsyncIteration_init(__pyx_m) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (__pyx_StopAsyncIteration_init() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
   /*--- Library function declarations ---*/
   /*--- Threads initialization code ---*/
-  #if defined(WITH_THREAD) && PY_VERSION_HEX < 0x030700F0 && defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #if defined(__PYX_FORCE_INIT_THREADS) && __PYX_FORCE_INIT_THREADS
+  #ifdef WITH_THREAD /* Python build with threading support? */
   PyEval_InitThreads();
   #endif
+  #endif
+  /*--- Module creation code ---*/
+  #if CYTHON_PEP489_MULTI_PHASE_INIT
+  __pyx_m = __pyx_pyinit_module;
+  Py_INCREF(__pyx_m);
+  #else
+  #if PY_MAJOR_VERSION < 3
+  __pyx_m = Py_InitModule4("stringSort", __pyx_methods, 0, 0, PYTHON_API_VERSION); Py_XINCREF(__pyx_m);
+  #else
+  __pyx_m = PyModule_Create(&__pyx_moduledef);
+  #endif
+  if (unlikely(!__pyx_m)) __PYX_ERR(0, 1, __pyx_L1_error)
+  #endif
+  __pyx_d = PyModule_GetDict(__pyx_m); if (unlikely(!__pyx_d)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_d);
+  __pyx_b = PyImport_AddModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_b)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_b);
+  __pyx_cython_runtime = PyImport_AddModule((char *) "cython_runtime"); if (unlikely(!__pyx_cython_runtime)) __PYX_ERR(0, 1, __pyx_L1_error)
+  Py_INCREF(__pyx_cython_runtime);
+  if (PyObject_SetAttrString(__pyx_m, "__builtins__", __pyx_b) < 0) __PYX_ERR(0, 1, __pyx_L1_error);
   /*--- Initialize various global constants etc. ---*/
-  if (__Pyx_InitConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  stringtab_initialized = 1;
   if (__Pyx_InitGlobals() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #if PY_MAJOR_VERSION < 3 && (__PYX_DEFAULT_STRING_ENCODING_IS_ASCII || __PYX_DEFAULT_STRING_ENCODING_IS_DEFAULT)
   if (__Pyx_init_sys_getdefaultencoding_params() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
-  if (__pyx_module_is_main_camSort__camSort) {
+  if (__pyx_module_is_main_camSort__stringSort) {
     if (PyObject_SetAttr(__pyx_m, __pyx_n_s_name, __pyx_n_s_main) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   }
   #if PY_MAJOR_VERSION >= 3
   {
     PyObject *modules = PyImport_GetModuleDict(); if (unlikely(!modules)) __PYX_ERR(0, 1, __pyx_L1_error)
-    if (!PyDict_GetItemString(modules, "camSort.camSort")) {
-      if (unlikely((PyDict_SetItemString(modules, "camSort.camSort", __pyx_m) < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+    if (!PyDict_GetItemString(modules, "camSort.stringSort")) {
+      if (unlikely(PyDict_SetItemString(modules, "camSort.stringSort", __pyx_m) < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
     }
   }
   #endif
   /*--- Builtin init code ---*/
   if (__Pyx_InitCachedBuiltins() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Constants init code ---*/
   if (__Pyx_InitCachedConstants() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   /*--- Global type/function init code ---*/
   (void)__Pyx_modinit_global_init_code();
   (void)__Pyx_modinit_variable_export_code();
   (void)__Pyx_modinit_function_export_code();
-  if (unlikely((__Pyx_modinit_type_init_code() < 0))) __PYX_ERR(0, 1, __pyx_L1_error)
+  if (unlikely(__Pyx_modinit_type_init_code() < 0)) __PYX_ERR(0, 1, __pyx_L1_error)
   (void)__Pyx_modinit_type_import_code();
   (void)__Pyx_modinit_variable_import_code();
   (void)__Pyx_modinit_function_import_code();
   /*--- Execution code ---*/
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
-  /* "camSort/camSort.pyx":2
+  /* "camSort/stringSort.pyx":2
  * # cython: language_level=3
  * from operator import attrgetter             # <<<<<<<<<<<<<<
  * 
  * cdef class StringWithKey:
  */
-  __pyx_t_2 = PyList_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_attrgetter);
   __Pyx_GIVEREF(__pyx_n_s_attrgetter);
-  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_s_attrgetter);
-  __pyx_t_3 = __Pyx_Import(__pyx_n_s_operator, __pyx_t_2, 0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 2, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __pyx_t_2 = __Pyx_ImportFrom(__pyx_t_3, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
+  PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_attrgetter);
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_operator, __pyx_t_1, 0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 2, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_attrgetter, __pyx_t_2) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_attrgetter); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_attrgetter, __pyx_t_1) < 0) __PYX_ERR(0, 2, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
 
-  /* "(tree fragment)":1
- * def __reduce_cython__(self):             # <<<<<<<<<<<<<<
- *     cdef tuple state
- *     cdef object _dict
- */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7camSort_7camSort_13StringWithKey_3__reduce_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_StringWithKey___reduce_cython, NULL, __pyx_n_s_camSort_camSort, __pyx_d, ((PyObject *)__pyx_codeobj__4)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_7camSort_7camSort_StringWithKey->tp_dict, __pyx_n_s_reduce_cython, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  PyType_Modified(__pyx_ptype_7camSort_7camSort_StringWithKey);
-
-  /* "(tree fragment)":16
- *     else:
- *         return __pyx_unpickle_StringWithKey, (type(self), 0x9b81d8b, state)
- * def __setstate_cython__(self, __pyx_state):             # <<<<<<<<<<<<<<
- *     __pyx_unpickle_StringWithKey__set_state(self, __pyx_state)
- */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7camSort_7camSort_13StringWithKey_5__setstate_cython__, __Pyx_CYFUNCTION_CCLASS, __pyx_n_s_StringWithKey___setstate_cython, NULL, __pyx_n_s_camSort_camSort, __pyx_d, ((PyObject *)__pyx_codeobj__6)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem((PyObject *)__pyx_ptype_7camSort_7camSort_StringWithKey->tp_dict, __pyx_n_s_setstate_cython, __pyx_t_3) < 0) __PYX_ERR(1, 16, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  PyType_Modified(__pyx_ptype_7camSort_7camSort_StringWithKey);
-
-  /* "camSort/camSort.pyx":20
+  /* "camSort/stringSort.pyx":20
  *         return length * 10000 + sum
  * 
- * def sortStrings(input_list):             # <<<<<<<<<<<<<<
+ * def byLength(input_list):             # <<<<<<<<<<<<<<
  *     cdef int n = len(input_list)
  *     cdef list array = [StringWithKey(s) for s in input_list]
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7camSort_7camSort_1sortStrings, 0, __pyx_n_s_sortStrings, NULL, __pyx_n_s_camSort_camSort, __pyx_d, ((PyObject *)__pyx_codeobj__8)); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_sortStrings, __pyx_t_3) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_1byLength, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_byLength, __pyx_t_2) < 0) __PYX_ERR(0, 20, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_StringWithKey(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_t_3 = __Pyx_CyFunction_New(&__pyx_mdef_7camSort_7camSort_3__pyx_unpickle_StringWithKey, 0, __pyx_n_s_pyx_unpickle_StringWithKey, NULL, __pyx_n_s_camSort_camSort, __pyx_d, ((PyObject *)__pyx_codeobj__10)); if (unlikely(!__pyx_t_3)) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_StringWithKey, __pyx_t_3) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_7camSort_10stringSort_3__pyx_unpickle_StringWithKey, NULL, __pyx_n_s_camSort_stringSort); if (unlikely(!__pyx_t_2)) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pyx_unpickle_StringWithKey, __pyx_t_2) < 0) __PYX_ERR(1, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "camSort/camSort.pyx":1
+  /* "camSort/stringSort.pyx":1
  * # cython: language_level=3             # <<<<<<<<<<<<<<
  * from operator import attrgetter
  * 
  */
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_3) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
-  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_2) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /*--- Wrapped vars code ---*/
 
   goto __pyx_L0;
   __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
   __Pyx_XDECREF(__pyx_t_2);
-  __Pyx_XDECREF(__pyx_t_3);
   if (__pyx_m) {
-    if (__pyx_d && stringtab_initialized) {
-      __Pyx_AddTraceback("init camSort.camSort", __pyx_clineno, __pyx_lineno, __pyx_filename);
+    if (__pyx_d) {
+      __Pyx_AddTraceback("init camSort.stringSort", __pyx_clineno, __pyx_lineno, __pyx_filename);
     }
-    #if !CYTHON_USE_MODULE_STATE
     Py_CLEAR(__pyx_m);
-    #else
-    Py_DECREF(__pyx_m);
-    if (pystate_addmodule_run) {
-      PyObject *tp, *value, *tb;
-      PyErr_Fetch(&tp, &value, &tb);
-      PyState_RemoveModule(&__pyx_moduledef);
-      PyErr_Restore(tp, value, tb);
-    }
-    #endif
   } else if (!PyErr_Occurred()) {
-    PyErr_SetString(PyExc_ImportError, "init camSort.camSort");
+    PyErr_SetString(PyExc_ImportError, "init camSort.stringSort");
   }
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   #if CYTHON_PEP489_MULTI_PHASE_INIT
   return (__pyx_m != NULL) ? 0 : -1;
   #elif PY_MAJOR_VERSION >= 3
   return __pyx_m;
   #else
   return;
   #endif
 }
-/* #### Code section: cleanup_globals ### */
-/* #### Code section: cleanup_module ### */
-/* #### Code section: main_method ### */
-/* #### Code section: utility_code_pragmas ### */
-#ifdef _MSC_VER
-#pragma warning( push )
-/* Warning 4127: conditional expression is constant
- * Cython uses constant conditional expressions to allow in inline functions to be optimized at
- * compile-time, so this warning is not useful
- */
-#pragma warning( disable : 4127 )
-#endif
-
-
-
-/* #### Code section: utility_code_def ### */
 
 /* --- Runtime support code --- */
 /* Refnanny */
 #if CYTHON_REFNANNY
 static __Pyx_RefNannyAPIStruct *__Pyx_RefNannyImportAPI(const char *modname) {
     PyObject *m = NULL, *p = NULL;
     void *r = NULL;
@@ -4916,371 +3395,42 @@
 end:
     Py_XDECREF(p);
     Py_XDECREF(m);
     return (__Pyx_RefNannyAPIStruct *)r;
 }
 #endif
 
-/* PyErrExceptionMatches */
-#if CYTHON_FAST_THREAD_STATE
-static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
-    Py_ssize_t i, n;
-    n = PyTuple_GET_SIZE(tuple);
-#if PY_MAJOR_VERSION >= 3
-    for (i=0; i<n; i++) {
-        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
-    }
-#endif
-    for (i=0; i<n; i++) {
-        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
-    }
-    return 0;
-}
-static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
-    int result;
-    PyObject *exc_type;
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject *current_exception = tstate->current_exception;
-    if (unlikely(!current_exception)) return 0;
-    exc_type = (PyObject*) Py_TYPE(current_exception);
-    if (exc_type == err) return 1;
-#else
-    exc_type = tstate->curexc_type;
-    if (exc_type == err) return 1;
-    if (unlikely(!exc_type)) return 0;
-#endif
-    #if CYTHON_AVOID_BORROWED_REFS
-    Py_INCREF(exc_type);
-    #endif
-    if (unlikely(PyTuple_Check(err))) {
-        result = __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
-    } else {
-        result = __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
-    }
-    #if CYTHON_AVOID_BORROWED_REFS
-    Py_DECREF(exc_type);
-    #endif
-    return result;
-}
-#endif
-
-/* PyErrFetchRestore */
-#if CYTHON_FAST_THREAD_STATE
-static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject *tmp_value;
-    assert(type == NULL || (value != NULL && type == (PyObject*) Py_TYPE(value)));
-    if (value) {
-        #if CYTHON_COMPILING_IN_CPYTHON
-        if (unlikely(((PyBaseExceptionObject*) value)->traceback != tb))
-        #endif
-            PyException_SetTraceback(value, tb);
-    }
-    tmp_value = tstate->current_exception;
-    tstate->current_exception = value;
-    Py_XDECREF(tmp_value);
-#else
-    PyObject *tmp_type, *tmp_value, *tmp_tb;
-    tmp_type = tstate->curexc_type;
-    tmp_value = tstate->curexc_value;
-    tmp_tb = tstate->curexc_traceback;
-    tstate->curexc_type = type;
-    tstate->curexc_value = value;
-    tstate->curexc_traceback = tb;
-    Py_XDECREF(tmp_type);
-    Py_XDECREF(tmp_value);
-    Py_XDECREF(tmp_tb);
-#endif
-}
-static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
-#if PY_VERSION_HEX >= 0x030C00A6
-    PyObject* exc_value;
-    exc_value = tstate->current_exception;
-    tstate->current_exception = 0;
-    *value = exc_value;
-    *type = NULL;
-    *tb = NULL;
-    if (exc_value) {
-        *type = (PyObject*) Py_TYPE(exc_value);
-        Py_INCREF(*type);
-        #if CYTHON_COMPILING_IN_CPYTHON
-        *tb = ((PyBaseExceptionObject*) exc_value)->traceback;
-        Py_XINCREF(*tb);
-        #else
-        *tb = PyException_GetTraceback(exc_value);
-        #endif
-    }
-#else
-    *type = tstate->curexc_type;
-    *value = tstate->curexc_value;
-    *tb = tstate->curexc_traceback;
-    tstate->curexc_type = 0;
-    tstate->curexc_value = 0;
-    tstate->curexc_traceback = 0;
-#endif
-}
-#endif
-
 /* PyObjectGetAttrStr */
 #if CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStr(PyObject* obj, PyObject* attr_name) {
     PyTypeObject* tp = Py_TYPE(obj);
     if (likely(tp->tp_getattro))
         return tp->tp_getattro(obj, attr_name);
 #if PY_MAJOR_VERSION < 3
     if (likely(tp->tp_getattr))
         return tp->tp_getattr(obj, PyString_AS_STRING(attr_name));
 #endif
     return PyObject_GetAttr(obj, attr_name);
 }
 #endif
 
-/* PyObjectGetAttrStrNoError */
-static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
-    __Pyx_PyThreadState_declare
-    __Pyx_PyThreadState_assign
-    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
-        __Pyx_PyErr_Clear();
-}
-static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
-    PyObject *result;
-#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
-    PyTypeObject* tp = Py_TYPE(obj);
-    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
-        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
-    }
-#endif
-    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
-    if (unlikely(!result)) {
-        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
-    }
-    return result;
-}
-
 /* GetBuiltinName */
 static PyObject *__Pyx_GetBuiltinName(PyObject *name) {
-    PyObject* result = __Pyx_PyObject_GetAttrStrNoError(__pyx_b, name);
-    if (unlikely(!result) && !PyErr_Occurred()) {
+    PyObject* result = __Pyx_PyObject_GetAttrStr(__pyx_b, name);
+    if (unlikely(!result)) {
         PyErr_Format(PyExc_NameError,
 #if PY_MAJOR_VERSION >= 3
             "name '%U' is not defined", name);
 #else
             "name '%.200s' is not defined", PyString_AS_STRING(name));
 #endif
     }
     return result;
 }
 
-/* TupleAndListFromArray */
-#if CYTHON_COMPILING_IN_CPYTHON
-static CYTHON_INLINE void __Pyx_copy_object_array(PyObject *const *CYTHON_RESTRICT src, PyObject** CYTHON_RESTRICT dest, Py_ssize_t length) {
-    PyObject *v;
-    Py_ssize_t i;
-    for (i = 0; i < length; i++) {
-        v = dest[i] = src[i];
-        Py_INCREF(v);
-    }
-}
-static CYTHON_INLINE PyObject *
-__Pyx_PyTuple_FromArray(PyObject *const *src, Py_ssize_t n)
-{
-    PyObject *res;
-    if (n <= 0) {
-        Py_INCREF(__pyx_empty_tuple);
-        return __pyx_empty_tuple;
-    }
-    res = PyTuple_New(n);
-    if (unlikely(res == NULL)) return NULL;
-    __Pyx_copy_object_array(src, ((PyTupleObject*)res)->ob_item, n);
-    return res;
-}
-static CYTHON_INLINE PyObject *
-__Pyx_PyList_FromArray(PyObject *const *src, Py_ssize_t n)
-{
-    PyObject *res;
-    if (n <= 0) {
-        return PyList_New(0);
-    }
-    res = PyList_New(n);
-    if (unlikely(res == NULL)) return NULL;
-    __Pyx_copy_object_array(src, ((PyListObject*)res)->ob_item, n);
-    return res;
-}
-#endif
-
-/* BytesEquals */
-static CYTHON_INLINE int __Pyx_PyBytes_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-    if (s1 == s2) {
-        return (equals == Py_EQ);
-    } else if (PyBytes_CheckExact(s1) & PyBytes_CheckExact(s2)) {
-        const char *ps1, *ps2;
-        Py_ssize_t length = PyBytes_GET_SIZE(s1);
-        if (length != PyBytes_GET_SIZE(s2))
-            return (equals == Py_NE);
-        ps1 = PyBytes_AS_STRING(s1);
-        ps2 = PyBytes_AS_STRING(s2);
-        if (ps1[0] != ps2[0]) {
-            return (equals == Py_NE);
-        } else if (length == 1) {
-            return (equals == Py_EQ);
-        } else {
-            int result;
-#if CYTHON_USE_UNICODE_INTERNALS && (PY_VERSION_HEX < 0x030B0000)
-            Py_hash_t hash1, hash2;
-            hash1 = ((PyBytesObject*)s1)->ob_shash;
-            hash2 = ((PyBytesObject*)s2)->ob_shash;
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                return (equals == Py_NE);
-            }
-#endif
-            result = memcmp(ps1, ps2, (size_t)length);
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & PyBytes_CheckExact(s2)) {
-        return (equals == Py_NE);
-    } else if ((s2 == Py_None) & PyBytes_CheckExact(s1)) {
-        return (equals == Py_NE);
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
-    }
-#endif
-}
-
-/* UnicodeEquals */
-static CYTHON_INLINE int __Pyx_PyUnicode_Equals(PyObject* s1, PyObject* s2, int equals) {
-#if CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API
-    return PyObject_RichCompareBool(s1, s2, equals);
-#else
-#if PY_MAJOR_VERSION < 3
-    PyObject* owned_ref = NULL;
-#endif
-    int s1_is_unicode, s2_is_unicode;
-    if (s1 == s2) {
-        goto return_eq;
-    }
-    s1_is_unicode = PyUnicode_CheckExact(s1);
-    s2_is_unicode = PyUnicode_CheckExact(s2);
-#if PY_MAJOR_VERSION < 3
-    if ((s1_is_unicode & (!s2_is_unicode)) && PyString_CheckExact(s2)) {
-        owned_ref = PyUnicode_FromObject(s2);
-        if (unlikely(!owned_ref))
-            return -1;
-        s2 = owned_ref;
-        s2_is_unicode = 1;
-    } else if ((s2_is_unicode & (!s1_is_unicode)) && PyString_CheckExact(s1)) {
-        owned_ref = PyUnicode_FromObject(s1);
-        if (unlikely(!owned_ref))
-            return -1;
-        s1 = owned_ref;
-        s1_is_unicode = 1;
-    } else if (((!s2_is_unicode) & (!s1_is_unicode))) {
-        return __Pyx_PyBytes_Equals(s1, s2, equals);
-    }
-#endif
-    if (s1_is_unicode & s2_is_unicode) {
-        Py_ssize_t length;
-        int kind;
-        void *data1, *data2;
-        if (unlikely(__Pyx_PyUnicode_READY(s1) < 0) || unlikely(__Pyx_PyUnicode_READY(s2) < 0))
-            return -1;
-        length = __Pyx_PyUnicode_GET_LENGTH(s1);
-        if (length != __Pyx_PyUnicode_GET_LENGTH(s2)) {
-            goto return_ne;
-        }
-#if CYTHON_USE_UNICODE_INTERNALS
-        {
-            Py_hash_t hash1, hash2;
-        #if CYTHON_PEP393_ENABLED
-            hash1 = ((PyASCIIObject*)s1)->hash;
-            hash2 = ((PyASCIIObject*)s2)->hash;
-        #else
-            hash1 = ((PyUnicodeObject*)s1)->hash;
-            hash2 = ((PyUnicodeObject*)s2)->hash;
-        #endif
-            if (hash1 != hash2 && hash1 != -1 && hash2 != -1) {
-                goto return_ne;
-            }
-        }
-#endif
-        kind = __Pyx_PyUnicode_KIND(s1);
-        if (kind != __Pyx_PyUnicode_KIND(s2)) {
-            goto return_ne;
-        }
-        data1 = __Pyx_PyUnicode_DATA(s1);
-        data2 = __Pyx_PyUnicode_DATA(s2);
-        if (__Pyx_PyUnicode_READ(kind, data1, 0) != __Pyx_PyUnicode_READ(kind, data2, 0)) {
-            goto return_ne;
-        } else if (length == 1) {
-            goto return_eq;
-        } else {
-            int result = memcmp(data1, data2, (size_t)(length * kind));
-            #if PY_MAJOR_VERSION < 3
-            Py_XDECREF(owned_ref);
-            #endif
-            return (equals == Py_EQ) ? (result == 0) : (result != 0);
-        }
-    } else if ((s1 == Py_None) & s2_is_unicode) {
-        goto return_ne;
-    } else if ((s2 == Py_None) & s1_is_unicode) {
-        goto return_ne;
-    } else {
-        int result;
-        PyObject* py_result = PyObject_RichCompare(s1, s2, equals);
-        #if PY_MAJOR_VERSION < 3
-        Py_XDECREF(owned_ref);
-        #endif
-        if (!py_result)
-            return -1;
-        result = __Pyx_PyObject_IsTrue(py_result);
-        Py_DECREF(py_result);
-        return result;
-    }
-return_eq:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_EQ);
-return_ne:
-    #if PY_MAJOR_VERSION < 3
-    Py_XDECREF(owned_ref);
-    #endif
-    return (equals == Py_NE);
-#endif
-}
-
-/* fastcall */
-#if CYTHON_METH_FASTCALL
-static CYTHON_INLINE PyObject * __Pyx_GetKwValue_FASTCALL(PyObject *kwnames, PyObject *const *kwvalues, PyObject *s)
-{
-    Py_ssize_t i, n = PyTuple_GET_SIZE(kwnames);
-    for (i = 0; i < n; i++)
-    {
-        if (s == PyTuple_GET_ITEM(kwnames, i)) return kwvalues[i];
-    }
-    for (i = 0; i < n; i++)
-    {
-        int eq = __Pyx_PyUnicode_Equals(s, PyTuple_GET_ITEM(kwnames, i), Py_EQ);
-        if (unlikely(eq != 0)) {
-            if (unlikely(eq < 0)) return NULL;  // error
-            return kwvalues[i];
-        }
-    }
-    return NULL;  // not found (no exception set)
-}
-#endif
-
 /* RaiseDoubleKeywords */
 static void __Pyx_RaiseDoubleKeywordsError(
     const char* func_name,
     PyObject* kw_name)
 {
     PyErr_Format(PyExc_TypeError,
         #if PY_MAJOR_VERSION >= 3
@@ -5290,37 +3440,25 @@
         PyString_AsString(kw_name));
         #endif
 }
 
 /* ParseKeywords */
 static int __Pyx_ParseOptionalKeywords(
     PyObject *kwds,
-    PyObject *const *kwvalues,
     PyObject **argnames[],
     PyObject *kwds2,
     PyObject *values[],
     Py_ssize_t num_pos_args,
     const char* function_name)
 {
     PyObject *key = 0, *value = 0;
     Py_ssize_t pos = 0;
     PyObject*** name;
     PyObject*** first_kw_arg = argnames + num_pos_args;
-    int kwds_is_tuple = CYTHON_METH_FASTCALL && likely(PyTuple_Check(kwds));
-    while (1) {
-        if (kwds_is_tuple) {
-            if (pos >= PyTuple_GET_SIZE(kwds)) break;
-            key = PyTuple_GET_ITEM(kwds, pos);
-            value = kwvalues[pos];
-            pos++;
-        }
-        else
-        {
-            if (!PyDict_Next(kwds, &pos, &key, &value)) break;
-        }
+    while (PyDict_Next(kwds, &pos, &key, &value)) {
         name = first_kw_arg;
         while (*name && (**name != key)) name++;
         if (*name) {
             values[name-argnames] = value;
             continue;
         }
         name = first_kw_arg;
@@ -5346,20 +3484,19 @@
                     argname++;
                 }
             }
         } else
         #endif
         if (likely(PyUnicode_Check(key))) {
             while (*name) {
-                int cmp = (
+                int cmp = (**name == key) ? 0 :
                 #if !CYTHON_COMPILING_IN_PYPY && PY_MAJOR_VERSION >= 3
                     (__Pyx_PyUnicode_GET_LENGTH(**name) != __Pyx_PyUnicode_GET_LENGTH(key)) ? 1 :
                 #endif
-                    PyUnicode_Compare(**name, key)
-                );
+                    PyUnicode_Compare(**name, key);
                 if (cmp < 0 && unlikely(PyErr_Occurred())) goto bad;
                 if (cmp == 0) {
                     values[name-argnames] = value;
                     break;
                 }
                 name++;
             }
@@ -5390,20 +3527,19 @@
     __Pyx_RaiseDoubleKeywordsError(function_name, key);
     goto bad;
 invalid_keyword_type:
     PyErr_Format(PyExc_TypeError,
         "%.200s() keywords must be strings", function_name);
     goto bad;
 invalid_keyword:
-    #if PY_MAJOR_VERSION < 3
     PyErr_Format(PyExc_TypeError,
+    #if PY_MAJOR_VERSION < 3
         "%.200s() got an unexpected keyword argument '%.200s'",
         function_name, PyString_AsString(key));
     #else
-    PyErr_Format(PyExc_TypeError,
         "%s() got an unexpected keyword argument '%U'",
         function_name, key);
     #endif
 bad:
     return -1;
 }
 
@@ -5429,25 +3565,14 @@
     }
     PyErr_Format(PyExc_TypeError,
                  "%.200s() takes %.8s %" CYTHON_FORMAT_SSIZE_T "d positional argument%.1s (%" CYTHON_FORMAT_SSIZE_T "d given)",
                  func_name, more_or_less, num_expected,
                  (num_expected == 1) ? "" : "s", num_found);
 }
 
-/* RaiseUnexpectedTypeError */
-static int
-__Pyx_RaiseUnexpectedTypeError(const char *expected, PyObject *obj)
-{
-    __Pyx_TypeName obj_type_name = __Pyx_PyType_GetName(Py_TYPE(obj));
-    PyErr_Format(PyExc_TypeError, "Expected %s, got " __Pyx_FMT_TYPENAME,
-                 expected, obj_type_name);
-    __Pyx_DECREF_TypeName(obj_type_name);
-    return 0;
-}
-
 /* UnicodeAsUCS4 */
 static CYTHON_INLINE Py_UCS4 __Pyx_PyUnicode_AsPy_UCS4(PyObject* x) {
    Py_ssize_t length;
    #if CYTHON_PEP393_ENABLED
    length = PyUnicode_GET_LENGTH(x);
    if (likely(length == 1)) {
        return PyUnicode_READ_CHAR(x, 0);
@@ -5491,105 +3616,139 @@
     } else if (PyByteArray_Check(c)) {
         size = PyByteArray_GET_SIZE(c);
         if (likely(size == 1)) {
             return (unsigned char) PyByteArray_AS_STRING(c)[0];
         }
 #endif
     } else {
-        __Pyx_TypeName c_type_name = __Pyx_PyType_GetName(Py_TYPE(c));
         PyErr_Format(PyExc_TypeError,
-            "ord() expected string of length 1, but " __Pyx_FMT_TYPENAME " found",
-            c_type_name);
-        __Pyx_DECREF_TypeName(c_type_name);
+            "ord() expected string of length 1, but %.200s found", c->ob_type->tp_name);
         return (long)(Py_UCS4)-1;
     }
     PyErr_Format(PyExc_TypeError,
         "ord() expected a character, but string of length %zd found", size);
     return (long)(Py_UCS4)-1;
 }
 
-/* KeywordStringCheck */
-static int __Pyx_CheckKeywordStrings(
-    PyObject *kw,
-    const char* function_name,
-    int kw_allowed)
-{
-    PyObject* key = 0;
-    Py_ssize_t pos = 0;
-#if CYTHON_COMPILING_IN_PYPY
-    if (!kw_allowed && PyDict_Next(kw, &pos, &key, 0))
-        goto invalid_keyword;
-    return 1;
-#else
-    if (CYTHON_METH_FASTCALL && likely(PyTuple_Check(kw))) {
-        if (unlikely(PyTuple_GET_SIZE(kw) == 0))
-            return 1;
-        if (!kw_allowed) {
-            key = PyTuple_GET_ITEM(kw, 0);
-            goto invalid_keyword;
-        }
-#if PY_VERSION_HEX < 0x03090000
-        for (pos = 0; pos < PyTuple_GET_SIZE(kw); pos++) {
-            key = PyTuple_GET_ITEM(kw, pos);
-            if (unlikely(!PyUnicode_Check(key)))
-                goto invalid_keyword_type;
-        }
+/* PyErrFetchRestore */
+#if CYTHON_FAST_THREAD_STATE
+static CYTHON_INLINE void __Pyx_ErrRestoreInState(PyThreadState *tstate, PyObject *type, PyObject *value, PyObject *tb) {
+    PyObject *tmp_type, *tmp_value, *tmp_tb;
+    tmp_type = tstate->curexc_type;
+    tmp_value = tstate->curexc_value;
+    tmp_tb = tstate->curexc_traceback;
+    tstate->curexc_type = type;
+    tstate->curexc_value = value;
+    tstate->curexc_traceback = tb;
+    Py_XDECREF(tmp_type);
+    Py_XDECREF(tmp_value);
+    Py_XDECREF(tmp_tb);
+}
+static CYTHON_INLINE void __Pyx_ErrFetchInState(PyThreadState *tstate, PyObject **type, PyObject **value, PyObject **tb) {
+    *type = tstate->curexc_type;
+    *value = tstate->curexc_value;
+    *tb = tstate->curexc_traceback;
+    tstate->curexc_type = 0;
+    tstate->curexc_value = 0;
+    tstate->curexc_traceback = 0;
+}
 #endif
-        return 1;
-    }
-    while (PyDict_Next(kw, &pos, &key, 0)) {
-        #if PY_MAJOR_VERSION < 3
-        if (unlikely(!PyString_Check(key)))
-        #endif
-            if (unlikely(!PyUnicode_Check(key)))
-                goto invalid_keyword_type;
-    }
-    if (!kw_allowed && unlikely(key))
-        goto invalid_keyword;
-    return 1;
-invalid_keyword_type:
-    PyErr_Format(PyExc_TypeError,
-        "%.200s() keywords must be strings", function_name);
-    return 0;
+
+/* WriteUnraisableException */
+static void __Pyx_WriteUnraisable(const char *name, CYTHON_UNUSED int clineno,
+                                  CYTHON_UNUSED int lineno, CYTHON_UNUSED const char *filename,
+                                  int full_traceback, CYTHON_UNUSED int nogil) {
+    PyObject *old_exc, *old_val, *old_tb;
+    PyObject *ctx;
+    __Pyx_PyThreadState_declare
+#ifdef WITH_THREAD
+    PyGILState_STATE state;
+    if (nogil)
+        state = PyGILState_Ensure();
+#ifdef _MSC_VER
+    else state = (PyGILState_STATE)-1;
 #endif
-invalid_keyword:
+#endif
+    __Pyx_PyThreadState_assign
+    __Pyx_ErrFetch(&old_exc, &old_val, &old_tb);
+    if (full_traceback) {
+        Py_XINCREF(old_exc);
+        Py_XINCREF(old_val);
+        Py_XINCREF(old_tb);
+        __Pyx_ErrRestore(old_exc, old_val, old_tb);
+        PyErr_PrintEx(1);
+    }
     #if PY_MAJOR_VERSION < 3
-    PyErr_Format(PyExc_TypeError,
-        "%.200s() got an unexpected keyword argument '%.200s'",
-        function_name, PyString_AsString(key));
+    ctx = PyString_FromString(name);
     #else
-    PyErr_Format(PyExc_TypeError,
-        "%s() got an unexpected keyword argument '%U'",
-        function_name, key);
+    ctx = PyUnicode_FromString(name);
     #endif
+    __Pyx_ErrRestore(old_exc, old_val, old_tb);
+    if (!ctx) {
+        PyErr_WriteUnraisable(Py_None);
+    } else {
+        PyErr_WriteUnraisable(ctx);
+        Py_DECREF(ctx);
+    }
+#ifdef WITH_THREAD
+    if (nogil)
+        PyGILState_Release(state);
+#endif
+}
+
+/* PyErrExceptionMatches */
+#if CYTHON_FAST_THREAD_STATE
+static int __Pyx_PyErr_ExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
+    Py_ssize_t i, n;
+    n = PyTuple_GET_SIZE(tuple);
+#if PY_MAJOR_VERSION >= 3
+    for (i=0; i<n; i++) {
+        if (exc_type == PyTuple_GET_ITEM(tuple, i)) return 1;
+    }
+#endif
+    for (i=0; i<n; i++) {
+        if (__Pyx_PyErr_GivenExceptionMatches(exc_type, PyTuple_GET_ITEM(tuple, i))) return 1;
+    }
     return 0;
 }
+static CYTHON_INLINE int __Pyx_PyErr_ExceptionMatchesInState(PyThreadState* tstate, PyObject* err) {
+    PyObject *exc_type = tstate->curexc_type;
+    if (exc_type == err) return 1;
+    if (unlikely(!exc_type)) return 0;
+    if (unlikely(PyTuple_Check(err)))
+        return __Pyx_PyErr_ExceptionMatchesTuple(exc_type, err);
+    return __Pyx_PyErr_GivenExceptionMatches(exc_type, err);
+}
+#endif
+
+/* GetAttr */
+static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
+#if CYTHON_USE_TYPE_SLOTS
+#if PY_MAJOR_VERSION >= 3
+    if (likely(PyUnicode_Check(n)))
+#else
+    if (likely(PyString_Check(n)))
+#endif
+        return __Pyx_PyObject_GetAttrStr(o, n);
+#endif
+    return PyObject_GetAttr(o, n);
+}
 
 /* GetAttr3 */
 static PyObject *__Pyx_GetAttr3Default(PyObject *d) {
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     if (unlikely(!__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
         return NULL;
     __Pyx_PyErr_Clear();
     Py_INCREF(d);
     return d;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetAttr3(PyObject *o, PyObject *n, PyObject *d) {
-    PyObject *r;
-#if CYTHON_USE_TYPE_SLOTS
-    if (likely(PyString_Check(n))) {
-        r = __Pyx_PyObject_GetAttrStrNoError(o, n);
-        if (unlikely(!r) && likely(!PyErr_Occurred())) {
-            r = __Pyx_NewRef(d);
-        }
-        return r;
-    }
-#endif
-    r = PyObject_GetAttr(o, n);
+    PyObject *r = __Pyx_GetAttr(o, n);
     return (likely(r)) ? r : __Pyx_GetAttr3Default(d);
 }
 
 /* PyDictVersioning */
 #if CYTHON_USE_DICT_VERSIONS && CYTHON_USE_TYPE_SLOTS
 static CYTHON_INLINE PY_UINT64_T __Pyx_get_tp_dict_version(PyObject *obj) {
     PyObject *dict = Py_TYPE(obj)->tp_dict;
@@ -5628,22 +3787,14 @@
     result = _PyDict_GetItem_KnownHash(__pyx_d, name, ((PyASCIIObject *) name)->hash);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     } else if (unlikely(PyErr_Occurred())) {
         return NULL;
     }
-#elif CYTHON_COMPILING_IN_LIMITED_API
-    if (unlikely(!__pyx_m)) {
-        return NULL;
-    }
-    result = PyObject_GetAttr(__pyx_m, name);
-    if (likely(result)) {
-        return result;
-    }
 #else
     result = PyDict_GetItem(__pyx_d, name);
     __PYX_UPDATE_DICT_CACHE(__pyx_d, result, *dict_cached_value, *dict_version)
     if (likely(result)) {
         return __Pyx_NewRef(result);
     }
 #endif
@@ -5654,16 +3805,39 @@
         return __Pyx_NewRef(result);
     }
     PyErr_Clear();
 #endif
     return __Pyx_GetBuiltinName(name);
 }
 
+/* PyCFunctionFastCall */
+#if CYTHON_FAST_PYCCALL
+static CYTHON_INLINE PyObject * __Pyx_PyCFunction_FastCall(PyObject *func_obj, PyObject **args, Py_ssize_t nargs) {
+    PyCFunctionObject *func = (PyCFunctionObject*)func_obj;
+    PyCFunction meth = PyCFunction_GET_FUNCTION(func);
+    PyObject *self = PyCFunction_GET_SELF(func);
+    int flags = PyCFunction_GET_FLAGS(func);
+    assert(PyCFunction_Check(func));
+    assert(METH_FASTCALL == (flags & ~(METH_CLASS | METH_STATIC | METH_COEXIST | METH_KEYWORDS | METH_STACKLESS)));
+    assert(nargs >= 0);
+    assert(nargs == 0 || args != NULL);
+    /* _PyCFunction_FastCallDict() must not be called with an exception set,
+       because it may clear it (directly or indirectly) and so the
+       caller loses its exception */
+    assert(!PyErr_Occurred());
+    if ((PY_VERSION_HEX < 0x030700A0) || unlikely(flags & METH_KEYWORDS)) {
+        return (*((__Pyx_PyCFunctionFastWithKeywords)(void*)meth)) (self, args, nargs, NULL);
+    } else {
+        return (*((__Pyx_PyCFunctionFast)(void*)meth)) (self, args, nargs);
+    }
+}
+#endif
+
 /* PyFunctionFastCall */
-#if CYTHON_FAST_PYCALL && !CYTHON_VECTORCALL
+#if CYTHON_FAST_PYCALL
 static PyObject* __Pyx_PyFunction_FastCallNoKw(PyCodeObject *co, PyObject **args, Py_ssize_t na,
                                                PyObject *globals) {
     PyFrameObject *f;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
     PyObject **fastlocals;
     Py_ssize_t i;
     PyObject *result;
@@ -5684,14 +3858,15 @@
     }
     result = PyEval_EvalFrameEx(f,0);
     ++tstate->recursion_depth;
     Py_DECREF(f);
     --tstate->recursion_depth;
     return result;
 }
+#if 1 || PY_VERSION_HEX < 0x030600B1
 static PyObject *__Pyx_PyFunction_FastCallDict(PyObject *func, PyObject **args, Py_ssize_t nargs, PyObject *kwargs) {
     PyCodeObject *co = (PyCodeObject *)PyFunction_GET_CODE(func);
     PyObject *globals = PyFunction_GET_GLOBALS(func);
     PyObject *argdefs = PyFunction_GET_DEFAULTS(func);
     PyObject *closure;
 #if PY_MAJOR_VERSION >= 3
     PyObject *kwdefs;
@@ -5699,15 +3874,15 @@
     PyObject *kwtuple, **k;
     PyObject **d;
     Py_ssize_t nd;
     Py_ssize_t nk;
     PyObject *result;
     assert(kwargs == NULL || PyDict_Check(kwargs));
     nk = kwargs ? PyDict_Size(kwargs) : 0;
-    if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object"))) {
+    if (Py_EnterRecursiveCall((char*)" while calling a Python object")) {
         return NULL;
     }
     if (
 #if PY_MAJOR_VERSION >= 3
             co->co_kwonlyargcount == 0 &&
 #endif
             likely(kwargs == NULL || nk == 0) &&
@@ -5770,20 +3945,21 @@
 #endif
     Py_XDECREF(kwtuple);
 done:
     Py_LeaveRecursiveCall();
     return result;
 }
 #endif
+#endif
 
 /* PyObjectCall */
 #if CYTHON_COMPILING_IN_CPYTHON
 static CYTHON_INLINE PyObject* __Pyx_PyObject_Call(PyObject *func, PyObject *arg, PyObject *kw) {
     PyObject *result;
-    ternaryfunc call = Py_TYPE(func)->tp_call;
+    ternaryfunc call = func->ob_type->tp_call;
     if (unlikely(!call))
         return PyObject_Call(func, arg, kw);
     if (unlikely(Py_EnterRecursiveCall((char*)" while calling a Python object")))
         return NULL;
     result = (*call)(func, arg, kw);
     Py_LeaveRecursiveCall();
     if (unlikely(!result) && unlikely(!PyErr_Occurred())) {
@@ -5811,213 +3987,167 @@
             PyExc_SystemError,
             "NULL result without error in PyObject_Call");
     }
     return result;
 }
 #endif
 
-/* PyObjectFastCall */
-static PyObject* __Pyx_PyObject_FastCall_fallback(PyObject *func, PyObject **args, size_t nargs, PyObject *kwargs) {
-    PyObject *argstuple;
+/* PyObjectCallOneArg */
+#if CYTHON_COMPILING_IN_CPYTHON
+static PyObject* __Pyx__PyObject_CallOneArg(PyObject *func, PyObject *arg) {
     PyObject *result;
-    size_t i;
-    argstuple = PyTuple_New((Py_ssize_t)nargs);
-    if (unlikely(!argstuple)) return NULL;
-    for (i = 0; i < nargs; i++) {
-        Py_INCREF(args[i]);
-        PyTuple_SET_ITEM(argstuple, (Py_ssize_t)i, args[i]);
-    }
-    result = __Pyx_PyObject_Call(func, argstuple, kwargs);
-    Py_DECREF(argstuple);
+    PyObject *args = PyTuple_New(1);
+    if (unlikely(!args)) return NULL;
+    Py_INCREF(arg);
+    PyTuple_SET_ITEM(args, 0, arg);
+    result = __Pyx_PyObject_Call(func, args, NULL);
+    Py_DECREF(args);
     return result;
 }
-static CYTHON_INLINE PyObject* __Pyx_PyObject_FastCallDict(PyObject *func, PyObject **args, size_t _nargs, PyObject *kwargs) {
-    Py_ssize_t nargs = __Pyx_PyVectorcall_NARGS(_nargs);
-#if CYTHON_COMPILING_IN_CPYTHON
-    if (nargs == 0 && kwargs == NULL) {
-#if defined(__Pyx_CyFunction_USED) && defined(NDEBUG)
-        if (__Pyx_IsCyOrPyCFunction(func))
-#else
-        if (PyCFunction_Check(func))
-#endif
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_NOARGS)) {
-                return __Pyx_PyObject_CallMethO(func, NULL);
-            }
-        }
-    }
-    else if (nargs == 1 && kwargs == NULL) {
-        if (PyCFunction_Check(func))
-        {
-            if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
-                return __Pyx_PyObject_CallMethO(func, args[0]);
-            }
-        }
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+#if CYTHON_FAST_PYCALL
+    if (PyFunction_Check(func)) {
+        return __Pyx_PyFunction_FastCall(func, &arg, 1);
     }
 #endif
-    #if PY_VERSION_HEX < 0x030800B1
-    #if CYTHON_FAST_PYCCALL
-    if (PyCFunction_Check(func)) {
-        if (kwargs) {
-            return _PyCFunction_FastCallDict(func, args, nargs, kwargs);
-        } else {
-            return _PyCFunction_FastCallKeywords(func, args, nargs, NULL);
+    if (likely(PyCFunction_Check(func))) {
+        if (likely(PyCFunction_GET_FLAGS(func) & METH_O)) {
+            return __Pyx_PyObject_CallMethO(func, arg);
+#if CYTHON_FAST_PYCCALL
+        } else if (PyCFunction_GET_FLAGS(func) & METH_FASTCALL) {
+            return __Pyx_PyCFunction_FastCall(func, &arg, 1);
+#endif
         }
     }
-    #if PY_VERSION_HEX >= 0x030700A1
-    if (!kwargs && __Pyx_IS_TYPE(func, &PyMethodDescr_Type)) {
-        return _PyMethodDescr_FastCallKeywords(func, args, nargs, NULL);
-    }
-    #endif
-    #endif
+    return __Pyx__PyObject_CallOneArg(func, arg);
+}
+#else
+static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
+    PyObject *result;
+    PyObject *args = PyTuple_Pack(1, arg);
+    if (unlikely(!args)) return NULL;
+    result = __Pyx_PyObject_Call(func, args, NULL);
+    Py_DECREF(args);
+    return result;
+}
+#endif
+
+/* PyObjectCall2Args */
+static CYTHON_UNUSED PyObject* __Pyx_PyObject_Call2Args(PyObject* function, PyObject* arg1, PyObject* arg2) {
+    PyObject *args, *result = NULL;
     #if CYTHON_FAST_PYCALL
-    if (PyFunction_Check(func)) {
-        return __Pyx_PyFunction_FastCallDict(func, args, nargs, kwargs);
+    if (PyFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyFunction_FastCall(function, args, 2);
     }
     #endif
-    #endif
-    #if CYTHON_VECTORCALL
-    vectorcallfunc f = _PyVectorcall_Function(func);
-    if (f) {
-        return f(func, args, (size_t)nargs, kwargs);
-    }
-    #elif defined(__Pyx_CyFunction_USED) && CYTHON_BACKPORT_VECTORCALL
-    if (__Pyx_CyFunction_CheckExact(func)) {
-        __pyx_vectorcallfunc f = __Pyx_CyFunction_func_vectorcall(func);
-        if (f) return f(func, args, (size_t)nargs, kwargs);
+    #if CYTHON_FAST_PYCCALL
+    if (__Pyx_PyFastCFunction_Check(function)) {
+        PyObject *args[2] = {arg1, arg2};
+        return __Pyx_PyCFunction_FastCall(function, args, 2);
     }
     #endif
-    if (nargs == 0) {
-        return __Pyx_PyObject_Call(func, __pyx_empty_tuple, kwargs);
-    }
-    return __Pyx_PyObject_FastCall_fallback(func, args, (size_t)nargs, kwargs);
-}
-
-/* PyObjectCallOneArg */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallOneArg(PyObject *func, PyObject *arg) {
-    PyObject *args[2] = {NULL, arg};
-    return __Pyx_PyObject_FastCall(func, args+1, 1 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
+    args = PyTuple_New(2);
+    if (unlikely(!args)) goto done;
+    Py_INCREF(arg1);
+    PyTuple_SET_ITEM(args, 0, arg1);
+    Py_INCREF(arg2);
+    PyTuple_SET_ITEM(args, 1, arg2);
+    Py_INCREF(function);
+    result = __Pyx_PyObject_Call(function, args, NULL);
+    Py_DECREF(args);
+    Py_DECREF(function);
+done:
+    return result;
 }
 
 /* Import */
 static PyObject *__Pyx_Import(PyObject *name, PyObject *from_list, int level) {
+    PyObject *empty_list = 0;
     PyObject *module = 0;
+    PyObject *global_dict = 0;
     PyObject *empty_dict = 0;
-    PyObject *empty_list = 0;
+    PyObject *list;
     #if PY_MAJOR_VERSION < 3
     PyObject *py_import;
     py_import = __Pyx_PyObject_GetAttrStr(__pyx_b, __pyx_n_s_import);
-    if (unlikely(!py_import))
+    if (!py_import)
         goto bad;
-    if (!from_list) {
+    #endif
+    if (from_list)
+        list = from_list;
+    else {
         empty_list = PyList_New(0);
-        if (unlikely(!empty_list))
+        if (!empty_list)
             goto bad;
-        from_list = empty_list;
+        list = empty_list;
     }
-    #endif
+    global_dict = PyModule_GetDict(__pyx_m);
+    if (!global_dict)
+        goto bad;
     empty_dict = PyDict_New();
-    if (unlikely(!empty_dict))
+    if (!empty_dict)
         goto bad;
     {
         #if PY_MAJOR_VERSION >= 3
         if (level == -1) {
             if ((1) && (strchr(__Pyx_MODULE_NAME, '.'))) {
-                #if CYTHON_COMPILING_IN_LIMITED_API
-                module = PyImport_ImportModuleLevelObject(
-                    name, empty_dict, empty_dict, from_list, 1);
-                #else
                 module = PyImport_ImportModuleLevelObject(
-                    name, __pyx_d, empty_dict, from_list, 1);
-                #endif
-                if (unlikely(!module)) {
-                    if (unlikely(!PyErr_ExceptionMatches(PyExc_ImportError)))
+                    name, global_dict, empty_dict, list, 1);
+                if (!module) {
+                    if (!PyErr_ExceptionMatches(PyExc_ImportError))
                         goto bad;
                     PyErr_Clear();
                 }
             }
             level = 0;
         }
         #endif
         if (!module) {
             #if PY_MAJOR_VERSION < 3
             PyObject *py_level = PyInt_FromLong(level);
-            if (unlikely(!py_level))
+            if (!py_level)
                 goto bad;
             module = PyObject_CallFunctionObjArgs(py_import,
-                name, __pyx_d, empty_dict, from_list, py_level, (PyObject *)NULL);
+                name, global_dict, empty_dict, list, py_level, (PyObject *)NULL);
             Py_DECREF(py_level);
             #else
-            #if CYTHON_COMPILING_IN_LIMITED_API
-            module = PyImport_ImportModuleLevelObject(
-                name, empty_dict, empty_dict, from_list, level);
-            #else
             module = PyImport_ImportModuleLevelObject(
-                name, __pyx_d, empty_dict, from_list, level);
-            #endif
+                name, global_dict, empty_dict, list, level);
             #endif
         }
     }
 bad:
-    Py_XDECREF(empty_dict);
-    Py_XDECREF(empty_list);
     #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_import);
     #endif
+    Py_XDECREF(empty_list);
+    Py_XDECREF(empty_dict);
     return module;
 }
 
 /* ImportFrom */
 static PyObject* __Pyx_ImportFrom(PyObject* module, PyObject* name) {
     PyObject* value = __Pyx_PyObject_GetAttrStr(module, name);
     if (unlikely(!value) && PyErr_ExceptionMatches(PyExc_AttributeError)) {
-        const char* module_name_str = 0;
-        PyObject* module_name = 0;
-        PyObject* module_dot = 0;
-        PyObject* full_name = 0;
-        PyErr_Clear();
-        module_name_str = PyModule_GetName(module);
-        if (unlikely(!module_name_str)) { goto modbad; }
-        module_name = PyUnicode_FromString(module_name_str);
-        if (unlikely(!module_name)) { goto modbad; }
-        module_dot = PyUnicode_Concat(module_name, __pyx_kp_u__2);
-        if (unlikely(!module_dot)) { goto modbad; }
-        full_name = PyUnicode_Concat(module_dot, name);
-        if (unlikely(!full_name)) { goto modbad; }
-        #if PY_VERSION_HEX < 0x030700A1 || (CYTHON_COMPILING_IN_PYPY && PYPY_VERSION_NUM  < 0x07030400)
-        {
-            PyObject *modules = PyImport_GetModuleDict();
-            if (unlikely(!modules))
-                goto modbad;
-            value = PyObject_GetItem(modules, full_name);
-        }
-        #else
-        value = PyImport_GetModule(full_name);
-        #endif
-      modbad:
-        Py_XDECREF(full_name);
-        Py_XDECREF(module_dot);
-        Py_XDECREF(module_name);
-    }
-    if (unlikely(!value)) {
         PyErr_Format(PyExc_ImportError,
         #if PY_MAJOR_VERSION < 3
             "cannot import name %.230s", PyString_AS_STRING(name));
         #else
             "cannot import name %S", name);
         #endif
     }
     return value;
 }
 
 /* RaiseException */
 #if PY_MAJOR_VERSION < 3
-static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb, PyObject *cause) {
+static void __Pyx_Raise(PyObject *type, PyObject *value, PyObject *tb,
+                        CYTHON_UNUSED PyObject *cause) {
     __Pyx_PyThreadState_declare
-    CYTHON_UNUSED_VAR(cause);
     Py_XINCREF(type);
     if (!value || value == Py_None)
         value = NULL;
     else
         Py_INCREF(value);
     if (!tb || tb == Py_None)
         tb = NULL;
@@ -6142,42 +4272,40 @@
                             "BaseException");
             goto bad;
         }
         PyException_SetCause(value, fixed_cause);
     }
     PyErr_SetObject(type, value);
     if (tb) {
-      #if PY_VERSION_HEX >= 0x030C00A6
-        PyException_SetTraceback(value, tb);
-      #elif CYTHON_FAST_THREAD_STATE
+#if CYTHON_COMPILING_IN_PYPY
+        PyObject *tmp_type, *tmp_value, *tmp_tb;
+        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
+        Py_INCREF(tb);
+        PyErr_Restore(tmp_type, tmp_value, tb);
+        Py_XDECREF(tmp_tb);
+#else
         PyThreadState *tstate = __Pyx_PyThreadState_Current;
         PyObject* tmp_tb = tstate->curexc_traceback;
         if (tb != tmp_tb) {
             Py_INCREF(tb);
             tstate->curexc_traceback = tb;
             Py_XDECREF(tmp_tb);
         }
-#else
-        PyObject *tmp_type, *tmp_value, *tmp_tb;
-        PyErr_Fetch(&tmp_type, &tmp_value, &tmp_tb);
-        Py_INCREF(tb);
-        PyErr_Restore(tmp_type, tmp_value, tb);
-        Py_XDECREF(tmp_tb);
 #endif
     }
 bad:
     Py_XDECREF(owned_instance);
     return;
 }
 #endif
 
 /* GetItemInt */
 static PyObject *__Pyx_GetItemInt_Generic(PyObject *o, PyObject* j) {
     PyObject *r;
-    if (unlikely(!j)) return NULL;
+    if (!j) return NULL;
     r = PyObject_GetItem(o, j);
     Py_DECREF(j);
     return r;
 }
 static CYTHON_INLINE PyObject *__Pyx_GetItemInt_List_Fast(PyObject *o, Py_ssize_t i,
                                                               CYTHON_NCP_UNUSED int wraparound,
                                                               CYTHON_NCP_UNUSED int boundscheck) {
@@ -6230,409 +4358,66 @@
         Py_ssize_t n = ((!wraparound) | likely(i >= 0)) ? i : i + PyTuple_GET_SIZE(o);
         if ((!boundscheck) || likely(__Pyx_is_valid_index(n, PyTuple_GET_SIZE(o)))) {
             PyObject *r = PyTuple_GET_ITEM(o, n);
             Py_INCREF(r);
             return r;
         }
     } else {
-        PyMappingMethods *mm = Py_TYPE(o)->tp_as_mapping;
-        PySequenceMethods *sm = Py_TYPE(o)->tp_as_sequence;
-        if (mm && mm->mp_subscript) {
-            PyObject *r, *key = PyInt_FromSsize_t(i);
-            if (unlikely(!key)) return NULL;
-            r = mm->mp_subscript(o, key);
-            Py_DECREF(key);
-            return r;
-        }
-        if (likely(sm && sm->sq_item)) {
-            if (wraparound && unlikely(i < 0) && likely(sm->sq_length)) {
-                Py_ssize_t l = sm->sq_length(o);
+        PySequenceMethods *m = Py_TYPE(o)->tp_as_sequence;
+        if (likely(m && m->sq_item)) {
+            if (wraparound && unlikely(i < 0) && likely(m->sq_length)) {
+                Py_ssize_t l = m->sq_length(o);
                 if (likely(l >= 0)) {
                     i += l;
                 } else {
                     if (!PyErr_ExceptionMatches(PyExc_OverflowError))
                         return NULL;
                     PyErr_Clear();
                 }
             }
-            return sm->sq_item(o, i);
+            return m->sq_item(o, i);
         }
     }
 #else
     if (is_list || PySequence_Check(o)) {
         return PySequence_GetItem(o, i);
     }
 #endif
     return __Pyx_GetItemInt_Generic(o, PyInt_FromSsize_t(i));
 }
 
-/* GetAttr */
-static CYTHON_INLINE PyObject *__Pyx_GetAttr(PyObject *o, PyObject *n) {
-#if CYTHON_USE_TYPE_SLOTS
-#if PY_MAJOR_VERSION >= 3
-    if (likely(PyUnicode_Check(n)))
-#else
-    if (likely(PyString_Check(n)))
-#endif
-        return __Pyx_PyObject_GetAttrStr(o, n);
-#endif
-    return PyObject_GetAttr(o, n);
-}
-
 /* HasAttr */
 static CYTHON_INLINE int __Pyx_HasAttr(PyObject *o, PyObject *n) {
     PyObject *r;
     if (unlikely(!__Pyx_PyBaseString_Check(n))) {
         PyErr_SetString(PyExc_TypeError,
                         "hasattr(): attribute name must be string");
         return -1;
     }
     r = __Pyx_GetAttr(o, n);
-    if (!r) {
+    if (unlikely(!r)) {
         PyErr_Clear();
         return 0;
     } else {
         Py_DECREF(r);
         return 1;
     }
 }
 
-/* FixUpExtensionType */
-#if CYTHON_USE_TYPE_SPECS
-static int __Pyx_fix_up_extension_type_from_spec(PyType_Spec *spec, PyTypeObject *type) {
-#if PY_VERSION_HEX > 0x030900B1 || CYTHON_COMPILING_IN_LIMITED_API
-    CYTHON_UNUSED_VAR(spec);
-    CYTHON_UNUSED_VAR(type);
-#else
-    const PyType_Slot *slot = spec->slots;
-    while (slot && slot->slot && slot->slot != Py_tp_members)
-        slot++;
-    if (slot && slot->slot == Py_tp_members) {
-        int changed = 0;
-#if !(PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON)
-        const
-#endif
-            PyMemberDef *memb = (PyMemberDef*) slot->pfunc;
-        while (memb && memb->name) {
-            if (memb->name[0] == '_' && memb->name[1] == '_') {
-#if PY_VERSION_HEX < 0x030900b1
-                if (strcmp(memb->name, "__weaklistoffset__") == 0) {
-                    assert(memb->type == T_PYSSIZET);
-                    assert(memb->flags == READONLY);
-                    type->tp_weaklistoffset = memb->offset;
-                    changed = 1;
-                }
-                else if (strcmp(memb->name, "__dictoffset__") == 0) {
-                    assert(memb->type == T_PYSSIZET);
-                    assert(memb->flags == READONLY);
-                    type->tp_dictoffset = memb->offset;
-                    changed = 1;
-                }
-#if CYTHON_METH_FASTCALL
-                else if (strcmp(memb->name, "__vectorcalloffset__") == 0) {
-                    assert(memb->type == T_PYSSIZET);
-                    assert(memb->flags == READONLY);
-#if PY_VERSION_HEX >= 0x030800b4
-                    type->tp_vectorcall_offset = memb->offset;
-#else
-                    type->tp_print = (printfunc) memb->offset;
-#endif
-                    changed = 1;
-                }
-#endif
-#else
-                if ((0));
-#endif
-#if PY_VERSION_HEX <= 0x030900b1 && CYTHON_COMPILING_IN_CPYTHON
-                else if (strcmp(memb->name, "__module__") == 0) {
-                    PyObject *descr;
-                    assert(memb->type == T_OBJECT);
-                    assert(memb->flags == 0 || memb->flags == READONLY);
-                    descr = PyDescr_NewMember(type, memb);
-                    if (unlikely(!descr))
-                        return -1;
-                    if (unlikely(PyDict_SetItem(type->tp_dict, PyDescr_NAME(descr), descr) < 0)) {
-                        Py_DECREF(descr);
-                        return -1;
-                    }
-                    Py_DECREF(descr);
-                    changed = 1;
-                }
-#endif
-            }
-            memb++;
-        }
-        if (changed)
-            PyType_Modified(type);
-    }
-#endif
-    return 0;
-}
-#endif
-
-/* PyObjectCallNoArg */
-static CYTHON_INLINE PyObject* __Pyx_PyObject_CallNoArg(PyObject *func) {
-    PyObject *arg = NULL;
-    return __Pyx_PyObject_FastCall(func, (&arg)+1, 0 | __Pyx_PY_VECTORCALL_ARGUMENTS_OFFSET);
-}
-
-/* PyObjectGetMethod */
-static int __Pyx_PyObject_GetMethod(PyObject *obj, PyObject *name, PyObject **method) {
-    PyObject *attr;
-#if CYTHON_UNPACK_METHODS && CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_PYTYPE_LOOKUP
-    __Pyx_TypeName type_name;
-    PyTypeObject *tp = Py_TYPE(obj);
-    PyObject *descr;
-    descrgetfunc f = NULL;
-    PyObject **dictptr, *dict;
-    int meth_found = 0;
-    assert (*method == NULL);
-    if (unlikely(tp->tp_getattro != PyObject_GenericGetAttr)) {
-        attr = __Pyx_PyObject_GetAttrStr(obj, name);
-        goto try_unpack;
-    }
-    if (unlikely(tp->tp_dict == NULL) && unlikely(PyType_Ready(tp) < 0)) {
-        return 0;
-    }
-    descr = _PyType_Lookup(tp, name);
-    if (likely(descr != NULL)) {
-        Py_INCREF(descr);
-#if defined(Py_TPFLAGS_METHOD_DESCRIPTOR) && Py_TPFLAGS_METHOD_DESCRIPTOR
-        if (__Pyx_PyType_HasFeature(Py_TYPE(descr), Py_TPFLAGS_METHOD_DESCRIPTOR))
-#elif PY_MAJOR_VERSION >= 3
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr) || __Pyx_IS_TYPE(descr, &PyMethodDescr_Type)))
-        #endif
-#else
-        #ifdef __Pyx_CyFunction_USED
-        if (likely(PyFunction_Check(descr) || __Pyx_CyFunction_Check(descr)))
-        #else
-        if (likely(PyFunction_Check(descr)))
-        #endif
-#endif
-        {
-            meth_found = 1;
-        } else {
-            f = Py_TYPE(descr)->tp_descr_get;
-            if (f != NULL && PyDescr_IsData(descr)) {
-                attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-                Py_DECREF(descr);
-                goto try_unpack;
-            }
-        }
-    }
-    dictptr = _PyObject_GetDictPtr(obj);
-    if (dictptr != NULL && (dict = *dictptr) != NULL) {
-        Py_INCREF(dict);
-        attr = __Pyx_PyDict_GetItemStr(dict, name);
-        if (attr != NULL) {
-            Py_INCREF(attr);
-            Py_DECREF(dict);
-            Py_XDECREF(descr);
-            goto try_unpack;
-        }
-        Py_DECREF(dict);
-    }
-    if (meth_found) {
-        *method = descr;
-        return 1;
-    }
-    if (f != NULL) {
-        attr = f(descr, obj, (PyObject *)Py_TYPE(obj));
-        Py_DECREF(descr);
-        goto try_unpack;
-    }
-    if (likely(descr != NULL)) {
-        *method = descr;
-        return 0;
-    }
-    type_name = __Pyx_PyType_GetName(tp);
-    PyErr_Format(PyExc_AttributeError,
-#if PY_MAJOR_VERSION >= 3
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
-                 type_name, name);
-#else
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
-                 type_name, PyString_AS_STRING(name));
-#endif
-    __Pyx_DECREF_TypeName(type_name);
-    return 0;
-#else
-    attr = __Pyx_PyObject_GetAttrStr(obj, name);
-    goto try_unpack;
-#endif
-try_unpack:
-#if CYTHON_UNPACK_METHODS
-    if (likely(attr) && PyMethod_Check(attr) && likely(PyMethod_GET_SELF(attr) == obj)) {
-        PyObject *function = PyMethod_GET_FUNCTION(attr);
-        Py_INCREF(function);
-        Py_DECREF(attr);
-        *method = function;
-        return 1;
-    }
-#endif
-    *method = attr;
-    return 0;
-}
-
-/* PyObjectCallMethod0 */
-static PyObject* __Pyx_PyObject_CallMethod0(PyObject* obj, PyObject* method_name) {
-    PyObject *method = NULL, *result = NULL;
-    int is_method = __Pyx_PyObject_GetMethod(obj, method_name, &method);
-    if (likely(is_method)) {
-        result = __Pyx_PyObject_CallOneArg(method, obj);
-        Py_DECREF(method);
-        return result;
-    }
-    if (unlikely(!method)) goto bad;
-    result = __Pyx_PyObject_CallNoArg(method);
-    Py_DECREF(method);
-bad:
-    return result;
-}
-
-/* ValidateBasesTuple */
-#if CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API || CYTHON_USE_TYPE_SPECS
-static int __Pyx_validate_bases_tuple(const char *type_name, Py_ssize_t dictoffset, PyObject *bases) {
-    Py_ssize_t i, n = PyTuple_GET_SIZE(bases);
-    for (i = 1; i < n; i++)
-    {
-        PyObject *b0 = PyTuple_GET_ITEM(bases, i);
-        PyTypeObject *b;
-#if PY_MAJOR_VERSION < 3
-        if (PyClass_Check(b0))
-        {
-            PyErr_Format(PyExc_TypeError, "base class '%.200s' is an old-style class",
-                         PyString_AS_STRING(((PyClassObject*)b0)->cl_name));
-            return -1;
-        }
-#endif
-        b = (PyTypeObject*) b0;
-        if (!__Pyx_PyType_HasFeature(b, Py_TPFLAGS_HEAPTYPE))
-        {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "base class '" __Pyx_FMT_TYPENAME "' is not a heap type", b_name);
-            __Pyx_DECREF_TypeName(b_name);
-            return -1;
-        }
-        if (dictoffset == 0 && b->tp_dictoffset)
-        {
-            __Pyx_TypeName b_name = __Pyx_PyType_GetName(b);
-            PyErr_Format(PyExc_TypeError,
-                "extension type '%.200s' has no __dict__ slot, "
-                "but base type '" __Pyx_FMT_TYPENAME "' has: "
-                "either add 'cdef dict __dict__' to the extension type "
-                "or add '__slots__ = [...]' to the base type",
-                type_name, b_name);
-            __Pyx_DECREF_TypeName(b_name);
-            return -1;
-        }
-    }
-    return 0;
-}
-#endif
-
-/* PyType_Ready */
-static int __Pyx_PyType_Ready(PyTypeObject *t) {
-#if CYTHON_USE_TYPE_SPECS || !(CYTHON_COMPILING_IN_CPYTHON || CYTHON_COMPILING_IN_LIMITED_API) || defined(PYSTON_MAJOR_VERSION)
-    (void)__Pyx_PyObject_CallMethod0;
-#if CYTHON_USE_TYPE_SPECS
-    (void)__Pyx_validate_bases_tuple;
-#endif
-    return PyType_Ready(t);
-#else
-    int r;
-    PyObject *bases = __Pyx_PyType_GetSlot(t, tp_bases, PyObject*);
-    if (bases && unlikely(__Pyx_validate_bases_tuple(t->tp_name, t->tp_dictoffset, bases) == -1))
-        return -1;
-#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
-    {
-        int gc_was_enabled;
-    #if PY_VERSION_HEX >= 0x030A00b1
-        gc_was_enabled = PyGC_Disable();
-        (void)__Pyx_PyObject_CallMethod0;
-    #else
-        PyObject *ret, *py_status;
-        PyObject *gc = NULL;
-        #if PY_VERSION_HEX >= 0x030700a1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM+0 >= 0x07030400)
-        gc = PyImport_GetModule(__pyx_kp_u_gc);
-        #endif
-        if (unlikely(!gc)) gc = PyImport_Import(__pyx_kp_u_gc);
-        if (unlikely(!gc)) return -1;
-        py_status = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_isenabled);
-        if (unlikely(!py_status)) {
-            Py_DECREF(gc);
-            return -1;
-        }
-        gc_was_enabled = __Pyx_PyObject_IsTrue(py_status);
-        Py_DECREF(py_status);
-        if (gc_was_enabled > 0) {
-            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_disable);
-            if (unlikely(!ret)) {
-                Py_DECREF(gc);
-                return -1;
-            }
-            Py_DECREF(ret);
-        } else if (unlikely(gc_was_enabled == -1)) {
-            Py_DECREF(gc);
-            return -1;
-        }
-    #endif
-        t->tp_flags |= Py_TPFLAGS_HEAPTYPE;
-#if PY_VERSION_HEX >= 0x030A0000
-        t->tp_flags |= Py_TPFLAGS_IMMUTABLETYPE;
-#endif
-#else
-        (void)__Pyx_PyObject_CallMethod0;
-#endif
-    r = PyType_Ready(t);
-#if PY_VERSION_HEX >= 0x03050000 && !defined(PYSTON_MAJOR_VERSION)
-        t->tp_flags &= ~Py_TPFLAGS_HEAPTYPE;
-    #if PY_VERSION_HEX >= 0x030A00b1
-        if (gc_was_enabled)
-            PyGC_Enable();
-    #else
-        if (gc_was_enabled) {
-            PyObject *tp, *v, *tb;
-            PyErr_Fetch(&tp, &v, &tb);
-            ret = __Pyx_PyObject_CallMethod0(gc, __pyx_kp_u_enable);
-            if (likely(ret || r == -1)) {
-                Py_XDECREF(ret);
-                PyErr_Restore(tp, v, tb);
-            } else {
-                Py_XDECREF(tp);
-                Py_XDECREF(v);
-                Py_XDECREF(tb);
-                r = -1;
-            }
-        }
-        Py_DECREF(gc);
-    #endif
-    }
-#endif
-    return r;
-#endif
-}
-
 /* PyObject_GenericGetAttrNoDict */
 #if CYTHON_USE_TYPE_SLOTS && CYTHON_USE_PYTYPE_LOOKUP && PY_VERSION_HEX < 0x03070000
 static PyObject *__Pyx_RaiseGenericGetAttributeError(PyTypeObject *tp, PyObject *attr_name) {
-    __Pyx_TypeName type_name = __Pyx_PyType_GetName(tp);
     PyErr_Format(PyExc_AttributeError,
 #if PY_MAJOR_VERSION >= 3
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%U'",
-                 type_name, attr_name);
+                 "'%.50s' object has no attribute '%U'",
+                 tp->tp_name, attr_name);
 #else
-                 "'" __Pyx_FMT_TYPENAME "' object has no attribute '%.400s'",
-                 type_name, PyString_AS_STRING(attr_name));
+                 "'%.50s' object has no attribute '%.400s'",
+                 tp->tp_name, PyString_AS_STRING(attr_name));
 #endif
-    __Pyx_DECREF_TypeName(type_name);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyObject_GenericGetAttrNoDict(PyObject* obj, PyObject* attr_name) {
     PyObject *descr;
     PyTypeObject *tp = Py_TYPE(obj);
     if (unlikely(!PyString_Check(attr_name))) {
         return PyObject_GenericGetAttr(obj, attr_name);
@@ -6665,110 +4450,58 @@
         return PyObject_GenericGetAttr(obj, attr_name);
     }
     return __Pyx_PyObject_GenericGetAttrNoDict(obj, attr_name);
 }
 #endif
 
 /* SetVTable */
-static int __Pyx_SetVtable(PyTypeObject *type, void *vtable) {
+static int __Pyx_SetVtable(PyObject *dict, void *vtable) {
+#if PY_VERSION_HEX >= 0x02070000
     PyObject *ob = PyCapsule_New(vtable, 0, 0);
-    if (unlikely(!ob))
-        goto bad;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    if (unlikely(PyObject_SetAttr((PyObject *) type, __pyx_n_s_pyx_vtable, ob) < 0))
 #else
-    if (unlikely(PyDict_SetItem(type->tp_dict, __pyx_n_s_pyx_vtable, ob) < 0))
+    PyObject *ob = PyCObject_FromVoidPtr(vtable, 0);
 #endif
+    if (!ob)
+        goto bad;
+    if (PyDict_SetItem(dict, __pyx_n_s_pyx_vtable, ob) < 0)
         goto bad;
     Py_DECREF(ob);
     return 0;
 bad:
     Py_XDECREF(ob);
     return -1;
 }
 
-/* GetVTable */
-static void* __Pyx_GetVtable(PyTypeObject *type) {
-    void* ptr;
-#if CYTHON_COMPILING_IN_LIMITED_API
-    PyObject *ob = PyObject_GetAttr((PyObject *)type, __pyx_n_s_pyx_vtable);
-#else
-    PyObject *ob = PyObject_GetItem(type->tp_dict, __pyx_n_s_pyx_vtable);
-#endif
-    if (!ob)
-        goto bad;
-    ptr = PyCapsule_GetPointer(ob, 0);
-    if (!ptr && !PyErr_Occurred())
-        PyErr_SetString(PyExc_RuntimeError, "invalid vtable found for imported type");
-    Py_DECREF(ob);
-    return ptr;
-bad:
-    Py_XDECREF(ob);
-    return NULL;
+/* PyObjectGetAttrStrNoError */
+static void __Pyx_PyObject_GetAttrStr_ClearAttributeError(void) {
+    __Pyx_PyThreadState_declare
+    __Pyx_PyThreadState_assign
+    if (likely(__Pyx_PyErr_ExceptionMatches(PyExc_AttributeError)))
+        __Pyx_PyErr_Clear();
 }
-
-/* MergeVTables */
-#if !CYTHON_COMPILING_IN_LIMITED_API
-static int __Pyx_MergeVtables(PyTypeObject *type) {
-    int i;
-    void** base_vtables;
-    __Pyx_TypeName tp_base_name;
-    __Pyx_TypeName base_name;
-    void* unknown = (void*)-1;
-    PyObject* bases = type->tp_bases;
-    int base_depth = 0;
-    {
-        PyTypeObject* base = type->tp_base;
-        while (base) {
-            base_depth += 1;
-            base = base->tp_base;
-        }
-    }
-    base_vtables = (void**) malloc(sizeof(void*) * (size_t)(base_depth + 1));
-    base_vtables[0] = unknown;
-    for (i = 1; i < PyTuple_GET_SIZE(bases); i++) {
-        void* base_vtable = __Pyx_GetVtable(((PyTypeObject*)PyTuple_GET_ITEM(bases, i)));
-        if (base_vtable != NULL) {
-            int j;
-            PyTypeObject* base = type->tp_base;
-            for (j = 0; j < base_depth; j++) {
-                if (base_vtables[j] == unknown) {
-                    base_vtables[j] = __Pyx_GetVtable(base);
-                    base_vtables[j + 1] = unknown;
-                }
-                if (base_vtables[j] == base_vtable) {
-                    break;
-                } else if (base_vtables[j] == NULL) {
-                    goto bad;
-                }
-                base = base->tp_base;
-            }
-        }
+static CYTHON_INLINE PyObject* __Pyx_PyObject_GetAttrStrNoError(PyObject* obj, PyObject* attr_name) {
+    PyObject *result;
+#if CYTHON_COMPILING_IN_CPYTHON && CYTHON_USE_TYPE_SLOTS && PY_VERSION_HEX >= 0x030700B1
+    PyTypeObject* tp = Py_TYPE(obj);
+    if (likely(tp->tp_getattro == PyObject_GenericGetAttr)) {
+        return _PyObject_GenericGetAttrWithDict(obj, attr_name, NULL, 1);
     }
-    PyErr_Clear();
-    free(base_vtables);
-    return 0;
-bad:
-    tp_base_name = __Pyx_PyType_GetName(type->tp_base);
-    base_name = __Pyx_PyType_GetName((PyTypeObject*)PyTuple_GET_ITEM(bases, i));
-    PyErr_Format(PyExc_TypeError,
-        "multiple bases have vtable conflict: '" __Pyx_FMT_TYPENAME "' and '" __Pyx_FMT_TYPENAME "'", tp_base_name, base_name);
-    __Pyx_DECREF_TypeName(tp_base_name);
-    __Pyx_DECREF_TypeName(base_name);
-    free(base_vtables);
-    return -1;
-}
 #endif
+    result = __Pyx_PyObject_GetAttrStr(obj, attr_name);
+    if (unlikely(!result)) {
+        __Pyx_PyObject_GetAttrStr_ClearAttributeError();
+    }
+    return result;
+}
 
 /* SetupReduce */
-#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce_is_named(PyObject* meth, PyObject* name) {
   int ret;
   PyObject *name_attr;
-  name_attr = __Pyx_PyObject_GetAttrStrNoError(meth, __pyx_n_s_name);
+  name_attr = __Pyx_PyObject_GetAttrStr(meth, __pyx_n_s_name);
   if (likely(name_attr)) {
       ret = PyObject_RichCompareBool(name_attr, name, Py_EQ);
   } else {
       ret = -1;
   }
   if (unlikely(ret < 0)) {
       PyErr_Clear();
@@ -6776,43 +4509,25 @@
   }
   Py_XDECREF(name_attr);
   return ret;
 }
 static int __Pyx_setup_reduce(PyObject* type_obj) {
     int ret = 0;
     PyObject *object_reduce = NULL;
-    PyObject *object_getstate = NULL;
     PyObject *object_reduce_ex = NULL;
     PyObject *reduce = NULL;
     PyObject *reduce_ex = NULL;
     PyObject *reduce_cython = NULL;
     PyObject *setstate = NULL;
     PyObject *setstate_cython = NULL;
-    PyObject *getstate = NULL;
-#if CYTHON_USE_PYTYPE_LOOKUP
-    getstate = _PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate);
-#else
-    getstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_getstate);
-    if (!getstate && PyErr_Occurred()) {
-        goto __PYX_BAD;
-    }
-#endif
-    if (getstate) {
 #if CYTHON_USE_PYTYPE_LOOKUP
-        object_getstate = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_getstate);
+    if (_PyType_Lookup((PyTypeObject*)type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
 #else
-        object_getstate = __Pyx_PyObject_GetAttrStrNoError((PyObject*)&PyBaseObject_Type, __pyx_n_s_getstate);
-        if (!object_getstate && PyErr_Occurred()) {
-            goto __PYX_BAD;
-        }
+    if (PyObject_HasAttr(type_obj, __pyx_n_s_getstate)) goto __PYX_GOOD;
 #endif
-        if (object_getstate != getstate) {
-            goto __PYX_GOOD;
-        }
-    }
 #if CYTHON_USE_PYTYPE_LOOKUP
     object_reduce_ex = _PyType_Lookup(&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #else
     object_reduce_ex = __Pyx_PyObject_GetAttrStr((PyObject*)&PyBaseObject_Type, __pyx_n_s_reduce_ex); if (!object_reduce_ex) goto __PYX_BAD;
 #endif
     reduce_ex = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_reduce_ex); if (unlikely(!reduce_ex)) goto __PYX_BAD;
     if (reduce_ex == object_reduce_ex) {
@@ -6826,15 +4541,15 @@
             reduce_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_reduce_cython);
             if (likely(reduce_cython)) {
                 ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce, reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                 ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_reduce_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
             } else if (reduce == object_reduce || PyErr_Occurred()) {
                 goto __PYX_BAD;
             }
-            setstate = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate);
+            setstate = __Pyx_PyObject_GetAttrStr(type_obj, __pyx_n_s_setstate);
             if (!setstate) PyErr_Clear();
             if (!setstate || __Pyx_setup_reduce_is_named(setstate, __pyx_n_s_setstate_cython)) {
                 setstate_cython = __Pyx_PyObject_GetAttrStrNoError(type_obj, __pyx_n_s_setstate_cython);
                 if (likely(setstate_cython)) {
                     ret = PyDict_SetItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate, setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                     ret = PyDict_DelItem(((PyTypeObject*)type_obj)->tp_dict, __pyx_n_s_setstate_cython); if (unlikely(ret < 0)) goto __PYX_BAD;
                 } else if (!setstate || PyErr_Occurred()) {
@@ -6842,1132 +4557,73 @@
                 }
             }
             PyType_Modified((PyTypeObject*)type_obj);
         }
     }
     goto __PYX_GOOD;
 __PYX_BAD:
-    if (!PyErr_Occurred()) {
-        __Pyx_TypeName type_obj_name =
-            __Pyx_PyType_GetName((PyTypeObject*)type_obj);
-        PyErr_Format(PyExc_RuntimeError,
-            "Unable to initialize pickling for " __Pyx_FMT_TYPENAME, type_obj_name);
-        __Pyx_DECREF_TypeName(type_obj_name);
-    }
+    if (!PyErr_Occurred())
+        PyErr_Format(PyExc_RuntimeError, "Unable to initialize pickling for %s", ((PyTypeObject*)type_obj)->tp_name);
     ret = -1;
 __PYX_GOOD:
 #if !CYTHON_USE_PYTYPE_LOOKUP
     Py_XDECREF(object_reduce);
     Py_XDECREF(object_reduce_ex);
-    Py_XDECREF(object_getstate);
-    Py_XDECREF(getstate);
 #endif
     Py_XDECREF(reduce);
     Py_XDECREF(reduce_ex);
     Py_XDECREF(reduce_cython);
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
-#endif
-
-/* FetchSharedCythonModule */
-static PyObject *__Pyx_FetchSharedCythonABIModule(void) {
-    PyObject *abi_module = PyImport_AddModule((char*) __PYX_ABI_MODULE_NAME);
-    if (unlikely(!abi_module)) return NULL;
-    Py_INCREF(abi_module);
-    return abi_module;
-}
-
-/* FetchCommonType */
-static int __Pyx_VerifyCachedType(PyObject *cached_type,
-                               const char *name,
-                               Py_ssize_t basicsize,
-                               Py_ssize_t expected_basicsize) {
-    if (!PyType_Check(cached_type)) {
-        PyErr_Format(PyExc_TypeError,
-            "Shared Cython type %.200s is not a type object", name);
-        return -1;
-    }
-    if (basicsize != expected_basicsize) {
-        PyErr_Format(PyExc_TypeError,
-            "Shared Cython type %.200s has the wrong size, try recompiling",
-            name);
-        return -1;
-    }
-    return 0;
-}
-#if !CYTHON_USE_TYPE_SPECS
-static PyTypeObject* __Pyx_FetchCommonType(PyTypeObject* type) {
-    PyObject* abi_module;
-    const char* object_name;
-    PyTypeObject *cached_type = NULL;
-    abi_module = __Pyx_FetchSharedCythonABIModule();
-    if (!abi_module) return NULL;
-    object_name = strrchr(type->tp_name, '.');
-    object_name = object_name ? object_name+1 : type->tp_name;
-    cached_type = (PyTypeObject*) PyObject_GetAttrString(abi_module, object_name);
-    if (cached_type) {
-        if (__Pyx_VerifyCachedType(
-              (PyObject *)cached_type,
-              object_name,
-              cached_type->tp_basicsize,
-              type->tp_basicsize) < 0) {
-            goto bad;
-        }
-        goto done;
-    }
-    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
-    PyErr_Clear();
-    if (PyType_Ready(type) < 0) goto bad;
-    if (PyObject_SetAttrString(abi_module, object_name, (PyObject *)type) < 0)
-        goto bad;
-    Py_INCREF(type);
-    cached_type = type;
-done:
-    Py_DECREF(abi_module);
-    return cached_type;
-bad:
-    Py_XDECREF(cached_type);
-    cached_type = NULL;
-    goto done;
-}
-#else
-static PyTypeObject *__Pyx_FetchCommonTypeFromSpec(PyObject *module, PyType_Spec *spec, PyObject *bases) {
-    PyObject *abi_module, *cached_type = NULL;
-    const char* object_name = strrchr(spec->name, '.');
-    object_name = object_name ? object_name+1 : spec->name;
-    abi_module = __Pyx_FetchSharedCythonABIModule();
-    if (!abi_module) return NULL;
-    cached_type = PyObject_GetAttrString(abi_module, object_name);
-    if (cached_type) {
-        Py_ssize_t basicsize;
-#if CYTHON_COMPILING_IN_LIMITED_API
-        PyObject *py_basicsize;
-        py_basicsize = PyObject_GetAttrString(cached_type, "__basicsize__");
-        if (unlikely(!py_basicsize)) goto bad;
-        basicsize = PyLong_AsSsize_t(py_basicsize);
-        Py_DECREF(py_basicsize);
-        py_basicsize = 0;
-        if (unlikely(basicsize == (Py_ssize_t)-1) && PyErr_Occurred()) goto bad;
-#else
-        basicsize = likely(PyType_Check(cached_type)) ? ((PyTypeObject*) cached_type)->tp_basicsize : -1;
-#endif
-        if (__Pyx_VerifyCachedType(
-              cached_type,
-              object_name,
-              basicsize,
-              spec->basicsize) < 0) {
-            goto bad;
-        }
-        goto done;
-    }
-    if (!PyErr_ExceptionMatches(PyExc_AttributeError)) goto bad;
-    PyErr_Clear();
-    CYTHON_UNUSED_VAR(module);
-    cached_type = __Pyx_PyType_FromModuleAndSpec(abi_module, spec, bases);
-    if (unlikely(!cached_type)) goto bad;
-    if (unlikely(__Pyx_fix_up_extension_type_from_spec(spec, (PyTypeObject *) cached_type) < 0)) goto bad;
-    if (PyObject_SetAttrString(abi_module, object_name, cached_type) < 0) goto bad;
-done:
-    Py_DECREF(abi_module);
-    assert(cached_type == NULL || PyType_Check(cached_type));
-    return (PyTypeObject *) cached_type;
-bad:
-    Py_XDECREF(cached_type);
-    cached_type = NULL;
-    goto done;
-}
-#endif
-
-/* PyVectorcallFastCallDict */
-#if CYTHON_METH_FASTCALL
-static PyObject *__Pyx_PyVectorcall_FastCallDict_kw(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
-{
-    PyObject *res = NULL;
-    PyObject *kwnames;
-    PyObject **newargs;
-    PyObject **kwvalues;
-    Py_ssize_t i, pos;
-    size_t j;
-    PyObject *key, *value;
-    unsigned long keys_are_strings;
-    Py_ssize_t nkw = PyDict_GET_SIZE(kw);
-    newargs = (PyObject **)PyMem_Malloc((nargs + (size_t)nkw) * sizeof(args[0]));
-    if (unlikely(newargs == NULL)) {
-        PyErr_NoMemory();
-        return NULL;
-    }
-    for (j = 0; j < nargs; j++) newargs[j] = args[j];
-    kwnames = PyTuple_New(nkw);
-    if (unlikely(kwnames == NULL)) {
-        PyMem_Free(newargs);
-        return NULL;
-    }
-    kwvalues = newargs + nargs;
-    pos = i = 0;
-    keys_are_strings = Py_TPFLAGS_UNICODE_SUBCLASS;
-    while (PyDict_Next(kw, &pos, &key, &value)) {
-        keys_are_strings &= Py_TYPE(key)->tp_flags;
-        Py_INCREF(key);
-        Py_INCREF(value);
-        PyTuple_SET_ITEM(kwnames, i, key);
-        kwvalues[i] = value;
-        i++;
-    }
-    if (unlikely(!keys_are_strings)) {
-        PyErr_SetString(PyExc_TypeError, "keywords must be strings");
-        goto cleanup;
-    }
-    res = vc(func, newargs, nargs, kwnames);
-cleanup:
-    Py_DECREF(kwnames);
-    for (i = 0; i < nkw; i++)
-        Py_DECREF(kwvalues[i]);
-    PyMem_Free(newargs);
-    return res;
-}
-static CYTHON_INLINE PyObject *__Pyx_PyVectorcall_FastCallDict(PyObject *func, __pyx_vectorcallfunc vc, PyObject *const *args, size_t nargs, PyObject *kw)
-{
-    if (likely(kw == NULL) || PyDict_GET_SIZE(kw) == 0) {
-        return vc(func, args, nargs, NULL);
-    }
-    return __Pyx_PyVectorcall_FastCallDict_kw(func, vc, args, nargs, kw);
-}
-#endif
-
-/* CythonFunctionShared */
-static CYTHON_INLINE void __Pyx__CyFunction_SetClassObj(__pyx_CyFunctionObject* f, PyObject* classobj) {
-#if PY_VERSION_HEX < 0x030900B1
-    __Pyx_Py_XDECREF_SET(
-        __Pyx_CyFunction_GetClassObj(f),
-            ((classobj) ? __Pyx_NewRef(classobj) : NULL));
-#else
-    __Pyx_Py_XDECREF_SET(
-        ((PyCMethodObject *) (f))->mm_class,
-        (PyTypeObject*)((classobj) ? __Pyx_NewRef(classobj) : NULL));
-#endif
-}
-static PyObject *
-__Pyx_CyFunction_get_doc(__pyx_CyFunctionObject *op, void *closure)
-{
-    CYTHON_UNUSED_VAR(closure);
-    if (unlikely(op->func_doc == NULL)) {
-        if (((PyCFunctionObject*)op)->m_ml->ml_doc) {
-#if PY_MAJOR_VERSION >= 3
-            op->func_doc = PyUnicode_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
-#else
-            op->func_doc = PyString_FromString(((PyCFunctionObject*)op)->m_ml->ml_doc);
-#endif
-            if (unlikely(op->func_doc == NULL))
-                return NULL;
-        } else {
-            Py_INCREF(Py_None);
-            return Py_None;
-        }
-    }
-    Py_INCREF(op->func_doc);
-    return op->func_doc;
-}
-static int
-__Pyx_CyFunction_set_doc(__pyx_CyFunctionObject *op, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    if (value == NULL) {
-        value = Py_None;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_doc, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_name(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(op->func_name == NULL)) {
-#if PY_MAJOR_VERSION >= 3
-        op->func_name = PyUnicode_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
-#else
-        op->func_name = PyString_InternFromString(((PyCFunctionObject*)op)->m_ml->ml_name);
-#endif
-        if (unlikely(op->func_name == NULL))
-            return NULL;
-    }
-    Py_INCREF(op->func_name);
-    return op->func_name;
-}
-static int
-__Pyx_CyFunction_set_name(__pyx_CyFunctionObject *op, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-#if PY_MAJOR_VERSION >= 3
-    if (unlikely(value == NULL || !PyUnicode_Check(value)))
-#else
-    if (unlikely(value == NULL || !PyString_Check(value)))
-#endif
-    {
-        PyErr_SetString(PyExc_TypeError,
-                        "__name__ must be set to a string object");
-        return -1;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_name, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_qualname(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    Py_INCREF(op->func_qualname);
-    return op->func_qualname;
-}
-static int
-__Pyx_CyFunction_set_qualname(__pyx_CyFunctionObject *op, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-#if PY_MAJOR_VERSION >= 3
-    if (unlikely(value == NULL || !PyUnicode_Check(value)))
-#else
-    if (unlikely(value == NULL || !PyString_Check(value)))
-#endif
-    {
-        PyErr_SetString(PyExc_TypeError,
-                        "__qualname__ must be set to a string object");
-        return -1;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_qualname, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_dict(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(op->func_dict == NULL)) {
-        op->func_dict = PyDict_New();
-        if (unlikely(op->func_dict == NULL))
-            return NULL;
-    }
-    Py_INCREF(op->func_dict);
-    return op->func_dict;
-}
-static int
-__Pyx_CyFunction_set_dict(__pyx_CyFunctionObject *op, PyObject *value, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(value == NULL)) {
-        PyErr_SetString(PyExc_TypeError,
-               "function's dictionary may not be deleted");
-        return -1;
-    }
-    if (unlikely(!PyDict_Check(value))) {
-        PyErr_SetString(PyExc_TypeError,
-               "setting function's dictionary to a non-dict");
-        return -1;
-    }
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_dict, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_globals(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(context);
-    Py_INCREF(op->func_globals);
-    return op->func_globals;
-}
-static PyObject *
-__Pyx_CyFunction_get_closure(__pyx_CyFunctionObject *op, void *context)
-{
-    CYTHON_UNUSED_VAR(op);
-    CYTHON_UNUSED_VAR(context);
-    Py_INCREF(Py_None);
-    return Py_None;
-}
-static PyObject *
-__Pyx_CyFunction_get_code(__pyx_CyFunctionObject *op, void *context)
-{
-    PyObject* result = (op->func_code) ? op->func_code : Py_None;
-    CYTHON_UNUSED_VAR(context);
-    Py_INCREF(result);
-    return result;
-}
-static int
-__Pyx_CyFunction_init_defaults(__pyx_CyFunctionObject *op) {
-    int result = 0;
-    PyObject *res = op->defaults_getter((PyObject *) op);
-    if (unlikely(!res))
-        return -1;
-    #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-    op->defaults_tuple = PyTuple_GET_ITEM(res, 0);
-    Py_INCREF(op->defaults_tuple);
-    op->defaults_kwdict = PyTuple_GET_ITEM(res, 1);
-    Py_INCREF(op->defaults_kwdict);
-    #else
-    op->defaults_tuple = PySequence_ITEM(res, 0);
-    if (unlikely(!op->defaults_tuple)) result = -1;
-    else {
-        op->defaults_kwdict = PySequence_ITEM(res, 1);
-        if (unlikely(!op->defaults_kwdict)) result = -1;
-    }
-    #endif
-    Py_DECREF(res);
-    return result;
-}
-static int
-__Pyx_CyFunction_set_defaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
-    CYTHON_UNUSED_VAR(context);
-    if (!value) {
-        value = Py_None;
-    } else if (unlikely(value != Py_None && !PyTuple_Check(value))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "__defaults__ must be set to a tuple object");
-        return -1;
-    }
-    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__defaults__ will not "
-                 "currently affect the values used in function calls", 1);
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->defaults_tuple, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_defaults(__pyx_CyFunctionObject *op, void *context) {
-    PyObject* result = op->defaults_tuple;
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(!result)) {
-        if (op->defaults_getter) {
-            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
-            result = op->defaults_tuple;
-        } else {
-            result = Py_None;
-        }
-    }
-    Py_INCREF(result);
-    return result;
-}
-static int
-__Pyx_CyFunction_set_kwdefaults(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
-    CYTHON_UNUSED_VAR(context);
-    if (!value) {
-        value = Py_None;
-    } else if (unlikely(value != Py_None && !PyDict_Check(value))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "__kwdefaults__ must be set to a dict object");
-        return -1;
-    }
-    PyErr_WarnEx(PyExc_RuntimeWarning, "changes to cyfunction.__kwdefaults__ will not "
-                 "currently affect the values used in function calls", 1);
-    Py_INCREF(value);
-    __Pyx_Py_XDECREF_SET(op->defaults_kwdict, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_kwdefaults(__pyx_CyFunctionObject *op, void *context) {
-    PyObject* result = op->defaults_kwdict;
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(!result)) {
-        if (op->defaults_getter) {
-            if (unlikely(__Pyx_CyFunction_init_defaults(op) < 0)) return NULL;
-            result = op->defaults_kwdict;
-        } else {
-            result = Py_None;
-        }
-    }
-    Py_INCREF(result);
-    return result;
-}
-static int
-__Pyx_CyFunction_set_annotations(__pyx_CyFunctionObject *op, PyObject* value, void *context) {
-    CYTHON_UNUSED_VAR(context);
-    if (!value || value == Py_None) {
-        value = NULL;
-    } else if (unlikely(!PyDict_Check(value))) {
-        PyErr_SetString(PyExc_TypeError,
-                        "__annotations__ must be set to a dict object");
-        return -1;
-    }
-    Py_XINCREF(value);
-    __Pyx_Py_XDECREF_SET(op->func_annotations, value);
-    return 0;
-}
-static PyObject *
-__Pyx_CyFunction_get_annotations(__pyx_CyFunctionObject *op, void *context) {
-    PyObject* result = op->func_annotations;
-    CYTHON_UNUSED_VAR(context);
-    if (unlikely(!result)) {
-        result = PyDict_New();
-        if (unlikely(!result)) return NULL;
-        op->func_annotations = result;
-    }
-    Py_INCREF(result);
-    return result;
-}
-static PyObject *
-__Pyx_CyFunction_get_is_coroutine(__pyx_CyFunctionObject *op, void *context) {
-    int is_coroutine;
-    CYTHON_UNUSED_VAR(context);
-    if (op->func_is_coroutine) {
-        return __Pyx_NewRef(op->func_is_coroutine);
-    }
-    is_coroutine = op->flags & __Pyx_CYFUNCTION_COROUTINE;
-#if PY_VERSION_HEX >= 0x03050000
-    if (is_coroutine) {
-        PyObject *module, *fromlist, *marker = __pyx_n_s_is_coroutine;
-        fromlist = PyList_New(1);
-        if (unlikely(!fromlist)) return NULL;
-        Py_INCREF(marker);
-        PyList_SET_ITEM(fromlist, 0, marker);
-        module = PyImport_ImportModuleLevelObject(__pyx_n_s_asyncio_coroutines, NULL, NULL, fromlist, 0);
-        Py_DECREF(fromlist);
-        if (unlikely(!module)) goto ignore;
-        op->func_is_coroutine = __Pyx_PyObject_GetAttrStr(module, marker);
-        Py_DECREF(module);
-        if (likely(op->func_is_coroutine)) {
-            return __Pyx_NewRef(op->func_is_coroutine);
-        }
-ignore:
-        PyErr_Clear();
-    }
-#endif
-    op->func_is_coroutine = __Pyx_PyBool_FromLong(is_coroutine);
-    return __Pyx_NewRef(op->func_is_coroutine);
-}
-static PyGetSetDef __pyx_CyFunction_getsets[] = {
-    {(char *) "func_doc", (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
-    {(char *) "__doc__",  (getter)__Pyx_CyFunction_get_doc, (setter)__Pyx_CyFunction_set_doc, 0, 0},
-    {(char *) "func_name", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
-    {(char *) "__name__", (getter)__Pyx_CyFunction_get_name, (setter)__Pyx_CyFunction_set_name, 0, 0},
-    {(char *) "__qualname__", (getter)__Pyx_CyFunction_get_qualname, (setter)__Pyx_CyFunction_set_qualname, 0, 0},
-    {(char *) "func_dict", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
-    {(char *) "__dict__", (getter)__Pyx_CyFunction_get_dict, (setter)__Pyx_CyFunction_set_dict, 0, 0},
-    {(char *) "func_globals", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
-    {(char *) "__globals__", (getter)__Pyx_CyFunction_get_globals, 0, 0, 0},
-    {(char *) "func_closure", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
-    {(char *) "__closure__", (getter)__Pyx_CyFunction_get_closure, 0, 0, 0},
-    {(char *) "func_code", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
-    {(char *) "__code__", (getter)__Pyx_CyFunction_get_code, 0, 0, 0},
-    {(char *) "func_defaults", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
-    {(char *) "__defaults__", (getter)__Pyx_CyFunction_get_defaults, (setter)__Pyx_CyFunction_set_defaults, 0, 0},
-    {(char *) "__kwdefaults__", (getter)__Pyx_CyFunction_get_kwdefaults, (setter)__Pyx_CyFunction_set_kwdefaults, 0, 0},
-    {(char *) "__annotations__", (getter)__Pyx_CyFunction_get_annotations, (setter)__Pyx_CyFunction_set_annotations, 0, 0},
-    {(char *) "_is_coroutine", (getter)__Pyx_CyFunction_get_is_coroutine, 0, 0, 0},
-    {0, 0, 0, 0, 0}
-};
-static PyMemberDef __pyx_CyFunction_members[] = {
-    {(char *) "__module__", T_OBJECT, offsetof(PyCFunctionObject, m_module), 0, 0},
-#if CYTHON_USE_TYPE_SPECS
-    {(char *) "__dictoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_dict), READONLY, 0},
-#if CYTHON_METH_FASTCALL
-#if CYTHON_BACKPORT_VECTORCALL
-    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_vectorcall), READONLY, 0},
-#else
-    {(char *) "__vectorcalloffset__", T_PYSSIZET, offsetof(PyCFunctionObject, vectorcall), READONLY, 0},
-#endif
-#endif
-#if PY_VERSION_HEX < 0x030500A0
-    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(__pyx_CyFunctionObject, func_weakreflist), READONLY, 0},
-#else
-    {(char *) "__weaklistoffset__", T_PYSSIZET, offsetof(PyCFunctionObject, m_weakreflist), READONLY, 0},
-#endif
-#endif
-    {0, 0, 0,  0, 0}
-};
-static PyObject *
-__Pyx_CyFunction_reduce(__pyx_CyFunctionObject *m, PyObject *args)
-{
-    CYTHON_UNUSED_VAR(args);
-#if PY_MAJOR_VERSION >= 3
-    Py_INCREF(m->func_qualname);
-    return m->func_qualname;
-#else
-    return PyString_FromString(((PyCFunctionObject*)m)->m_ml->ml_name);
-#endif
-}
-static PyMethodDef __pyx_CyFunction_methods[] = {
-    {"__reduce__", (PyCFunction)__Pyx_CyFunction_reduce, METH_VARARGS, 0},
-    {0, 0, 0, 0}
-};
-#if PY_VERSION_HEX < 0x030500A0
-#define __Pyx_CyFunction_weakreflist(cyfunc) ((cyfunc)->func_weakreflist)
-#else
-#define __Pyx_CyFunction_weakreflist(cyfunc) (((PyCFunctionObject*)cyfunc)->m_weakreflist)
-#endif
-static PyObject *__Pyx_CyFunction_Init(__pyx_CyFunctionObject *op, PyMethodDef *ml, int flags, PyObject* qualname,
-                                       PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-    PyCFunctionObject *cf = (PyCFunctionObject*) op;
-    if (unlikely(op == NULL))
-        return NULL;
-    op->flags = flags;
-    __Pyx_CyFunction_weakreflist(op) = NULL;
-    cf->m_ml = ml;
-    cf->m_self = (PyObject *) op;
-    Py_XINCREF(closure);
-    op->func_closure = closure;
-    Py_XINCREF(module);
-    cf->m_module = module;
-    op->func_dict = NULL;
-    op->func_name = NULL;
-    Py_INCREF(qualname);
-    op->func_qualname = qualname;
-    op->func_doc = NULL;
-#if PY_VERSION_HEX < 0x030900B1
-    op->func_classobj = NULL;
-#else
-    ((PyCMethodObject*)op)->mm_class = NULL;
-#endif
-    op->func_globals = globals;
-    Py_INCREF(op->func_globals);
-    Py_XINCREF(code);
-    op->func_code = code;
-    op->defaults_pyobjects = 0;
-    op->defaults_size = 0;
-    op->defaults = NULL;
-    op->defaults_tuple = NULL;
-    op->defaults_kwdict = NULL;
-    op->defaults_getter = NULL;
-    op->func_annotations = NULL;
-    op->func_is_coroutine = NULL;
-#if CYTHON_METH_FASTCALL
-    switch (ml->ml_flags & (METH_VARARGS | METH_FASTCALL | METH_NOARGS | METH_O | METH_KEYWORDS | METH_METHOD)) {
-    case METH_NOARGS:
-        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_NOARGS;
-        break;
-    case METH_O:
-        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_O;
-        break;
-    case METH_METHOD | METH_FASTCALL | METH_KEYWORDS:
-        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD;
-        break;
-    case METH_FASTCALL | METH_KEYWORDS:
-        __Pyx_CyFunction_func_vectorcall(op) = __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS;
-        break;
-    case METH_VARARGS | METH_KEYWORDS:
-        __Pyx_CyFunction_func_vectorcall(op) = NULL;
-        break;
-    default:
-        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
-        Py_DECREF(op);
-        return NULL;
-    }
-#endif
-    return (PyObject *) op;
-}
-static int
-__Pyx_CyFunction_clear(__pyx_CyFunctionObject *m)
-{
-    Py_CLEAR(m->func_closure);
-    Py_CLEAR(((PyCFunctionObject*)m)->m_module);
-    Py_CLEAR(m->func_dict);
-    Py_CLEAR(m->func_name);
-    Py_CLEAR(m->func_qualname);
-    Py_CLEAR(m->func_doc);
-    Py_CLEAR(m->func_globals);
-    Py_CLEAR(m->func_code);
-#if PY_VERSION_HEX < 0x030900B1
-    Py_CLEAR(__Pyx_CyFunction_GetClassObj(m));
-#else
-    {
-        PyObject *cls = (PyObject*) ((PyCMethodObject *) (m))->mm_class;
-        ((PyCMethodObject *) (m))->mm_class = NULL;
-        Py_XDECREF(cls);
-    }
-#endif
-    Py_CLEAR(m->defaults_tuple);
-    Py_CLEAR(m->defaults_kwdict);
-    Py_CLEAR(m->func_annotations);
-    Py_CLEAR(m->func_is_coroutine);
-    if (m->defaults) {
-        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
-        int i;
-        for (i = 0; i < m->defaults_pyobjects; i++)
-            Py_XDECREF(pydefaults[i]);
-        PyObject_Free(m->defaults);
-        m->defaults = NULL;
-    }
-    return 0;
-}
-static void __Pyx__CyFunction_dealloc(__pyx_CyFunctionObject *m)
-{
-    if (__Pyx_CyFunction_weakreflist(m) != NULL)
-        PyObject_ClearWeakRefs((PyObject *) m);
-    __Pyx_CyFunction_clear(m);
-    __Pyx_PyHeapTypeObject_GC_Del(m);
-}
-static void __Pyx_CyFunction_dealloc(__pyx_CyFunctionObject *m)
-{
-    PyObject_GC_UnTrack(m);
-    __Pyx__CyFunction_dealloc(m);
-}
-static int __Pyx_CyFunction_traverse(__pyx_CyFunctionObject *m, visitproc visit, void *arg)
-{
-    Py_VISIT(m->func_closure);
-    Py_VISIT(((PyCFunctionObject*)m)->m_module);
-    Py_VISIT(m->func_dict);
-    Py_VISIT(m->func_name);
-    Py_VISIT(m->func_qualname);
-    Py_VISIT(m->func_doc);
-    Py_VISIT(m->func_globals);
-    Py_VISIT(m->func_code);
-    Py_VISIT(__Pyx_CyFunction_GetClassObj(m));
-    Py_VISIT(m->defaults_tuple);
-    Py_VISIT(m->defaults_kwdict);
-    Py_VISIT(m->func_is_coroutine);
-    if (m->defaults) {
-        PyObject **pydefaults = __Pyx_CyFunction_Defaults(PyObject *, m);
-        int i;
-        for (i = 0; i < m->defaults_pyobjects; i++)
-            Py_VISIT(pydefaults[i]);
-    }
-    return 0;
-}
-static PyObject*
-__Pyx_CyFunction_repr(__pyx_CyFunctionObject *op)
-{
-#if PY_MAJOR_VERSION >= 3
-    return PyUnicode_FromFormat("<cyfunction %U at %p>",
-                                op->func_qualname, (void *)op);
-#else
-    return PyString_FromFormat("<cyfunction %s at %p>",
-                               PyString_AsString(op->func_qualname), (void *)op);
-#endif
-}
-static PyObject * __Pyx_CyFunction_CallMethod(PyObject *func, PyObject *self, PyObject *arg, PyObject *kw) {
-    PyCFunctionObject* f = (PyCFunctionObject*)func;
-    PyCFunction meth = f->m_ml->ml_meth;
-    Py_ssize_t size;
-    switch (f->m_ml->ml_flags & (METH_VARARGS | METH_KEYWORDS | METH_NOARGS | METH_O)) {
-    case METH_VARARGS:
-        if (likely(kw == NULL || PyDict_Size(kw) == 0))
-            return (*meth)(self, arg);
-        break;
-    case METH_VARARGS | METH_KEYWORDS:
-        return (*(PyCFunctionWithKeywords)(void*)meth)(self, arg, kw);
-    case METH_NOARGS:
-        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
-            size = PyTuple_GET_SIZE(arg);
-            if (likely(size == 0))
-                return (*meth)(self, NULL);
-            PyErr_Format(PyExc_TypeError,
-                "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                f->m_ml->ml_name, size);
-            return NULL;
-        }
-        break;
-    case METH_O:
-        if (likely(kw == NULL || PyDict_Size(kw) == 0)) {
-            size = PyTuple_GET_SIZE(arg);
-            if (likely(size == 1)) {
-                PyObject *result, *arg0;
-                #if CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS
-                arg0 = PyTuple_GET_ITEM(arg, 0);
-                #else
-                arg0 = PySequence_ITEM(arg, 0); if (unlikely(!arg0)) return NULL;
-                #endif
-                result = (*meth)(self, arg0);
-                #if !(CYTHON_ASSUME_SAFE_MACROS && !CYTHON_AVOID_BORROWED_REFS)
-                Py_DECREF(arg0);
-                #endif
-                return result;
-            }
-            PyErr_Format(PyExc_TypeError,
-                "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
-                f->m_ml->ml_name, size);
-            return NULL;
-        }
-        break;
-    default:
-        PyErr_SetString(PyExc_SystemError, "Bad call flags for CyFunction");
-        return NULL;
-    }
-    PyErr_Format(PyExc_TypeError, "%.200s() takes no keyword arguments",
-                 f->m_ml->ml_name);
-    return NULL;
-}
-static CYTHON_INLINE PyObject *__Pyx_CyFunction_Call(PyObject *func, PyObject *arg, PyObject *kw) {
-    return __Pyx_CyFunction_CallMethod(func, ((PyCFunctionObject*)func)->m_self, arg, kw);
-}
-static PyObject *__Pyx_CyFunction_CallAsMethod(PyObject *func, PyObject *args, PyObject *kw) {
-    PyObject *result;
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *) func;
-#if CYTHON_METH_FASTCALL
-     __pyx_vectorcallfunc vc = __Pyx_CyFunction_func_vectorcall(cyfunc);
-    if (vc) {
-#if CYTHON_ASSUME_SAFE_MACROS
-        return __Pyx_PyVectorcall_FastCallDict(func, vc, &PyTuple_GET_ITEM(args, 0), (size_t)PyTuple_GET_SIZE(args), kw);
-#else
-        (void) &__Pyx_PyVectorcall_FastCallDict;
-        return PyVectorcall_Call(func, args, kw);
-#endif
-    }
-#endif
-    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
-        Py_ssize_t argc;
-        PyObject *new_args;
-        PyObject *self;
-        argc = PyTuple_GET_SIZE(args);
-        new_args = PyTuple_GetSlice(args, 1, argc);
-        if (unlikely(!new_args))
-            return NULL;
-        self = PyTuple_GetItem(args, 0);
-        if (unlikely(!self)) {
-            Py_DECREF(new_args);
-#if PY_MAJOR_VERSION > 2
-            PyErr_Format(PyExc_TypeError,
-                         "unbound method %.200S() needs an argument",
-                         cyfunc->func_qualname);
-#else
-            PyErr_SetString(PyExc_TypeError,
-                            "unbound method needs an argument");
-#endif
-            return NULL;
-        }
-        result = __Pyx_CyFunction_CallMethod(func, self, new_args, kw);
-        Py_DECREF(new_args);
-    } else {
-        result = __Pyx_CyFunction_Call(func, args, kw);
-    }
-    return result;
-}
-#if CYTHON_METH_FASTCALL
-static CYTHON_INLINE int __Pyx_CyFunction_Vectorcall_CheckArgs(__pyx_CyFunctionObject *cyfunc, Py_ssize_t nargs, PyObject *kwnames)
-{
-    int ret = 0;
-    if ((cyfunc->flags & __Pyx_CYFUNCTION_CCLASS) && !(cyfunc->flags & __Pyx_CYFUNCTION_STATICMETHOD)) {
-        if (unlikely(nargs < 1)) {
-            PyErr_Format(PyExc_TypeError, "%.200s() needs an argument",
-                         ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
-            return -1;
-        }
-        ret = 1;
-    }
-    if (unlikely(kwnames) && unlikely(PyTuple_GET_SIZE(kwnames))) {
-        PyErr_Format(PyExc_TypeError,
-                     "%.200s() takes no keyword arguments", ((PyCFunctionObject*)cyfunc)->m_ml->ml_name);
-        return -1;
-    }
-    return ret;
-}
-static PyObject * __Pyx_CyFunction_Vectorcall_NOARGS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
-{
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
-    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
-#if CYTHON_BACKPORT_VECTORCALL
-    Py_ssize_t nargs = (Py_ssize_t)nargsf;
-#else
-    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
-#endif
-    PyObject *self;
-    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
-    case 1:
-        self = args[0];
-        args += 1;
-        nargs -= 1;
-        break;
-    case 0:
-        self = ((PyCFunctionObject*)cyfunc)->m_self;
-        break;
-    default:
-        return NULL;
-    }
-    if (unlikely(nargs != 0)) {
-        PyErr_Format(PyExc_TypeError,
-            "%.200s() takes no arguments (%" CYTHON_FORMAT_SSIZE_T "d given)",
-            def->ml_name, nargs);
-        return NULL;
-    }
-    return def->ml_meth(self, NULL);
-}
-static PyObject * __Pyx_CyFunction_Vectorcall_O(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
-{
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
-    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
-#if CYTHON_BACKPORT_VECTORCALL
-    Py_ssize_t nargs = (Py_ssize_t)nargsf;
-#else
-    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
-#endif
-    PyObject *self;
-    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, kwnames)) {
-    case 1:
-        self = args[0];
-        args += 1;
-        nargs -= 1;
-        break;
-    case 0:
-        self = ((PyCFunctionObject*)cyfunc)->m_self;
-        break;
-    default:
-        return NULL;
-    }
-    if (unlikely(nargs != 1)) {
-        PyErr_Format(PyExc_TypeError,
-            "%.200s() takes exactly one argument (%" CYTHON_FORMAT_SSIZE_T "d given)",
-            def->ml_name, nargs);
-        return NULL;
-    }
-    return def->ml_meth(self, args[0]);
-}
-static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
-{
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
-    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
-#if CYTHON_BACKPORT_VECTORCALL
-    Py_ssize_t nargs = (Py_ssize_t)nargsf;
-#else
-    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
-#endif
-    PyObject *self;
-    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
-    case 1:
-        self = args[0];
-        args += 1;
-        nargs -= 1;
-        break;
-    case 0:
-        self = ((PyCFunctionObject*)cyfunc)->m_self;
-        break;
-    default:
-        return NULL;
-    }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
-}
-static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
-{
-    __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
-    PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
-    PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
-#if CYTHON_BACKPORT_VECTORCALL
-    Py_ssize_t nargs = (Py_ssize_t)nargsf;
-#else
-    Py_ssize_t nargs = PyVectorcall_NARGS(nargsf);
-#endif
-    PyObject *self;
-    switch (__Pyx_CyFunction_Vectorcall_CheckArgs(cyfunc, nargs, NULL)) {
-    case 1:
-        self = args[0];
-        args += 1;
-        nargs -= 1;
-        break;
-    case 0:
-        self = ((PyCFunctionObject*)cyfunc)->m_self;
-        break;
-    default:
-        return NULL;
-    }
-    return ((__Pyx_PyCMethod)(void(*)(void))def->ml_meth)(self, cls, args, (size_t)nargs, kwnames);
-}
-#endif
-#if CYTHON_USE_TYPE_SPECS
-static PyType_Slot __pyx_CyFunctionType_slots[] = {
-    {Py_tp_dealloc, (void *)__Pyx_CyFunction_dealloc},
-    {Py_tp_repr, (void *)__Pyx_CyFunction_repr},
-    {Py_tp_call, (void *)__Pyx_CyFunction_CallAsMethod},
-    {Py_tp_traverse, (void *)__Pyx_CyFunction_traverse},
-    {Py_tp_clear, (void *)__Pyx_CyFunction_clear},
-    {Py_tp_methods, (void *)__pyx_CyFunction_methods},
-    {Py_tp_members, (void *)__pyx_CyFunction_members},
-    {Py_tp_getset, (void *)__pyx_CyFunction_getsets},
-    {Py_tp_descr_get, (void *)__Pyx_PyMethod_New},
-    {0, 0},
-};
-static PyType_Spec __pyx_CyFunctionType_spec = {
-    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
-    sizeof(__pyx_CyFunctionObject),
-    0,
-#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
-    Py_TPFLAGS_METHOD_DESCRIPTOR |
-#endif
-#if (defined(_Py_TPFLAGS_HAVE_VECTORCALL) && CYTHON_METH_FASTCALL)
-    _Py_TPFLAGS_HAVE_VECTORCALL |
-#endif
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
-    __pyx_CyFunctionType_slots
-};
-#else
-static PyTypeObject __pyx_CyFunctionType_type = {
-    PyVarObject_HEAD_INIT(0, 0)
-    __PYX_TYPE_MODULE_PREFIX "cython_function_or_method",
-    sizeof(__pyx_CyFunctionObject),
-    0,
-    (destructor) __Pyx_CyFunction_dealloc,
-#if !CYTHON_METH_FASTCALL
-    0,
-#elif CYTHON_BACKPORT_VECTORCALL
-    (printfunc)offsetof(__pyx_CyFunctionObject, func_vectorcall),
-#else
-    offsetof(PyCFunctionObject, vectorcall),
-#endif
-    0,
-    0,
-#if PY_MAJOR_VERSION < 3
-    0,
-#else
-    0,
-#endif
-    (reprfunc) __Pyx_CyFunction_repr,
-    0,
-    0,
-    0,
-    0,
-    __Pyx_CyFunction_CallAsMethod,
-    0,
-    0,
-    0,
-    0,
-#ifdef Py_TPFLAGS_METHOD_DESCRIPTOR
-    Py_TPFLAGS_METHOD_DESCRIPTOR |
-#endif
-#ifdef _Py_TPFLAGS_HAVE_VECTORCALL
-    _Py_TPFLAGS_HAVE_VECTORCALL |
-#endif
-    Py_TPFLAGS_DEFAULT | Py_TPFLAGS_HAVE_GC | Py_TPFLAGS_BASETYPE,
-    0,
-    (traverseproc) __Pyx_CyFunction_traverse,
-    (inquiry) __Pyx_CyFunction_clear,
-    0,
-#if PY_VERSION_HEX < 0x030500A0
-    offsetof(__pyx_CyFunctionObject, func_weakreflist),
-#else
-    offsetof(PyCFunctionObject, m_weakreflist),
-#endif
-    0,
-    0,
-    __pyx_CyFunction_methods,
-    __pyx_CyFunction_members,
-    __pyx_CyFunction_getsets,
-    0,
-    0,
-    __Pyx_PyMethod_New,
-    0,
-    offsetof(__pyx_CyFunctionObject, func_dict),
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-    0,
-#if PY_VERSION_HEX >= 0x030400a1
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030800b1 && (!CYTHON_COMPILING_IN_PYPY || PYPY_VERSION_NUM >= 0x07030800)
-    0,
-#endif
-#if __PYX_NEED_TP_PRINT_SLOT
-    0,
-#endif
-#if PY_VERSION_HEX >= 0x030C0000
-    0,
-#endif
-#if CYTHON_COMPILING_IN_PYPY && PY_VERSION_HEX >= 0x03090000 && PY_VERSION_HEX < 0x030a0000
-    0,
-#endif
-};
-#endif
-static int __pyx_CyFunction_init(PyObject *module) {
-#if CYTHON_USE_TYPE_SPECS
-    __pyx_CyFunctionType = __Pyx_FetchCommonTypeFromSpec(module, &__pyx_CyFunctionType_spec, NULL);
-#else
-    CYTHON_UNUSED_VAR(module);
-    __pyx_CyFunctionType = __Pyx_FetchCommonType(&__pyx_CyFunctionType_type);
-#endif
-    if (unlikely(__pyx_CyFunctionType == NULL)) {
-        return -1;
-    }
-    return 0;
-}
-static CYTHON_INLINE void *__Pyx_CyFunction_InitDefaults(PyObject *func, size_t size, int pyobjects) {
-    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
-    m->defaults = PyObject_Malloc(size);
-    if (unlikely(!m->defaults))
-        return PyErr_NoMemory();
-    memset(m->defaults, 0, size);
-    m->defaults_pyobjects = pyobjects;
-    m->defaults_size = size;
-    return m->defaults;
-}
-static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsTuple(PyObject *func, PyObject *tuple) {
-    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
-    m->defaults_tuple = tuple;
-    Py_INCREF(tuple);
-}
-static CYTHON_INLINE void __Pyx_CyFunction_SetDefaultsKwDict(PyObject *func, PyObject *dict) {
-    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
-    m->defaults_kwdict = dict;
-    Py_INCREF(dict);
-}
-static CYTHON_INLINE void __Pyx_CyFunction_SetAnnotationsDict(PyObject *func, PyObject *dict) {
-    __pyx_CyFunctionObject *m = (__pyx_CyFunctionObject *) func;
-    m->func_annotations = dict;
-    Py_INCREF(dict);
-}
-
-/* CythonFunction */
-static PyObject *__Pyx_CyFunction_New(PyMethodDef *ml, int flags, PyObject* qualname,
-                                      PyObject *closure, PyObject *module, PyObject* globals, PyObject* code) {
-    PyObject *op = __Pyx_CyFunction_Init(
-        PyObject_GC_New(__pyx_CyFunctionObject, __pyx_CyFunctionType),
-        ml, flags, qualname, closure, module, globals, code
-    );
-    if (likely(op)) {
-        PyObject_GC_Track(op);
-    }
-    return op;
-}
 
 /* CLineInTraceback */
 #ifndef CYTHON_CLINE_IN_TRACEBACK
-static int __Pyx_CLineForTraceback(PyThreadState *tstate, int c_line) {
+static int __Pyx_CLineForTraceback(CYTHON_NCP_UNUSED PyThreadState *tstate, int c_line) {
     PyObject *use_cline;
     PyObject *ptype, *pvalue, *ptraceback;
 #if CYTHON_COMPILING_IN_CPYTHON
     PyObject **cython_runtime_dict;
 #endif
-    CYTHON_MAYBE_UNUSED_VAR(tstate);
     if (unlikely(!__pyx_cython_runtime)) {
         return c_line;
     }
     __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
 #if CYTHON_COMPILING_IN_CPYTHON
     cython_runtime_dict = _PyObject_GetDictPtr(__pyx_cython_runtime);
     if (likely(cython_runtime_dict)) {
         __PYX_PY_DICT_LOOKUP_IF_MODIFIED(
             use_cline, *cython_runtime_dict,
             __Pyx_PyDict_GetItemStr(*cython_runtime_dict, __pyx_n_s_cline_in_traceback))
     } else
 #endif
     {
-      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStrNoError(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
+      PyObject *use_cline_obj = __Pyx_PyObject_GetAttrStr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback);
       if (use_cline_obj) {
         use_cline = PyObject_Not(use_cline_obj) ? Py_False : Py_True;
         Py_DECREF(use_cline_obj);
       } else {
         PyErr_Clear();
         use_cline = NULL;
       }
     }
     if (!use_cline) {
         c_line = 0;
-        (void) PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
+        PyObject_SetAttr(__pyx_cython_runtime, __pyx_n_s_cline_in_traceback, Py_False);
     }
     else if (use_cline == Py_False || (use_cline != Py_True && PyObject_Not(use_cline) != 0)) {
         c_line = 0;
     }
     __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
     return c_line;
 }
 #endif
 
 /* CodeObjectCache */
-#if !CYTHON_COMPILING_IN_LIMITED_API
 static int __pyx_bisect_code_objects(__Pyx_CodeObjectCacheEntry* entries, int count, int code_line) {
     int start = 0, mid = 0, end = count - 1;
     if (end >= 0 && code_line > entries[end].code_line) {
         return count;
     }
     while (start < end) {
         mid = start + (end - start) / 2;
@@ -8038,118 +4694,84 @@
         entries[i] = entries[i-1];
     }
     entries[pos].code_line = code_line;
     entries[pos].code_object = code_object;
     __pyx_code_cache.count++;
     Py_INCREF(code_object);
 }
-#endif
 
 /* AddTraceback */
 #include "compile.h"
 #include "frameobject.h"
 #include "traceback.h"
-#if PY_VERSION_HEX >= 0x030b00a6
-  #ifndef Py_BUILD_CORE
-    #define Py_BUILD_CORE 1
-  #endif
-  #include "internal/pycore_frame.h"
-#endif
-#if CYTHON_COMPILING_IN_LIMITED_API
-static void __Pyx_AddTraceback(const char *funcname, int c_line,
-                               int py_line, const char *filename) {
-    if (c_line) {
-        (void) __pyx_cfilenm;
-        (void) __Pyx_CLineForTraceback(__Pyx_PyThreadState_Current, c_line);
-    }
-    _PyTraceback_Add(funcname, filename, py_line);
-}
-#else
 static PyCodeObject* __Pyx_CreateCodeObjectForTraceback(
             const char *funcname, int c_line,
             int py_line, const char *filename) {
-    PyCodeObject *py_code = NULL;
-    PyObject *py_funcname = NULL;
+    PyCodeObject *py_code = 0;
+    PyObject *py_srcfile = 0;
+    PyObject *py_funcname = 0;
     #if PY_MAJOR_VERSION < 3
-    PyObject *py_srcfile = NULL;
     py_srcfile = PyString_FromString(filename);
-    if (!py_srcfile) goto bad;
+    #else
+    py_srcfile = PyUnicode_FromString(filename);
     #endif
+    if (!py_srcfile) goto bad;
     if (c_line) {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
         #else
         py_funcname = PyUnicode_FromFormat( "%s (%s:%d)", funcname, __pyx_cfilenm, c_line);
-        if (!py_funcname) goto bad;
-        funcname = PyUnicode_AsUTF8(py_funcname);
-        if (!funcname) goto bad;
         #endif
     }
     else {
         #if PY_MAJOR_VERSION < 3
         py_funcname = PyString_FromString(funcname);
-        if (!py_funcname) goto bad;
+        #else
+        py_funcname = PyUnicode_FromString(funcname);
         #endif
     }
-    #if PY_MAJOR_VERSION < 3
+    if (!py_funcname) goto bad;
     py_code = __Pyx_PyCode_New(
         0,
         0,
         0,
         0,
         0,
-        0,
         __pyx_empty_bytes, /*PyObject *code,*/
         __pyx_empty_tuple, /*PyObject *consts,*/
         __pyx_empty_tuple, /*PyObject *names,*/
         __pyx_empty_tuple, /*PyObject *varnames,*/
         __pyx_empty_tuple, /*PyObject *freevars,*/
         __pyx_empty_tuple, /*PyObject *cellvars,*/
         py_srcfile,   /*PyObject *filename,*/
         py_funcname,  /*PyObject *name,*/
         py_line,
         __pyx_empty_bytes  /*PyObject *lnotab*/
     );
     Py_DECREF(py_srcfile);
-    #else
-    py_code = PyCode_NewEmpty(filename, funcname, py_line);
-    #endif
-    Py_XDECREF(py_funcname);  // XDECREF since it's only set on Py3 if cline
+    Py_DECREF(py_funcname);
     return py_code;
 bad:
-    Py_XDECREF(py_funcname);
-    #if PY_MAJOR_VERSION < 3
     Py_XDECREF(py_srcfile);
-    #endif
+    Py_XDECREF(py_funcname);
     return NULL;
 }
 static void __Pyx_AddTraceback(const char *funcname, int c_line,
                                int py_line, const char *filename) {
     PyCodeObject *py_code = 0;
     PyFrameObject *py_frame = 0;
     PyThreadState *tstate = __Pyx_PyThreadState_Current;
-    PyObject *ptype, *pvalue, *ptraceback;
     if (c_line) {
         c_line = __Pyx_CLineForTraceback(tstate, c_line);
     }
     py_code = __pyx_find_code_object(c_line ? -c_line : py_line);
     if (!py_code) {
-        __Pyx_ErrFetchInState(tstate, &ptype, &pvalue, &ptraceback);
         py_code = __Pyx_CreateCodeObjectForTraceback(
             funcname, c_line, py_line, filename);
-        if (!py_code) {
-            /* If the code object creation fails, then we should clear the
-               fetched exception references and propagate the new exception */
-            Py_XDECREF(ptype);
-            Py_XDECREF(pvalue);
-            Py_XDECREF(ptraceback);
-            goto bad;
-        }
-        __Pyx_ErrRestoreInState(tstate, ptype, pvalue, ptraceback);
+        if (!py_code) goto bad;
         __pyx_insert_code_object(c_line ? -c_line : py_line, py_code);
     }
     py_frame = PyFrame_New(
         tstate,            /*PyThreadState *tstate,*/
         py_code,           /*PyCodeObject *code,*/
         __pyx_d,    /*PyObject *globals,*/
         0                  /*PyObject *locals*/
@@ -8157,15 +4779,45 @@
     if (!py_frame) goto bad;
     __Pyx_PyFrame_SetLineNumber(py_frame, py_line);
     PyTraceBack_Here(py_frame);
 bad:
     Py_XDECREF(py_code);
     Py_XDECREF(py_frame);
 }
+
+/* CIntToPy */
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value) {
+    const PY_LONG_LONG neg_one = (PY_LONG_LONG) ((PY_LONG_LONG) 0 - (PY_LONG_LONG) 1), const_zero = (PY_LONG_LONG) 0;
+    const int is_unsigned = neg_one > const_zero;
+    if (is_unsigned) {
+        if (sizeof(PY_LONG_LONG) < sizeof(long)) {
+            return PyInt_FromLong((long) value);
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned long)) {
+            return PyLong_FromUnsignedLong((unsigned long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
+            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
+        }
+    } else {
+        if (sizeof(PY_LONG_LONG) <= sizeof(long)) {
+            return PyInt_FromLong((long) value);
+#ifdef HAVE_LONG_LONG
+        } else if (sizeof(PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
+            return PyLong_FromLongLong((PY_LONG_LONG) value);
+#endif
+        }
+    }
+    {
+        int one = 1; int little = (int)*(unsigned char *)&one;
+        unsigned char *bytes = (unsigned char *)&value;
+        return _PyLong_FromByteArray(bytes, sizeof(PY_LONG_LONG),
+                                     little, !is_unsigned);
+    }
+}
 
 /* CIntFromPyVerify */
 #define __PYX_VERIFY_RETURN_INT(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 0)
 #define __PYX_VERIFY_RETURN_INT_EXC(target_type, func_type, func_value)\
     __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, 1)
 #define __PYX__VERIFY_RETURN_INT(target_type, func_type, func_value, exc)\
@@ -8182,304 +4834,213 @@
                     goto raise_overflow;\
             }\
         }\
         return (target_type) value;\
     }
 
 /* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_PY_LONG_LONG(PY_LONG_LONG value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const PY_LONG_LONG neg_one = (PY_LONG_LONG) -1, const_zero = (PY_LONG_LONG) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
+    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
     if (is_unsigned) {
-        if (sizeof(PY_LONG_LONG) < sizeof(long)) {
+        if (sizeof(long) < sizeof(long)) {
             return PyInt_FromLong((long) value);
-        } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned long)) {
+        } else if (sizeof(long) <= sizeof(unsigned long)) {
             return PyLong_FromUnsignedLong((unsigned long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
             return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
 #endif
         }
     } else {
-        if (sizeof(PY_LONG_LONG) <= sizeof(long)) {
+        if (sizeof(long) <= sizeof(long)) {
             return PyInt_FromLong((long) value);
 #ifdef HAVE_LONG_LONG
-        } else if (sizeof(PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
+        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
             return PyLong_FromLongLong((PY_LONG_LONG) value);
 #endif
         }
     }
     {
         int one = 1; int little = (int)*(unsigned char *)&one;
         unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(PY_LONG_LONG),
+        return _PyLong_FromByteArray(bytes, sizeof(long),
                                      little, !is_unsigned);
     }
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE PY_LONG_LONG __Pyx_PyInt_As_PY_LONG_LONG(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const PY_LONG_LONG neg_one = (PY_LONG_LONG) -1, const_zero = (PY_LONG_LONG) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const PY_LONG_LONG neg_one = (PY_LONG_LONG) ((PY_LONG_LONG) 0 - (PY_LONG_LONG) 1), const_zero = (PY_LONG_LONG) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(PY_LONG_LONG) < sizeof(long))) {
+        if (sizeof(PY_LONG_LONG) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (PY_LONG_LONG) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
-                goto raise_neg_overflow;
-            } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
-            } else {
-                const digit* digits = __Pyx_PyLong_Digits(x);
-                assert(__Pyx_PyLong_DigitCount(x) > 1);
-                switch (__Pyx_PyLong_DigitCount(x)) {
-                    case 2:
-                        if ((8 * sizeof(PY_LONG_LONG) > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) >= 2 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) (((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
-                            }
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (PY_LONG_LONG) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, digit, digits[0])
+                case 2:
+                    if (8 * sizeof(PY_LONG_LONG) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) >= 2 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
-                        break;
-                    case 3:
-                        if ((8 * sizeof(PY_LONG_LONG) > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) >= 3 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) (((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
-                            }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(PY_LONG_LONG) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) >= 3 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
-                        break;
-                    case 4:
-                        if ((8 * sizeof(PY_LONG_LONG) > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
-                            }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(PY_LONG_LONG) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) >= 4 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0]));
                         }
-                        break;
-                }
+                    }
+                    break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (PY_LONG_LONG) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(PY_LONG_LONG) <= sizeof(unsigned long))) {
+            if (sizeof(PY_LONG_LONG) <= sizeof(unsigned long)) {
                 __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG))) {
+            } else if (sizeof(PY_LONG_LONG) <= sizeof(unsigned PY_LONG_LONG)) {
                 __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
-            } else {
-                const digit* digits = __Pyx_PyLong_Digits(x);
-                assert(__Pyx_PyLong_DigitCount(x) > 1);
-                switch (__Pyx_PyLong_SignedDigitCount(x)) {
-                    case -2:
-                        if ((8 * sizeof(PY_LONG_LONG) - 1 > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                            }
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (PY_LONG_LONG) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(PY_LONG_LONG,  digit, +digits[0])
+                case -2:
+                    if (8 * sizeof(PY_LONG_LONG) - 1 > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
-                        break;
-                    case 2:
-                        if ((8 * sizeof(PY_LONG_LONG) > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) ((((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                            }
+                    }
+                    break;
+                case 2:
+                    if (8 * sizeof(PY_LONG_LONG) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) ((((((PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
-                        break;
-                    case -3:
-                        if ((8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                            }
+                    }
+                    break;
+                case -3:
+                    if (8 * sizeof(PY_LONG_LONG) - 1 > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
-                        break;
-                    case 3:
-                        if ((8 * sizeof(PY_LONG_LONG) > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) ((((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                            }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(PY_LONG_LONG) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) ((((((((PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
-                        break;
-                    case -4:
-                        if ((8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                            }
+                    }
+                    break;
+                case -4:
+                    if (8 * sizeof(PY_LONG_LONG) - 1 > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) (((PY_LONG_LONG)-1)*(((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
-                        break;
-                    case 4:
-                        if ((8 * sizeof(PY_LONG_LONG) > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT)) {
-                                return (PY_LONG_LONG) ((((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
-                            }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(PY_LONG_LONG) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(PY_LONG_LONG, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(PY_LONG_LONG) - 1 > 4 * PyLong_SHIFT) {
+                            return (PY_LONG_LONG) ((((((((((PY_LONG_LONG)digits[3]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[2]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[1]) << PyLong_SHIFT) | (PY_LONG_LONG)digits[0])));
                         }
-                        break;
-                }
+                    }
+                    break;
             }
 #endif
-            if ((sizeof(PY_LONG_LONG) <= sizeof(long))) {
+            if (sizeof(PY_LONG_LONG) <= sizeof(long)) {
                 __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(PY_LONG_LONG) <= sizeof(PY_LONG_LONG))) {
+            } else if (sizeof(PY_LONG_LONG) <= sizeof(PY_LONG_LONG)) {
                 __PYX_VERIFY_RETURN_INT_EXC(PY_LONG_LONG, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
+#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+            PyErr_SetString(PyExc_RuntimeError,
+                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+#else
             PY_LONG_LONG val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
-#if PY_MAJOR_VERSION < 3
+ #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
-#endif
+ #endif
             if (likely(v)) {
-                int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                           bytes, sizeof(val),
-                                           is_little, !is_unsigned);
-#else
-                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
-                int bits, remaining_bits, is_negative = 0;
-                long idigit;
-                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
-                if (unlikely(!PyLong_CheckExact(v))) {
-                    PyObject *tmp = v;
-                    v = PyNumber_Long(v);
-                    assert(PyLong_CheckExact(v));
-                    Py_DECREF(tmp);
-                    if (unlikely(!v)) return (PY_LONG_LONG) -1;
-                }
-#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-                if (Py_SIZE(x) == 0)
-                    return (PY_LONG_LONG) 0;
-                is_negative = Py_SIZE(x) < 0;
-#else
-                {
-                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                    if (unlikely(result < 0))
-                        return (PY_LONG_LONG) -1;
-                    is_negative = result == 1;
-                }
-#endif
-                if (is_unsigned && unlikely(is_negative)) {
-                    goto raise_neg_overflow;
-                } else if (is_negative) {
-                    stepval = PyNumber_Invert(v);
-                    if (unlikely(!stepval))
-                        return (PY_LONG_LONG) -1;
-                } else {
-                    stepval = __Pyx_NewRef(v);
-                }
-                val = (PY_LONG_LONG) 0;
-                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
-                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(PY_LONG_LONG) * 8 - chunk_size; bits += chunk_size) {
-                    PyObject *tmp, *digit;
-                    digit = PyNumber_And(stepval, mask);
-                    if (unlikely(!digit)) goto done;
-                    idigit = PyLong_AsLong(digit);
-                    Py_DECREF(digit);
-                    if (unlikely(idigit < 0)) goto done;
-                    tmp = PyNumber_Rshift(stepval, shift);
-                    if (unlikely(!tmp)) goto done;
-                    Py_DECREF(stepval); stepval = tmp;
-                    val |= ((PY_LONG_LONG) idigit) << bits;
-                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-                    if (Py_SIZE(stepval) == 0)
-                        goto unpacking_done;
-                    #endif
-                }
-                idigit = PyLong_AsLong(stepval);
-                if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(PY_LONG_LONG) * 8) - bits - (is_unsigned ? 0 : 1);
-                if (unlikely(idigit >= (1L << remaining_bits)))
-                    goto raise_overflow;
-                val |= ((PY_LONG_LONG) idigit) << bits;
-            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-            unpacking_done:
-            #endif
-                if (!is_unsigned) {
-                    if (unlikely(val & (((PY_LONG_LONG) 1) << (sizeof(PY_LONG_LONG) * 8 - 1))))
-                        goto raise_overflow;
-                    if (is_negative)
-                        val = ~val;
-                }
-                ret = 0;
-            done:
-                Py_XDECREF(shift);
-                Py_XDECREF(mask);
-                Py_XDECREF(stepval);
-#endif
+                int ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                              bytes, sizeof(val),
+                                              is_little, !is_unsigned);
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
+#endif
             return (PY_LONG_LONG) -1;
         }
     } else {
         PY_LONG_LONG val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (PY_LONG_LONG) -1;
         val = __Pyx_PyInt_As_PY_LONG_LONG(tmp);
@@ -8494,265 +5055,181 @@
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to PY_LONG_LONG");
     return (PY_LONG_LONG) -1;
 }
 
 /* CIntFromPy */
 static CYTHON_INLINE long __Pyx_PyInt_As_long(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const long neg_one = (long) ((long) 0 - (long) 1), const_zero = (long) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(long) < sizeof(long))) {
+        if (sizeof(long) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(long, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (long) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
-                goto raise_neg_overflow;
-            } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
-            } else {
-                const digit* digits = __Pyx_PyLong_Digits(x);
-                assert(__Pyx_PyLong_DigitCount(x) > 1);
-                switch (__Pyx_PyLong_DigitCount(x)) {
-                    case 2:
-                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 2 * PyLong_SHIFT)) {
-                                return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
-                            }
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (long) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(long, digit, digits[0])
+                case 2:
+                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) >= 2 * PyLong_SHIFT) {
+                            return (long) (((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
-                        break;
-                    case 3:
-                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 3 * PyLong_SHIFT)) {
-                                return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
-                            }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) >= 3 * PyLong_SHIFT) {
+                            return (long) (((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
-                        break;
-                    case 4:
-                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) >= 4 * PyLong_SHIFT)) {
-                                return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
-                            }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) >= 4 * PyLong_SHIFT) {
+                            return (long) (((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0]));
                         }
-                        break;
-                }
+                    }
+                    break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (long) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(long) <= sizeof(unsigned long))) {
+            if (sizeof(long) <= sizeof(unsigned long)) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(long) <= sizeof(unsigned PY_LONG_LONG))) {
+            } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(long, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
-            } else {
-                const digit* digits = __Pyx_PyLong_Digits(x);
-                assert(__Pyx_PyLong_DigitCount(x) > 1);
-                switch (__Pyx_PyLong_SignedDigitCount(x)) {
-                    case -2:
-                        if ((8 * sizeof(long) - 1 > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
-                            }
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (long) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(long, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(long,  digit, +digits[0])
+                case -2:
+                    if (8 * sizeof(long) - 1 > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                            return (long) (((long)-1)*(((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
-                        break;
-                    case 2:
-                        if ((8 * sizeof(long) > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                                return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
-                            }
+                    }
+                    break;
+                case 2:
+                    if (8 * sizeof(long) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                            return (long) ((((((long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
-                        break;
-                    case -3:
-                        if ((8 * sizeof(long) - 1 > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
-                            }
+                    }
+                    break;
+                case -3:
+                    if (8 * sizeof(long) - 1 > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                            return (long) (((long)-1)*(((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
-                        break;
-                    case 3:
-                        if ((8 * sizeof(long) > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                                return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
-                            }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(long) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                            return (long) ((((((((long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
-                        break;
-                    case -4:
-                        if ((8 * sizeof(long) - 1 > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
-                            }
+                    }
+                    break;
+                case -4:
+                    if (8 * sizeof(long) - 1 > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                            return (long) (((long)-1)*(((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
-                        break;
-                    case 4:
-                        if ((8 * sizeof(long) > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(long) - 1 > 4 * PyLong_SHIFT)) {
-                                return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
-                            }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(long) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(long, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(long) - 1 > 4 * PyLong_SHIFT) {
+                            return (long) ((((((((((long)digits[3]) << PyLong_SHIFT) | (long)digits[2]) << PyLong_SHIFT) | (long)digits[1]) << PyLong_SHIFT) | (long)digits[0])));
                         }
-                        break;
-                }
+                    }
+                    break;
             }
 #endif
-            if ((sizeof(long) <= sizeof(long))) {
+            if (sizeof(long) <= sizeof(long)) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(long) <= sizeof(PY_LONG_LONG))) {
+            } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
                 __PYX_VERIFY_RETURN_INT_EXC(long, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
+#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+            PyErr_SetString(PyExc_RuntimeError,
+                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+#else
             long val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
-#if PY_MAJOR_VERSION < 3
+ #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
-#endif
+ #endif
             if (likely(v)) {
-                int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                           bytes, sizeof(val),
-                                           is_little, !is_unsigned);
-#else
-                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
-                int bits, remaining_bits, is_negative = 0;
-                long idigit;
-                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
-                if (unlikely(!PyLong_CheckExact(v))) {
-                    PyObject *tmp = v;
-                    v = PyNumber_Long(v);
-                    assert(PyLong_CheckExact(v));
-                    Py_DECREF(tmp);
-                    if (unlikely(!v)) return (long) -1;
-                }
-#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-                if (Py_SIZE(x) == 0)
-                    return (long) 0;
-                is_negative = Py_SIZE(x) < 0;
-#else
-                {
-                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                    if (unlikely(result < 0))
-                        return (long) -1;
-                    is_negative = result == 1;
-                }
-#endif
-                if (is_unsigned && unlikely(is_negative)) {
-                    goto raise_neg_overflow;
-                } else if (is_negative) {
-                    stepval = PyNumber_Invert(v);
-                    if (unlikely(!stepval))
-                        return (long) -1;
-                } else {
-                    stepval = __Pyx_NewRef(v);
-                }
-                val = (long) 0;
-                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
-                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(long) * 8 - chunk_size; bits += chunk_size) {
-                    PyObject *tmp, *digit;
-                    digit = PyNumber_And(stepval, mask);
-                    if (unlikely(!digit)) goto done;
-                    idigit = PyLong_AsLong(digit);
-                    Py_DECREF(digit);
-                    if (unlikely(idigit < 0)) goto done;
-                    tmp = PyNumber_Rshift(stepval, shift);
-                    if (unlikely(!tmp)) goto done;
-                    Py_DECREF(stepval); stepval = tmp;
-                    val |= ((long) idigit) << bits;
-                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-                    if (Py_SIZE(stepval) == 0)
-                        goto unpacking_done;
-                    #endif
-                }
-                idigit = PyLong_AsLong(stepval);
-                if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(long) * 8) - bits - (is_unsigned ? 0 : 1);
-                if (unlikely(idigit >= (1L << remaining_bits)))
-                    goto raise_overflow;
-                val |= ((long) idigit) << bits;
-            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-            unpacking_done:
-            #endif
-                if (!is_unsigned) {
-                    if (unlikely(val & (((long) 1) << (sizeof(long) * 8 - 1))))
-                        goto raise_overflow;
-                    if (is_negative)
-                        val = ~val;
-                }
-                ret = 0;
-            done:
-                Py_XDECREF(shift);
-                Py_XDECREF(mask);
-                Py_XDECREF(stepval);
-#endif
+                int ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                              bytes, sizeof(val),
+                                              is_little, !is_unsigned);
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
+#endif
             return (long) -1;
         }
     } else {
         long val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (long) -1;
         val = __Pyx_PyInt_As_long(tmp);
@@ -8765,320 +5242,183 @@
     return (long) -1;
 raise_neg_overflow:
     PyErr_SetString(PyExc_OverflowError,
         "can't convert negative value to long");
     return (long) -1;
 }
 
-/* CIntToPy */
-static CYTHON_INLINE PyObject* __Pyx_PyInt_From_long(long value) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const long neg_one = (long) -1, const_zero = (long) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
-    const int is_unsigned = neg_one > const_zero;
-    if (is_unsigned) {
-        if (sizeof(long) < sizeof(long)) {
-            return PyInt_FromLong((long) value);
-        } else if (sizeof(long) <= sizeof(unsigned long)) {
-            return PyLong_FromUnsignedLong((unsigned long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(unsigned PY_LONG_LONG)) {
-            return PyLong_FromUnsignedLongLong((unsigned PY_LONG_LONG) value);
-#endif
-        }
-    } else {
-        if (sizeof(long) <= sizeof(long)) {
-            return PyInt_FromLong((long) value);
-#ifdef HAVE_LONG_LONG
-        } else if (sizeof(long) <= sizeof(PY_LONG_LONG)) {
-            return PyLong_FromLongLong((PY_LONG_LONG) value);
-#endif
-        }
-    }
-    {
-        int one = 1; int little = (int)*(unsigned char *)&one;
-        unsigned char *bytes = (unsigned char *)&value;
-        return _PyLong_FromByteArray(bytes, sizeof(long),
-                                     little, !is_unsigned);
-    }
-}
-
-/* FormatTypeName */
-#if CYTHON_COMPILING_IN_LIMITED_API
-static __Pyx_TypeName
-__Pyx_PyType_GetName(PyTypeObject* tp)
-{
-    PyObject *name = __Pyx_PyObject_GetAttrStr((PyObject *)tp,
-                                               __pyx_n_s_name);
-    if (unlikely(name == NULL) || unlikely(!PyUnicode_Check(name))) {
-        PyErr_Clear();
-        Py_XSETREF(name, __Pyx_NewRef(__pyx_n_s__11));
-    }
-    return name;
-}
-#endif
-
 /* CIntFromPy */
 static CYTHON_INLINE int __Pyx_PyInt_As_int(PyObject *x) {
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic push
-#pragma GCC diagnostic ignored "-Wconversion"
-#endif
-    const int neg_one = (int) -1, const_zero = (int) 0;
-#ifdef __Pyx_HAS_GCC_DIAGNOSTIC
-#pragma GCC diagnostic pop
-#endif
+    const int neg_one = (int) ((int) 0 - (int) 1), const_zero = (int) 0;
     const int is_unsigned = neg_one > const_zero;
 #if PY_MAJOR_VERSION < 3
     if (likely(PyInt_Check(x))) {
-        if ((sizeof(int) < sizeof(long))) {
+        if (sizeof(int) < sizeof(long)) {
             __PYX_VERIFY_RETURN_INT(int, long, PyInt_AS_LONG(x))
         } else {
             long val = PyInt_AS_LONG(x);
             if (is_unsigned && unlikely(val < 0)) {
                 goto raise_neg_overflow;
             }
             return (int) val;
         }
     } else
 #endif
     if (likely(PyLong_Check(x))) {
         if (is_unsigned) {
 #if CYTHON_USE_PYLONG_INTERNALS
-            if (unlikely(__Pyx_PyLong_IsNeg(x))) {
-                goto raise_neg_overflow;
-            } else if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_upylong, __Pyx_PyLong_CompactValueUnsigned(x))
-            } else {
-                const digit* digits = __Pyx_PyLong_Digits(x);
-                assert(__Pyx_PyLong_DigitCount(x) > 1);
-                switch (__Pyx_PyLong_DigitCount(x)) {
-                    case 2:
-                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 2 * PyLong_SHIFT)) {
-                                return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
-                            }
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (int) 0;
+                case  1: __PYX_VERIFY_RETURN_INT(int, digit, digits[0])
+                case 2:
+                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 2 * PyLong_SHIFT) {
+                            return (int) (((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
-                        break;
-                    case 3:
-                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 3 * PyLong_SHIFT)) {
-                                return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
-                            }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 3 * PyLong_SHIFT) {
+                            return (int) (((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
-                        break;
-                    case 4:
-                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) >= 4 * PyLong_SHIFT)) {
-                                return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
-                            }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) >= 4 * PyLong_SHIFT) {
+                            return (int) (((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0]));
                         }
-                        break;
-                }
+                    }
+                    break;
             }
 #endif
-#if CYTHON_COMPILING_IN_CPYTHON && PY_VERSION_HEX < 0x030C00A7
+#if CYTHON_COMPILING_IN_CPYTHON
             if (unlikely(Py_SIZE(x) < 0)) {
                 goto raise_neg_overflow;
             }
 #else
             {
                 int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
                 if (unlikely(result < 0))
                     return (int) -1;
                 if (unlikely(result == 1))
                     goto raise_neg_overflow;
             }
 #endif
-            if ((sizeof(int) <= sizeof(unsigned long))) {
+            if (sizeof(int) <= sizeof(unsigned long)) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned long, PyLong_AsUnsignedLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(int) <= sizeof(unsigned PY_LONG_LONG))) {
+            } else if (sizeof(int) <= sizeof(unsigned PY_LONG_LONG)) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, unsigned PY_LONG_LONG, PyLong_AsUnsignedLongLong(x))
 #endif
             }
         } else {
 #if CYTHON_USE_PYLONG_INTERNALS
-            if (__Pyx_PyLong_IsCompact(x)) {
-                __PYX_VERIFY_RETURN_INT(int, __Pyx_compact_pylong, __Pyx_PyLong_CompactValue(x))
-            } else {
-                const digit* digits = __Pyx_PyLong_Digits(x);
-                assert(__Pyx_PyLong_DigitCount(x) > 1);
-                switch (__Pyx_PyLong_SignedDigitCount(x)) {
-                    case -2:
-                        if ((8 * sizeof(int) - 1 > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                            }
+            const digit* digits = ((PyLongObject*)x)->ob_digit;
+            switch (Py_SIZE(x)) {
+                case  0: return (int) 0;
+                case -1: __PYX_VERIFY_RETURN_INT(int, sdigit, (sdigit) (-(sdigit)digits[0]))
+                case  1: __PYX_VERIFY_RETURN_INT(int,  digit, +digits[0])
+                case -2:
+                    if (8 * sizeof(int) - 1 > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
-                        break;
-                    case 2:
-                        if ((8 * sizeof(int) > 1 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 2 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                                return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                            }
+                    }
+                    break;
+                case 2:
+                    if (8 * sizeof(int) > 1 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 2 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                            return (int) ((((((int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
-                        break;
-                    case -3:
-                        if ((8 * sizeof(int) - 1 > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                            }
+                    }
+                    break;
+                case -3:
+                    if (8 * sizeof(int) - 1 > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
-                        break;
-                    case 3:
-                        if ((8 * sizeof(int) > 2 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 3 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                                return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                            }
+                    }
+                    break;
+                case 3:
+                    if (8 * sizeof(int) > 2 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 3 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                            return (int) ((((((((int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
-                        break;
-                    case -4:
-                        if ((8 * sizeof(int) - 1 > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                                return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                            }
+                    }
+                    break;
+                case -4:
+                    if (8 * sizeof(int) - 1 > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, long, -(long) (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                            return (int) (((int)-1)*(((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
-                        break;
-                    case 4:
-                        if ((8 * sizeof(int) > 3 * PyLong_SHIFT)) {
-                            if ((8 * sizeof(unsigned long) > 4 * PyLong_SHIFT)) {
-                                __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
-                            } else if ((8 * sizeof(int) - 1 > 4 * PyLong_SHIFT)) {
-                                return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
-                            }
+                    }
+                    break;
+                case 4:
+                    if (8 * sizeof(int) > 3 * PyLong_SHIFT) {
+                        if (8 * sizeof(unsigned long) > 4 * PyLong_SHIFT) {
+                            __PYX_VERIFY_RETURN_INT(int, unsigned long, (((((((((unsigned long)digits[3]) << PyLong_SHIFT) | (unsigned long)digits[2]) << PyLong_SHIFT) | (unsigned long)digits[1]) << PyLong_SHIFT) | (unsigned long)digits[0])))
+                        } else if (8 * sizeof(int) - 1 > 4 * PyLong_SHIFT) {
+                            return (int) ((((((((((int)digits[3]) << PyLong_SHIFT) | (int)digits[2]) << PyLong_SHIFT) | (int)digits[1]) << PyLong_SHIFT) | (int)digits[0])));
                         }
-                        break;
-                }
+                    }
+                    break;
             }
 #endif
-            if ((sizeof(int) <= sizeof(long))) {
+            if (sizeof(int) <= sizeof(long)) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, long, PyLong_AsLong(x))
 #ifdef HAVE_LONG_LONG
-            } else if ((sizeof(int) <= sizeof(PY_LONG_LONG))) {
+            } else if (sizeof(int) <= sizeof(PY_LONG_LONG)) {
                 __PYX_VERIFY_RETURN_INT_EXC(int, PY_LONG_LONG, PyLong_AsLongLong(x))
 #endif
             }
         }
         {
+#if CYTHON_COMPILING_IN_PYPY && !defined(_PyLong_AsByteArray)
+            PyErr_SetString(PyExc_RuntimeError,
+                            "_PyLong_AsByteArray() not available in PyPy, cannot convert large numbers");
+#else
             int val;
             PyObject *v = __Pyx_PyNumber_IntOrLong(x);
-#if PY_MAJOR_VERSION < 3
+ #if PY_MAJOR_VERSION < 3
             if (likely(v) && !PyLong_Check(v)) {
                 PyObject *tmp = v;
                 v = PyNumber_Long(tmp);
                 Py_DECREF(tmp);
             }
-#endif
+ #endif
             if (likely(v)) {
-                int ret = -1;
-#if !(CYTHON_COMPILING_IN_PYPY || CYTHON_COMPILING_IN_LIMITED_API) || defined(_PyLong_AsByteArray)
                 int one = 1; int is_little = (int)*(unsigned char *)&one;
                 unsigned char *bytes = (unsigned char *)&val;
-                ret = _PyLong_AsByteArray((PyLongObject *)v,
-                                           bytes, sizeof(val),
-                                           is_little, !is_unsigned);
-#else
-                PyObject *stepval = NULL, *mask = NULL, *shift = NULL;
-                int bits, remaining_bits, is_negative = 0;
-                long idigit;
-                int chunk_size = (sizeof(long) < 8) ? 30 : 62;
-                if (unlikely(!PyLong_CheckExact(v))) {
-                    PyObject *tmp = v;
-                    v = PyNumber_Long(v);
-                    assert(PyLong_CheckExact(v));
-                    Py_DECREF(tmp);
-                    if (unlikely(!v)) return (int) -1;
-                }
-#if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-                if (Py_SIZE(x) == 0)
-                    return (int) 0;
-                is_negative = Py_SIZE(x) < 0;
-#else
-                {
-                    int result = PyObject_RichCompareBool(x, Py_False, Py_LT);
-                    if (unlikely(result < 0))
-                        return (int) -1;
-                    is_negative = result == 1;
-                }
-#endif
-                if (is_unsigned && unlikely(is_negative)) {
-                    goto raise_neg_overflow;
-                } else if (is_negative) {
-                    stepval = PyNumber_Invert(v);
-                    if (unlikely(!stepval))
-                        return (int) -1;
-                } else {
-                    stepval = __Pyx_NewRef(v);
-                }
-                val = (int) 0;
-                mask = PyLong_FromLong((1L << chunk_size) - 1); if (unlikely(!mask)) goto done;
-                shift = PyLong_FromLong(chunk_size); if (unlikely(!shift)) goto done;
-                for (bits = 0; bits < (int) sizeof(int) * 8 - chunk_size; bits += chunk_size) {
-                    PyObject *tmp, *digit;
-                    digit = PyNumber_And(stepval, mask);
-                    if (unlikely(!digit)) goto done;
-                    idigit = PyLong_AsLong(digit);
-                    Py_DECREF(digit);
-                    if (unlikely(idigit < 0)) goto done;
-                    tmp = PyNumber_Rshift(stepval, shift);
-                    if (unlikely(!tmp)) goto done;
-                    Py_DECREF(stepval); stepval = tmp;
-                    val |= ((int) idigit) << bits;
-                    #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-                    if (Py_SIZE(stepval) == 0)
-                        goto unpacking_done;
-                    #endif
-                }
-                idigit = PyLong_AsLong(stepval);
-                if (unlikely(idigit < 0)) goto done;
-                remaining_bits = ((int) sizeof(int) * 8) - bits - (is_unsigned ? 0 : 1);
-                if (unlikely(idigit >= (1L << remaining_bits)))
-                    goto raise_overflow;
-                val |= ((int) idigit) << bits;
-            #if CYTHON_COMPILING_IN_LIMITED_API && PY_VERSION_HEX < 0x030B0000
-            unpacking_done:
-            #endif
-                if (!is_unsigned) {
-                    if (unlikely(val & (((int) 1) << (sizeof(int) * 8 - 1))))
-                        goto raise_overflow;
-                    if (is_negative)
-                        val = ~val;
-                }
-                ret = 0;
-            done:
-                Py_XDECREF(shift);
-                Py_XDECREF(mask);
-                Py_XDECREF(stepval);
-#endif
+                int ret = _PyLong_AsByteArray((PyLongObject *)v,
+                                              bytes, sizeof(val),
+                                              is_little, !is_unsigned);
                 Py_DECREF(v);
                 if (likely(!ret))
                     return val;
             }
+#endif
             return (int) -1;
         }
     } else {
         int val;
         PyObject *tmp = __Pyx_PyNumber_IntOrLong(x);
         if (!tmp) return (int) -1;
         val = __Pyx_PyInt_As_int(tmp);
@@ -9095,15 +5435,15 @@
     return (int) -1;
 }
 
 /* FastTypeChecks */
 #if CYTHON_COMPILING_IN_CPYTHON
 static int __Pyx_InBases(PyTypeObject *a, PyTypeObject *b) {
     while (a) {
-        a = __Pyx_PyType_GetSlot(a, tp_base, PyTypeObject*);
+        a = a->tp_base;
         if (a == b)
             return 1;
     }
     return b == &PyBaseObject_Type;
 }
 static CYTHON_INLINE int __Pyx_IsSubtype(PyTypeObject *a, PyTypeObject *b) {
     PyObject *mro;
@@ -9116,30 +5456,14 @@
             if (PyTuple_GET_ITEM(mro, i) == (PyObject *)b)
                 return 1;
         }
         return 0;
     }
     return __Pyx_InBases(a, b);
 }
-static CYTHON_INLINE int __Pyx_IsAnySubtype2(PyTypeObject *cls, PyTypeObject *a, PyTypeObject *b) {
-    PyObject *mro;
-    if (cls == a || cls == b) return 1;
-    mro = cls->tp_mro;
-    if (likely(mro)) {
-        Py_ssize_t i, n;
-        n = PyTuple_GET_SIZE(mro);
-        for (i = 0; i < n; i++) {
-            PyObject *base = PyTuple_GET_ITEM(mro, i);
-            if (base == (PyObject *)a || base == (PyObject *)b)
-                return 1;
-        }
-        return 0;
-    }
-    return __Pyx_InBases(cls, a) || __Pyx_InBases(cls, b);
-}
 #if PY_MAJOR_VERSION == 2
 static int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject* exc_type2) {
     PyObject *exception, *value, *tb;
     int res;
     __Pyx_PyThreadState_declare
     __Pyx_PyThreadState_assign
     __Pyx_ErrFetch(&exception, &value, &tb);
@@ -9156,19 +5480,19 @@
         }
     }
     __Pyx_ErrRestore(exception, value, tb);
     return res;
 }
 #else
 static CYTHON_INLINE int __Pyx_inner_PyErr_GivenExceptionMatches2(PyObject *err, PyObject* exc_type1, PyObject *exc_type2) {
-    if (exc_type1) {
-        return __Pyx_IsAnySubtype2((PyTypeObject*)err, (PyTypeObject*)exc_type1, (PyTypeObject*)exc_type2);
-    } else {
-        return __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
+    int res = exc_type1 ? __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type1) : 0;
+    if (!res) {
+        res = __Pyx_IsSubtype((PyTypeObject*)err, (PyTypeObject*)exc_type2);
     }
+    return res;
 }
 #endif
 static int __Pyx_PyErr_GivenExceptionMatchesTuple(PyObject *exc_type, PyObject *tuple) {
     Py_ssize_t i, n;
     assert(PyExceptionClass_Check(exc_type));
     n = PyTuple_GET_SIZE(tuple);
 #if PY_MAJOR_VERSION >= 3
@@ -9209,88 +5533,56 @@
     }
     return (PyErr_GivenExceptionMatches(err, exc_type1) || PyErr_GivenExceptionMatches(err, exc_type2));
 }
 #endif
 
 /* CheckBinaryVersion */
 static int __Pyx_check_binary_version(void) {
-    char ctversion[5];
-    int same=1, i, found_dot;
-    const char* rt_from_call = Py_GetVersion();
-    PyOS_snprintf(ctversion, 5, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
-    found_dot = 0;
-    for (i = 0; i < 4; i++) {
-        if (!ctversion[i]) {
-            same = (rt_from_call[i] < '0' || rt_from_call[i] > '9');
-            break;
-        }
-        if (rt_from_call[i] != ctversion[i]) {
-            same = 0;
-            break;
-        }
-    }
-    if (!same) {
-        char rtversion[5] = {'\0'};
+    char ctversion[4], rtversion[4];
+    PyOS_snprintf(ctversion, 4, "%d.%d", PY_MAJOR_VERSION, PY_MINOR_VERSION);
+    PyOS_snprintf(rtversion, 4, "%s", Py_GetVersion());
+    if (ctversion[0] != rtversion[0] || ctversion[2] != rtversion[2]) {
         char message[200];
-        for (i=0; i<4; ++i) {
-            if (rt_from_call[i] == '.') {
-                if (found_dot) break;
-                found_dot = 1;
-            } else if (rt_from_call[i] < '0' || rt_from_call[i] > '9') {
-                break;
-            }
-            rtversion[i] = rt_from_call[i];
-        }
         PyOS_snprintf(message, sizeof(message),
-                      "compile time version %s of module '%.100s' "
+                      "compiletime version %s of module '%.100s' "
                       "does not match runtime version %s",
                       ctversion, __Pyx_MODULE_NAME, rtversion);
         return PyErr_WarnEx(NULL, message, 1);
     }
     return 0;
 }
 
 /* InitStrings */
-#if PY_MAJOR_VERSION >= 3
-static int __Pyx_InitString(__Pyx_StringTabEntry t, PyObject **str) {
-    if (t.is_unicode | t.is_str) {
-        if (t.intern) {
-            *str = PyUnicode_InternFromString(t.s);
-        } else if (t.encoding) {
-            *str = PyUnicode_Decode(t.s, t.n - 1, t.encoding, NULL);
-        } else {
-            *str = PyUnicode_FromStringAndSize(t.s, t.n - 1);
-        }
-    } else {
-        *str = PyBytes_FromStringAndSize(t.s, t.n - 1);
-    }
-    if (!*str)
-        return -1;
-    if (PyObject_Hash(*str) == -1)
-        return -1;
-    return 0;
-}
-#endif
 static int __Pyx_InitStrings(__Pyx_StringTabEntry *t) {
     while (t->p) {
-        #if PY_MAJOR_VERSION >= 3
-        __Pyx_InitString(*t, t->p);
-        #else
+        #if PY_MAJOR_VERSION < 3
         if (t->is_unicode) {
             *t->p = PyUnicode_DecodeUTF8(t->s, t->n - 1, NULL);
         } else if (t->intern) {
             *t->p = PyString_InternFromString(t->s);
         } else {
             *t->p = PyString_FromStringAndSize(t->s, t->n - 1);
         }
+        #else
+        if (t->is_unicode | t->is_str) {
+            if (t->intern) {
+                *t->p = PyUnicode_InternFromString(t->s);
+            } else if (t->encoding) {
+                *t->p = PyUnicode_Decode(t->s, t->n - 1, t->encoding, NULL);
+            } else {
+                *t->p = PyUnicode_FromStringAndSize(t->s, t->n - 1);
+            }
+        } else {
+            *t->p = PyBytes_FromStringAndSize(t->s, t->n - 1);
+        }
+        #endif
         if (!*t->p)
             return -1;
         if (PyObject_Hash(*t->p) == -1)
             return -1;
-        #endif
         ++t;
     }
     return 0;
 }
 
 static CYTHON_INLINE PyObject* __Pyx_PyUnicode_FromString(const char* c_str) {
     return __Pyx_PyUnicode_FromStringAndSize(c_str, (Py_ssize_t)strlen(c_str));
@@ -9344,15 +5636,15 @@
 #if PY_MAJOR_VERSION < 3 && __PYX_DEFAULT_STRING_ENCODING_IS_ASCII
             __Pyx_sys_getdefaultencoding_not_ascii &&
 #endif
             PyUnicode_Check(o)) {
         return __Pyx_PyUnicode_AsStringAndSize(o, length);
     } else
 #endif
-#if (!CYTHON_COMPILING_IN_PYPY && !CYTHON_COMPILING_IN_LIMITED_API) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
+#if (!CYTHON_COMPILING_IN_PYPY) || (defined(PyByteArray_AS_STRING) && defined(PyByteArray_GET_SIZE))
     if (PyByteArray_Check(o)) {
         *length = PyByteArray_GET_SIZE(o);
         return PyByteArray_AS_STRING(o);
     } else
 #endif
     {
         char* result;
@@ -9373,34 +5665,30 @@
     int retval;
     if (unlikely(!x)) return -1;
     retval = __Pyx_PyObject_IsTrue(x);
     Py_DECREF(x);
     return retval;
 }
 static PyObject* __Pyx_PyNumber_IntOrLongWrongResultType(PyObject* result, const char* type_name) {
-    __Pyx_TypeName result_type_name = __Pyx_PyType_GetName(Py_TYPE(result));
 #if PY_MAJOR_VERSION >= 3
     if (PyLong_Check(result)) {
         if (PyErr_WarnFormat(PyExc_DeprecationWarning, 1,
-                "__int__ returned non-int (type " __Pyx_FMT_TYPENAME ").  "
-                "The ability to return an instance of a strict subclass of int is deprecated, "
-                "and may be removed in a future version of Python.",
-                result_type_name)) {
-            __Pyx_DECREF_TypeName(result_type_name);
+                "__int__ returned non-int (type %.200s).  "
+                "The ability to return an instance of a strict subclass of int "
+                "is deprecated, and may be removed in a future version of Python.",
+                Py_TYPE(result)->tp_name)) {
             Py_DECREF(result);
             return NULL;
         }
-        __Pyx_DECREF_TypeName(result_type_name);
         return result;
     }
 #endif
     PyErr_Format(PyExc_TypeError,
-                 "__%.4s__ returned non-%.4s (type " __Pyx_FMT_TYPENAME ")",
-                 type_name, type_name, result_type_name);
-    __Pyx_DECREF_TypeName(result_type_name);
+                 "__%.4s__ returned non-%.4s (type %.200s)",
+                 type_name, type_name, Py_TYPE(result)->tp_name);
     Py_DECREF(result);
     return NULL;
 }
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x) {
 #if CYTHON_USE_TYPE_SLOTS
   PyNumberMethods *m;
 #endif
@@ -9458,19 +5746,21 @@
         return PyInt_AS_LONG(b);
     else
         return PyInt_AsSsize_t(b);
   }
 #endif
   if (likely(PyLong_CheckExact(b))) {
     #if CYTHON_USE_PYLONG_INTERNALS
-    if (likely(__Pyx_PyLong_IsCompact(b))) {
-        return __Pyx_PyLong_CompactValue(b);
+    const digit* digits = ((PyLongObject*)b)->ob_digit;
+    const Py_ssize_t size = Py_SIZE(b);
+    if (likely(__Pyx_sst_abs(size) <= 1)) {
+        ival = likely(size) ? digits[0] : 0;
+        if (size == -1) ival = -ival;
+        return ival;
     } else {
-      const digit* digits = __Pyx_PyLong_Digits(b);
-      const Py_ssize_t size = __Pyx_PyLong_SignedDigitCount(b);
       switch (size) {
          case 2:
            if (8 * sizeof(Py_ssize_t) > 2 * PyLong_SHIFT) {
              return (Py_ssize_t) (((((size_t)digits[1]) << PyLong_SHIFT) | (size_t)digits[0]));
            }
            break;
          case -2:
@@ -9505,41 +5795,16 @@
   }
   x = PyNumber_Index(b);
   if (!x) return -1;
   ival = PyInt_AsSsize_t(x);
   Py_DECREF(x);
   return ival;
 }
-static CYTHON_INLINE Py_hash_t __Pyx_PyIndex_AsHash_t(PyObject* o) {
-  if (sizeof(Py_hash_t) == sizeof(Py_ssize_t)) {
-    return (Py_hash_t) __Pyx_PyIndex_AsSsize_t(o);
-#if PY_MAJOR_VERSION < 3
-  } else if (likely(PyInt_CheckExact(o))) {
-    return PyInt_AS_LONG(o);
-#endif
-  } else {
-    Py_ssize_t ival;
-    PyObject *x;
-    x = PyNumber_Index(o);
-    if (!x) return -1;
-    ival = PyInt_AsLong(x);
-    Py_DECREF(x);
-    return ival;
-  }
-}
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b) {
   return b ? __Pyx_NewRef(Py_True) : __Pyx_NewRef(Py_False);
 }
 static CYTHON_INLINE PyObject * __Pyx_PyInt_FromSize_t(size_t ival) {
     return PyInt_FromSize_t(ival);
 }
 
 
-/* #### Code section: utility_code_pragmas_end ### */
-#ifdef _MSC_VER
-#pragma warning( pop )
-#endif
-
-
-
-/* #### Code section: end ### */
 #endif /* Py_PYTHON_H */
```

### Comparing `camSort-0.2.7/camSort.egg-info/PKG-INFO` & `camSort-0.2.8/camSort.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 Metadata-Version: 2.1
 Name: camSort
-Version: 0.2.7
+Version: 0.2.8
 Summary: make sorted() fast for strings
+Home-page: UNKNOWN
 Author: ['cameronbae / cameron jay']
 Author-email: <contact@camjay.io>
+License: UNKNOWN
+Description: 
+        # camSort
+        
+        Working on `python 3.7.1`!
+        
+        `camSort` is a Python library that makes sorted() look slow while also using sorted(). It's built on Cython, and provides preallocation to string sorting by using a custom key calculation for each string. Normal key calculation and object creation are often computationally expensive—but here we optimize that with Cython >:)!
+        
+        ## Overview
+        
+        The `camSort` library sorts a list of strings by creating a custom object for each string. This custom object, `StringWithKey`, holds the string and a unique key calculated from it. The key is a long integer derived from the sum of Unicode code points of the characters in the string, and the string's length.
+        
+        The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
+        
+        The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
+        
+        ## Installation
+        
+        ```pip install camSort``` or compile locally :)
+        
+        ## Usage
+        
+        ```python
+        import camSort
+        # or
+        from camSort import sortStrings
+        
+        myList = ['your', 'list', 'of', 'strings', ':)!']
+        
+        sortedStrings = camSort.sortStrings(myList)
+        # or
+        sortedStrings = sortStrings(myList)
+        
+        ```
+        
+        ## Performance
+        
+        Average output on my 2017 macbook pro:
+            (1 million strings, with a random legnth of 1 to 1000 chararacters)
+        
+        Time taken by Python sorted(): 56.08621883392334 seconds
+        Time taken by camSort: 6.356221914291382 seconds
 Keywords: python,sorted,sort,camSort
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-
-
-# camSort
-
-Working on `python 3.7.1`!
-
-`camSort` is a Python library that makes sorted() look slow while also using sorted(). It's built on Cython, and provides preallocation to string sorting by using a custom key calculation for each string. Normal key calculation and object creation are often computationally expensive—but here we optimize that with Cython >:)!
-
-## Overview
-
-The `camSort` library sorts a list of strings by creating a custom object for each string. This custom object, `StringWithKey`, holds the string and a unique key calculated from it. The key is a long integer derived from the sum of Unicode code points of the characters in the string, and the string's length.
-
-The actual sorting operation uses Python's built-in `sorted` function (based on Timsort), however, now with precalculated keys, rather than comparing the strings themselves. Making sorting quite faster.
-
-The primary benefit of using `camSort` is realized when working with very large lists of strings, see: Performance).
-
-## Installation
-
-```pip install camSort``` or compile locally :)
-
-## Usage
-
-```python
-import camSort
-# or
-from camSort import sortStrings
-
-myList = ['your', 'list', 'of', 'strings', ':)!']
-
-sortedStrings = camSort.sortStrings(myList)
-# or
-sortedStrings = sortStrings(myList)
-
-```
-
-## Performance
-
-Average output on my 2017 macbook pro:
-    (1 million strings, with a random legnth of 1 to 1000 chararacters)
-
-Time taken by Python sorted(): 56.08621883392334 seconds
-Time taken by camSort: 6.356221914291382 seconds
```

### Comparing `camSort-0.2.7/setup.py` & `camSort-0.2.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,36 @@
-from setuptools import setup, find_packages
+from setuptools import Extension
 from Cython.Build import cythonize
 import codecs
 import os
+from distutils.core import setup
 
-here = os.path.abspath(os.path.dirname(__file__))
 
 LONG_DESCRIPTION = ''
 
-with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
+with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
+
     name="camSort",
-    version="0.2.7",
-    packages=find_packages(),
+    version="0.2.8",
     install_requires=["setuptools", "wheel", "cython"],
-    ext_modules = cythonize('camSort/camSort.pyx'),
-    package_data={'camSort': ['*.pyx']},
+
+    ext_modules = cythonize(['camSort/stringSort.pyx']),
+
     author=["cameronbae / cameron jay"],
     author_email="<contact@camjay.io>",
     description="make sorted() fast for strings",
     long_description_content_type="text/markdown",
     long_description=long_description,
     keywords=['python', 'sorted', 'sort', 'camSort'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
     ],
-)
+)
+
```

