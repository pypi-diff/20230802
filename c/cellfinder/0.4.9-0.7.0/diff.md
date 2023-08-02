# Comparing `tmp/cellfinder-0.4.9.tar.gz` & `tmp/cellfinder-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellfinder-0.4.9.tar", last modified: Wed Mar 10 19:55:18 2021, max compression
+gzip compressed data, was "cellfinder-0.7.0.tar", last modified: Wed Aug  2 11:38:10 2023, max compression
```

## Comparing `cellfinder-0.4.9.tar` & `cellfinder-0.7.0.tar`

### file list

```diff
@@ -1,218 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.474750 cellfinder-0.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.446750 cellfinder-0.4.9/.eggs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.446750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.446750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.450750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Compiler/
--rw-r--r--   0 runner    (1001) docker     (116)     3321 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Compiler/Code.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2918 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Compiler/FlowControl.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2468 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Compiler/ParseTreeTransforms.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     8984 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Compiler/Parsing.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2113 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Compiler/Scanning.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1792 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Compiler/Visitor.pxd
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.450750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.454750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/
--rw-r--r--   0 runner    (1001) docker     (116)       61 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       66 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_bool.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       67 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_bytes.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_cobject.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_complex.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       66 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_dict.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       65 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_exc.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       67 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_float.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       70 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_function.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_getargs.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       70 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_instance.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       65 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_int.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       70 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_iterator.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       66 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_list.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       66 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_long.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_mapping.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       65 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_mem.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_method.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_module.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_number.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_object.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       71 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_oldbuffer.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       71 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_pycapsule.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       65 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_ref.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       70 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_sequence.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       65 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_set.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       68 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_string.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       67 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_tuple.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       66 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_type.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_unicode.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_version.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       69 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/python_weakref.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       64 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/stdio.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       65 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/stdlib.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2187 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/Deprecated/stl.pxd
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.462750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/
--rw-r--r--   0 runner    (1001) docker     (116)     8254 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     6056 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/array.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1359 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/bool.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     4870 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/buffer.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1443 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/bytearray.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     9906 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/bytes.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1390 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/cellobject.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      236 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/ceval.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1524 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/cobject.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     5084 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/codecs.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1777 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/complex.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1696 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/conversion.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     6776 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/datetime.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     6877 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/dict.pxd
--rw-r--r--   0 runner    (1001) docker     (116)    13606 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/exc.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1424 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/float.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2671 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/function.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1052 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/genobject.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      775 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/getargs.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      985 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/instance.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     4131 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/int.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1319 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/iterator.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1036 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/iterobject.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     4084 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/list.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     7051 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/long.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      445 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/longintrepr.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2693 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/mapping.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     5386 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/mem.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2504 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/memoryview.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2196 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/method.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     9226 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/module.pxd
--rw-r--r--   0 runner    (1001) docker     (116)    11922 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/number.pxd
--rw-r--r--   0 runner    (1001) docker     (116)    18366 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/object.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2916 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/oldbuffer.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     5692 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/pycapsule.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2000 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/pylifecycle.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3683 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/pystate.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1946 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/pythread.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2557 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/ref.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     6008 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/sequence.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     5383 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/set.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3111 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/slice.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     9944 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/string.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3206 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/tuple.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1831 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/type.pxd
--rw-r--r--   0 runner    (1001) docker     (116)    26247 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/unicode.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      847 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/version.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1984 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/cpython/weakref.pxd
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.462750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2050 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/errno.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      966 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/float.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      621 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/limits.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1140 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/locale.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2948 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/math.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      297 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/setjmp.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1170 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/signal.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      164 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/stddef.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3449 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/stdint.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2476 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/stdio.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2444 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/stdlib.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2038 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/string.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1317 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libc/time.pxd
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.466750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/
--rw-r--r--   0 runner    (1001) docker     (116)       94 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1770 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/algorithm.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      501 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/cast.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3012 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/complex.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3106 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/deque.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2392 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/forward_list.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      381 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/functional.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1432 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/iterator.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1661 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/limits.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2658 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/list.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2551 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/map.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3600 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/memory.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       27 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/pair.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      649 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/queue.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2170 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/set.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      292 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/stack.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     5071 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/string.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      524 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/typeindex.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      304 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/typeinfo.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2867 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/unordered_map.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     2622 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/unordered_set.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      903 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/utility.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3350 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/libcpp/vector.pxd
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.466750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/numpy/
--rw-r--r--   0 runner    (1001) docker     (116)    38138 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/numpy/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     5807 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/numpy/math.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1713 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/openmp.pxd
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.466750 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/
--rw-r--r--   0 runner    (1001) docker     (116)       13 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      355 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/dlfcn.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1194 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/fcntl.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       99 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/ioctl.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     3362 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/mman.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1254 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/resource.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      546 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/select.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1876 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/signal.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1734 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/stat.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1054 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/stdio.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      934 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/stdlib.pxd
--rw-r--r--   0 runner    (1001) docker     (116)      374 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/strings.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1980 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/time.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1162 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/types.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     8061 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/unistd.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1244 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Includes/posix/wait.pxd
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Plex/
--rw-r--r--   0 runner    (1001) docker     (116)      585 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Plex/Actions.pxd
--rw-r--r--   0 runner    (1001) docker     (116)     1481 2021-03-10 19:55:17.000000 cellfinder-0.4.9/.eggs/Cython-0.29.22-py3.9-linux-x86_64.egg/Cython/Plex/Scanners.pxd
--rw-r--r--   0 runner    (1001) docker     (116)       48 2021-03-10 19:55:03.000000 cellfinder-0.4.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     7928 2021-03-10 19:55:18.474750 cellfinder-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     5918 2021-03-10 19:55:03.000000 cellfinder-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/cellfinder/
--rw-r--r--   0 runner    (1001) docker     (116)      110 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/cellfinder/analyse/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/analyse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     9177 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/analyse/analyse.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/cellfinder/export/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      203 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/export/to_brainrender.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/cellfinder/extract/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15918 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/extract/extract_cubes.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/cellfinder/figures/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/figures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      386 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/figures/figures.py
--rw-r--r--   0 runner    (1001) docker     (116)     1920 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/figures/heatmap.py
--rw-r--r--   0 runner    (1001) docker     (116)     6430 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/main.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/cellfinder/tools/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2259 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/tools/image_processing.py
--rw-r--r--   0 runner    (1001) docker     (116)    13543 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/tools/parser.py
--rw-r--r--   0 runner    (1001) docker     (116)    10987 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/tools/prep.py
--rw-r--r--   0 runner    (1001) docker     (116)     2221 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/tools/system.py
--rw-r--r--   0 runner    (1001) docker     (116)     3627 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/cellfinder/train/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10595 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/train/curation.py
--rw-r--r--   0 runner    (1001) docker     (116)     8953 2021-03-10 19:55:03.000000 cellfinder-0.4.9/cellfinder/train/curation_old.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.470749 cellfinder-0.4.9/cellfinder.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     7928 2021-03-10 19:55:17.000000 cellfinder-0.4.9/cellfinder.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    13180 2021-03-10 19:55:18.000000 cellfinder-0.4.9/cellfinder.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-10 19:55:17.000000 cellfinder-0.4.9/cellfinder.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      163 2021-03-10 19:55:17.000000 cellfinder-0.4.9/cellfinder.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-10 19:55:17.000000 cellfinder-0.4.9/cellfinder.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      354 2021-03-10 19:55:17.000000 cellfinder-0.4.9/cellfinder.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       27 2021-03-10 19:55:17.000000 cellfinder-0.4.9/cellfinder.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      283 2021-03-10 19:55:03.000000 cellfinder-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      420 2021-03-10 19:55:18.474750 cellfinder-0.4.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2490 2021-03-10 19:55:03.000000 cellfinder-0.4.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.446750 cellfinder-0.4.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.446750 cellfinder-0.4.9/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.474750 cellfinder-0.4.9/tests/data/config/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:03.000000 cellfinder-0.4.9/tests/data/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.474750 cellfinder-0.4.9/tests/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1587 2021-03-10 19:55:04.000000 cellfinder-0.4.9/tests/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.474750 cellfinder-0.4.9/tests/tests/test_integration/
--rw-r--r--   0 runner    (1001) docker     (116)     1741 2021-03-10 19:55:04.000000 cellfinder-0.4.9/tests/tests/test_integration/test_detection.py
--rw-r--r--   0 runner    (1001) docker     (116)     4897 2021-03-10 19:55:04.000000 cellfinder-0.4.9/tests/tests/test_integration/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (116)     2920 2021-03-10 19:55:04.000000 cellfinder-0.4.9/tests/tests/test_integration/test_registration.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.450750 cellfinder-0.4.9/tests/tests/test_unit/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-10 19:55:18.474750 cellfinder-0.4.9/tests/tests/test_unit/test_tools/
--rw-r--r--   0 runner    (1001) docker     (116)     1097 2021-03-10 19:55:04.000000 cellfinder-0.4.9/tests/tests/test_unit/test_tools/test_image_processing.py
--rw-r--r--   0 runner    (1001) docker     (116)     6741 2021-03-10 19:55:04.000000 cellfinder-0.4.9/tests/tests/test_unit/test_tools/test_prep.py
--rw-r--r--   0 runner    (1001) docker     (116)     2840 2021-03-10 19:55:04.000000 cellfinder-0.4.9/tests/tests/test_unit/test_tools/test_system.py
--rw-r--r--   0 runner    (1001) docker     (116)     1751 2021-03-10 19:55:04.000000 cellfinder-0.4.9/tests/tests/test_unit/test_tools/test_tools_general.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.793478 cellfinder-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-08-02 11:37:55.000000 cellfinder-0.7.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-08-02 11:37:55.000000 cellfinder-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-02 11:37:55.000000 cellfinder-0.7.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-08-02 11:37:55.000000 cellfinder-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-02 11:37:55.000000 cellfinder-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-08-02 11:38:10.793478 cellfinder-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7886 2023-08-02 11:37:55.000000 cellfinder-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.789478 cellfinder-0.7.0/cellfinder/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.789478 cellfinder-0.7.0/cellfinder/analyse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/analyse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11010 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/analyse/analyse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.789478 cellfinder-0.7.0/cellfinder/export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/export/abc4d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/export/brainrender.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/export/export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.789478 cellfinder-0.7.0/cellfinder/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/extract/extract_cubes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.789478 cellfinder-0.7.0/cellfinder/figures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/figures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/figures/figures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1951 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/figures/heatmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.793478 cellfinder-0.7.0/cellfinder/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/tools/image_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13567 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/tools/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11119 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/tools/prep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/tools/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3627 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.793478 cellfinder-0.7.0/cellfinder/train/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10588 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/train/curation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9019 2023-08-02 11:37:55.000000 cellfinder-0.7.0/cellfinder/train/curation_old.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 11:38:10.789478 cellfinder-0.7.0/cellfinder.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9002 2023-08-02 11:38:09.000000 cellfinder-0.7.0/cellfinder.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-08-02 11:38:10.000000 cellfinder-0.7.0/cellfinder.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:38:09.000000 cellfinder-0.7.0/cellfinder.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-02 11:38:09.000000 cellfinder-0.7.0/cellfinder.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 11:38:09.000000 cellfinder-0.7.0/cellfinder.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-08-02 11:38:09.000000 cellfinder-0.7.0/cellfinder.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-02 11:38:09.000000 cellfinder-0.7.0/cellfinder.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-02 11:37:55.000000 cellfinder-0.7.0/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-02 11:37:55.000000 cellfinder-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-02 11:37:55.000000 cellfinder-0.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-08-02 11:38:10.793478 cellfinder-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-08-02 11:37:55.000000 cellfinder-0.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-08-02 11:37:57.000000 cellfinder-0.7.0/tox.ini
```

### Comparing `cellfinder-0.4.9/PKG-INFO` & `cellfinder-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,144 +1,176 @@
 Metadata-Version: 2.1
 Name: cellfinder
-Version: 0.4.9
+Version: 0.7.0
 Summary: Automated 3D cell detection and registration of whole-brain images
-Home-page: https://cellfinder.info
+Home-page: https://brainglobe.info/cellfinder
 Author: Adam Tyson, Christian Niedworok, Charly Rousseau
-Author-email: adam.tyson@ucl.ac.uk
-License: UNKNOWN
+Author-email: code@adamltyson.com
 Project-URL: Source Code, https://github.com/brainglobe/cellfinder
 Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
 Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
-Description: [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
-        [![PyPI](https://img.shields.io/pypi/v/cellfinder.svg)](https://pypi.org/project/cellfinder)
-        [![Downloads](https://pepy.tech/badge/cellfinder)](https://pepy.tech/project/cellfinder)
-        [![Wheel](https://img.shields.io/pypi/wheel/cellfinder.svg)](https://pypi.org/project/cellfinder)
-        [![Development Status](https://img.shields.io/pypi/status/cellfinder.svg)](https://github.com/brainglobe/cellfinder)
-        [![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder/tests)](
-            https://github.com/brainglobe/cellfinder/actions)
-        [![Coverage Status](https://coveralls.io/repos/github/brainglobe/cellfinder/badge.svg?branch=master)](https://coveralls.io/github/brainglobe/cellfinder?branch=master)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-        [![Gitter](https://badges.gitter.im/brainglobe.svg)](https://gitter.im/BrainGlobe/cellfinder/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3891338.svg)](https://doi.org/10.5281/zenodo.3891338)
-        [![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
-        [![Website](https://img.shields.io/website?up_message=online&url=https%3A%2F%2Fcellfinder.info)](https://cellfinder.info)
-        [![Twitter](https://img.shields.io/twitter/follow/findingcells?style=social)](https://twitter.com/findingcells)
-        # Cellfinder
-        Whole-brain cell detection, registration and analysis.
-        
-        ---
-        
-        
-        Cellfinder is a collection of tools from the 
-        [Margrie Lab](https://www.sainsburywellcome.org/web/groups/margrie-lab) and
-         others at the [Sainsbury Wellcome Centre](https://www.sainsburywellcome.org/web/), [UCL](https://www.ucl.ac.uk/)
-         for the analysis of whole-brain imaging data such as 
-         [serial-section imaging](https://sainsburywellcomecentre.github.io/OpenSerialSection/)
-         and lightsheet imaging in cleared tissue.
-         
-         The aim is to provide a single solution for:
-         
-         * Cell detection (initial cell candidate detection and refinement using 
-         deep learning).
-         * Atlas registration (using [brainreg](https://github.com/brainglobe/brainreg))
-         * Analysis of cell positions in a common space
-         
-        Installation is with 
-        `pip install cellfinder`.
-        
-        Basic usage:
-        ```bash
-        cellfinder -s signal_images -b background_images -o output_dir --metadata metadata
-        ```
-        Full documentation can be 
-        found [here](https://docs.brainglobe.info/cellfinder).
-         
-        This software is at a very early stage, and was written with our data in mind. 
-        Over time we hope to support other data types/formats. If you have any 
-        questions or issues, please get in touch by 
-        [email](mailto:adam.tyson@ucl.ac.uk?subject=cellfinder), 
-        [gitter](https://gitter.im/BrainGlobe/cellfinder) or by 
-        [raising an issue](https://github.com/brainglobe/cellfinder/issues/new/choose).
-        
-        
-        ---
-        ## Illustration
-        
-        ### Introduction
-        cellfinder takes a stitched, but otherwise raw whole-brain dataset with at least 
-        two channels:
-         * Background channel (i.e. autofluorescence)
-         * Signal channel, the one with the cells to be detected:
-         
-        ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/raw.png)
-        **Raw coronal serial two-photon mouse brain image showing labelled cells**
-        
-        
-        ### Cell candidate detection
-        Classical image analysis (e.g. filters, thresholding) is used to find 
-        cell-like objects (with false positives):
-        
-        ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/detect.png)
-        **Candidate cells (including many artefacts)**
-        
-        
-        ### Cell candidate classification
-        A deep-learning network (ResNet) is used to classify cell candidates as true 
-        cells or artefacts:
-        
-        ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/classify.png)
-        **Cassified cell candidates. Yellow - cells, Blue - artefacts**
-        
-        ### Registration and segmentation (brainreg)
-        Using [brainreg](https://github.com/brainglobe/brainreg), 
-        cellfinder aligns a template brain and atlas annotations (e.g. 
-        the Allen Reference Atlas, ARA) to the sample allowing detected cells to be assigned 
-        a brain region.
-        
-        This transformation can be inverted, allowing detected cells to be
-        transformed to a standard anatomical space.
-        
-        ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/register.png)
-        **ARA overlaid on sample image**
-        
-        ### Analysis of cell positions in a common anatomical space
-        Registration to a template allows for powerful group-level analysis of cellular
-        disributions. *(Example to come)*
-        
-        ## Examples
-        *(more to come)*
-        
-        ### Tracing of inputs to retrosplenial cortex (RSP)
-        Input cell somas detected by cellfinder, aligned to the Allen Reference Atlas, 
-        and visualised in [brainrender](https://github.com/brancolab/brainrender) along 
-        with RSP.
-        
-        ![brainrender](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/brainrender.png)
-        
-        Data courtesy of Sepiedeh Keshavarzi and Chryssanthi Tsitoura. [Details here](https://www.youtube.com/watch?v=pMHP0o-KsoQ)
-        
-        
-        ## Citing cellfinder
-        
-        If you find cellfinder useful, and use it in your research, please cite the preprint outlining the cell detection algorithm:
-        > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ bioRxiv, [doi.org/10.1101/2020.10.21.348771](https://doi.org/10.1101/2020.10.21.348771)
-        
-        If you use any of the image registration functions in cellfinder, please also cite [brainreg](https://github.com/brainglobe/brainreg#citing-brainreg).
-        
-        **If you use this, or any other tools in the brainglobe suite, please
-         [let us know](mailto:adam.tyson@ucl.ac.uk?subject=cellfinder), and 
-         we'd be happy to promote your paper/talk etc.**
-        
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows :: Windows 10
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: napari
 Provides-Extra: dev
+License-File: LICENSE
+
+[![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![PyPI](https://img.shields.io/pypi/v/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Downloads](https://pepy.tech/badge/cellfinder)](https://pepy.tech/project/cellfinder)
+[![Wheel](https://img.shields.io/pypi/wheel/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Development Status](https://img.shields.io/pypi/status/cellfinder.svg)](https://github.com/brainglobe/cellfinder)
+[![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder/tests)](
+    https://github.com/brainglobe/cellfinder/actions)
+[![codecov](https://codecov.io/gh/brainglobe/cellfinder/branch/master/graph/badge.svg?token=s3MweEFPhl)](https://codecov.io/gh/brainglobe/cellfinder)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
+[![Website](https://img.shields.io/website?up_message=online&url=https%3A%2F%2Fbrainglobe.info)](https://brainglobe.info/documentation/cellfinder/index.html)
+[![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
+
+# Cellfinder
+Whole-brain cell detection, registration and analysis.
+
+**N.B. If you want to just use the cell detection part of cellfinder, please
+see the standalone [cellfinder-core](https://github.com/brainglobe/cellfinder-core)
+package, or the [cellfinder plugin](https://github.com/brainglobe/cellfinder-napari)
+for [napari](https://napari.org/).**
+
+---
+`cellfinder` is a collection of tools developed by [Adam Tyson](https://github.com/adamltyson), [Charly Rousseau](https://github.com/crousseau) and [Christian Niedworok](https://github.com/cniedwor) in the [Margrie Lab](https://www.sainsburywellcome.org/web/groups/margrie-lab), generously supported by the [Sainsbury Wellcome Centre](https://www.sainsburywellcome.org/web/).
+
+`cellfinder` is a designed for the analysis of whole-brain imaging data such as
+ [serial-section imaging](https://sainsburywellcomecentre.github.io/OpenSerialSection/)
+ and lightsheet imaging in cleared tissue. The aim is to provide a single solution for:
+
+ * Cell detection (initial cell candidate detection and refinement using
+ deep learning) (using [cellfinder-core](https://github.com/brainglobe/cellfinder-core))
+ * Atlas registration (using [brainreg](https://github.com/brainglobe/brainreg))
+ * Analysis of cell positions in a common space
+
+ ---
+Installation is with
+`pip install cellfinder`
+
+---
+Basic usage:
+```bash
+cellfinder -s signal_images -b background_images -o output_dir --metadata metadata
+```
+Full documentation can be
+found [here](https://brainglobe.info/documentation/cellfinder/index.html).
+
+This software is at a very early stage, and was written with our data in mind.
+Over time we hope to support other data types/formats. If you have any issues, please get in touch [on the forum](https://forum.image.sc/tag/brainglobe) or by
+[raising an issue](https://github.com/brainglobe/cellfinder/issues/new/choose).
+
+
+---
+## Illustration
+
+### Introduction
+cellfinder takes a stitched, but otherwise raw whole-brain dataset with at least
+two channels:
+ * Background channel (i.e. autofluorescence)
+ * Signal channel, the one with the cells to be detected:
+
+![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/raw.png)
+**Raw coronal serial two-photon mouse brain image showing labelled cells**
+
+
+### Cell candidate detection
+Classical image analysis (e.g. filters, thresholding) is used to find
+cell-like objects (with false positives):
+
+![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/detect.png)
+**Candidate cells (including many artefacts)**
+
+
+### Cell candidate classification
+A deep-learning network (ResNet) is used to classify cell candidates as true
+cells or artefacts:
+
+![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/classify.png)
+**Cassified cell candidates. Yellow - cells, Blue - artefacts**
+
+### Registration and segmentation (brainreg)
+Using [brainreg](https://github.com/brainglobe/brainreg),
+cellfinder aligns a template brain and atlas annotations (e.g.
+the Allen Reference Atlas, ARA) to the sample allowing detected cells to be assigned
+a brain region.
+
+This transformation can be inverted, allowing detected cells to be
+transformed to a standard anatomical space.
+
+![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/register.png)
+**ARA overlaid on sample image**
+
+### Analysis of cell positions in a common anatomical space
+Registration to a template allows for powerful group-level analysis of cellular
+disributions. *(Example to come)*
+
+## Examples
+*(more to come)*
+
+### Tracing of inputs to retrosplenial cortex (RSP)
+Input cell somas detected by cellfinder, aligned to the Allen Reference Atlas,
+and visualised in [brainrender](https://github.com/brainglobe/brainrender) along
+with RSP.
+
+![brainrender](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/brainrender.png)
+
+Data courtesy of Sepiedeh Keshavarzi and Chryssanthi Tsitoura. [Details here](https://www.youtube.com/watch?v=pMHP0o-KsoQ)
+
+## Visualisation
+
+cellfinder comes with a plugin ([brainglobe-napari-io](https://github.com/brainglobe/brainglobe-napari-io)) for [napari](https://github.com/napari/napari) to view your data
+
+#### Usage
+* Open napari (however you normally do it, but typically just type `napari` into your terminal, or click on your desktop icon)
+
+#### Load cellfinder XML file
+* Load your raw data (drag and drop the data directories into napari, one at a time)
+* Drag and drop your cellfinder XML file (e.g. `cell_classification.xml`) into napari.
+
+#### Load cellfinder directory
+* Load your raw data (drag and drop the data directories into napari, one at a time)
+* Drag and drop your cellfinder output directory into napari.
+
+The plugin will then load your detected cells (in yellow) and the rejected cell
+candidates (in blue). If you carried out registration, then these results will be
+overlaid (similarly to the loading brainreg data, but transformed to the
+coordinate space of your raw data).
+
+![load_data](https://raw.githubusercontent.com/brainglobe/brainglobe-napari-io/master/resources/load_data.gif)
+**Loading raw data**
+
+![load_data](https://raw.githubusercontent.com/brainglobe/brainglobe-napari-io/master/resources/load_results.gif)
+**Loading cellfinder results**
+
+
+## Contributing
+Contributions to cellfinder are more than welcome. Please see the [developers guide](https://brainglobe.info/developers/index.html).
+
+
+## Citing cellfinder
+
+If you find cellfinder useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
+> Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
+[https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
+>
+If you use any of the image registration functions in cellfinder, please also cite [brainreg](https://github.com/brainglobe/brainreg#citing-brainreg).
+
+**If you use this, or any other tools in the brainglobe suite, please
+ [let us know](mailto:code@adamltyson.com?subject=cellfinder), and
+ we'd be happy to promote your paper/talk etc.**
```

### Comparing `cellfinder-0.4.9/README.md` & `cellfinder-0.7.0/cellfinder.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,117 @@
+Metadata-Version: 2.1
+Name: cellfinder
+Version: 0.7.0
+Summary: Automated 3D cell detection and registration of whole-brain images
+Home-page: https://brainglobe.info/cellfinder
+Author: Adam Tyson, Christian Niedworok, Charly Rousseau
+Author-email: code@adamltyson.com
+Project-URL: Source Code, https://github.com/brainglobe/cellfinder
+Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
+Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
+Classifier: Development Status :: 3 - Alpha
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 10
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Scientific/Engineering :: Image Recognition
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: napari
+Provides-Extra: dev
+License-File: LICENSE
+
 [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
 [![PyPI](https://img.shields.io/pypi/v/cellfinder.svg)](https://pypi.org/project/cellfinder)
 [![Downloads](https://pepy.tech/badge/cellfinder)](https://pepy.tech/project/cellfinder)
 [![Wheel](https://img.shields.io/pypi/wheel/cellfinder.svg)](https://pypi.org/project/cellfinder)
 [![Development Status](https://img.shields.io/pypi/status/cellfinder.svg)](https://github.com/brainglobe/cellfinder)
 [![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder/tests)](
     https://github.com/brainglobe/cellfinder/actions)
-[![Coverage Status](https://coveralls.io/repos/github/brainglobe/cellfinder/badge.svg?branch=master)](https://coveralls.io/github/brainglobe/cellfinder?branch=master)
+[![codecov](https://codecov.io/gh/brainglobe/cellfinder/branch/master/graph/badge.svg?token=s3MweEFPhl)](https://codecov.io/gh/brainglobe/cellfinder)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-[![Gitter](https://badges.gitter.im/brainglobe.svg)](https://gitter.im/BrainGlobe/cellfinder/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3891338.svg)](https://doi.org/10.5281/zenodo.3891338)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
-[![Website](https://img.shields.io/website?up_message=online&url=https%3A%2F%2Fcellfinder.info)](https://cellfinder.info)
-[![Twitter](https://img.shields.io/twitter/follow/findingcells?style=social)](https://twitter.com/findingcells)
+[![Website](https://img.shields.io/website?up_message=online&url=https%3A%2F%2Fbrainglobe.info)](https://brainglobe.info/documentation/cellfinder/index.html)
+[![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
+
 # Cellfinder
 Whole-brain cell detection, registration and analysis.
 
----
+**N.B. If you want to just use the cell detection part of cellfinder, please
+see the standalone [cellfinder-core](https://github.com/brainglobe/cellfinder-core)
+package, or the [cellfinder plugin](https://github.com/brainglobe/cellfinder-napari)
+for [napari](https://napari.org/).**
 
+---
+`cellfinder` is a collection of tools developed by [Adam Tyson](https://github.com/adamltyson), [Charly Rousseau](https://github.com/crousseau) and [Christian Niedworok](https://github.com/cniedwor) in the [Margrie Lab](https://www.sainsburywellcome.org/web/groups/margrie-lab), generously supported by the [Sainsbury Wellcome Centre](https://www.sainsburywellcome.org/web/).
 
-Cellfinder is a collection of tools from the 
-[Margrie Lab](https://www.sainsburywellcome.org/web/groups/margrie-lab) and
- others at the [Sainsbury Wellcome Centre](https://www.sainsburywellcome.org/web/), [UCL](https://www.ucl.ac.uk/)
- for the analysis of whole-brain imaging data such as 
+`cellfinder` is a designed for the analysis of whole-brain imaging data such as
  [serial-section imaging](https://sainsburywellcomecentre.github.io/OpenSerialSection/)
- and lightsheet imaging in cleared tissue.
- 
- The aim is to provide a single solution for:
- 
- * Cell detection (initial cell candidate detection and refinement using 
- deep learning).
+ and lightsheet imaging in cleared tissue. The aim is to provide a single solution for:
+
+ * Cell detection (initial cell candidate detection and refinement using
+ deep learning) (using [cellfinder-core](https://github.com/brainglobe/cellfinder-core))
  * Atlas registration (using [brainreg](https://github.com/brainglobe/brainreg))
  * Analysis of cell positions in a common space
- 
-Installation is with 
-`pip install cellfinder`.
 
+ ---
+Installation is with
+`pip install cellfinder`
+
+---
 Basic usage:
 ```bash
 cellfinder -s signal_images -b background_images -o output_dir --metadata metadata
 ```
-Full documentation can be 
-found [here](https://docs.brainglobe.info/cellfinder).
- 
-This software is at a very early stage, and was written with our data in mind. 
-Over time we hope to support other data types/formats. If you have any 
-questions or issues, please get in touch by 
-[email](mailto:adam.tyson@ucl.ac.uk?subject=cellfinder), 
-[gitter](https://gitter.im/BrainGlobe/cellfinder) or by 
+Full documentation can be
+found [here](https://brainglobe.info/documentation/cellfinder/index.html).
+
+This software is at a very early stage, and was written with our data in mind.
+Over time we hope to support other data types/formats. If you have any issues, please get in touch [on the forum](https://forum.image.sc/tag/brainglobe) or by
 [raising an issue](https://github.com/brainglobe/cellfinder/issues/new/choose).
 
 
 ---
 ## Illustration
 
 ### Introduction
-cellfinder takes a stitched, but otherwise raw whole-brain dataset with at least 
+cellfinder takes a stitched, but otherwise raw whole-brain dataset with at least
 two channels:
  * Background channel (i.e. autofluorescence)
  * Signal channel, the one with the cells to be detected:
- 
+
 ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/raw.png)
 **Raw coronal serial two-photon mouse brain image showing labelled cells**
 
 
 ### Cell candidate detection
-Classical image analysis (e.g. filters, thresholding) is used to find 
+Classical image analysis (e.g. filters, thresholding) is used to find
 cell-like objects (with false positives):
 
 ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/detect.png)
 **Candidate cells (including many artefacts)**
 
 
 ### Cell candidate classification
-A deep-learning network (ResNet) is used to classify cell candidates as true 
+A deep-learning network (ResNet) is used to classify cell candidates as true
 cells or artefacts:
 
 ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/classify.png)
 **Cassified cell candidates. Yellow - cells, Blue - artefacts**
 
 ### Registration and segmentation (brainreg)
-Using [brainreg](https://github.com/brainglobe/brainreg), 
-cellfinder aligns a template brain and atlas annotations (e.g. 
-the Allen Reference Atlas, ARA) to the sample allowing detected cells to be assigned 
+Using [brainreg](https://github.com/brainglobe/brainreg),
+cellfinder aligns a template brain and atlas annotations (e.g.
+the Allen Reference Atlas, ARA) to the sample allowing detected cells to be assigned
 a brain region.
 
 This transformation can be inverted, allowing detected cells to be
 transformed to a standard anatomical space.
 
 ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/register.png)
 **ARA overlaid on sample image**
@@ -94,26 +120,57 @@
 Registration to a template allows for powerful group-level analysis of cellular
 disributions. *(Example to come)*
 
 ## Examples
 *(more to come)*
 
 ### Tracing of inputs to retrosplenial cortex (RSP)
-Input cell somas detected by cellfinder, aligned to the Allen Reference Atlas, 
-and visualised in [brainrender](https://github.com/brancolab/brainrender) along 
+Input cell somas detected by cellfinder, aligned to the Allen Reference Atlas,
+and visualised in [brainrender](https://github.com/brainglobe/brainrender) along
 with RSP.
 
 ![brainrender](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/brainrender.png)
 
 Data courtesy of Sepiedeh Keshavarzi and Chryssanthi Tsitoura. [Details here](https://www.youtube.com/watch?v=pMHP0o-KsoQ)
 
+## Visualisation
 
-## Citing cellfinder
+cellfinder comes with a plugin ([brainglobe-napari-io](https://github.com/brainglobe/brainglobe-napari-io)) for [napari](https://github.com/napari/napari) to view your data
 
-If you find cellfinder useful, and use it in your research, please cite the preprint outlining the cell detection algorithm:
-> Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ bioRxiv, [doi.org/10.1101/2020.10.21.348771](https://doi.org/10.1101/2020.10.21.348771)
+#### Usage
+* Open napari (however you normally do it, but typically just type `napari` into your terminal, or click on your desktop icon)
+
+#### Load cellfinder XML file
+* Load your raw data (drag and drop the data directories into napari, one at a time)
+* Drag and drop your cellfinder XML file (e.g. `cell_classification.xml`) into napari.
+
+#### Load cellfinder directory
+* Load your raw data (drag and drop the data directories into napari, one at a time)
+* Drag and drop your cellfinder output directory into napari.
+
+The plugin will then load your detected cells (in yellow) and the rejected cell
+candidates (in blue). If you carried out registration, then these results will be
+overlaid (similarly to the loading brainreg data, but transformed to the
+coordinate space of your raw data).
+
+![load_data](https://raw.githubusercontent.com/brainglobe/brainglobe-napari-io/master/resources/load_data.gif)
+**Loading raw data**
+
+![load_data](https://raw.githubusercontent.com/brainglobe/brainglobe-napari-io/master/resources/load_results.gif)
+**Loading cellfinder results**
+
+
+## Contributing
+Contributions to cellfinder are more than welcome. Please see the [developers guide](https://brainglobe.info/developers/index.html).
+
+
+## Citing cellfinder
 
+If you find cellfinder useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
+> Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
+[https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
+>
 If you use any of the image registration functions in cellfinder, please also cite [brainreg](https://github.com/brainglobe/brainreg#citing-brainreg).
 
 **If you use this, or any other tools in the brainglobe suite, please
- [let us know](mailto:adam.tyson@ucl.ac.uk?subject=cellfinder), and 
+ [let us know](mailto:code@adamltyson.com?subject=cellfinder), and
  we'd be happy to promote your paper/talk etc.**
```

### Comparing `cellfinder-0.4.9/cellfinder/extract/extract_cubes.py` & `cellfinder-0.7.0/cellfinder/extract/extract_cubes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+"""
+Cube extraction for CNN-based classification.
+
+Based on, and mostly copied from,
+https://github.com/SainsburyWellcomeCentre/cell_count_analysis by
+Charly Rousseau (https://github.com/crousseau).
+"""
+
+import logging
 import os
 from collections import deque
 from concurrent.futures import ProcessPoolExecutor
-import logging
 from datetime import datetime
+from math import floor
 
 import numpy as np
-from skimage import transform
+from brainglobe_utils.cells.cells import group_cells_by_z
+from brainglobe_utils.general.numerical import is_even
+from brainglobe_utils.general.system import get_num_processes
 from numpy.linalg.linalg import LinAlgError
-from math import floor
+from skimage import transform
 from tifffile import tifffile
 from tqdm import tqdm
-from imlib.general.system import get_num_processes
-from imlib.cells.cells import group_cells_by_z
-from imlib.general.numerical import is_even
 
 from cellfinder.tools import image_processing as img_tools
 from cellfinder.tools import system
 
 
 class StackSizeError(Exception):
     pass
@@ -348,18 +356,18 @@
 
     logging.debug(
         "File size: {:.2f} GB, "
         "number of channels: {}, "
         "cube depth: {}, "
         "Therefore theoretically {:.2f} GB is needed per CPU core."
         "".format(
-            (file_size / (1024 ** 3)),
+            (file_size / (1024**3)),
             num_channels,
             cube_depth,
-            (total_mem_need / (1024 ** 3)),
+            (total_mem_need / (1024**3)),
         )
     )
 
     return total_mem_need
 
 
 def main(
@@ -371,15 +379,14 @@
     cube_height,
     voxel_sizes,
     network_voxel_sizes,
     max_ram,
     n_free_cpus=4,
     save_empty_cubes=False,
 ):
-
     start_time = datetime.now()
 
     if voxel_sizes[0] != network_voxel_sizes[0]:
         plane_scaling_factor = float(network_voxel_sizes[0]) / float(
             voxel_sizes[0]
         )
         num_planes_needed_for_cube = round(cube_depth * plane_scaling_factor)
@@ -398,15 +405,15 @@
     planes_shape = first_plane.shape
     brain_depth = len(list(planes_paths.values())[0])
 
     # TODO: use to assert all centre planes processed
     center_planes = sorted(list(set([cell.z for cell in cells])))
 
     # REFACTOR: rename (clashes with different meaning of planes_to_read below)
-    planes_to_read = np.zeros(brain_depth, dtype=np.bool)
+    planes_to_read = np.zeros(brain_depth, dtype=bool)
 
     if is_even(num_planes_needed_for_cube):
         half_nz = num_planes_needed_for_cube // 2
         # WARNING: not centered because even
         for p in center_planes:
             planes_to_read[p - half_nz : p + half_nz] = 1
     else:
```

### Comparing `cellfinder-0.4.9/cellfinder/figures/heatmap.py` & `cellfinder-0.7.0/cellfinder/figures/heatmap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import logging
-import tifffile
-import imio
+from pathlib import Path
 
+import imio
 import numpy as np
 import pandas as pd
-
-from pathlib import Path
+import tifffile
+from brainglobe_utils.general.system import ensure_directory_exists
+from brainglobe_utils.image.masking import mask_image_threshold
+from brainglobe_utils.image.scale import scale_and_convert_to_16_bits
 from skimage.filters import gaussian
-from imlib.image.scale import scale_and_convert_to_16_bits
-from imlib.image.masking import mask_image_threshold
-from imlib.general.system import ensure_directory_exists
 
 
 def get_bins(image_size, bin_sizes):
     """
     Given an image size, and bin size, return a list of the bin boundaries
     :param image_size: Size of the final image (tuple/list)
     :param bin_sizes: Bin sizes corresponding to the dimensions of
@@ -31,15 +30,14 @@
     atlas,
     downsampled_shape,
     registered_atlas_path,
     output_filename,
     smoothing=None,
     mask=True,
 ):
-
     points = pd.read_hdf(downsampled_points).values
 
     bins = get_bins(downsampled_shape, (1, 1, 1))
     heatmap_array, _ = np.histogramdd(points, bins=bins)
     heatmap_array = heatmap_array.astype(np.uint16)
 
     if smoothing is not None:
```

### Comparing `cellfinder-0.4.9/cellfinder/main.py` & `cellfinder-0.7.0/cellfinder/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 
 Runs each part of the cellfinder pipeline in turn.
 
 N.B imports are within functions to prevent tensorflow being imported before
 it's warnings are silenced
 """
 
-import os
 import logging
-import tifffile
+import os
 from datetime import datetime
-import bg_space as bgs
-from imlib.IO.cells import save_cells, get_cells
-from imlib.cells.cells import MissingCellsError
-from imlib.general.system import ensure_directory_exists
 
+import bg_space as bgs
+import tifffile
+from brainglobe_utils.cells.cells import MissingCellsError
+from brainglobe_utils.general.system import ensure_directory_exists
+from brainglobe_utils.IO.cells import get_cells, save_cells
 from cellfinder_core.main import suppress_tf_logging, tf_suppress_log_messages
 
+BRAINREG_PRE_PROCESSING_ARGS = None
+
 
 def get_downsampled_space(atlas, downsampled_image_path):
     target_shape = tifffile.imread(downsampled_image_path).shape
     downsampled_space = bgs.AnatomicalSpace(
         atlas.metadata["orientation"],
         shape=target_shape,
         resolution=atlas.resolution,
@@ -37,14 +39,15 @@
     except MissingCellsError:
         return False
 
 
 def main():
     suppress_tf_logging(tf_suppress_log_messages)
     from brainreg.main import main as register
+
     from cellfinder.tools import prep
 
     start_time = datetime.now()
     args, arg_groups, what_to_run, atlas = prep.prep_cellfinder_general()
 
     if what_to_run.register:
         # TODO: add register_part_brain option
@@ -53,14 +56,15 @@
         register(
             args.atlas,
             args.orientation,
             args.target_brain_path,
             args.brainreg_paths,
             args.voxel_sizes,
             arg_groups["NiftyReg registration backend options"],
+            BRAINREG_PRE_PROCESSING_ARGS,
             sort_input_file=args.sort_input_file,
             n_free_cpus=args.n_free_cpus,
             additional_images_downsample=additional_images_downsample,
             backend=args.backend,
             debug=args.debug,
         )
 
@@ -92,28 +96,28 @@
         run_all(args, what_to_run, atlas)
     logging.info(
         "Finished. Total time taken: {}".format(datetime.now() - start_time)
     )
 
 
 def run_all(args, what_to_run, atlas):
-
-    from cellfinder_core.detect import detect
     from cellfinder_core.classify import classify
+    from cellfinder_core.detect import detect
     from cellfinder_core.tools import prep
     from cellfinder_core.tools.IO import read_with_dask
 
     from cellfinder.analyse import analyse
     from cellfinder.figures import figures
-
     from cellfinder.tools.prep import (
         prep_candidate_detection,
         prep_channel_specific_general,
     )
 
+    points = None
+    signal_array = None
     args, what_to_run = prep_channel_specific_general(args, what_to_run)
 
     if what_to_run.detect:
         logging.info("Detecting cell candidates")
         args = prep_candidate_detection(args)
         signal_array = read_with_dask(
             args.signal_planes_paths[args.signal_channel]
@@ -129,36 +133,45 @@
             args.ball_xy_size,
             args.ball_z_size,
             args.ball_overlap_fraction,
             args.soma_spread_factor,
             args.n_free_cpus,
             args.log_sigma_size,
             args.n_sds_above_mean_thresh,
+            save_planes=args.save_planes,
+            plane_directory=args.plane_directory,
         )
         ensure_directory_exists(args.paths.points_directory)
 
         save_cells(
             points,
             args.paths.detected_points,
             save_csv=args.save_csv,
             artifact_keep=args.artifact_keep,
         )
 
     else:
         logging.info("Skipping cell detection")
+        points = get_cells(args.paths.detected_points)
 
     if what_to_run.classify:
         model_weights = prep.prep_classification(
             args.trained_model,
             args.model_weights,
             args.install_path,
             args.model,
             args.n_free_cpus,
         )
         if what_to_run.classify:
+            if points is None:
+                points = get_cells(args.paths.detected_points)
+            if signal_array is None:
+                signal_array = read_with_dask(
+                    args.signal_planes_paths[args.signal_channel]
+                )
             logging.info("Running cell classification")
             background_array = read_with_dask(args.background_planes_path[0])
 
             points = classify.main(
                 points,
                 signal_array,
                 background_array,
@@ -191,21 +204,29 @@
 
     if what_to_run.analyse or what_to_run.figures:
         downsampled_space = get_downsampled_space(
             atlas, args.brainreg_paths.boundaries_file_path
         )
 
     if what_to_run.analyse:
-        logging.info("Analysing cell positions")
-        analyse.run(args, atlas, downsampled_space)
+        points = get_cells(args.paths.classified_points, cells_only=True)
+        if len(points) == 0:
+            logging.info("No cells detected, skipping cell position analysis")
+        else:
+            logging.info("Analysing cell positions")
+            analyse.run(args, points, atlas, downsampled_space)
     else:
         logging.info("Skipping cell position analysis")
 
     if what_to_run.figures:
-        logging.info("Generating figures")
-        figures.run(args, atlas, downsampled_space.shape)
+        points = get_cells(args.paths.classified_points, cells_only=True)
+        if len(points) == 0:
+            logging.info("No cells detected, skipping")
+        else:
+            logging.info("Generating figures")
+            figures.run(args, atlas, downsampled_space.shape)
     else:
         logging.info("Skipping figure generation")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `cellfinder-0.4.9/cellfinder/tools/image_processing.py` & `cellfinder-0.7.0/cellfinder/tools/image_processing.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
-
-from imlib.general.numerical import is_even
+from brainglobe_utils.general.numerical import is_even
 
 
 def crop_center_2d(img, crop_x=None, crop_y=None):
     """
     Crops the centre of a 2D image, and returns a smaller array. If the desired
     dimension is larger than the original dimension, nothing is changed.
     :param img: 2D input image
```

### Comparing `cellfinder-0.4.9/cellfinder/tools/parser.py` & `cellfinder-0.7.0/cellfinder/tools/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,29 +3,32 @@
 ========
 All the various arguments that may be needed by the various submodules.
 Defined together so they can also be called by any other entry points.
 """
 
 
 from argparse import (
-    ArgumentParser,
     ArgumentDefaultsHelpFormatter,
+    ArgumentParser,
     ArgumentTypeError,
 )
-from cellfinder import __version__
-from imlib.general.numerical import check_positive_float, check_positive_int
-from cellfinder_core.tools.source_files import source_custom_config_cellfinder
 
+from brainglobe_utils.general.numerical import (
+    check_positive_float,
+    check_positive_int,
+)
+from brainreg.cli import atlas_parse, geometry_parser, niftyreg_parse
+from brainreg.cli import backend_parse as brainreg_backend_parse
 from cellfinder_core.download.cli import (
-    model_parser,
     download_directory_parser,
+    model_parser,
 )
+from cellfinder_core.tools.source_files import source_custom_config_cellfinder
 
-from brainreg.cli import atlas_parse, geometry_parser, niftyreg_parse
-from brainreg.cli import backend_parse as brainreg_backend_parse
+from cellfinder import __version__
 
 # TODO: Gradually move all paths as strings to Path objects
 
 models = {
     "18": "18-layer",
     "34": "34-layer",
     "50": "50-layer",
```

### Comparing `cellfinder-0.4.9/cellfinder/tools/prep.py` & `cellfinder-0.7.0/cellfinder/tools/prep.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 """
 prep
 ==================
 Functions to prepare files and directories needed for other functions
 """
 
 
-import os
-import logging
 import json
-
-from fancylog import fancylog
+import logging
+import os
+from argparse import Namespace
 from pathlib import PurePath
 
-from imlib.general.system import ensure_directory_exists
-
-from imlib.general.exceptions import CommandLineInputError
-
+from bg_atlasapi import BrainGlobeAtlas
+from brainglobe_utils.general.exceptions import CommandLineInputError
+from brainglobe_utils.general.system import ensure_directory_exists
+from brainreg.paths import Paths as BrainRegPaths
+from fancylog import fancylog
 
-from cellfinder.tools.parser import cellfinder_parser
 import cellfinder as program_for_log
 import cellfinder.tools.parser as parser
-from cellfinder.tools import tools, system
-from argparse import Namespace
-from brainreg.paths import Paths as BrainRegPaths
-from bg_atlasapi import BrainGlobeAtlas
+from cellfinder.tools import system, tools
+from cellfinder.tools.parser import cellfinder_parser
 
 
 def get_arg_groups(args, parser):
     arg_groups = {}
     for group in parser._action_groups:
         group_dict = {
             a.dest: getattr(args, a.dest, None) for a in group._group_actions
@@ -78,14 +75,15 @@
         self.downsampled_points = os.path.join(
             self.points_directory, "downsampled.points"
         )
         self.atlas_points = os.path.join(self.points_directory, "atlas.points")
         self.brainrender_points = os.path.join(
             self.points_directory, "points.npy"
         )
+        self.abc4d_points = os.path.join(self.points_directory, "abc4d.npy")
 
         self.tmp__cubes_output_dir = os.path.join(self.output_dir, "cubes")
 
         self.figures_directory = os.path.join(self.output_dir, "figures")
         self.heatmap = os.path.join(self.figures_directory, "heatmap.tiff")
 
         self.analysis_directory = os.path.join(self.output_dir, "analysis")
@@ -120,14 +118,15 @@
 
     fancylog.start_logging(
         args.output_dir,
         program_for_log,
         variables=[args, args.paths],
         verbose=args.debug,
         log_header="CELLFINDER LOG",
+        multiprocessing_aware=True,
     )
 
     log_metadata(args.paths.metadata_path, args)
 
     what_to_run = CalcWhatToRun(args)
     args.signal_ch_ids, args.background_ch_id = check_and_return_ch_ids(
         args.signal_ch_ids, args.background_ch_id, args.signal_planes_paths
```

### Comparing `cellfinder-0.4.9/cellfinder/tools/system.py` & `cellfinder-0.7.0/cellfinder/tools/system.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pathlib import Path
 
-from imlib.general.exceptions import CommandLineInputError
+from brainglobe_utils.general.exceptions import CommandLineInputError
 
 
 def get_subdirectories(directory, names_only=False):
     """
     Return all subdirectories in a given directory
     :param directory:
     :param names_only: If true, dont return paths, but the names
```

### Comparing `cellfinder-0.4.9/cellfinder/tools/tools.py` & `cellfinder-0.7.0/cellfinder/tools/tools.py`

 * *Files identical despite different names*

### Comparing `cellfinder-0.4.9/cellfinder/train/curation.py` & `cellfinder-0.7.0/cellfinder/train/curation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,39 +1,25 @@
 import json
-import napari
-
-import numpy as np
-
 from pathlib import Path
-from qtpy import QtCore
-
 
+import napari
+import numpy as np
 from bg_atlasapi import BrainGlobeAtlas
-from imlib.IO.cells import save_cells
-from imlib.cells.cells import Cell
-from napari_cellfinder.cellfinder import get_cell_arrays
+from brainglobe_utils.cells.cells import Cell
+from brainglobe_utils.general.system import get_sorted_file_paths
+from brainglobe_utils.IO.cells import save_cells
 from brainreg.paths import Paths as BrainregPaths
-from brainreg_segment.layout.gui_elements import (
-    add_button,
-)
-from qtpy.QtWidgets import (
-    QLabel,
-    QFileDialog,
-    QGridLayout,
-    QGroupBox,
-    QWidget,
-)
-
-
-from cellfinder.main import get_downsampled_space
-from cellfinder.analyse.analyse import run_analysis
-
-from imlib.general.system import get_sorted_file_paths
+from brainreg_segment.layout.gui_elements import add_button
 from napari.utils.io import magic_imread
+from napari_cellfinder.cellfinder import get_cell_arrays
+from qtpy import QtCore
+from qtpy.QtWidgets import QFileDialog, QGridLayout, QGroupBox, QLabel, QWidget
 
+from cellfinder.analyse.analyse import run_analysis
+from cellfinder.main import get_downsampled_space
 
 # Constants used throughout
 WINDOW_HEIGHT = 750
 WINDOW_WIDTH = 1500
 COLUMN_WIDTH = 150
```

### Comparing `cellfinder-0.4.9/cellfinder/train/curation_old.py` & `cellfinder-0.7.0/cellfinder/train/curation_old.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-from argparse import ArgumentParser, ArgumentDefaultsHelpFormatter
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser
+from pathlib import Path
+
 import napari
 import numpy as np
+from brainglobe_utils.cells.cells import Cell
+from brainglobe_utils.general.list import unique_elements_lists
+from brainglobe_utils.general.system import (
+    ensure_directory_exists,
+    get_sorted_file_paths,
+)
+from brainglobe_utils.IO.cells import cells_xml_to_df, get_cells, save_cells
+from brainglobe_utils.IO.yaml import save_yaml
 from napari.utils.io import magic_imread
-from pathlib import Path
-
 from qtpy.QtWidgets import QApplication
 
-from imlib.general.system import get_sorted_file_paths, ensure_directory_exists
-from imlib.general.list import unique_elements_lists
-
-from imlib.IO.cells import cells_xml_to_df, save_cells, get_cells
-from imlib.cells.cells import Cell
-from imlib.IO.yaml import save_yaml
-
-from cellfinder.extract.extract_cubes import main as extract_cubes_main
 import cellfinder.tools.parser as cellfinder_parse
+from cellfinder.extract.extract_cubes import main as extract_cubes_main
 
 OUTPUT_NAME = "curated_cells.xml"
 CURATED_POINTS = []
 
 
 def parser():
     parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter)
```

### Comparing `cellfinder-0.4.9/cellfinder.egg-info/PKG-INFO` & `cellfinder-0.7.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,144 +1,150 @@
-Metadata-Version: 2.1
-Name: cellfinder
-Version: 0.4.9
-Summary: Automated 3D cell detection and registration of whole-brain images
-Home-page: https://cellfinder.info
-Author: Adam Tyson, Christian Niedworok, Charly Rousseau
-Author-email: adam.tyson@ucl.ac.uk
-License: UNKNOWN
-Project-URL: Source Code, https://github.com/brainglobe/cellfinder
-Project-URL: Bug Tracker, https://github.com/brainglobe/cellfinder/issues
-Project-URL: Documentation, https://docs.brainglobe.info/cellfinder
-Description: [![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
-        [![PyPI](https://img.shields.io/pypi/v/cellfinder.svg)](https://pypi.org/project/cellfinder)
-        [![Downloads](https://pepy.tech/badge/cellfinder)](https://pepy.tech/project/cellfinder)
-        [![Wheel](https://img.shields.io/pypi/wheel/cellfinder.svg)](https://pypi.org/project/cellfinder)
-        [![Development Status](https://img.shields.io/pypi/status/cellfinder.svg)](https://github.com/brainglobe/cellfinder)
-        [![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder/tests)](
-            https://github.com/brainglobe/cellfinder/actions)
-        [![Coverage Status](https://coveralls.io/repos/github/brainglobe/cellfinder/badge.svg?branch=master)](https://coveralls.io/github/brainglobe/cellfinder?branch=master)
-        [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
-        [![Gitter](https://badges.gitter.im/brainglobe.svg)](https://gitter.im/BrainGlobe/cellfinder/?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.3891338.svg)](https://doi.org/10.5281/zenodo.3891338)
-        [![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
-        [![Website](https://img.shields.io/website?up_message=online&url=https%3A%2F%2Fcellfinder.info)](https://cellfinder.info)
-        [![Twitter](https://img.shields.io/twitter/follow/findingcells?style=social)](https://twitter.com/findingcells)
-        # Cellfinder
-        Whole-brain cell detection, registration and analysis.
-        
-        ---
-        
-        
-        Cellfinder is a collection of tools from the 
-        [Margrie Lab](https://www.sainsburywellcome.org/web/groups/margrie-lab) and
-         others at the [Sainsbury Wellcome Centre](https://www.sainsburywellcome.org/web/), [UCL](https://www.ucl.ac.uk/)
-         for the analysis of whole-brain imaging data such as 
-         [serial-section imaging](https://sainsburywellcomecentre.github.io/OpenSerialSection/)
-         and lightsheet imaging in cleared tissue.
-         
-         The aim is to provide a single solution for:
-         
-         * Cell detection (initial cell candidate detection and refinement using 
-         deep learning).
-         * Atlas registration (using [brainreg](https://github.com/brainglobe/brainreg))
-         * Analysis of cell positions in a common space
-         
-        Installation is with 
-        `pip install cellfinder`.
-        
-        Basic usage:
-        ```bash
-        cellfinder -s signal_images -b background_images -o output_dir --metadata metadata
-        ```
-        Full documentation can be 
-        found [here](https://docs.brainglobe.info/cellfinder).
-         
-        This software is at a very early stage, and was written with our data in mind. 
-        Over time we hope to support other data types/formats. If you have any 
-        questions or issues, please get in touch by 
-        [email](mailto:adam.tyson@ucl.ac.uk?subject=cellfinder), 
-        [gitter](https://gitter.im/BrainGlobe/cellfinder) or by 
-        [raising an issue](https://github.com/brainglobe/cellfinder/issues/new/choose).
-        
-        
-        ---
-        ## Illustration
-        
-        ### Introduction
-        cellfinder takes a stitched, but otherwise raw whole-brain dataset with at least 
-        two channels:
-         * Background channel (i.e. autofluorescence)
-         * Signal channel, the one with the cells to be detected:
-         
-        ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/raw.png)
-        **Raw coronal serial two-photon mouse brain image showing labelled cells**
-        
-        
-        ### Cell candidate detection
-        Classical image analysis (e.g. filters, thresholding) is used to find 
-        cell-like objects (with false positives):
-        
-        ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/detect.png)
-        **Candidate cells (including many artefacts)**
-        
-        
-        ### Cell candidate classification
-        A deep-learning network (ResNet) is used to classify cell candidates as true 
-        cells or artefacts:
-        
-        ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/classify.png)
-        **Cassified cell candidates. Yellow - cells, Blue - artefacts**
-        
-        ### Registration and segmentation (brainreg)
-        Using [brainreg](https://github.com/brainglobe/brainreg), 
-        cellfinder aligns a template brain and atlas annotations (e.g. 
-        the Allen Reference Atlas, ARA) to the sample allowing detected cells to be assigned 
-        a brain region.
-        
-        This transformation can be inverted, allowing detected cells to be
-        transformed to a standard anatomical space.
-        
-        ![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/register.png)
-        **ARA overlaid on sample image**
-        
-        ### Analysis of cell positions in a common anatomical space
-        Registration to a template allows for powerful group-level analysis of cellular
-        disributions. *(Example to come)*
-        
-        ## Examples
-        *(more to come)*
-        
-        ### Tracing of inputs to retrosplenial cortex (RSP)
-        Input cell somas detected by cellfinder, aligned to the Allen Reference Atlas, 
-        and visualised in [brainrender](https://github.com/brancolab/brainrender) along 
-        with RSP.
-        
-        ![brainrender](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/brainrender.png)
-        
-        Data courtesy of Sepiedeh Keshavarzi and Chryssanthi Tsitoura. [Details here](https://www.youtube.com/watch?v=pMHP0o-KsoQ)
-        
-        
-        ## Citing cellfinder
-        
-        If you find cellfinder useful, and use it in your research, please cite the preprint outlining the cell detection algorithm:
-        > Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ bioRxiv, [doi.org/10.1101/2020.10.21.348771](https://doi.org/10.1101/2020.10.21.348771)
-        
-        If you use any of the image registration functions in cellfinder, please also cite [brainreg](https://github.com/brainglobe/brainreg#citing-brainreg).
-        
-        **If you use this, or any other tools in the brainglobe suite, please
-         [let us know](mailto:adam.tyson@ucl.ac.uk?subject=cellfinder), and 
-         we'd be happy to promote your paper/talk etc.**
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows :: Windows 10
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Image Recognition
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: dev
+[![Python Version](https://img.shields.io/pypi/pyversions/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![PyPI](https://img.shields.io/pypi/v/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Downloads](https://pepy.tech/badge/cellfinder)](https://pepy.tech/project/cellfinder)
+[![Wheel](https://img.shields.io/pypi/wheel/cellfinder.svg)](https://pypi.org/project/cellfinder)
+[![Development Status](https://img.shields.io/pypi/status/cellfinder.svg)](https://github.com/brainglobe/cellfinder)
+[![Tests](https://img.shields.io/github/workflow/status/brainglobe/cellfinder/tests)](
+    https://github.com/brainglobe/cellfinder/actions)
+[![codecov](https://codecov.io/gh/brainglobe/cellfinder/branch/master/graph/badge.svg?token=s3MweEFPhl)](https://codecov.io/gh/brainglobe/cellfinder)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/python/black)
+[![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
+[![Contributions](https://img.shields.io/badge/Contributions-Welcome-brightgreen.svg)](https://docs.brainglobe.info/cellfinder/contributing)
+[![Website](https://img.shields.io/website?up_message=online&url=https%3A%2F%2Fbrainglobe.info)](https://brainglobe.info/documentation/cellfinder/index.html)
+[![Twitter](https://img.shields.io/twitter/follow/brain_globe?style=social)](https://twitter.com/brain_globe)
+
+# Cellfinder
+Whole-brain cell detection, registration and analysis.
+
+**N.B. If you want to just use the cell detection part of cellfinder, please
+see the standalone [cellfinder-core](https://github.com/brainglobe/cellfinder-core)
+package, or the [cellfinder plugin](https://github.com/brainglobe/cellfinder-napari)
+for [napari](https://napari.org/).**
+
+---
+`cellfinder` is a collection of tools developed by [Adam Tyson](https://github.com/adamltyson), [Charly Rousseau](https://github.com/crousseau) and [Christian Niedworok](https://github.com/cniedwor) in the [Margrie Lab](https://www.sainsburywellcome.org/web/groups/margrie-lab), generously supported by the [Sainsbury Wellcome Centre](https://www.sainsburywellcome.org/web/).
+
+`cellfinder` is a designed for the analysis of whole-brain imaging data such as
+ [serial-section imaging](https://sainsburywellcomecentre.github.io/OpenSerialSection/)
+ and lightsheet imaging in cleared tissue. The aim is to provide a single solution for:
+
+ * Cell detection (initial cell candidate detection and refinement using
+ deep learning) (using [cellfinder-core](https://github.com/brainglobe/cellfinder-core))
+ * Atlas registration (using [brainreg](https://github.com/brainglobe/brainreg))
+ * Analysis of cell positions in a common space
+
+ ---
+Installation is with
+`pip install cellfinder`
+
+---
+Basic usage:
+```bash
+cellfinder -s signal_images -b background_images -o output_dir --metadata metadata
+```
+Full documentation can be
+found [here](https://brainglobe.info/documentation/cellfinder/index.html).
+
+This software is at a very early stage, and was written with our data in mind.
+Over time we hope to support other data types/formats. If you have any issues, please get in touch [on the forum](https://forum.image.sc/tag/brainglobe) or by
+[raising an issue](https://github.com/brainglobe/cellfinder/issues/new/choose).
+
+
+---
+## Illustration
+
+### Introduction
+cellfinder takes a stitched, but otherwise raw whole-brain dataset with at least
+two channels:
+ * Background channel (i.e. autofluorescence)
+ * Signal channel, the one with the cells to be detected:
+
+![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/raw.png)
+**Raw coronal serial two-photon mouse brain image showing labelled cells**
+
+
+### Cell candidate detection
+Classical image analysis (e.g. filters, thresholding) is used to find
+cell-like objects (with false positives):
+
+![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/detect.png)
+**Candidate cells (including many artefacts)**
+
+
+### Cell candidate classification
+A deep-learning network (ResNet) is used to classify cell candidates as true
+cells or artefacts:
+
+![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/classify.png)
+**Cassified cell candidates. Yellow - cells, Blue - artefacts**
+
+### Registration and segmentation (brainreg)
+Using [brainreg](https://github.com/brainglobe/brainreg),
+cellfinder aligns a template brain and atlas annotations (e.g.
+the Allen Reference Atlas, ARA) to the sample allowing detected cells to be assigned
+a brain region.
+
+This transformation can be inverted, allowing detected cells to be
+transformed to a standard anatomical space.
+
+![raw](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/register.png)
+**ARA overlaid on sample image**
+
+### Analysis of cell positions in a common anatomical space
+Registration to a template allows for powerful group-level analysis of cellular
+disributions. *(Example to come)*
+
+## Examples
+*(more to come)*
+
+### Tracing of inputs to retrosplenial cortex (RSP)
+Input cell somas detected by cellfinder, aligned to the Allen Reference Atlas,
+and visualised in [brainrender](https://github.com/brainglobe/brainrender) along
+with RSP.
+
+![brainrender](https://raw.githubusercontent.com/brainglobe/cellfinder/master/resources/brainrender.png)
+
+Data courtesy of Sepiedeh Keshavarzi and Chryssanthi Tsitoura. [Details here](https://www.youtube.com/watch?v=pMHP0o-KsoQ)
+
+## Visualisation
+
+cellfinder comes with a plugin ([brainglobe-napari-io](https://github.com/brainglobe/brainglobe-napari-io)) for [napari](https://github.com/napari/napari) to view your data
+
+#### Usage
+* Open napari (however you normally do it, but typically just type `napari` into your terminal, or click on your desktop icon)
+
+#### Load cellfinder XML file
+* Load your raw data (drag and drop the data directories into napari, one at a time)
+* Drag and drop your cellfinder XML file (e.g. `cell_classification.xml`) into napari.
+
+#### Load cellfinder directory
+* Load your raw data (drag and drop the data directories into napari, one at a time)
+* Drag and drop your cellfinder output directory into napari.
+
+The plugin will then load your detected cells (in yellow) and the rejected cell
+candidates (in blue). If you carried out registration, then these results will be
+overlaid (similarly to the loading brainreg data, but transformed to the
+coordinate space of your raw data).
+
+![load_data](https://raw.githubusercontent.com/brainglobe/brainglobe-napari-io/master/resources/load_data.gif)
+**Loading raw data**
+
+![load_data](https://raw.githubusercontent.com/brainglobe/brainglobe-napari-io/master/resources/load_results.gif)
+**Loading cellfinder results**
+
+
+## Contributing
+Contributions to cellfinder are more than welcome. Please see the [developers guide](https://brainglobe.info/developers/index.html).
+
+
+## Citing cellfinder
+
+If you find cellfinder useful, and use it in your research, please cite the paper outlining the cell detection algorithm:
+> Tyson, A. L., Rousseau, C. V., Niedworok, C. J., Keshavarzi, S., Tsitoura, C., Cossell, L., Strom, M. and Margrie, T. W. (2021) “A deep learning algorithm for 3D cell detection in whole mouse brain image datasets’ PLOS Computational Biology, 17(5), e1009074
+[https://doi.org/10.1371/journal.pcbi.1009074](https://doi.org/10.1371/journal.pcbi.1009074)
+>
+If you use any of the image registration functions in cellfinder, please also cite [brainreg](https://github.com/brainglobe/brainreg#citing-brainreg).
+
+**If you use this, or any other tools in the brainglobe suite, please
+ [let us know](mailto:code@adamltyson.com?subject=cellfinder), and
+ we'd be happy to promote your paper/talk etc.**
```

### Comparing `cellfinder-0.4.9/setup.py` & `cellfinder-0.7.0/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,84 +1,83 @@
-from setuptools import setup, find_namespace_packages
 from os import path
 
+from setuptools import find_packages, setup
+
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 requirements = [
-    "cellfinder-core",
+    "brainreg",
+    "cellfinder-core>=0.2.4",
+    "configobj",
+    "fancylog>=0.0.7",
+    "imio",
+    "brainglobe-utils>=0.2.5",
+    "multiprocessing-logging>=0.3.4",
+    "natsort",
     "numpy",
-    "scikit-learn",
-    "configparser",
     "pandas",
     "packaging",
     "scikit-image",
     "tifffile",
-    "natsort",
     "tqdm",
-    "multiprocessing-logging",
-    "psutil",
-    "configobj",
-    "tensorflow>=2.4.0",
-    "napari[pyside2]>=0.3.7",
-    "napari-cellfinder>=0.1.1",
-    "slurmio>=0.0.4",
-    "fancylog>=0.0.7",
-    "imlib>=0.0.26",
-    "brainreg",
-    "imio",
 ]
 
 
 setup(
     name="cellfinder",
-    version="0.4.9",
+    version="0.7.0",
     description="Automated 3D cell detection and registration of "
     "whole-brain images",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=requirements,
     extras_require={
+        "napari": [
+            "napari[pyside2]",
+            "brainglobe-napari-io",
+            "cellfinder-napari",
+        ],
         "dev": [
             "black",
             "pytest-cov",
             "pytest",
             "gitpython",
             "coverage>=5.0.3",
             "bump2version",
             "pre-commit",
             "flake8",
-        ]
+        ],
     },
-    setup_requires=["cython"],
-    python_requires=">=3.7",
-    packages=find_namespace_packages(exclude=("docs", "doc_build", "tests")),
+    python_requires=">=3.8",
+    packages=find_packages(),
     include_package_data=True,
     entry_points={
         "console_scripts": [
             "cellfinder = cellfinder.main:main",
             "cellfinder_curate_new = cellfinder.train.curation:main",
             "cellfinder_curate = cellfinder.train.curation_old:main",
         ]
     },
-    url="https://cellfinder.info",
+    url="https://brainglobe.info/cellfinder",
     project_urls={
         "Source Code": "https://github.com/brainglobe/cellfinder",
         "Bug Tracker": "https://github.com/brainglobe/cellfinder/issues",
         "Documentation": "https://docs.brainglobe.info/cellfinder",
     },
     author="Adam Tyson, Christian Niedworok, Charly Rousseau",
-    author_email="adam.tyson@ucl.ac.uk",
+    author_email="code@adamltyson.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Operating System :: POSIX :: Linux",
         "Operating System :: Microsoft :: Windows :: Windows 10",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Intended Audience :: Developers",
         "Intended Audience :: Science/Research",
     ],
     zip_safe=False,
 )
```

