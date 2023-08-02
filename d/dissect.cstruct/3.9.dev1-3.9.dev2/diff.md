# Comparing `tmp/dissect.cstruct-3.9.dev1.tar.gz` & `tmp/dissect.cstruct-3.9.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dissect.cstruct-3.9.dev1.tar", last modified: Fri Jul  7 13:06:24 2023, max compression
+gzip compressed data, was "dissect.cstruct-3.9.dev2.tar", last modified: Wed Aug  2 13:33:56 2023, max compression
```

## Comparing `dissect.cstruct-3.9.dev1.tar` & `dissect.cstruct-3.9.dev2.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.916671 dissect.cstruct-3.9.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-07 13:06:24.912671 dissect.cstruct-3.9.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.884671 dissect.cstruct-3.9.dev1/dissect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.896671 dissect.cstruct-3.9.dev1/dissect/cstruct/
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/cstruct.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.900671 dissect.cstruct-3.9.dev1/dissect/cstruct/types/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/bytesinteger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/chartype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/packedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/structure.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/voidtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/types/wchartype.py
--rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/dissect/cstruct/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.892671 dissect.cstruct-3.9.dev1/dissect.cstruct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-07-07 13:06:24.000000 dissect.cstruct-3.9.dev1/dissect.cstruct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-07-07 13:06:24.000000 dissect.cstruct-3.9.dev1/dissect.cstruct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 13:06:24.000000 dissect.cstruct-3.9.dev1/dissect.cstruct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 13:06:24.000000 dissect.cstruct-3.9.dev1/dissect.cstruct.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.904671 dissect.cstruct-3.9.dev1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/examples/disk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/examples/mirai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/examples/pe.py
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/examples/secdesc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-07-07 13:06:13.000000 dissect.cstruct-3.9.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 13:06:24.916671 dissect.cstruct-3.9.dev1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.912671 dissect.cstruct-3.9.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.912671 dissect.cstruct-3.9.dev1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/data/testdef.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 13:06:24.912671 dissect.cstruct-3.9.dev1/tests/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_align.py
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_bitbuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_bitfield.py
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_bytesinteger.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_ctypes_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_packedtype.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_pointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_union.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-07 13:06:05.000000 dissect.cstruct-3.9.dev1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.958210 dissect.cstruct-3.9.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-02 13:33:56.958210 dissect.cstruct-3.9.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.950209 dissect.cstruct-3.9.dev2/dissect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.954210 dissect.cstruct-3.9.dev2/dissect/cstruct/
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15117 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/cstruct.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19445 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.954210 dissect.cstruct-3.9.dev2/dissect/cstruct/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/bytesinteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/chartype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/packedtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/voidtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/types/wchartype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9669 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/dissect/cstruct/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.954210 dissect.cstruct-3.9.dev2/dissect.cstruct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8302 2023-08-02 13:33:56.000000 dissect.cstruct-3.9.dev2/dissect.cstruct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-08-02 13:33:56.000000 dissect.cstruct-3.9.dev2/dissect.cstruct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 13:33:56.000000 dissect.cstruct-3.9.dev2/dissect.cstruct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-02 13:33:56.000000 dissect.cstruct-3.9.dev2/dissect.cstruct.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.954210 dissect.cstruct-3.9.dev2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/examples/disk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/examples/mirai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4720 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/examples/pe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/examples/secdesc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-08-02 13:33:47.000000 dissect.cstruct-3.9.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 13:33:56.958210 dissect.cstruct-3.9.dev2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.958210 dissect.cstruct-3.9.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.958210 dissect.cstruct-3.9.dev2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/data/testdef.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 13:33:56.958210 dissect.cstruct-3.9.dev2/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_align.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_bitbuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5581 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_bitfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_bytesinteger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_ctypes_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_packedtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_pointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_union.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2949 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-02 13:33:43.000000 dissect.cstruct-3.9.dev2/tox.ini
```

### Comparing `dissect.cstruct-3.9.dev1/LICENSE` & `dissect.cstruct-3.9.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/PKG-INFO` & `dissect.cstruct-3.9.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 3.9.dev1
+Version: 3.9.dev2
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.cstruct-3.9.dev1/README.md` & `dissect.cstruct-3.9.dev2/README.md`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/__init__.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/bitbuffer.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/bitbuffer.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/compiler.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/compiler.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/cstruct.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/cstruct.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/expression.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/expression.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/parser.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
                 key = key.strip()
                 val = val.strip()
                 if not key:
                     continue
                 if not val:
                     val = nextval
                 else:
-                    val = Expression(self.cstruct, val).evaluate()
+                    val = Expression(self.cstruct, val).evaluate(values)
 
                 if enumtype == "flag":
                     high_bit = val.bit_length() - 1
                     nextval = 2 ** (high_bit + 1)
                 else:
                     nextval = val + 1
```

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/__init__.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/__init__.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/base.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/base.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/bytesinteger.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/bytesinteger.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/chartype.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/chartype.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/enum.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/enum.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/flag.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/flag.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/instance.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/instance.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/packedtype.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/packedtype.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/pointer.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/pointer.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/structure.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/structure.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/types/wchartype.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/types/wchartype.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect/cstruct/utils.py` & `dissect.cstruct-3.9.dev2/dissect/cstruct/utils.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/dissect.cstruct.egg-info/PKG-INFO` & `dissect.cstruct-3.9.dev2/dissect.cstruct.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dissect.cstruct
-Version: 3.9.dev1
+Version: 3.9.dev2
 Summary: A Dissect module implementing a parser for C-like structures: structure parsing in Python made easy
 Author-email: Dissect Team <dissect@fox-it.com>
 License: Apache License 2.0
 Project-URL: homepage, https://dissect.tools
 Project-URL: documentation, https://docs.dissect.tools/en/latest/projects/dissect.cstruct
 Project-URL: repository, https://github.com/fox-it/dissect.cstruct
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `dissect.cstruct-3.9.dev1/dissect.cstruct.egg-info/SOURCES.txt` & `dissect.cstruct-3.9.dev2/dissect.cstruct.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/examples/disk.py` & `dissect.cstruct-3.9.dev2/examples/disk.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/examples/mirai.py` & `dissect.cstruct-3.9.dev2/examples/mirai.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/examples/pe.py` & `dissect.cstruct-3.9.dev2/examples/pe.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/examples/secdesc.py` & `dissect.cstruct-3.9.dev2/examples/secdesc.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/pyproject.toml` & `dissect.cstruct-3.9.dev2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/docs/Makefile` & `dissect.cstruct-3.9.dev2/tests/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/docs/conf.py` & `dissect.cstruct-3.9.dev2/tests/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_align.py` & `dissect.cstruct-3.9.dev2/tests/test_align.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_basic.py` & `dissect.cstruct-3.9.dev2/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_bitbuffer.py` & `dissect.cstruct-3.9.dev2/tests/test_bitbuffer.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_bitfield.py` & `dissect.cstruct-3.9.dev2/tests/test_bitfield.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_bytesinteger.py` & `dissect.cstruct-3.9.dev2/tests/test_bytesinteger.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_ctypes_type.py` & `dissect.cstruct-3.9.dev2/tests/test_ctypes_type.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_enum.py` & `dissect.cstruct-3.9.dev2/tests/test_enum.py`

 * *Files 4% similar despite different names*

```diff
@@ -256,7 +256,23 @@
     cs = cstruct.cstruct()
     cs.load(cdef, compiled=compiled)
 
     test = cs.test
 
     t = test(b"\xff\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x00\x0A\x00\x00\x00")
     assert t.arr == [255, 0, 0, 10]
+
+
+def test_enum_reference_own_member(compiled):
+    cdef = """
+    enum test {
+        A,
+        B = A + 3,
+        C
+    };
+    """
+    cs = cstruct.cstruct()
+    cs.load(cdef, compiled=compiled)
+
+    assert cs.test.A == 0
+    assert cs.test.B == 3
+    assert cs.test.C == 4
```

### Comparing `dissect.cstruct-3.9.dev1/tests/test_expression.py` & `dissect.cstruct-3.9.dev2/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_flag.py` & `dissect.cstruct-3.9.dev2/tests/test_flag.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_packedtype.py` & `dissect.cstruct-3.9.dev2/tests/test_packedtype.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_pointer.py` & `dissect.cstruct-3.9.dev2/tests/test_pointer.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_struct.py` & `dissect.cstruct-3.9.dev2/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_union.py` & `dissect.cstruct-3.9.dev2/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_util.py` & `dissect.cstruct-3.9.dev2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tests/test_utils.py` & `dissect.cstruct-3.9.dev2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dissect.cstruct-3.9.dev1/tox.ini` & `dissect.cstruct-3.9.dev2/tox.ini`

 * *Files identical despite different names*

