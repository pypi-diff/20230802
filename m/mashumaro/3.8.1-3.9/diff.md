# Comparing `tmp/mashumaro-3.8.1.tar.gz` & `tmp/mashumaro-3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mashumaro-3.8.1.tar", last modified: Fri Jun 23 16:33:05 2023, max compression
+gzip compressed data, was "mashumaro-3.9.tar", last modified: Wed Aug  2 20:00:20 2023, max compression
```

## Comparing `mashumaro-3.8.1.tar` & `mashumaro-3.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.749565 mashumaro-3.8.1/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-06-22 18:41:04.000000 mashumaro-3.8.1/LICENSE
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    97544 2023-06-23 16:33:05.749426 mashumaro-3.8.1/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    96623 2023-06-22 18:41:04.000000 mashumaro-3.8.1/README.md
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.729716 mashumaro-3.8.1/mashumaro/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      258 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1674 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/config.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.731257 mashumaro-3.8.1/mashumaro/core/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1013 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/const.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      825 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/helpers.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.731884 mashumaro-3.8.1/mashumaro/core/meta/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/__init__.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.745778 mashumaro-3.8.1/mashumaro/core/meta/code/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/code/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    41377 2023-06-23 16:32:39.000000 mashumaro-3.8.1/mashumaro/core/meta/code/builder.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      815 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/code/lines.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    22129 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/helpers.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1366 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/mixin.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.746642 mashumaro-3.8.1/mashumaro/core/meta/types/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/types/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     4882 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/types/common.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    25094 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/types/pack.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    42599 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/core/meta/types/unpack.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      469 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/dialect.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5491 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/exceptions.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1472 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/helper.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.747807 mashumaro-3.8.1/mashumaro/jsonschema/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      214 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/jsonschema/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2151 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/jsonschema/annotations.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2837 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/jsonschema/builder.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      746 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/jsonschema/dialects.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     5946 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/jsonschema/models.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    25698 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/jsonschema/schema.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.748973 mashumaro-3.8.1/mashumaro/mixins/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/mixins/__init__.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1867 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/mixins/dict.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      790 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/mixins/json.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1558 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/mixins/msgpack.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1731 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/mixins/orjson.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1000 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/mixins/orjson.pyi
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1392 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/mixins/toml.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1108 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/mixins/yaml.py
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/py.typed
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     2715 2023-06-22 18:41:04.000000 mashumaro-3.8.1/mashumaro/types.py
-drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-06-23 16:33:05.730925 mashumaro-3.8.1/mashumaro.egg-info/
--rw-r--r--   0 tikhonov_a   (501) staff       (20)    97544 2023-06-23 16:33:05.000000 mashumaro-3.8.1/mashumaro.egg-info/PKG-INFO
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1210 2023-06-23 16:33:05.000000 mashumaro-3.8.1/mashumaro.egg-info/SOURCES.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-06-23 16:33:05.000000 mashumaro-3.8.1/mashumaro.egg-info/dependency_links.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-06-22 18:41:44.000000 mashumaro-3.8.1/mashumaro.egg-info/not-zip-safe
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      155 2023-06-23 16:33:05.000000 mashumaro-3.8.1/mashumaro.egg-info/requires.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-06-23 16:33:05.000000 mashumaro-3.8.1/mashumaro.egg-info/top_level.txt
--rw-r--r--   0 tikhonov_a   (501) staff       (20)      689 2023-06-22 18:41:04.000000 mashumaro-3.8.1/pyproject.toml
--rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-06-23 16:33:05.749603 mashumaro-3.8.1/setup.cfg
--rw-r--r--   0 tikhonov_a   (501) staff       (20)     1465 2023-06-23 16:32:39.000000 mashumaro-3.8.1/setup.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.399084 mashumaro-3.9/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    10763 2023-06-22 18:41:04.000000 mashumaro-3.9/LICENSE
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    95909 2023-08-02 20:00:20.398848 mashumaro-3.9/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    94990 2023-08-02 19:58:06.000000 mashumaro-3.9/README.md
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.382670 mashumaro-3.9/mashumaro/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      258 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1674 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/config.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.384059 mashumaro-3.9/mashumaro/core/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1013 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/const.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      825 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/helpers.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.384634 mashumaro-3.9/mashumaro/core/meta/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/__init__.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.385145 mashumaro-3.9/mashumaro/core/meta/code/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/code/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    43193 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/core/meta/code/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      815 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/code/lines.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    22345 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/core/meta/helpers.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1366 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/mixin.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.385743 mashumaro-3.9/mashumaro/core/meta/types/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/types/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     4882 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/core/meta/types/common.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    25046 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/core/meta/types/pack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    42525 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/core/meta/types/unpack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      469 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/dialect.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5491 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/exceptions.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1472 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/helper.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.386654 mashumaro-3.9/mashumaro/jsonschema/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      214 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/jsonschema/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2151 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/jsonschema/annotations.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2837 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/jsonschema/builder.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      747 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/jsonschema/dialects.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     5946 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/jsonschema/models.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    26112 2023-08-02 19:56:28.000000 mashumaro-3.9/mashumaro/jsonschema/schema.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.397990 mashumaro-3.9/mashumaro/mixins/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/__init__.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1867 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/dict.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      790 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/json.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1558 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/msgpack.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1731 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/orjson.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1000 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/orjson.pyi
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1392 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/toml.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1108 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/mixins/yaml.py
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        0 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/py.typed
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     2715 2023-06-22 18:41:04.000000 mashumaro-3.9/mashumaro/types.py
+drwxr-xr-x   0 tikhonov_a   (501) staff       (20)        0 2023-08-02 20:00:20.383597 mashumaro-3.9/mashumaro.egg-info/
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)    95909 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/PKG-INFO
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1210 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)        1 2023-06-22 18:41:44.000000 mashumaro-3.9/mashumaro.egg-info/not-zip-safe
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      155 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/requires.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       10 2023-08-02 20:00:20.000000 mashumaro-3.9/mashumaro.egg-info/top_level.txt
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)      689 2023-06-22 18:41:04.000000 mashumaro-3.9/pyproject.toml
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)       38 2023-08-02 20:00:20.399135 mashumaro-3.9/setup.cfg
+-rw-r--r--   0 tikhonov_a   (501) staff       (20)     1463 2023-08-02 20:00:13.000000 mashumaro-3.9/setup.py
```

### Comparing `mashumaro-3.8.1/LICENSE` & `mashumaro-3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/PKG-INFO` & `mashumaro-3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,10 @@
-Metadata-Version: 2.1
-Name: mashumaro
-Version: 3.8.1
-Summary: Fast serialization library on top of dataclasses
-Home-page: https://github.com/Fatal1ty/mashumaro
-Author: Alexander Tikhonov
-Author-email: random.gauss@gmail.com
-License: Apache License, Version 2.0
-Platform: all
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Development Status :: 5 - Production/Stable
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: orjson
-Provides-Extra: msgpack
-Provides-Extra: yaml
-Provides-Extra: toml
-License-File: LICENSE
-
 <div align="center">
 
-<img alt="logo" width="175" src="https://github.com/Fatal1ty/mashumaro/blob/master/img/logo.svg">
+<img alt="logo" width="175" src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/ac2f924591d488dbd9a776a6b1ae7dede2d8c73e/img/logo.svg">
 
 ###### Fast and well tested serialization library on top of dataclasses
 
 [![Build Status](https://github.com/Fatal1ty/mashumaro/workflows/tests/badge.svg)](https://github.com/Fatal1ty/mashumaro/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Fatal1ty/mashumaro/badge.svg?branch=master)](https://coveralls.io/github/Fatal1ty/mashumaro?branch=master)
 [![Latest Version](https://img.shields.io/pypi/v/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![Python Version](https://img.shields.io/pypi/pyversions/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
@@ -327,102 +301,40 @@
 runtime in some cases) and are set as attributes to your dataclasses.
 To minimize the import time, you can explicitly enable
 [lazy compilation](#lazy_compilation-config-option).
 
 Benchmark
 --------------------------------------------------------------------------------
 
-* macOS 13.0.1 Ventura
+* macOS 13.3.1 Ventura
 * Apple M1
-* 8GB RAM
-* Python 3.11.0
-
-Load and dump [sample data](https://github.com/Fatal1ty/mashumaro/blob/master/benchmark/sample.py) 100 times in 5 runs.
-The following figures show the best overall time in each case.
-
-[//]: # (<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.png" width="400">)
+* 16GB RAM
+* Python 3.11.4
 
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg">
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_dark.svg">
-  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg" width="400">
-</picture>
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg">
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_dark.svg">
-  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg" width="400">
-</picture>
-
-<table>
-  <col>
-  <colgroup span="2"></colgroup>
-  <colgroup span="2"></colgroup>
-  <tr>
-    <th rowspan="2">Library</th>
-    <th colspan="2" scope="colgroup">From dict</th>
-    <th colspan="2" scope="colgroup">To dict</th>
-</tr>
-<tr>
-    <th scope="col">Time</th>
-    <th scope="col">Slowdown factor</th>
-    <th scope="col">Time</th>
-    <th scope="col">Slowdown factor</th>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/Fatal1ty/mashumaro">mashumaro</a></th>
-    <td align="right">0.14724</td>
-    <td align="left">1x</td>
-    <td align="right">0.10128</td>
-    <td align="left">1x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/Tinche/cattrs">cattrs</a></th>
-    <td align="right">0.18906</td>
-    <td align="left">1.28x</td>
-    <td align="right">0.14072</td>
-    <td align="left">1.39x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/samuelcolvin/pydantic/">pydantic</a></th>
-    <td align="right">1.02666</td>
-    <td align="left">6.97x</td>
-    <td align="right">0.81932</td>
-    <td align="left">8.09x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/marshmallow-code/marshmallow">marshmallow</a></th>
-    <td align="right">1.38348</td>
-    <td align="left">9.4x</td>
-    <td align="right">0.45695</td>
-    <td align="left">4.51x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict">dataclasses</a></th>
-    <td align="left">—</td>
-    <td align="left">—</td>
-    <td align="right">0.68057</td>
-    <td align="left">6.72x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/konradhalas/dacite">dacite</a></th>
-    <td align="right">2.37315</td>
-    <td align="left">16.12x</td>
-    <td align="left">—</td>
-    <td align="left">—</td>
-</tr>
-</table>
+Benchmark using [pyperf](https://github.com/psf/pyperf) with GitHub Issue model. Please note that the
+following charts use logarithmic scale, as it is convenient for displaying
+very large ranges of values.
+
+<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/381306ea92808c256354fe890bb5aa60cd3bb787/benchmark/charts/load_light.svg" width="604">
+<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/381306ea92808c256354fe890bb5aa60cd3bb787/benchmark/charts/dump_light.svg" width="604">
+
+> [!NOTE]\
+> Benchmark results may vary depending on the specific configuration and
+> parameters used for serialization and deserialization. However, we have made
+> an attempt to use the available options that can speed up and smooth out the
+> differences in how libraries work.
 
 To run benchmark in your environment:
 ```bash
 git clone git@github.com:Fatal1ty/mashumaro.git
 cd mashumaro
 python3 -m venv env && source env/bin/activate
 pip install -e .
 pip install -r requirements-dev.txt
-python benchmark/run.py
+./benchmark/run.sh
 ```
 
 Serialization mixins
 --------------------------------------------------------------------------------
 
 `mashumaro` provides mixins for each serialization format.
 
@@ -674,18 +586,19 @@
 assert my_plan.to_dict() == input_data
 ```
 
 Here we add annotations to the only argument of `_deserialize` method and
 to the return value of `_serialize` method as well. The latter is needed for
 correct serialization.
 
-The importance of explicit passing `use_annotations=True` when defining a class
-is that otherwise implicit using annotations might break compatibility with old
-code that wasn't aware of this feature. It will be enabled by default in the
-future major release.
+> [!IMPORTANT]\
+> The importance of explicit passing `use_annotations=True` when defining a
+> class is that otherwise implicit using annotations might break compatibility
+> with old code that wasn't aware of this feature. It will be enabled by
+> default in the future major release.
 
 #### User-defined generic types
 
 The great thing to note about using annotations in `SerializableType` is that
 they work seamlessly with [generic](https://docs.python.org/3/library/typing.html#user-defined-generic-types)
 and [variadic generic](https://peps.python.org/pep-0646/) types.
 Let's see how this can be useful:
@@ -815,15 +728,17 @@
 print(example.to_dict())
 # {'dt': 1672531200.0}
 ```
 
 Here the passed string value `"1672531200"` will be converted to `float` before being passed to `deserialize` method
 thanks to the `float` annotation.
 
-As well as for `SerializableType`, the value of `use_annotatons` will be `True` by default in the future major release.
+> [!IMPORTANT]\
+> As well as for `SerializableType`, the value of `use_annotatons` will be
+> `True` by default in the future major release.
 
 #### Third-party generic types
 
 To create a generic version of a serialization strategy you need to follow these steps:
 * inherit [`Generic[...]`](https://docs.python.org/3/library/typing.html#typing.Generic) type
 with the number of parameters matching the number of parameters
 of the target generic type
@@ -905,15 +820,16 @@
 with. At this moment there are next serialization engines to choose from:
 
 | Applicable data types      | Supported engines    | Description                                                                                                                                                                                                  |
 |:---------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `NamedTuple`, `namedtuple` | `as_list`, `as_dict` | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
 | `Any`                      | `omit`               | Skip the field during serialization                                                                                                                                                                          |
 
-In addition, you can pass a field value as is without changes using
+> [!NOTE]\
+> You can pass a field value as is without changes on serialization using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
 from datetime import datetime
 from dataclasses import dataclass, field
@@ -949,15 +865,16 @@
 with. At this moment there are next deserialization engines to choose from:
 
 | Applicable data types      | Supported engines                                                                                                                   | Description                                                                                                                                                                                                                                                                                             |
 |:---------------------------|:------------------------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `datetime`, `date`, `time` | [`ciso8601`](https://github.com/closeio/ciso8601#supported-subset-of-iso-8601), [`pendulum`](https://github.com/sdispater/pendulum) | How to parse datetime string. By default native [`fromisoformat`](https://docs.python.org/3/library/datetime.html#datetime.datetime.fromisoformat) of corresponding class will be used for `datetime`, `date` and `time` fields. It's the fastest way in most cases, but you can choose an alternative. |
 | `NamedTuple`, `namedtuple` | `as_list`, `as_dict`                                                                                                                | How to unpack named tuples. By default `as_list` engine is used that means your named tuple class instance will be created from a list of its values. You can unpack it from a dictionary using `as_dict` engine.                                                                                       |
 
-In addition, you can pass a field value as is without changes using
+> [!NOTE]\
+> You can pass a field value as is without changes on deserialization using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
 from datetime import datetime
 from dataclasses import dataclass, field
@@ -993,17 +910,21 @@
 class D(DataClassDictMixin):
     x: MyNamedTuple = field(metadata={"deserialize": "as_dict"})
 ```
 
 #### `serialization_strategy` option
 
 This option is useful when you want to change the serialization logic
-for a dataclass field depending on some defined parameters using a reusable serialization scheme.
-You can find an example in the [`SerializationStrategy`](#serializationstrategy) chapter.
-In addition, you can pass a field value as is without changes using
+for a dataclass field depending on some defined parameters using a reusable
+serialization scheme. You can find an example in the
+[`SerializationStrategy`](#serializationstrategy) chapter.
+
+> [!NOTE]\
+> You can pass a field value as is without changes on
+> serialization / deserialization using
 [`pass_through`](#passing-field-values-as-is).
 
 #### `alias` option
 
 In some cases it's better to have different names for a field in your class and
 in its serialized view. For example, a third-party legacy API you are working
 with might operate with camel case style, but you stick to snake case style in
@@ -1156,16 +1077,16 @@
 instance = DataClass.from_dict({"x": "2021", "y": "2021"})
 # DataClass(x=datetime.datetime(2021, 1, 1, 0, 0), y=Date(2021, 1, 1))
 dictionary = instance.to_dict()
 # {'x': '2021', 'y': '2021-01-01'}
 ```
 
 Note that you can register different methods for multiple logical types which
-are based on the same type using `NewType` and `Annotated`.
-See [Extending existing types](#extending-existing-types) for details.
+are based on the same type using `NewType` and `Annotated`,
+see [Extending existing types](#extending-existing-types) for details.
 
 #### `aliases` config option
 
 Sometimes it's better to write the field aliases in one place. You can mix
 aliases here with [aliases in the field options](#alias-option), but the last ones will always
 take precedence.
 
@@ -1378,29 +1299,28 @@
 #### `lazy_compilation` config option
 
 By using this option, the compilation of the `from_*` and `to_*` methods will
 be deferred until they are called first time. This will reduce the import time
 and, in certain instances, may enhance the speed of deserialization
 by leveraging the data that is accessible after the class has been created.
 
-> **Warning**
->
+> [!Warning]\
 > If you need to save a reference to `from_*` or `to_*` method, you should
 > do it after the method is compiled. To be safe, you can always use lambda
 > function:
 > ```python
 > from_dict = lambda x: MyModel.from_dict(x)
 > to_dict = lambda x: x.to_dict()
 > ```
 
 ### Passing field values as is
 
 In some cases it's needed to pass a field value as is without any changes
 during serialization / deserialization. There is a predefined
-[`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L49)
+[`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L58)
 object that can be used as `serialization_strategy` or
 `serialize` / `deserialize` options:
 
 ```python
 from dataclasses import dataclass, field
 from mashumaro import DataClassDictMixin, pass_through
 
@@ -1627,16 +1547,15 @@
 
 * without annotations: `type = 42`
 * annotated as ClassVar: `type: ClassVar[int] = 42`
 * annotated as Final: `type: Final[int] = 42`
 * annotated as Literal: `type: Literal[42] = 42`
 * annotated as StrEnum: `type: ResponseType = ResponseType.OK`
 
-> **Note**
->
+> [!NOTE]\
 > Keep in mind that by default only Final, Literal and StrEnum fields are
 > processed during serialization.
 
 Next, we will look at different use cases, as well as their pros and cons.
 
 #### Subclasses distinguishable by a field
 
@@ -1648,16 +1567,15 @@
 impractical. Moreover, deserialization of the union would be slow, since we
 need to iterate over each variant in the list until we find the right one.
 
 We can improve subclass deserialization using `Discriminator` as annotation
 within `Annotated` type. We will use `field` parameter and set
 `include_subtypes` to `True`.
 
-> **Note**
->
+> [!IMPORTANT]\
 > The discriminator field should be accessible from the `__dict__` attribute
 > of a specific descendant, i.e. defined at the level of that descendant.
 > A descendant class without a discriminator field will be ignored, but
 > its descendants won't.
 
 Suppose we have a hierarchy of client events distinguishable by a class
 attribute "type":
@@ -1953,20 +1871,22 @@
 
 Again, it's not necessary to have a common superclass. If you have a union of
 dataclasses without a field that they can be distinguishable by, you can still
 use `Discriminator`, but deserialization will almost be the same as for `Union`
 type without `Discriminator` except that it could be possible to deserialize
 subclasses with `include_subtypes=True`.
 
-> **Note**
->
+> [!IMPORTANT]\
 > When both `include_subtypes` and `include_supertypes` are enabled,
 > all subclasses will be attempted to be deserialized first,
 > superclasses — at the end.
 
+In the following example you can see how priority works — first we try
+to deserialize `ChickpeaHummus`, and if it fails, then we try `Hummus`:
+
 ```python
 @dataclass
 class Hummus(DataClassDictMixin):
     made_of: Literal["chickpeas", "artichoke"]
     grams: int
 
 @dataclass
@@ -2386,25 +2306,25 @@
 ### Building JSON Schema
 
 For simple one-time cases it's recommended to start from using a configurable
 `build_json_schema` function. It returns `JSONSchema` object that can be
 serialized to json or to dict:
 
 ```python
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import List
 from uuid import UUID
 
 from mashumaro.jsonschema import build_json_schema
 
 
 @dataclass
 class User:
     id: UUID
-    name: str
+    name: str = field(metadata={"description": "User name"})
 
 
 print(build_json_schema(List[User]).to_json())
 ```
 
 <details>
 <summary>Click to show the result</summary>
@@ -2417,15 +2337,16 @@
         "title": "User",
         "properties": {
             "id": {
                 "type": "string",
                 "format": "uuid"
             },
             "name": {
-                "type": "string"
+                "type": "string",
+                "description": "User name"
             }
         },
         "additionalProperties": false,
         "required": [
             "id",
             "name"
         ]
@@ -2541,15 +2462,15 @@
             "required": [
                 "id",
                 "name"
             ]
         }
     },
     "items": {
-        "$ref": "#/defs/User"
+        "$ref": "#/$defs/User"
     }
 }
 ```
 </details>
 
 The definitions section can be omitted from the final document by setting
 `with_definitions` parameter to `False`:
@@ -2720,15 +2641,17 @@
 * [`MaxProperties`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-maxproperties)
 * [`MinProperties`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-minproperties)
 * [`DependentRequired`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-dependentrequired)
 
 ### Extending JSON Schema
 
 Using a `Config` class it is possible to override some parts of the schema.
-Currently, it works for dataclass fields via "properties" key:
+Currently, you can do the following:
+* override some field schemas using the "properties" key
+* change `additionalProperties` using the "additionalProperties" key
 
 ```python
 from dataclasses import dataclass
 from mashumaro.jsonschema import build_json_schema
 
 @dataclass
 class FooBar:
@@ -2738,15 +2661,16 @@
     class Config:
         json_schema = {
             "properties": {
                 "foo": {
                     "type": "string",
                     "description": "bar"
                 }
-            }
+            },
+            "additionalProperties": True,
         }
 
 print(build_json_schema(FooBar).to_json())
 ```
 
 <details>
 <summary>Click to show the result</summary>
@@ -2760,23 +2684,26 @@
             "type": "string",
             "description": "bar"
         },
         "bar": {
             "type": "integer"
         }
     },
-    "additionalProperties": false,
+    "additionalProperties": true,
     "required": [
         "foo",
         "bar"
     ]
 }
 ```
 </details>
 
+You can also change the "additionalProperties" key to a specific schema
+by passing it a `JSONSchema` instance instead of a bool value.
+
 ### JSON Schema and custom serialization methods
 
 Mashumaro provides different ways to override default serialization methods for
 dataclass fields or specific data types. In order for these overrides to be
 reflected in the schema, you need to make sure that the methods have
 annotations of the return value type.
```

### Comparing `mashumaro-3.8.1/README.md` & `mashumaro-3.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,36 @@
+Metadata-Version: 2.1
+Name: mashumaro
+Version: 3.9
+Summary: Fast serialization library on top of dataclasses
+Home-page: https://github.com/Fatal1ty/mashumaro
+Author: Alexander Tikhonov
+Author-email: random.gauss@gmail.com
+License: Apache License, Version 2.0
+Platform: all
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Development Status :: 5 - Production/Stable
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: orjson
+Provides-Extra: msgpack
+Provides-Extra: yaml
+Provides-Extra: toml
+License-File: LICENSE
+
 <div align="center">
 
-<img alt="logo" width="175" src="https://github.com/Fatal1ty/mashumaro/blob/master/img/logo.svg">
+<img alt="logo" width="175" src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/ac2f924591d488dbd9a776a6b1ae7dede2d8c73e/img/logo.svg">
 
 ###### Fast and well tested serialization library on top of dataclasses
 
 [![Build Status](https://github.com/Fatal1ty/mashumaro/workflows/tests/badge.svg)](https://github.com/Fatal1ty/mashumaro/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Fatal1ty/mashumaro/badge.svg?branch=master)](https://coveralls.io/github/Fatal1ty/mashumaro?branch=master)
 [![Latest Version](https://img.shields.io/pypi/v/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![Python Version](https://img.shields.io/pypi/pyversions/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
@@ -301,102 +327,40 @@
 runtime in some cases) and are set as attributes to your dataclasses.
 To minimize the import time, you can explicitly enable
 [lazy compilation](#lazy_compilation-config-option).
 
 Benchmark
 --------------------------------------------------------------------------------
 
-* macOS 13.0.1 Ventura
+* macOS 13.3.1 Ventura
 * Apple M1
-* 8GB RAM
-* Python 3.11.0
-
-Load and dump [sample data](https://github.com/Fatal1ty/mashumaro/blob/master/benchmark/sample.py) 100 times in 5 runs.
-The following figures show the best overall time in each case.
-
-[//]: # (<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.png" width="400">)
+* 16GB RAM
+* Python 3.11.4
 
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg">
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_dark.svg">
-  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg" width="400">
-</picture>
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg">
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_dark.svg">
-  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg" width="400">
-</picture>
-
-<table>
-  <col>
-  <colgroup span="2"></colgroup>
-  <colgroup span="2"></colgroup>
-  <tr>
-    <th rowspan="2">Library</th>
-    <th colspan="2" scope="colgroup">From dict</th>
-    <th colspan="2" scope="colgroup">To dict</th>
-</tr>
-<tr>
-    <th scope="col">Time</th>
-    <th scope="col">Slowdown factor</th>
-    <th scope="col">Time</th>
-    <th scope="col">Slowdown factor</th>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/Fatal1ty/mashumaro">mashumaro</a></th>
-    <td align="right">0.14724</td>
-    <td align="left">1x</td>
-    <td align="right">0.10128</td>
-    <td align="left">1x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/Tinche/cattrs">cattrs</a></th>
-    <td align="right">0.18906</td>
-    <td align="left">1.28x</td>
-    <td align="right">0.14072</td>
-    <td align="left">1.39x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/samuelcolvin/pydantic/">pydantic</a></th>
-    <td align="right">1.02666</td>
-    <td align="left">6.97x</td>
-    <td align="right">0.81932</td>
-    <td align="left">8.09x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/marshmallow-code/marshmallow">marshmallow</a></th>
-    <td align="right">1.38348</td>
-    <td align="left">9.4x</td>
-    <td align="right">0.45695</td>
-    <td align="left">4.51x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict">dataclasses</a></th>
-    <td align="left">—</td>
-    <td align="left">—</td>
-    <td align="right">0.68057</td>
-    <td align="left">6.72x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/konradhalas/dacite">dacite</a></th>
-    <td align="right">2.37315</td>
-    <td align="left">16.12x</td>
-    <td align="left">—</td>
-    <td align="left">—</td>
-</tr>
-</table>
+Benchmark using [pyperf](https://github.com/psf/pyperf) with GitHub Issue model. Please note that the
+following charts use logarithmic scale, as it is convenient for displaying
+very large ranges of values.
+
+<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/381306ea92808c256354fe890bb5aa60cd3bb787/benchmark/charts/load_light.svg" width="604">
+<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/381306ea92808c256354fe890bb5aa60cd3bb787/benchmark/charts/dump_light.svg" width="604">
+
+> [!NOTE]\
+> Benchmark results may vary depending on the specific configuration and
+> parameters used for serialization and deserialization. However, we have made
+> an attempt to use the available options that can speed up and smooth out the
+> differences in how libraries work.
 
 To run benchmark in your environment:
 ```bash
 git clone git@github.com:Fatal1ty/mashumaro.git
 cd mashumaro
 python3 -m venv env && source env/bin/activate
 pip install -e .
 pip install -r requirements-dev.txt
-python benchmark/run.py
+./benchmark/run.sh
 ```
 
 Serialization mixins
 --------------------------------------------------------------------------------
 
 `mashumaro` provides mixins for each serialization format.
 
@@ -648,18 +612,19 @@
 assert my_plan.to_dict() == input_data
 ```
 
 Here we add annotations to the only argument of `_deserialize` method and
 to the return value of `_serialize` method as well. The latter is needed for
 correct serialization.
 
-The importance of explicit passing `use_annotations=True` when defining a class
-is that otherwise implicit using annotations might break compatibility with old
-code that wasn't aware of this feature. It will be enabled by default in the
-future major release.
+> [!IMPORTANT]\
+> The importance of explicit passing `use_annotations=True` when defining a
+> class is that otherwise implicit using annotations might break compatibility
+> with old code that wasn't aware of this feature. It will be enabled by
+> default in the future major release.
 
 #### User-defined generic types
 
 The great thing to note about using annotations in `SerializableType` is that
 they work seamlessly with [generic](https://docs.python.org/3/library/typing.html#user-defined-generic-types)
 and [variadic generic](https://peps.python.org/pep-0646/) types.
 Let's see how this can be useful:
@@ -789,15 +754,17 @@
 print(example.to_dict())
 # {'dt': 1672531200.0}
 ```
 
 Here the passed string value `"1672531200"` will be converted to `float` before being passed to `deserialize` method
 thanks to the `float` annotation.
 
-As well as for `SerializableType`, the value of `use_annotatons` will be `True` by default in the future major release.
+> [!IMPORTANT]\
+> As well as for `SerializableType`, the value of `use_annotatons` will be
+> `True` by default in the future major release.
 
 #### Third-party generic types
 
 To create a generic version of a serialization strategy you need to follow these steps:
 * inherit [`Generic[...]`](https://docs.python.org/3/library/typing.html#typing.Generic) type
 with the number of parameters matching the number of parameters
 of the target generic type
@@ -879,15 +846,16 @@
 with. At this moment there are next serialization engines to choose from:
 
 | Applicable data types      | Supported engines    | Description                                                                                                                                                                                                  |
 |:---------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `NamedTuple`, `namedtuple` | `as_list`, `as_dict` | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
 | `Any`                      | `omit`               | Skip the field during serialization                                                                                                                                                                          |
 
-In addition, you can pass a field value as is without changes using
+> [!NOTE]\
+> You can pass a field value as is without changes on serialization using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
 from datetime import datetime
 from dataclasses import dataclass, field
@@ -923,15 +891,16 @@
 with. At this moment there are next deserialization engines to choose from:
 
 | Applicable data types      | Supported engines                                                                                                                   | Description                                                                                                                                                                                                                                                                                             |
 |:---------------------------|:------------------------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `datetime`, `date`, `time` | [`ciso8601`](https://github.com/closeio/ciso8601#supported-subset-of-iso-8601), [`pendulum`](https://github.com/sdispater/pendulum) | How to parse datetime string. By default native [`fromisoformat`](https://docs.python.org/3/library/datetime.html#datetime.datetime.fromisoformat) of corresponding class will be used for `datetime`, `date` and `time` fields. It's the fastest way in most cases, but you can choose an alternative. |
 | `NamedTuple`, `namedtuple` | `as_list`, `as_dict`                                                                                                                | How to unpack named tuples. By default `as_list` engine is used that means your named tuple class instance will be created from a list of its values. You can unpack it from a dictionary using `as_dict` engine.                                                                                       |
 
-In addition, you can pass a field value as is without changes using
+> [!NOTE]\
+> You can pass a field value as is without changes on deserialization using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
 from datetime import datetime
 from dataclasses import dataclass, field
@@ -967,17 +936,21 @@
 class D(DataClassDictMixin):
     x: MyNamedTuple = field(metadata={"deserialize": "as_dict"})
 ```
 
 #### `serialization_strategy` option
 
 This option is useful when you want to change the serialization logic
-for a dataclass field depending on some defined parameters using a reusable serialization scheme.
-You can find an example in the [`SerializationStrategy`](#serializationstrategy) chapter.
-In addition, you can pass a field value as is without changes using
+for a dataclass field depending on some defined parameters using a reusable
+serialization scheme. You can find an example in the
+[`SerializationStrategy`](#serializationstrategy) chapter.
+
+> [!NOTE]\
+> You can pass a field value as is without changes on
+> serialization / deserialization using
 [`pass_through`](#passing-field-values-as-is).
 
 #### `alias` option
 
 In some cases it's better to have different names for a field in your class and
 in its serialized view. For example, a third-party legacy API you are working
 with might operate with camel case style, but you stick to snake case style in
@@ -1130,16 +1103,16 @@
 instance = DataClass.from_dict({"x": "2021", "y": "2021"})
 # DataClass(x=datetime.datetime(2021, 1, 1, 0, 0), y=Date(2021, 1, 1))
 dictionary = instance.to_dict()
 # {'x': '2021', 'y': '2021-01-01'}
 ```
 
 Note that you can register different methods for multiple logical types which
-are based on the same type using `NewType` and `Annotated`.
-See [Extending existing types](#extending-existing-types) for details.
+are based on the same type using `NewType` and `Annotated`,
+see [Extending existing types](#extending-existing-types) for details.
 
 #### `aliases` config option
 
 Sometimes it's better to write the field aliases in one place. You can mix
 aliases here with [aliases in the field options](#alias-option), but the last ones will always
 take precedence.
 
@@ -1352,29 +1325,28 @@
 #### `lazy_compilation` config option
 
 By using this option, the compilation of the `from_*` and `to_*` methods will
 be deferred until they are called first time. This will reduce the import time
 and, in certain instances, may enhance the speed of deserialization
 by leveraging the data that is accessible after the class has been created.
 
-> **Warning**
->
+> [!Warning]\
 > If you need to save a reference to `from_*` or `to_*` method, you should
 > do it after the method is compiled. To be safe, you can always use lambda
 > function:
 > ```python
 > from_dict = lambda x: MyModel.from_dict(x)
 > to_dict = lambda x: x.to_dict()
 > ```
 
 ### Passing field values as is
 
 In some cases it's needed to pass a field value as is without any changes
 during serialization / deserialization. There is a predefined
-[`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L49)
+[`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L58)
 object that can be used as `serialization_strategy` or
 `serialize` / `deserialize` options:
 
 ```python
 from dataclasses import dataclass, field
 from mashumaro import DataClassDictMixin, pass_through
 
@@ -1601,16 +1573,15 @@
 
 * without annotations: `type = 42`
 * annotated as ClassVar: `type: ClassVar[int] = 42`
 * annotated as Final: `type: Final[int] = 42`
 * annotated as Literal: `type: Literal[42] = 42`
 * annotated as StrEnum: `type: ResponseType = ResponseType.OK`
 
-> **Note**
->
+> [!NOTE]\
 > Keep in mind that by default only Final, Literal and StrEnum fields are
 > processed during serialization.
 
 Next, we will look at different use cases, as well as their pros and cons.
 
 #### Subclasses distinguishable by a field
 
@@ -1622,16 +1593,15 @@
 impractical. Moreover, deserialization of the union would be slow, since we
 need to iterate over each variant in the list until we find the right one.
 
 We can improve subclass deserialization using `Discriminator` as annotation
 within `Annotated` type. We will use `field` parameter and set
 `include_subtypes` to `True`.
 
-> **Note**
->
+> [!IMPORTANT]\
 > The discriminator field should be accessible from the `__dict__` attribute
 > of a specific descendant, i.e. defined at the level of that descendant.
 > A descendant class without a discriminator field will be ignored, but
 > its descendants won't.
 
 Suppose we have a hierarchy of client events distinguishable by a class
 attribute "type":
@@ -1927,20 +1897,22 @@
 
 Again, it's not necessary to have a common superclass. If you have a union of
 dataclasses without a field that they can be distinguishable by, you can still
 use `Discriminator`, but deserialization will almost be the same as for `Union`
 type without `Discriminator` except that it could be possible to deserialize
 subclasses with `include_subtypes=True`.
 
-> **Note**
->
+> [!IMPORTANT]\
 > When both `include_subtypes` and `include_supertypes` are enabled,
 > all subclasses will be attempted to be deserialized first,
 > superclasses — at the end.
 
+In the following example you can see how priority works — first we try
+to deserialize `ChickpeaHummus`, and if it fails, then we try `Hummus`:
+
 ```python
 @dataclass
 class Hummus(DataClassDictMixin):
     made_of: Literal["chickpeas", "artichoke"]
     grams: int
 
 @dataclass
@@ -2360,25 +2332,25 @@
 ### Building JSON Schema
 
 For simple one-time cases it's recommended to start from using a configurable
 `build_json_schema` function. It returns `JSONSchema` object that can be
 serialized to json or to dict:
 
 ```python
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import List
 from uuid import UUID
 
 from mashumaro.jsonschema import build_json_schema
 
 
 @dataclass
 class User:
     id: UUID
-    name: str
+    name: str = field(metadata={"description": "User name"})
 
 
 print(build_json_schema(List[User]).to_json())
 ```
 
 <details>
 <summary>Click to show the result</summary>
@@ -2391,15 +2363,16 @@
         "title": "User",
         "properties": {
             "id": {
                 "type": "string",
                 "format": "uuid"
             },
             "name": {
-                "type": "string"
+                "type": "string",
+                "description": "User name"
             }
         },
         "additionalProperties": false,
         "required": [
             "id",
             "name"
         ]
@@ -2515,15 +2488,15 @@
             "required": [
                 "id",
                 "name"
             ]
         }
     },
     "items": {
-        "$ref": "#/defs/User"
+        "$ref": "#/$defs/User"
     }
 }
 ```
 </details>
 
 The definitions section can be omitted from the final document by setting
 `with_definitions` parameter to `False`:
@@ -2694,15 +2667,17 @@
 * [`MaxProperties`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-maxproperties)
 * [`MinProperties`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-minproperties)
 * [`DependentRequired`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-dependentrequired)
 
 ### Extending JSON Schema
 
 Using a `Config` class it is possible to override some parts of the schema.
-Currently, it works for dataclass fields via "properties" key:
+Currently, you can do the following:
+* override some field schemas using the "properties" key
+* change `additionalProperties` using the "additionalProperties" key
 
 ```python
 from dataclasses import dataclass
 from mashumaro.jsonschema import build_json_schema
 
 @dataclass
 class FooBar:
@@ -2712,15 +2687,16 @@
     class Config:
         json_schema = {
             "properties": {
                 "foo": {
                     "type": "string",
                     "description": "bar"
                 }
-            }
+            },
+            "additionalProperties": True,
         }
 
 print(build_json_schema(FooBar).to_json())
 ```
 
 <details>
 <summary>Click to show the result</summary>
@@ -2734,23 +2710,26 @@
             "type": "string",
             "description": "bar"
         },
         "bar": {
             "type": "integer"
         }
     },
-    "additionalProperties": false,
+    "additionalProperties": true,
     "required": [
         "foo",
         "bar"
     ]
 }
 ```
 </details>
 
+You can also change the "additionalProperties" key to a specific schema
+by passing it a `JSONSchema` instance instead of a bool value.
+
 ### JSON Schema and custom serialization methods
 
 Mashumaro provides different ways to override default serialization methods for
 dataclass fields or specific data types. In order for these overrides to be
 reflected in the schema, you need to make sure that the methods have
 annotations of the return value type.
```

### Comparing `mashumaro-3.8.1/mashumaro/config.py` & `mashumaro-3.9/mashumaro/config.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/core/const.py` & `mashumaro-3.9/mashumaro/core/const.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/core/helpers.py` & `mashumaro-3.9/mashumaro/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/core/meta/code/builder.py` & `mashumaro-3.9/mashumaro/core/meta/code/builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,17 @@
     get_class_that_defines_field,
     get_class_that_defines_method,
     get_literal_values,
     get_name_error_name,
     hash_type_args,
     is_class_var,
     is_dataclass_dict_mixin,
+    is_dataclass_dict_mixin_subclass,
     is_dialect_subclass,
+    is_hashable,
     is_init_var,
     is_literal,
     is_optional,
     is_type_var_any,
     resolve_type_params,
     substitute_type_params,
     type_name,
@@ -70,14 +72,27 @@
 
 __PRE_SERIALIZE__ = "__pre_serialize__"
 __PRE_DESERIALIZE__ = "__pre_deserialize__"
 __POST_SERIALIZE__ = "__post_serialize__"
 __POST_DESERIALIZE__ = "__post_deserialize__"
 
 
+class InternalMethodName(str):
+    _PREFIX = "__mashumaro_"
+    _SUFFIX = "__"
+
+    @classmethod
+    def from_public(cls, value: str) -> "InternalMethodName":
+        return cls(f"{cls._PREFIX}{value}{cls._SUFFIX}")
+
+    @property
+    def public(self) -> str:
+        return self[len(self._PREFIX) : -len(self._SUFFIX)]
+
+
 class CodeBuilder:
     def __init__(
         self,
         cls: typing.Type,
         type_args: typing.Tuple[typing.Type, ...] = (),
         dialect: typing.Optional[typing.Type[Dialect]] = None,
         first_method: str = "from_dict",
@@ -455,14 +470,18 @@
                     self._add_unpack_method_lines(method_name)
                 with self.indent("else:"):
                     self._add_unpack_method_with_dialect_lines(method_name)
             else:
                 self._add_unpack_method_lines(method_name)
         if self.dialect is None:
             self.add_line(f"setattr(cls, '{method_name}', {method_name})")
+            if is_dataclass_dict_mixin_subclass(self.cls):
+                self.add_line(
+                    f"setattr(cls, '{method_name.public}', {method_name})"
+                )
         else:
             self.add_line(f"cls.{cache_name}[dialect] = {method_name}")
         self.compile()
 
     def _add_unpack_method_definition(self, method_name: str) -> None:
         kwargs = ""
         default_kwargs = self.get_unpack_method_default_flag_values(
@@ -732,41 +751,41 @@
 
     @classmethod
     def get_unpack_method_name(
         cls,
         type_args: typing.Iterable = (),
         format_name: str = "dict",
         decoder: typing.Optional[typing.Any] = None,
-    ) -> str:
+    ) -> InternalMethodName:
         if format_name != "dict" and decoder is not None:
-            return f"from_{format_name}"
+            return InternalMethodName.from_public(f"from_{format_name}")
         else:
             method_name = "from_dict"
             if format_name != "dict":
                 method_name += f"_{format_name}"
             if type_args:
                 method_name += f"_{hash_type_args(type_args)}"
-            return method_name
+            return InternalMethodName.from_public(method_name)
 
     @classmethod
     def get_pack_method_name(
         cls,
         type_args: typing.Tuple[typing.Type, ...] = (),
         format_name: str = "dict",
         encoder: typing.Optional[typing.Any] = None,
-    ) -> str:
+    ) -> InternalMethodName:
         if format_name != "dict" and encoder is not None:
-            return f"to_{format_name}"
+            return InternalMethodName.from_public(f"to_{format_name}")
         else:
             method_name = "to_dict"
             if format_name != "dict":
                 method_name += f"_{format_name}"
             if type_args:
                 method_name += f"_{hash_type_args(type_args)}"
-            return method_name
+            return InternalMethodName.from_public(f"{method_name}")
 
     def _add_pack_method_lines_lazy(self, method_name: str) -> None:
         if self.default_dialect is not None:
             self.add_type_modules(self.default_dialect)
         self.add_line(
             f"CodeBuilder("
             f"self.__class__,"
@@ -813,32 +832,50 @@
             omit_none_feature = self.is_code_generation_option_enabled(
                 TO_DICT_ADD_OMIT_NONE_FLAG
             )
             serialize_by_alias = self.get_config().serialize_by_alias
             omit_none = self._get_dialect_or_config_option("omit_none", False)
             packers = {}
             aliases = {}
-            fields_could_be_none = set()
+            nullable_fields = set()
+            nontrivial_nullable_fields = set()
             for fname, ftype in field_types.items():
                 if self.metadatas.get(fname, {}).get("serialize") == "omit":
                     continue
                 packer, alias, could_be_none = self._get_field_packer(
                     fname, ftype, config
                 )
                 packers[fname] = packer
                 if alias:
                     aliases[fname] = alias
                 if could_be_none:
-                    fields_could_be_none.add(fname)
-            if fields_could_be_none or by_alias_feature and aliases:
+                    nullable_fields.add(fname)
+                    if packer != "value":
+                        nontrivial_nullable_fields.add(fname)
+            if (
+                nontrivial_nullable_fields
+                or nullable_fields
+                and (omit_none or omit_none_feature)
+                or by_alias_feature
+                and aliases
+            ):
                 kwargs = "kwargs"
                 self.add_line("kwargs = {}")
                 for fname, packer in packers.items():
                     alias = aliases.get(fname)
-                    if fname in fields_could_be_none:
+                    if fname in nullable_fields:
+                        if (
+                            packer == "value"
+                            and not omit_none
+                            and not omit_none_feature
+                        ):
+                            self._pack_method_set_value(
+                                fname, alias, by_alias_feature, f"self.{fname}"
+                            )
+                            continue
                         self.add_line(f"value = self.{fname}")
                         with self.indent("if value is not None:"):
                             self._pack_method_set_value(
                                 fname, alias, by_alias_feature, packer
                             )
                         if omit_none and not omit_none_feature:
                             continue
@@ -859,15 +896,20 @@
             else:
                 kwargs_parts = []
                 for fname, packer in packers.items():
                     if serialize_by_alias:
                         fname_or_alias = aliases.get(fname, fname)
                     else:
                         fname_or_alias = fname
-                    kwargs_parts.append((fname_or_alias, packer))
+                    kwargs_parts.append(
+                        (
+                            fname_or_alias,
+                            packer if packer != "value" else f"self.{fname}",
+                        )
+                    )
                 kwargs = ", ".join(f"'{k}': {v}" for k, v in kwargs_parts)
                 kwargs = f"{{{kwargs}}}"
             post_serialize = self.get_declared_hook(__POST_SERIALIZE__)
             if self.encoder is not None:
                 if self.encoder_kwargs:
                     encoder_options = ", ".join(
                         f"{k}={v[0]}" for k, v in self.encoder_kwargs.items()
@@ -986,14 +1028,18 @@
                     self._add_pack_method_lines(method_name)
                 with self.indent("else:"):
                     self._add_pack_method_with_dialect_lines(method_name)
             else:
                 self._add_pack_method_lines(method_name)
         if self.dialect is None:
             self.add_line(f"setattr(cls, '{method_name}', {method_name})")
+            if is_dataclass_dict_mixin_subclass(self.cls):
+                self.add_line(
+                    f"setattr(cls, '{method_name.public}', {method_name})"
+                )
         else:
             self.add_line(f"cls.{cache_name}[dialect] = {method_name}")
         self.compile()
 
     def _get_field_packer(
         self,
         fname: str,
@@ -1025,16 +1071,17 @@
         )
         return packer, alias, could_be_none
 
     @typing.no_type_check
     def iter_serialization_strategies(
         self, metadata: typing.Mapping, ftype: typing.Type
     ) -> typing.Iterator[SerializationStrategyValueType]:
-        yield metadata.get("serialization_strategy")
-        yield from self.__iter_serialization_strategies(ftype)
+        if is_hashable(ftype):
+            yield metadata.get("serialization_strategy")
+            yield from self.__iter_serialization_strategies(ftype)
 
     @typing.no_type_check
     def __iter_serialization_strategies(
         self, ftype: typing.Type
     ) -> typing.Iterator[SerializationStrategyValueType]:
         if self.dialect is not None:
             yield self.dialect.serialization_strategy.get(ftype)
```

### Comparing `mashumaro-3.8.1/mashumaro/core/meta/code/lines.py` & `mashumaro-3.9/mashumaro/core/meta/code/lines.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/core/meta/helpers.py` & `mashumaro-3.9/mashumaro/core/meta/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     "is_not_required",
     "get_function_arg_annotation",
     "get_function_return_annotation",
     "is_unpack",
     "is_type_var_tuple",
     "hash_type_args",
     "iter_all_subclasses",
+    "is_hashable",
 ]
 
 
 NoneType = type(None)
 DataClassDictMixinPath = (
     f"{__name__.rsplit('.', 3)[:-3][0]}" f".mixins.dict.DataClassDictMixin"
 )
@@ -631,15 +632,18 @@
     else:
         new_type_args = []
         for type_param in collect_type_params(typ):
             new_type_args.append(substitutions.get(type_param, type_param))
         if new_type_args:
             with suppress(TypeError, KeyError):
                 return typ[tuple(new_type_args)]
-        return substitutions.get(typ, typ)
+        if is_hashable(typ):
+            return substitutions.get(typ, typ)
+        else:
+            return typ
 
 
 def get_name_error_name(e: NameError) -> str:
     if PY_310_MIN:
         return e.name  # type: ignore
     else:
         match = re.search("'(.*)'", e.args[0])
@@ -718,7 +722,15 @@
     return md5(",".join(map(type_name, type_args)).encode()).hexdigest()
 
 
 def iter_all_subclasses(cls: Type) -> typing.Iterator[Type]:
     for subclass in cls.__subclasses__():
         yield subclass
         yield from iter_all_subclasses(subclass)
+
+
+def is_hashable(typ: Any) -> bool:
+    try:
+        hash(typ)
+        return True
+    except TypeError:
+        return False
```

### Comparing `mashumaro-3.8.1/mashumaro/core/meta/mixin.py` & `mashumaro-3.9/mashumaro/core/meta/mixin.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/core/meta/types/common.py` & `mashumaro-3.9/mashumaro/core/meta/types/common.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/core/meta/types/pack.py` & `mashumaro-3.9/mashumaro/core/meta/types/pack.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 import enum
 import ipaddress
 import os
 import typing
 import uuid
 from base64 import encodebytes
 from contextlib import suppress
+from dataclasses import is_dataclass
 from decimal import Decimal
 from fractions import Fraction
 from typing import Any, Callable, List, Optional, Tuple, Type, Union
 
 import typing_extensions
 
 from mashumaro.core.const import PY_39_MIN, PY_311_MIN
 from mashumaro.core.meta.code.lines import CodeLines
 from mashumaro.core.meta.helpers import (
     get_args,
     get_class_that_defines_method,
     get_function_return_annotation,
     get_literal_values,
-    is_dataclass_dict_mixin_subclass,
     is_final,
     is_generic,
     is_literal,
     is_named_tuple,
     is_new_type,
     is_not_required,
     is_optional,
@@ -201,18 +201,16 @@
             type_args = get_args(spec.type)
             spec.builder.add_type_modules(*type_args)
             type_arg_names = ", ".join(list(map(type_name, type_args)))
             return f"{spec.expression}._serialize([{type_arg_names}])"
 
 
 @register
-def pack_dataclass_dict_mixin_subclass(
-    spec: ValueSpec,
-) -> Optional[Expression]:
-    if is_dataclass_dict_mixin_subclass(spec.origin_type):
+def pack_dataclass(spec: ValueSpec) -> Optional[Expression]:
+    if is_dataclass(spec.origin_type):
         type_args = get_args(spec.type)
         method_name = spec.builder.get_pack_method_name(
             type_args, spec.builder.format_name
         )
         if get_class_that_defines_method(
             method_name, spec.origin_type
         ) != spec.origin_type and (
```

### Comparing `mashumaro-3.8.1/mashumaro/core/meta/types/unpack.py` & `mashumaro-3.9/mashumaro/core/meta/types/unpack.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import pathlib
 import types
 import typing
 import uuid
 from abc import ABC, abstractmethod
 from base64 import decodebytes
 from contextlib import suppress
+from dataclasses import is_dataclass
 from decimal import Decimal
 from fractions import Fraction
 from typing import Any, Callable, Iterable, List, Optional, Tuple, Type, Union
 
 import typing_extensions
 
 from mashumaro.core.const import PY_39_MIN, PY_311_MIN
 from mashumaro.core.helpers import parse_timezone
 from mashumaro.core.meta.code.lines import CodeLines
 from mashumaro.core.meta.helpers import (
     get_args,
     get_class_that_defines_method,
     get_function_arg_annotation,
     get_literal_values,
-    is_dataclass_dict_mixin_subclass,
     is_final,
     is_generic,
     is_literal,
     is_named_tuple,
     is_new_type,
     is_not_required,
     is_optional,
@@ -443,16 +443,15 @@
 def _unpack_with_annotated_serialization_strategy(
     spec: ValueSpec,
     strategy: SerializationStrategy,
 ) -> Expression:
     strategy_type = type(strategy)
     try:
         value_type: Union[Type, Any] = get_function_arg_annotation(
-            strategy.deserialize,
-            arg_pos=0,
+            strategy.deserialize, arg_pos=0
         )
     except (KeyError, ValueError):
         value_type = Any
     value_type = substitute_type_params(
         value_type,
         resolve_type_params(strategy_type, get_args(spec.type))[strategy_type],
     )
@@ -510,16 +509,15 @@
 def _unpack_annotated_serializable_type(
     spec: ValueSpec,
 ) -> Optional[Expression]:
     try:
         # noinspection PyProtectedMember
         # noinspection PyUnresolvedReferences
         value_type = get_function_arg_annotation(
-            spec.origin_type._deserialize,
-            arg_pos=0,
+            spec.origin_type._deserialize, arg_pos=0
         )
     except (KeyError, ValueError):
         raise UnserializableField(
             field_name=spec.field_ctx.name,
             field_type=spec.type,
             holder_class=spec.builder.cls,
             msg='Method _deserialize must have annotated "value" argument',
@@ -559,18 +557,16 @@
             return (
                 f"{type_name(spec.type)}._deserialize({spec.expression}, "
                 f"[{type_arg_names}])"
             )
 
 
 @register
-def unpack_dataclass_dict_mixin_subclass(
-    spec: ValueSpec,
-) -> Optional[Expression]:
-    if is_dataclass_dict_mixin_subclass(spec.origin_type):
+def unpack_dataclass(spec: ValueSpec) -> Optional[Expression]:
+    if is_dataclass(spec.origin_type):
         for annotation in spec.annotations:
             if isinstance(annotation, Discriminator):
                 return DiscriminatedUnionUnpackerBuilder(annotation).build(
                     spec
                 )
         type_args = get_args(spec.type)
         method_name = spec.builder.get_unpack_method_name(
```

### Comparing `mashumaro-3.8.1/mashumaro/exceptions.py` & `mashumaro-3.9/mashumaro/exceptions.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/helper.py` & `mashumaro-3.9/mashumaro/helper.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/jsonschema/annotations.py` & `mashumaro-3.9/mashumaro/jsonschema/annotations.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/jsonschema/builder.py` & `mashumaro-3.9/mashumaro/jsonschema/builder.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/jsonschema/dialects.py` & `mashumaro-3.9/mashumaro/jsonschema/dialects.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     definitions_root_pointer: str
     all_refs: bool
 
 
 @dataclass(frozen=True)
 class JSONSchemaDraft202012Dialect(JSONSchemaDialect):
     uri: str = "https://json-schema.org/draft/2020-12/schema"
-    definitions_root_pointer: str = "#/defs"
+    definitions_root_pointer: str = "#/$defs"
     all_refs: bool = False
 
 
 @dataclass(frozen=True)
 class OpenAPISchema31Dialect(JSONSchemaDialect):
     uri: str = "https://spec.openapis.org/oas/3.1/dialect/base"
     definitions_root_pointer: str = "#/components/schemas"
```

### Comparing `mashumaro-3.8.1/mashumaro/jsonschema/models.py` & `mashumaro-3.9/mashumaro/jsonschema/models.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/jsonschema/schema.py` & `mashumaro-3.9/mashumaro/jsonschema/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,27 +150,32 @@
             )
         self.origin_type = get_type_origin(self.type)
         if is_dataclass(self.origin_type):
             type_args = get_args(self.type)
             self.__builder = CodeBuilder(self.origin_type, type_args)
             self.__builder.reset()
 
-    def fields(self) -> Iterable[Tuple[str, Type, Any]]:
+    def fields(self) -> Iterable[Tuple[str, Type, bool, Any]]:
         for f_name, f_type in self._builder.get_field_types(
             include_extras=True
         ).items():
             f = self._builder.dataclass_fields.get(f_name)  # type: ignore
             if f and not f.init:
                 continue
             f_default = f.default
             if f_default is MISSING:
                 f_default = self._builder.namespace.get(f_name, MISSING)
             if f_default is not MISSING:
                 f_default = _default(f_type, f_default)
-            yield f_name, f_type, f_default
+
+            has_default = (
+                f.default is not MISSING or f.default_factory is not MISSING
+            )
+
+            yield f_name, f_type, has_default, f_default
 
     def get_overridden_serialization_method(
         self,
     ) -> Optional[Union[Callable, str]]:
         if not self.__builder:
             return None
         serialize_option = self.metadata.get("serialize")
@@ -276,37 +281,43 @@
             field_instance.update_type(Any)  # type: ignore[arg-type]
 
 
 @register
 def on_dataclass(instance: Instance, ctx: Context) -> Optional[JSONSchema]:
     # TODO: Self references might not work
     if is_dataclass(instance.origin_type):
+        jsonschema_config = instance.get_config().json_schema
         schema = JSONObjectSchema(
             title=instance.origin_type.__name__,
-            additionalProperties=False,
+            additionalProperties=jsonschema_config.get(
+                "additionalProperties", False
+            ),
         )
         properties: Dict[str, JSONSchema] = {}
         required = []
-        field_schema_overrides = instance.get_config().json_schema.get(
-            "properties", {}
-        )
-        for f_name, f_type, f_default in instance.fields():
+        field_schema_overrides = jsonschema_config.get("properties", {})
+        for f_name, f_type, has_default, f_default in instance.fields():
             override = field_schema_overrides.get(f_name)
             f_instance = instance.copy(type=f_type, name=f_name)
             if override:
                 f_schema = JSONSchema.from_dict(override)
             else:
                 override_field_instance_type_if_needed(instance, f_instance)
                 f_schema = get_schema(f_instance, ctx)
             if f_instance.alias:
                 f_name = f_instance.alias
             if f_default is not MISSING:
                 f_schema.default = f_default
-            else:
+            description = f_instance.metadata.get("description")
+            if description:
+                f_schema.description = description
+
+            if not has_default:
                 required.append(f_name)
+
             properties[f_name] = f_schema
         if properties:
             schema.properties = properties
         if required:
             schema.required = required
         if ctx.all_refs:
             ctx.definitions[instance.origin_type.__name__] = schema
```

### Comparing `mashumaro-3.8.1/mashumaro/mixins/dict.py` & `mashumaro-3.9/mashumaro/mixins/dict.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/mixins/json.py` & `mashumaro-3.9/mashumaro/mixins/json.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/mixins/msgpack.py` & `mashumaro-3.9/mashumaro/mixins/msgpack.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/mixins/orjson.py` & `mashumaro-3.9/mashumaro/mixins/orjson.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/mixins/orjson.pyi` & `mashumaro-3.9/mashumaro/mixins/orjson.pyi`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/mixins/toml.py` & `mashumaro-3.9/mashumaro/mixins/toml.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/mixins/yaml.py` & `mashumaro-3.9/mashumaro/mixins/yaml.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro/types.py` & `mashumaro-3.9/mashumaro/types.py`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/mashumaro.egg-info/PKG-INFO` & `mashumaro-3.9/mashumaro.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mashumaro
-Version: 3.8.1
+Version: 3.9
 Summary: Fast serialization library on top of dataclasses
 Home-page: https://github.com/Fatal1ty/mashumaro
 Author: Alexander Tikhonov
 Author-email: random.gauss@gmail.com
 License: Apache License, Version 2.0
 Platform: all
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 Provides-Extra: msgpack
 Provides-Extra: yaml
 Provides-Extra: toml
 License-File: LICENSE
 
 <div align="center">
 
-<img alt="logo" width="175" src="https://github.com/Fatal1ty/mashumaro/blob/master/img/logo.svg">
+<img alt="logo" width="175" src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/ac2f924591d488dbd9a776a6b1ae7dede2d8c73e/img/logo.svg">
 
 ###### Fast and well tested serialization library on top of dataclasses
 
 [![Build Status](https://github.com/Fatal1ty/mashumaro/workflows/tests/badge.svg)](https://github.com/Fatal1ty/mashumaro/actions)
 [![Coverage Status](https://coveralls.io/repos/github/Fatal1ty/mashumaro/badge.svg?branch=master)](https://coveralls.io/github/Fatal1ty/mashumaro?branch=master)
 [![Latest Version](https://img.shields.io/pypi/v/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
 [![Python Version](https://img.shields.io/pypi/pyversions/mashumaro.svg)](https://pypi.python.org/pypi/mashumaro)
@@ -327,102 +327,40 @@
 runtime in some cases) and are set as attributes to your dataclasses.
 To minimize the import time, you can explicitly enable
 [lazy compilation](#lazy_compilation-config-option).
 
 Benchmark
 --------------------------------------------------------------------------------
 
-* macOS 13.0.1 Ventura
+* macOS 13.3.1 Ventura
 * Apple M1
-* 8GB RAM
-* Python 3.11.0
+* 16GB RAM
+* Python 3.11.4
 
-Load and dump [sample data](https://github.com/Fatal1ty/mashumaro/blob/master/benchmark/sample.py) 100 times in 5 runs.
-The following figures show the best overall time in each case.
-
-[//]: # (<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.png" width="400"><img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.png" width="400">)
-
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg">
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_dark.svg">
-  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/load_light.svg" width="400">
-</picture>
-<picture>
-  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg">
-  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_dark.svg">
-  <img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/master/benchmark/charts/dump_light.svg" width="400">
-</picture>
-
-<table>
-  <col>
-  <colgroup span="2"></colgroup>
-  <colgroup span="2"></colgroup>
-  <tr>
-    <th rowspan="2">Library</th>
-    <th colspan="2" scope="colgroup">From dict</th>
-    <th colspan="2" scope="colgroup">To dict</th>
-</tr>
-<tr>
-    <th scope="col">Time</th>
-    <th scope="col">Slowdown factor</th>
-    <th scope="col">Time</th>
-    <th scope="col">Slowdown factor</th>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/Fatal1ty/mashumaro">mashumaro</a></th>
-    <td align="right">0.14724</td>
-    <td align="left">1x</td>
-    <td align="right">0.10128</td>
-    <td align="left">1x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/Tinche/cattrs">cattrs</a></th>
-    <td align="right">0.18906</td>
-    <td align="left">1.28x</td>
-    <td align="right">0.14072</td>
-    <td align="left">1.39x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/samuelcolvin/pydantic/">pydantic</a></th>
-    <td align="right">1.02666</td>
-    <td align="left">6.97x</td>
-    <td align="right">0.81932</td>
-    <td align="left">8.09x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/marshmallow-code/marshmallow">marshmallow</a></th>
-    <td align="right">1.38348</td>
-    <td align="left">9.4x</td>
-    <td align="right">0.45695</td>
-    <td align="left">4.51x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://docs.python.org/3/library/dataclasses.html#dataclasses.asdict">dataclasses</a></th>
-    <td align="left">—</td>
-    <td align="left">—</td>
-    <td align="right">0.68057</td>
-    <td align="left">6.72x</td>
-</tr>
-<tr>
-    <th scope="row"><a href="https://github.com/konradhalas/dacite">dacite</a></th>
-    <td align="right">2.37315</td>
-    <td align="left">16.12x</td>
-    <td align="left">—</td>
-    <td align="left">—</td>
-</tr>
-</table>
+Benchmark using [pyperf](https://github.com/psf/pyperf) with GitHub Issue model. Please note that the
+following charts use logarithmic scale, as it is convenient for displaying
+very large ranges of values.
+
+<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/381306ea92808c256354fe890bb5aa60cd3bb787/benchmark/charts/load_light.svg" width="604">
+<img src="https://raw.githubusercontent.com/Fatal1ty/mashumaro/381306ea92808c256354fe890bb5aa60cd3bb787/benchmark/charts/dump_light.svg" width="604">
+
+> [!NOTE]\
+> Benchmark results may vary depending on the specific configuration and
+> parameters used for serialization and deserialization. However, we have made
+> an attempt to use the available options that can speed up and smooth out the
+> differences in how libraries work.
 
 To run benchmark in your environment:
 ```bash
 git clone git@github.com:Fatal1ty/mashumaro.git
 cd mashumaro
 python3 -m venv env && source env/bin/activate
 pip install -e .
 pip install -r requirements-dev.txt
-python benchmark/run.py
+./benchmark/run.sh
 ```
 
 Serialization mixins
 --------------------------------------------------------------------------------
 
 `mashumaro` provides mixins for each serialization format.
 
@@ -674,18 +612,19 @@
 assert my_plan.to_dict() == input_data
 ```
 
 Here we add annotations to the only argument of `_deserialize` method and
 to the return value of `_serialize` method as well. The latter is needed for
 correct serialization.
 
-The importance of explicit passing `use_annotations=True` when defining a class
-is that otherwise implicit using annotations might break compatibility with old
-code that wasn't aware of this feature. It will be enabled by default in the
-future major release.
+> [!IMPORTANT]\
+> The importance of explicit passing `use_annotations=True` when defining a
+> class is that otherwise implicit using annotations might break compatibility
+> with old code that wasn't aware of this feature. It will be enabled by
+> default in the future major release.
 
 #### User-defined generic types
 
 The great thing to note about using annotations in `SerializableType` is that
 they work seamlessly with [generic](https://docs.python.org/3/library/typing.html#user-defined-generic-types)
 and [variadic generic](https://peps.python.org/pep-0646/) types.
 Let's see how this can be useful:
@@ -815,15 +754,17 @@
 print(example.to_dict())
 # {'dt': 1672531200.0}
 ```
 
 Here the passed string value `"1672531200"` will be converted to `float` before being passed to `deserialize` method
 thanks to the `float` annotation.
 
-As well as for `SerializableType`, the value of `use_annotatons` will be `True` by default in the future major release.
+> [!IMPORTANT]\
+> As well as for `SerializableType`, the value of `use_annotatons` will be
+> `True` by default in the future major release.
 
 #### Third-party generic types
 
 To create a generic version of a serialization strategy you need to follow these steps:
 * inherit [`Generic[...]`](https://docs.python.org/3/library/typing.html#typing.Generic) type
 with the number of parameters matching the number of parameters
 of the target generic type
@@ -905,15 +846,16 @@
 with. At this moment there are next serialization engines to choose from:
 
 | Applicable data types      | Supported engines    | Description                                                                                                                                                                                                  |
 |:---------------------------|:---------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `NamedTuple`, `namedtuple` | `as_list`, `as_dict` | How to pack named tuples. By default `as_list` engine is used that means your named tuple class instance will be packed into a list of its values. You can pack it into a dictionary using `as_dict` engine. |
 | `Any`                      | `omit`               | Skip the field during serialization                                                                                                                                                                          |
 
-In addition, you can pass a field value as is without changes using
+> [!NOTE]\
+> You can pass a field value as is without changes on serialization using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
 from datetime import datetime
 from dataclasses import dataclass, field
@@ -949,15 +891,16 @@
 with. At this moment there are next deserialization engines to choose from:
 
 | Applicable data types      | Supported engines                                                                                                                   | Description                                                                                                                                                                                                                                                                                             |
 |:---------------------------|:------------------------------------------------------------------------------------------------------------------------------------|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | `datetime`, `date`, `time` | [`ciso8601`](https://github.com/closeio/ciso8601#supported-subset-of-iso-8601), [`pendulum`](https://github.com/sdispater/pendulum) | How to parse datetime string. By default native [`fromisoformat`](https://docs.python.org/3/library/datetime.html#datetime.datetime.fromisoformat) of corresponding class will be used for `datetime`, `date` and `time` fields. It's the fastest way in most cases, but you can choose an alternative. |
 | `NamedTuple`, `namedtuple` | `as_list`, `as_dict`                                                                                                                | How to unpack named tuples. By default `as_list` engine is used that means your named tuple class instance will be created from a list of its values. You can unpack it from a dictionary using `as_dict` engine.                                                                                       |
 
-In addition, you can pass a field value as is without changes using
+> [!NOTE]\
+> You can pass a field value as is without changes on deserialization using
 [`pass_through`](#passing-field-values-as-is).
 
 Example:
 
 ```python
 from datetime import datetime
 from dataclasses import dataclass, field
@@ -993,17 +936,21 @@
 class D(DataClassDictMixin):
     x: MyNamedTuple = field(metadata={"deserialize": "as_dict"})
 ```
 
 #### `serialization_strategy` option
 
 This option is useful when you want to change the serialization logic
-for a dataclass field depending on some defined parameters using a reusable serialization scheme.
-You can find an example in the [`SerializationStrategy`](#serializationstrategy) chapter.
-In addition, you can pass a field value as is without changes using
+for a dataclass field depending on some defined parameters using a reusable
+serialization scheme. You can find an example in the
+[`SerializationStrategy`](#serializationstrategy) chapter.
+
+> [!NOTE]\
+> You can pass a field value as is without changes on
+> serialization / deserialization using
 [`pass_through`](#passing-field-values-as-is).
 
 #### `alias` option
 
 In some cases it's better to have different names for a field in your class and
 in its serialized view. For example, a third-party legacy API you are working
 with might operate with camel case style, but you stick to snake case style in
@@ -1156,16 +1103,16 @@
 instance = DataClass.from_dict({"x": "2021", "y": "2021"})
 # DataClass(x=datetime.datetime(2021, 1, 1, 0, 0), y=Date(2021, 1, 1))
 dictionary = instance.to_dict()
 # {'x': '2021', 'y': '2021-01-01'}
 ```
 
 Note that you can register different methods for multiple logical types which
-are based on the same type using `NewType` and `Annotated`.
-See [Extending existing types](#extending-existing-types) for details.
+are based on the same type using `NewType` and `Annotated`,
+see [Extending existing types](#extending-existing-types) for details.
 
 #### `aliases` config option
 
 Sometimes it's better to write the field aliases in one place. You can mix
 aliases here with [aliases in the field options](#alias-option), but the last ones will always
 take precedence.
 
@@ -1378,29 +1325,28 @@
 #### `lazy_compilation` config option
 
 By using this option, the compilation of the `from_*` and `to_*` methods will
 be deferred until they are called first time. This will reduce the import time
 and, in certain instances, may enhance the speed of deserialization
 by leveraging the data that is accessible after the class has been created.
 
-> **Warning**
->
+> [!Warning]\
 > If you need to save a reference to `from_*` or `to_*` method, you should
 > do it after the method is compiled. To be safe, you can always use lambda
 > function:
 > ```python
 > from_dict = lambda x: MyModel.from_dict(x)
 > to_dict = lambda x: x.to_dict()
 > ```
 
 ### Passing field values as is
 
 In some cases it's needed to pass a field value as is without any changes
 during serialization / deserialization. There is a predefined
-[`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L49)
+[`pass_through`](https://github.com/Fatal1ty/mashumaro/blob/master/mashumaro/helper.py#L58)
 object that can be used as `serialization_strategy` or
 `serialize` / `deserialize` options:
 
 ```python
 from dataclasses import dataclass, field
 from mashumaro import DataClassDictMixin, pass_through
 
@@ -1627,16 +1573,15 @@
 
 * without annotations: `type = 42`
 * annotated as ClassVar: `type: ClassVar[int] = 42`
 * annotated as Final: `type: Final[int] = 42`
 * annotated as Literal: `type: Literal[42] = 42`
 * annotated as StrEnum: `type: ResponseType = ResponseType.OK`
 
-> **Note**
->
+> [!NOTE]\
 > Keep in mind that by default only Final, Literal and StrEnum fields are
 > processed during serialization.
 
 Next, we will look at different use cases, as well as their pros and cons.
 
 #### Subclasses distinguishable by a field
 
@@ -1648,16 +1593,15 @@
 impractical. Moreover, deserialization of the union would be slow, since we
 need to iterate over each variant in the list until we find the right one.
 
 We can improve subclass deserialization using `Discriminator` as annotation
 within `Annotated` type. We will use `field` parameter and set
 `include_subtypes` to `True`.
 
-> **Note**
->
+> [!IMPORTANT]\
 > The discriminator field should be accessible from the `__dict__` attribute
 > of a specific descendant, i.e. defined at the level of that descendant.
 > A descendant class without a discriminator field will be ignored, but
 > its descendants won't.
 
 Suppose we have a hierarchy of client events distinguishable by a class
 attribute "type":
@@ -1953,20 +1897,22 @@
 
 Again, it's not necessary to have a common superclass. If you have a union of
 dataclasses without a field that they can be distinguishable by, you can still
 use `Discriminator`, but deserialization will almost be the same as for `Union`
 type without `Discriminator` except that it could be possible to deserialize
 subclasses with `include_subtypes=True`.
 
-> **Note**
->
+> [!IMPORTANT]\
 > When both `include_subtypes` and `include_supertypes` are enabled,
 > all subclasses will be attempted to be deserialized first,
 > superclasses — at the end.
 
+In the following example you can see how priority works — first we try
+to deserialize `ChickpeaHummus`, and if it fails, then we try `Hummus`:
+
 ```python
 @dataclass
 class Hummus(DataClassDictMixin):
     made_of: Literal["chickpeas", "artichoke"]
     grams: int
 
 @dataclass
@@ -2386,25 +2332,25 @@
 ### Building JSON Schema
 
 For simple one-time cases it's recommended to start from using a configurable
 `build_json_schema` function. It returns `JSONSchema` object that can be
 serialized to json or to dict:
 
 ```python
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import List
 from uuid import UUID
 
 from mashumaro.jsonschema import build_json_schema
 
 
 @dataclass
 class User:
     id: UUID
-    name: str
+    name: str = field(metadata={"description": "User name"})
 
 
 print(build_json_schema(List[User]).to_json())
 ```
 
 <details>
 <summary>Click to show the result</summary>
@@ -2417,15 +2363,16 @@
         "title": "User",
         "properties": {
             "id": {
                 "type": "string",
                 "format": "uuid"
             },
             "name": {
-                "type": "string"
+                "type": "string",
+                "description": "User name"
             }
         },
         "additionalProperties": false,
         "required": [
             "id",
             "name"
         ]
@@ -2541,15 +2488,15 @@
             "required": [
                 "id",
                 "name"
             ]
         }
     },
     "items": {
-        "$ref": "#/defs/User"
+        "$ref": "#/$defs/User"
     }
 }
 ```
 </details>
 
 The definitions section can be omitted from the final document by setting
 `with_definitions` parameter to `False`:
@@ -2720,15 +2667,17 @@
 * [`MaxProperties`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-maxproperties)
 * [`MinProperties`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-minproperties)
 * [`DependentRequired`](https://json-schema.org/draft/2020-12/json-schema-validation.html#name-dependentrequired)
 
 ### Extending JSON Schema
 
 Using a `Config` class it is possible to override some parts of the schema.
-Currently, it works for dataclass fields via "properties" key:
+Currently, you can do the following:
+* override some field schemas using the "properties" key
+* change `additionalProperties` using the "additionalProperties" key
 
 ```python
 from dataclasses import dataclass
 from mashumaro.jsonschema import build_json_schema
 
 @dataclass
 class FooBar:
@@ -2738,15 +2687,16 @@
     class Config:
         json_schema = {
             "properties": {
                 "foo": {
                     "type": "string",
                     "description": "bar"
                 }
-            }
+            },
+            "additionalProperties": True,
         }
 
 print(build_json_schema(FooBar).to_json())
 ```
 
 <details>
 <summary>Click to show the result</summary>
@@ -2760,23 +2710,26 @@
             "type": "string",
             "description": "bar"
         },
         "bar": {
             "type": "integer"
         }
     },
-    "additionalProperties": false,
+    "additionalProperties": true,
     "required": [
         "foo",
         "bar"
     ]
 }
 ```
 </details>
 
+You can also change the "additionalProperties" key to a specific schema
+by passing it a `JSONSchema` instance instead of a bool value.
+
 ### JSON Schema and custom serialization methods
 
 Mashumaro provides different ways to override default serialization methods for
 dataclass fields or specific data types. In order for these overrides to be
 reflected in the schema, you need to make sure that the methods have
 annotations of the return value type.
```

### Comparing `mashumaro-3.8.1/mashumaro.egg-info/SOURCES.txt` & `mashumaro-3.9/mashumaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/pyproject.toml` & `mashumaro-3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mashumaro-3.8.1/setup.py` & `mashumaro-3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
 setup(
     name="mashumaro",
-    version="3.8.1",
+    version="3.9",
     description="Fast serialization library on top of dataclasses",
     long_description=open("README.md", encoding="utf8").read(),
     long_description_content_type="text/markdown",
     platforms="all",
     classifiers=[
         "License :: OSI Approved :: Apache Software License",
         "Intended Audience :: Developers",
```

