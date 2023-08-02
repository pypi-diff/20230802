# Comparing `tmp/rdt-1.6.1.dev0.tar.gz` & `tmp/rdt-1.6.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rdt-1.6.1.dev0.tar", last modified: Mon Jul 17 20:29:35 2023, max compression
+gzip compressed data, was "rdt-1.6.1.dev1.tar", last modified: Wed Aug  2 16:15:49 2023, max compression
```

## Comparing `rdt-1.6.1.dev0.tar` & `rdt-1.6.1.dev1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.508049 rdt-1.6.1.dev0/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/AUTHORS.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/CONTRIBUTING.rst
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    46119 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/HISTORY.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/LICENSE
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/MANIFEST.in
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    54128 2023-07-17 20:29:35.508217 rdt-1.6.1.dev0/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7109 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/RELEASE.md
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.489971 rdt-1.6.1.dev0/rdt/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5342 2023-07-12 20:34:53.000000 rdt-1.6.1.dev0/rdt/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/rdt/errors.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    30614 2023-07-17 20:29:05.000000 rdt-1.6.1.dev0/rdt/hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.491479 rdt-1.6.1.dev0/rdt/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/rdt/performance/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.493501 rdt-1.6.1.dev0/rdt/performance/datasets/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/rdt/performance/datasets/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/rdt/performance/datasets/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.6.1.dev0/rdt/performance/datasets/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/rdt/performance/datasets/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/rdt/performance/datasets/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/rdt/performance/datasets/numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/rdt/performance/datasets/pii.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/rdt/performance/datasets/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/rdt/performance/datasets/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3372 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/rdt/performance/performance.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.6.1.dev0/rdt/performance/profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.495198 rdt-1.6.1.dev0/rdt/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5023 2023-07-17 20:29:05.000000 rdt-1.6.1.dev0/rdt/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.495464 rdt-1.6.1.dev0/rdt/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3345 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/rdt/transformers/addons/addons_setup.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    15934 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/rdt/transformers/base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3792 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/rdt/transformers/boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    21541 2023-07-17 20:29:05.000000 rdt-1.6.1.dev0/rdt/transformers/categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10281 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/rdt/transformers/datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5878 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/rdt/transformers/null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    22319 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/rdt/transformers/numerical.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.496157 rdt-1.6.1.dev0/rdt/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.6.1.dev0/rdt/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13633 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/rdt/transformers/pii/anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/rdt/transformers/pii/utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/rdt/transformers/text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.6.1.dev0/rdt/transformers/utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.490947 rdt-1.6.1.dev0/rdt.egg-info/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    54128 2023-07-17 20:29:35.000000 rdt-1.6.1.dev0/rdt.egg-info/PKG-INFO
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2835 2023-07-17 20:29:35.000000 rdt-1.6.1.dev0/rdt.egg-info/SOURCES.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-17 20:29:35.000000 rdt-1.6.1.dev0/rdt.egg-info/dependency_links.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-07-17 20:29:35.000000 rdt-1.6.1.dev0/rdt.egg-info/not-zip-safe
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-07-17 20:29:35.000000 rdt-1.6.1.dev0/rdt.egg-info/requires.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-07-17 20:29:35.000000 rdt-1.6.1.dev0/rdt.egg-info/top_level.txt
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-07-17 20:29:35.508788 rdt-1.6.1.dev0/setup.cfg
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4134 2023-07-12 20:34:53.000000 rdt-1.6.1.dev0/setup.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.496707 rdt-1.6.1.dev0/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/tests/code_style.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/tests/contributing.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.486377 rdt-1.6.1.dev0/tests/datasets/
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.497665 rdt-1.6.1.dev0/tests/datasets/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/datasets/tests/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/datasets/tests/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/datasets/tests/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/datasets/tests/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/datasets/tests/test_utils.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.498196 rdt-1.6.1.dev0/tests/integration/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/integration/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    45910 2023-07-17 20:29:05.000000 rdt-1.6.1.dev0/tests/integration/test_hyper_transformer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/tests/integration/test_transformers.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.499862 rdt-1.6.1.dev0/tests/integration/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/integration/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.500334 rdt-1.6.1.dev0/tests/integration/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/integration/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     7106 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/tests/integration/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/tests/integration/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/tests/integration/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.6.1.dev0/tests/integration/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/tests/integration/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/tests/integration/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.6.1.dev0/tests/integration/transformers/test_text.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.501024 rdt-1.6.1.dev0/tests/performance/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/performance/README.md
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/performance/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.6.1.dev0/tests/performance/test_performance.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.501422 rdt-1.6.1.dev0/tests/performance/tests/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/performance/tests/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.6.1.dev0/tests/performance/tests/test_profiling.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.502145 rdt-1.6.1.dev0/tests/unit/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/unit/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/tests/unit/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)   104228 2023-07-17 20:29:05.000000 rdt-1.6.1.dev0/tests/unit/test_hyper_transformer.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.505203 rdt-1.6.1.dev0/tests/unit/transformers/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/unit/transformers/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.505703 rdt-1.6.1.dev0/tests/unit/transformers/addons/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/unit/transformers/addons/__init__.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.506358 rdt-1.6.1.dev0/tests/unit/transformers/addons/identity/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/unit/transformers/addons/identity/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/tests/unit/transformers/addons/identity/test_identity.py
-drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-07-17 20:29:35.507794 rdt-1.6.1.dev0/tests/unit/transformers/pii/
--rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.6.1.dev0/tests/unit/transformers/pii/__init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    29367 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/tests/unit/transformers/pii/test_anonymizer.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.6.1.dev0/tests/unit/transformers/pii/test_utils.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     3221 2023-07-17 20:29:05.000000 rdt-1.6.1.dev0/tests/unit/transformers/test___init__.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/tests/unit/transformers/test_base.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/tests/unit/transformers/test_boolean.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.6.1.dev0/tests/unit/transformers/test_categorical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/tests/unit/transformers/test_datetime.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-07-12 20:34:31.000000 rdt-1.6.1.dev0/tests/unit/transformers/test_null.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt-1.6.1.dev0/tests/unit/transformers/test_numerical.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.6.1.dev0/tests/unit/transformers/test_text.py
--rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.6.1.dev0/tests/unit/transformers/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.575110 rdt-1.6.1.dev1/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       56 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/AUTHORS.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22812 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/CONTRIBUTING.rst
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    46119 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/HISTORY.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4872 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/LICENSE
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      284 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/MANIFEST.in
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    54161 2023-08-02 16:15:49.575326 rdt-1.6.1.dev1/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7134 2023-08-02 16:15:08.000000 rdt-1.6.1.dev1/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6499 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/RELEASE.md
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.563022 rdt-1.6.1.dev1/rdt/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5342 2023-07-17 20:30:00.000000 rdt-1.6.1.dev1/rdt/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      729 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/rdt/errors.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30614 2023-07-17 20:29:05.000000 rdt-1.6.1.dev1/rdt/hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.564301 rdt-1.6.1.dev1/rdt/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      262 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/rdt/performance/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.565520 rdt-1.6.1.dev1/rdt/performance/datasets/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      847 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/rdt/performance/datasets/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1158 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/rdt/performance/datasets/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     6125 2022-08-18 00:01:17.000000 rdt-1.6.1.dev1/rdt/performance/datasets/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    11724 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/rdt/performance/datasets/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5734 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/rdt/performance/datasets/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8406 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/rdt/performance/datasets/numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1893 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/rdt/performance/datasets/pii.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1898 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/rdt/performance/datasets/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      558 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/rdt/performance/datasets/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3372 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/rdt/performance/performance.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3442 2022-08-18 00:01:17.000000 rdt-1.6.1.dev1/rdt/performance/profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.566737 rdt-1.6.1.dev1/rdt/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5023 2023-07-17 20:29:05.000000 rdt-1.6.1.dev1/rdt/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.566868 rdt-1.6.1.dev1/rdt/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3345 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/rdt/transformers/addons/addons_setup.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    15934 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/rdt/transformers/base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3792 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/rdt/transformers/boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    21541 2023-07-17 20:29:05.000000 rdt-1.6.1.dev1/rdt/transformers/categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10281 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/rdt/transformers/datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5878 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/rdt/transformers/null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    22319 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/rdt/transformers/numerical.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.567314 rdt-1.6.1.dev1/rdt/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      212 2022-08-18 00:01:17.000000 rdt-1.6.1.dev1/rdt/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    14275 2023-08-02 16:15:08.000000 rdt-1.6.1.dev1/rdt/transformers/pii/anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1052 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/rdt/transformers/pii/utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4847 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/rdt/transformers/text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4576 2023-04-26 21:05:25.000000 rdt-1.6.1.dev1/rdt/transformers/utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.563904 rdt-1.6.1.dev1/rdt.egg-info/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    54161 2023-08-02 16:15:49.000000 rdt-1.6.1.dev1/rdt.egg-info/PKG-INFO
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2835 2023-08-02 16:15:49.000000 rdt-1.6.1.dev1/rdt.egg-info/SOURCES.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-08-02 16:15:49.000000 rdt-1.6.1.dev1/rdt.egg-info/dependency_links.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        1 2023-08-02 16:15:49.000000 rdt-1.6.1.dev1/rdt.egg-info/not-zip-safe
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1448 2023-08-02 16:15:49.000000 rdt-1.6.1.dev1/rdt.egg-info/requires.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)        4 2023-08-02 16:15:49.000000 rdt-1.6.1.dev1/rdt.egg-info/top_level.txt
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1595 2023-08-02 16:15:49.575873 rdt-1.6.1.dev1/setup.cfg
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4142 2023-08-02 16:15:08.000000 rdt-1.6.1.dev1/setup.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.567746 rdt-1.6.1.dev1/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      536 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8197 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/tests/code_style.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18316 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/tests/contributing.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.559961 rdt-1.6.1.dev1/tests/datasets/
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.568534 rdt-1.6.1.dev1/tests/datasets/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3770 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/datasets/tests/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     4044 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/datasets/tests/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1980 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/datasets/tests/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2886 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/datasets/tests/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      671 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/datasets/tests/test_utils.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.569016 rdt-1.6.1.dev1/tests/integration/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      153 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/integration/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    45910 2023-07-17 20:29:05.000000 rdt-1.6.1.dev1/tests/integration/test_hyper_transformer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     9434 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/tests/integration/test_transformers.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.570087 rdt-1.6.1.dev1/tests/integration/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       52 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/integration/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.570405 rdt-1.6.1.dev1/tests/integration/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       86 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/integration/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     7350 2023-08-02 16:15:08.000000 rdt-1.6.1.dev1/tests/integration/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3880 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/tests/integration/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3425 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/tests/integration/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    13328 2023-04-13 17:39:49.000000 rdt-1.6.1.dev1/tests/integration/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5946 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/tests/integration/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    10507 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/tests/integration/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8389 2023-04-13 17:39:49.000000 rdt-1.6.1.dev1/tests/integration/transformers/test_text.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.571054 rdt-1.6.1.dev1/tests/performance/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       81 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/performance/README.md
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      190 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/performance/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5112 2023-04-13 17:39:49.000000 rdt-1.6.1.dev1/tests/performance/test_performance.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.571584 rdt-1.6.1.dev1/tests/performance/tests/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       39 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/performance/tests/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3224 2022-08-18 00:01:17.000000 rdt-1.6.1.dev1/tests/performance/tests/test_profiling.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.572159 rdt-1.6.1.dev1/tests/unit/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       32 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/unit/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     5961 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/tests/unit/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)   104228 2023-07-17 20:29:05.000000 rdt-1.6.1.dev1/tests/unit/test_hyper_transformer.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.573977 rdt-1.6.1.dev1/tests/unit/transformers/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       45 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/unit/transformers/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.574133 rdt-1.6.1.dev1/tests/unit/transformers/addons/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       33 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/unit/transformers/addons/__init__.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.574431 rdt-1.6.1.dev1/tests/unit/transformers/addons/identity/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       41 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/unit/transformers/addons/identity/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     2234 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/tests/unit/transformers/addons/identity/test_identity.py
+drwxr-xr-x   0 andrewmontanez   (501) staff       (20)        0 2023-08-02 16:15:49.574965 rdt-1.6.1.dev1/tests/unit/transformers/pii/
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)       60 2022-08-17 01:38:30.000000 rdt-1.6.1.dev1/tests/unit/transformers/pii/__init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    30828 2023-08-02 16:15:08.000000 rdt-1.6.1.dev1/tests/unit/transformers/pii/test_anonymizer.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)      985 2023-01-18 20:52:41.000000 rdt-1.6.1.dev1/tests/unit/transformers/pii/test_utils.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     3221 2023-07-17 20:29:05.000000 rdt-1.6.1.dev1/tests/unit/transformers/test___init__.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    42015 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/tests/unit/transformers/test_base.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     8973 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/tests/unit/transformers/test_boolean.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    60429 2023-04-13 17:39:49.000000 rdt-1.6.1.dev1/tests/unit/transformers/test_categorical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    18310 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/tests/unit/transformers/test_datetime.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    19138 2023-07-12 20:34:31.000000 rdt-1.6.1.dev1/tests/unit/transformers/test_null.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    57532 2023-06-01 21:46:38.000000 rdt-1.6.1.dev1/tests/unit/transformers/test_numerical.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)    12685 2023-04-13 17:39:49.000000 rdt-1.6.1.dev1/tests/unit/transformers/test_text.py
+-rw-r--r--   0 andrewmontanez   (501) staff       (20)     1513 2023-04-26 21:05:25.000000 rdt-1.6.1.dev1/tests/unit/transformers/test_utils.py
```

### Comparing `rdt-1.6.1.dev0/CONTRIBUTING.rst` & `rdt-1.6.1.dev1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/HISTORY.md` & `rdt-1.6.1.dev1/HISTORY.md`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/LICENSE` & `rdt-1.6.1.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/PKG-INFO` & `rdt-1.6.1.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.6.1.dev0
+Version: 1.6.1.dev1
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,15 @@
 
 <div align="center">
 <br/>
 <p align="center">
     <i>This repository is part of <a href="https://sdv.dev">The Synthetic Data Vault Project</a>, a project from <a href="https://datacebo.com">DataCebo</a>.</i>
 </p>
 
-[![Development Status](https://img.shields.io/badge/Development%20Status-3%20--%20Alpha-yellow)](https://pypi.org/search/?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha)
+[![Development Status](https://img.shields.io/badge/Development%20Status-5%20--%20Production/Stable-green)](https://pypi.org/search/?q=&o=&c=Development+Status+%3A%3A+5+-+Production%2FStable)
 [![PyPi Shield](https://img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT)
 [![Unit Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/badge.svg)](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml)
 [![Downloads](https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt)
 [![Coverage Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/badge.svg)](https://codecov.io/gh/sdv-dev/RDT)
 [![Slack](https://img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-invite)
 
 <div align="left">
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.6.1.dev0 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.6.1.dev1 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: License :: Free for non-commercial use Classifier: Natural Language
-:: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.12
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: Free for non-commercial use Classifier:
+Natural Language :: English Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown Provides-Extra: copulas Provides-Extra:
 test Provides-Extra: dev License-File: LICENSE License-File: AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
-[![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
-                  %20Alpha-yellow)](https://pypi.org/search/
-    ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
-   img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
- Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/badge.svg)]
-   (https://github.com/sdv-dev/RDT/actions/workflows/unit.yml) [![Downloads]
-   (https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt) [![Coverage
-   Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/badge.svg)]
-  (https://codecov.io/gh/sdv-dev/RDT) [![Slack](https://img.shields.io/badge/
-   Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-
-                                    invite)
+[![Development Status](https://img.shields.io/badge/Development%20Status-5%20--
+             %20Production/Stable-green)](https://pypi.org/search/
+  ?q=&o=&c=Development+Status+%3A%3A+5+-+Production%2FStable) [![PyPi Shield]
+ (https://img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [!
+    [Unit Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/
+   badge.svg)](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml) [!
+  [Downloads](https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt) [!
+   [Coverage Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/
+       badge.svg)](https://codecov.io/gh/sdv-dev/RDT) [![Slack](https://
+ img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://
+                           bit.ly/sdv-slack-invite)
 
    [https://github.com/sdv-dev/SDV/blob/master/docs/images/RDT-DataCebo.png]
 # Overview RDT (Reversible Data Transforms) is a Python library that transforms
 raw data into fully numerical data, ready for data science. The transforms are
 reversible, allowing you to convert from numerical data back into your original
 format. [https://github.com/sdv-dev/SDV/blob/master/docs/images/
 rdt_main_tranformation.png] # Install Install **RDT** using ``pip`` or
```

### Comparing `rdt-1.6.1.dev0/README.md` & `rdt-1.6.1.dev1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <div align="center">
 <br/>
 <p align="center">
     <i>This repository is part of <a href="https://sdv.dev">The Synthetic Data Vault Project</a>, a project from <a href="https://datacebo.com">DataCebo</a>.</i>
 </p>
 
-[![Development Status](https://img.shields.io/badge/Development%20Status-3%20--%20Alpha-yellow)](https://pypi.org/search/?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha)
+[![Development Status](https://img.shields.io/badge/Development%20Status-5%20--%20Production/Stable-green)](https://pypi.org/search/?q=&o=&c=Development+Status+%3A%3A+5+-+Production%2FStable)
 [![PyPi Shield](https://img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT)
 [![Unit Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/badge.svg)](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml)
 [![Downloads](https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt)
 [![Coverage Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/badge.svg)](https://codecov.io/gh/sdv-dev/RDT)
 [![Slack](https://img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-invite)
 
 <div align="left">
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
-[![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
-                  %20Alpha-yellow)](https://pypi.org/search/
-    ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
-   img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
- Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/badge.svg)]
-   (https://github.com/sdv-dev/RDT/actions/workflows/unit.yml) [![Downloads]
-   (https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt) [![Coverage
-   Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/badge.svg)]
-  (https://codecov.io/gh/sdv-dev/RDT) [![Slack](https://img.shields.io/badge/
-   Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-
-                                    invite)
+[![Development Status](https://img.shields.io/badge/Development%20Status-5%20--
+             %20Production/Stable-green)](https://pypi.org/search/
+  ?q=&o=&c=Development+Status+%3A%3A+5+-+Production%2FStable) [![PyPi Shield]
+ (https://img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [!
+    [Unit Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/
+   badge.svg)](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml) [!
+  [Downloads](https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt) [!
+   [Coverage Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/
+       badge.svg)](https://codecov.io/gh/sdv-dev/RDT) [![Slack](https://
+ img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://
+                           bit.ly/sdv-slack-invite)
 
    [https://github.com/sdv-dev/SDV/blob/master/docs/images/RDT-DataCebo.png]
 # Overview RDT (Reversible Data Transforms) is a Python library that transforms
 raw data into fully numerical data, ready for data science. The transforms are
 reversible, allowing you to convert from numerical data back into your original
 format. [https://github.com/sdv-dev/SDV/blob/master/docs/images/
 rdt_main_tranformation.png] # Install Install **RDT** using ``pip`` or
```

### Comparing `rdt-1.6.1.dev0/RELEASE.md` & `rdt-1.6.1.dev1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/__init__.py` & `rdt-1.6.1.dev1/rdt/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 """Top-level package for RDT."""
 
 
 __author__ = 'DataCebo, Inc.'
 __email__ = 'info@sdv.dev'
-__version__ = '1.6.1.dev0'
+__version__ = '1.6.1.dev1'
 
 
 import sys
 import warnings
 from operator import attrgetter
 from types import ModuleType
```

### Comparing `rdt-1.6.1.dev0/rdt/errors.py` & `rdt-1.6.1.dev1/rdt/errors.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/hyper_transformer.py` & `rdt-1.6.1.dev1/rdt/hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/__init__.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/base.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/boolean.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/categorical.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/datetime.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/numerical.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/pii.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/pii.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/text.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/datasets/utils.py` & `rdt-1.6.1.dev1/rdt/performance/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/performance.py` & `rdt-1.6.1.dev1/rdt/performance/performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/performance/profiling.py` & `rdt-1.6.1.dev1/rdt/performance/profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/__init__.py` & `rdt-1.6.1.dev1/rdt/transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/addons/addons_setup.py` & `rdt-1.6.1.dev1/rdt/transformers/addons/addons_setup.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/base.py` & `rdt-1.6.1.dev1/rdt/transformers/base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/boolean.py` & `rdt-1.6.1.dev1/rdt/transformers/boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/categorical.py` & `rdt-1.6.1.dev1/rdt/transformers/categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/datetime.py` & `rdt-1.6.1.dev1/rdt/transformers/datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/null.py` & `rdt-1.6.1.dev1/rdt/transformers/null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/numerical.py` & `rdt-1.6.1.dev1/rdt/transformers/numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/pii/anonymizer.py` & `rdt-1.6.1.dev1/rdt/transformers/pii/anonymizer.py`

 * *Files 7% similar despite different names*

```diff
@@ -120,14 +120,31 @@
                 f"Missing value generation '{missing_value_generation}' is not supported "
                 "for AnonymizedFaker. Please use either 'random' or None."
             )
 
         self.missing_value_generation = missing_value_generation
         self._nan_frequency = 0.0
 
+    @classmethod
+    def get_supported_sdtypes(cls):
+        """Return the supported sdtypes by the transformer.
+
+        Returns:
+            list:
+                Accepted input sdtypes of the transformer.
+        """
+        unsupported_sdtypes = {'numerical', 'datetime', 'categorical', 'boolean', 'text', None}
+        all_sdtypes = {cls.INPUT_SDTYPE}
+        for transformer in BaseTransformer.get_subclasses():
+            if not issubclass(transformer, cls):
+                all_sdtypes.update(transformer.get_supported_sdtypes())
+
+        supported_sdtypes = all_sdtypes - unsupported_sdtypes
+        return list(supported_sdtypes)
+
     def reset_randomization(self):
         """Create a new ``Faker`` instance."""
         super().reset_randomization()
         self.faker = faker.Faker(self.locales)
         self.faker.seed_instance(self._faker_random_seed)
 
     def _function(self):
```

### Comparing `rdt-1.6.1.dev0/rdt/transformers/pii/utils.py` & `rdt-1.6.1.dev1/rdt/transformers/pii/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/text.py` & `rdt-1.6.1.dev1/rdt/transformers/text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt/transformers/utils.py` & `rdt-1.6.1.dev1/rdt/transformers/utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt.egg-info/PKG-INFO` & `rdt-1.6.1.dev1/rdt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: rdt
-Version: 1.6.1.dev0
+Version: 1.6.1.dev1
 Summary: Reversible Data Transforms
 Home-page: https://github.com/sdv-dev/RDT
 Author: DataCebo, Inc.
 Author-email: info@sdv.dev
 License: BSL-1.1
 Keywords: rdt
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Free for non-commercial use
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -27,15 +27,15 @@
 
 <div align="center">
 <br/>
 <p align="center">
     <i>This repository is part of <a href="https://sdv.dev">The Synthetic Data Vault Project</a>, a project from <a href="https://datacebo.com">DataCebo</a>.</i>
 </p>
 
-[![Development Status](https://img.shields.io/badge/Development%20Status-3%20--%20Alpha-yellow)](https://pypi.org/search/?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha)
+[![Development Status](https://img.shields.io/badge/Development%20Status-5%20--%20Production/Stable-green)](https://pypi.org/search/?q=&o=&c=Development+Status+%3A%3A+5+-+Production%2FStable)
 [![PyPi Shield](https://img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT)
 [![Unit Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/badge.svg)](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml)
 [![Downloads](https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt)
 [![Coverage Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/badge.svg)](https://codecov.io/gh/sdv-dev/RDT)
 [![Slack](https://img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-invite)
 
 <div align="left">
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: rdt Version: 1.6.1.dev0 Summary: Reversible Data
+Metadata-Version: 2.1 Name: rdt Version: 1.6.1.dev1 Summary: Reversible Data
 Transforms Home-page: https://github.com/sdv-dev/RDT Author: DataCebo, Inc.
 Author-email: info@sdv.dev License: BSL-1.1 Keywords: rdt Classifier:
-Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
-Classifier: License :: Free for non-commercial use Classifier: Natural Language
-:: English Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.8 Classifier: Programming Language ::
-Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
-Programming Language :: Python :: 3.11 Classifier: Topic :: Scientific/
-Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.12
+Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
+Developers Classifier: License :: Free for non-commercial use Classifier:
+Natural Language :: English Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Classifier: Topic ::
+Scientific/Engineering :: Artificial Intelligence Requires-Python: >=3.8,<3.12
 Description-Content-Type: text/markdown Provides-Extra: copulas Provides-Extra:
 test Provides-Extra: dev License-File: LICENSE License-File: AUTHORS.rst
 
   This repository is part of The_Synthetic_Data_Vault_Project, a project from
                                    DataCebo.
-[![Development Status](https://img.shields.io/badge/Development%20Status-3%20--
-                  %20Alpha-yellow)](https://pypi.org/search/
-    ?q=&o=&c=Development+Status+%3A%3A+3+-+Alpha) [![PyPi Shield](https://
-   img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [![Unit
- Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/badge.svg)]
-   (https://github.com/sdv-dev/RDT/actions/workflows/unit.yml) [![Downloads]
-   (https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt) [![Coverage
-   Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/badge.svg)]
-  (https://codecov.io/gh/sdv-dev/RDT) [![Slack](https://img.shields.io/badge/
-   Community-Slack-blue?style=plastic&logo=slack)](https://bit.ly/sdv-slack-
-                                    invite)
+[![Development Status](https://img.shields.io/badge/Development%20Status-5%20--
+             %20Production/Stable-green)](https://pypi.org/search/
+  ?q=&o=&c=Development+Status+%3A%3A+5+-+Production%2FStable) [![PyPi Shield]
+ (https://img.shields.io/pypi/v/RDT.svg)](https://pypi.python.org/pypi/RDT) [!
+    [Unit Tests](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml/
+   badge.svg)](https://github.com/sdv-dev/RDT/actions/workflows/unit.yml) [!
+  [Downloads](https://pepy.tech/badge/rdt)](https://pepy.tech/project/rdt) [!
+   [Coverage Status](https://codecov.io/gh/sdv-dev/RDT/branch/master/graph/
+       badge.svg)](https://codecov.io/gh/sdv-dev/RDT) [![Slack](https://
+ img.shields.io/badge/Community-Slack-blue?style=plastic&logo=slack)](https://
+                           bit.ly/sdv-slack-invite)
 
    [https://github.com/sdv-dev/SDV/blob/master/docs/images/RDT-DataCebo.png]
 # Overview RDT (Reversible Data Transforms) is a Python library that transforms
 raw data into fully numerical data, ready for data science. The transforms are
 reversible, allowing you to convert from numerical data back into your original
 format. [https://github.com/sdv-dev/SDV/blob/master/docs/images/
 rdt_main_tranformation.png] # Install Install **RDT** using ``pip`` or
```

### Comparing `rdt-1.6.1.dev0/rdt.egg-info/SOURCES.txt` & `rdt-1.6.1.dev1/rdt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/rdt.egg-info/requires.txt` & `rdt-1.6.1.dev1/rdt.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/setup.cfg` & `rdt-1.6.1.dev1/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 1.6.1.dev0
+current_version = 1.6.1.dev1
 commit = True
 tag = True
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\.(?P<release>[a-z]+)(?P<candidate>\d+))?
 serialize = 
 	{major}.{minor}.{patch}.{release}{candidate}
 	{major}.{minor}.{patch}
```

### Comparing `rdt-1.6.1.dev0/setup.py` & `rdt-1.6.1.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     'invoke'
 ]
 
 setup(
     author='DataCebo, Inc.',
     author_email='info@sdv.dev',
     classifiers=[
-        'Development Status :: 2 - Pre-Alpha',
+        'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: Free for non-commercial use',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
@@ -135,10 +135,10 @@
         exclude=['rdt.transformers.addons.*']
     ),
     python_requires='>=3.8,<3.12',
     setup_requires=setup_requires,
     test_suite='tests',
     tests_require=tests_require,
     url='https://github.com/sdv-dev/RDT',
-    version='1.6.1.dev0',
+    version='1.6.1.dev1',
     zip_safe=False,
 )
```

### Comparing `rdt-1.6.1.dev0/tests/__init__.py` & `rdt-1.6.1.dev1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/code_style.py` & `rdt-1.6.1.dev1/tests/code_style.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/contributing.py` & `rdt-1.6.1.dev1/tests/contributing.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/datasets/tests/test_boolean.py` & `rdt-1.6.1.dev1/tests/datasets/tests/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/datasets/tests/test_categorical.py` & `rdt-1.6.1.dev1/tests/datasets/tests/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/datasets/tests/test_datetime.py` & `rdt-1.6.1.dev1/tests/datasets/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/datasets/tests/test_numerical.py` & `rdt-1.6.1.dev1/tests/datasets/tests/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/datasets/tests/test_utils.py` & `rdt-1.6.1.dev1/tests/datasets/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/integration/test_hyper_transformer.py` & `rdt-1.6.1.dev1/tests/integration/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/integration/test_transformers.py` & `rdt-1.6.1.dev1/tests/integration/test_transformers.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/integration/transformers/pii/test_anonymizer.py` & `rdt-1.6.1.dev1/tests/integration/transformers/pii/test_anonymizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,23 @@
         'id': [1, 2, 3, 4, 5]
     })
 
     pd.testing.assert_frame_equal(transformed, expected_transformed)
     assert len(reverse_transform['username']) == 5
 
 
+def test_anonymizedfaker_get_supported_sdtypes():
+    """Test that the correct supported sdtypes are returned."""
+    # Run
+    supported_sdtypes = AnonymizedFaker.get_supported_sdtypes()
+
+    # Assert
+    assert supported_sdtypes == ['pii']
+
+
 def test_anonymizedfaker_custom_provider():
     """End to end test with a custom provider and function for the ``AnonymizedFaker``."""
     data = pd.DataFrame({
         'id': [1, 2, 3, 4, 5],
         'username': ['a', 'b', 'c', 'd', 'e'],
         'cc': [
             '2276346007210438',
```

### Comparing `rdt-1.6.1.dev0/tests/integration/transformers/test_base.py` & `rdt-1.6.1.dev1/tests/integration/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/integration/transformers/test_boolean.py` & `rdt-1.6.1.dev1/tests/integration/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/integration/transformers/test_categorical.py` & `rdt-1.6.1.dev1/tests/integration/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/integration/transformers/test_datetime.py` & `rdt-1.6.1.dev1/tests/integration/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/integration/transformers/test_numerical.py` & `rdt-1.6.1.dev1/tests/integration/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/integration/transformers/test_text.py` & `rdt-1.6.1.dev1/tests/integration/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/performance/test_performance.py` & `rdt-1.6.1.dev1/tests/performance/test_performance.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/performance/tests/test_profiling.py` & `rdt-1.6.1.dev1/tests/performance/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/test___init__.py` & `rdt-1.6.1.dev1/tests/unit/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/test_hyper_transformer.py` & `rdt-1.6.1.dev1/tests/unit/test_hyper_transformer.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/addons/identity/test_identity.py` & `rdt-1.6.1.dev1/tests/unit/transformers/addons/identity/test_identity.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/pii/test_anonymizer.py` & `rdt-1.6.1.dev1/tests/unit/transformers/pii/test_anonymizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -294,14 +294,50 @@
         expected_message = (
             'Please specify the function name to use from the '
             "'credit_card' provider."
         )
         with pytest.raises(TransformerInputError, match=expected_message):
             AnonymizedFaker(provider_name='credit_card', locales=['en_US', 'fr_FR'])
 
+    @patch('rdt.transformers.pii.anonymizer.issubclass')
+    @patch('rdt.transformers.pii.anonymizer.BaseTransformer')
+    def test_get_supported_sdtypes(self, base_mock, issubclass_mock):
+        """Test that the method returns all sdtypes except the basic ones."""
+        # Setup
+        issubclass_mock.return_value = False
+        numerical_mock = Mock()
+        numerical_mock.get_supported_sdtypes.return_value = ['numerical']
+        categorical_mock = Mock()
+        categorical_mock.get_supported_sdtypes.return_value = ['categorical']
+        datetime_mock = Mock()
+        datetime_mock.get_supported_sdtypes.return_value = ['datetime']
+        boolean_mock = Mock()
+        boolean_mock.get_supported_sdtypes.return_value = ['boolean', 'categorical']
+        text_mock = Mock()
+        text_mock.get_supported_sdtypes.return_value = ['text']
+        phone_mock = Mock()
+        phone_mock.get_supported_sdtypes.return_value = ['phone_number']
+        pii_mock = Mock()
+        pii_mock.get_supported_sdtypes.return_value = ['pii']
+        base_mock.get_subclasses.return_value = [
+            numerical_mock,
+            categorical_mock,
+            datetime_mock,
+            boolean_mock,
+            text_mock,
+            phone_mock,
+            pii_mock
+        ]
+
+        # Run
+        supported_sdtypes = AnonymizedFaker.get_supported_sdtypes()
+
+        # Assert
+        assert sorted(supported_sdtypes) == sorted(['phone_number', 'pii'])
+
     @patch('rdt.transformers.pii.anonymizer.BaseTransformer.reset_randomization')
     @patch('rdt.transformers.pii.anonymizer.faker')
     def test_reset_randomization(self, mock_faker, mock_base_reset):
         """Test that this function creates a new faker instance."""
         # Setup
         instance = AnonymizedFaker()
         instance.locales = ['en_US']
```

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/pii/test_utils.py` & `rdt-1.6.1.dev1/tests/unit/transformers/pii/test_utils.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test___init__.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test___init__.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test_base.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test_base.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test_boolean.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test_boolean.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test_categorical.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test_categorical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test_datetime.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test_datetime.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test_null.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test_null.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test_numerical.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test_numerical.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test_text.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test_text.py`

 * *Files identical despite different names*

### Comparing `rdt-1.6.1.dev0/tests/unit/transformers/test_utils.py` & `rdt-1.6.1.dev1/tests/unit/transformers/test_utils.py`

 * *Files identical despite different names*

