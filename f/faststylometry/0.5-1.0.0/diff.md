# Comparing `tmp/faststylometry-0.5.tar.gz` & `tmp/faststylometry-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/faststylometry-0.5.tar", last modified: Fri Jan 29 10:44:33 2021, max compression
+gzip compressed data, was "faststylometry-1.0.0.tar", last modified: Tue Aug  1 23:08:30 2023, max compression
```

## Comparing `faststylometry-0.5.tar` & `faststylometry-1.0.0.tar`

### file list

```diff
@@ -1,12 +1,24 @@
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2021-01-29 10:44:33.095436 faststylometry-0.5/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     5137 2021-01-29 10:44:33.095436 faststylometry-0.5/PKG-INFO
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     3455 2021-01-28 15:53:40.089804 faststylometry-0.5/README.rst
-drwxrwxr-x   0 thomas    (1000) thomas    (1000)        0 2021-01-29 10:44:33.095436 faststylometry-0.5/faststylometry/
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      307 2021-01-29 10:26:50.558611 faststylometry-0.5/faststylometry/__init__.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     7192 2021-01-27 13:55:19.664196 faststylometry-0.5/faststylometry/burrows_delta.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2919 2021-01-27 13:55:06.416277 faststylometry-0.5/faststylometry/corpus.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1170 2021-01-27 11:29:37.401428 faststylometry-0.5/faststylometry/en.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     2980 2021-01-28 10:56:35.631129 faststylometry-0.5/faststylometry/probability.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)      998 2021-01-27 11:24:26.765789 faststylometry-0.5/faststylometry/util.py
--rw-rw-r--   0 thomas    (1000) thomas    (1000)       61 2020-08-26 08:31:08.962848 faststylometry-0.5/setup.cfg
--rw-rw-r--   0 thomas    (1000) thomas    (1000)     1149 2021-01-29 10:13:14.597981 faststylometry-0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:08:30.558164 faststylometry-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-08-01 23:08:20.000000 faststylometry-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-08-01 23:08:20.000000 faststylometry-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-08-01 23:08:30.558164 faststylometry-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6676 2023-08-01 23:08:20.000000 faststylometry-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-08-01 23:08:20.000000 faststylometry-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-01 23:08:30.558164 faststylometry-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-01 23:08:20.000000 faststylometry-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:08:30.554164 faststylometry-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:08:30.558164 faststylometry-1.0.0/src/faststylometry/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-08-01 23:08:20.000000 faststylometry-1.0.0/src/faststylometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-08-01 23:08:20.000000 faststylometry-1.0.0/src/faststylometry/burrows_delta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-08-01 23:08:20.000000 faststylometry-1.0.0/src/faststylometry/corpus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2386 2023-08-01 23:08:20.000000 faststylometry-1.0.0/src/faststylometry/en.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-08-01 23:08:20.000000 faststylometry-1.0.0/src/faststylometry/probability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-08-01 23:08:20.000000 faststylometry-1.0.0/src/faststylometry/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:08:30.558164 faststylometry-1.0.0/src/faststylometry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-08-01 23:08:30.000000 faststylometry-1.0.0/src/faststylometry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-08-01 23:08:30.000000 faststylometry-1.0.0/src/faststylometry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-01 23:08:30.000000 faststylometry-1.0.0/src/faststylometry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-08-01 23:08:30.000000 faststylometry-1.0.0/src/faststylometry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-08-01 23:08:30.000000 faststylometry-1.0.0/src/faststylometry.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-01 23:08:30.558164 faststylometry-1.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-08-01 23:08:20.000000 faststylometry-1.0.0/tests/test_drugs_finder.py
```

