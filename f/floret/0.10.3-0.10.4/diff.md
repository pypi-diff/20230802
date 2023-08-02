# Comparing `tmp/floret-0.10.3.tar.gz` & `tmp/floret-0.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "floret-0.10.3.tar", last modified: Tue May  9 06:21:25 2023, max compression
+gzip compressed data, was "floret-0.10.4.tar", last modified: Wed Aug  2 12:14:43 2023, max compression
```

## Comparing `floret-0.10.3.tar` & `floret-0.10.4.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.487887 floret-0.10.3/
--rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-05-09 06:21:09.000000 floret-0.10.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-05-09 06:21:09.000000 floret-0.10.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     2968 2023-05-09 06:21:25.487887 floret-0.10.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)    20392 2023-05-09 06:21:09.000000 floret-0.10.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-05-09 06:21:09.000000 floret-0.10.3/pyproject.toml
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/
--rw-r--r--   0 vsts      (1001) docker     (122)     2068 2023-05-09 06:21:09.000000 floret-0.10.3/python/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.479886 floret-0.10.3/python/floret_module/
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret/
--rw-r--r--   0 vsts      (1001) docker     (122)      639 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    20068 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/floret.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret/pybind/
--rw-r--r--   0 vsts      (1001) docker     (122)    20431 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/pybind/floret_pybind.cc
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret/tests/
--rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      475 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10914 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/data.txt
--rw-r--r--   0 vsts      (1001) docker     (122)     7060 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/test_configurations.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21765 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/test_script.py
--rw-r--r--   0 vsts      (1001) docker     (122)       96 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/test_tokenize.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2111 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/tests/test_train.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret/util/
--rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7490 2023-05-09 06:21:09.000000 floret-0.10.3/python/floret_module/floret/util/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.483886 floret-0.10.3/python/floret_module/floret.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     2968 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-05-09 06:21:25.000000 floret-0.10.3/python/floret_module/floret.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       79 2023-05-09 06:21:25.487887 floret-0.10.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     5975 2023-05-09 06:21:09.000000 floret-0.10.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-09 06:21:25.487887 floret-0.10.3/src/
--rw-r--r--   0 vsts      (1001) docker     (122)     8609 2023-05-09 06:21:09.000000 floret-0.10.3/src/MurmurHash3.cpp
--rw-r--r--   0 vsts      (1001) docker     (122)      804 2023-05-09 06:21:09.000000 floret-0.10.3/src/MurmurHash3.h
--rw-r--r--   0 vsts      (1001) docker     (122)    17847 2023-05-09 06:21:09.000000 floret-0.10.3/src/args.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2309 2023-05-09 06:21:09.000000 floret-0.10.3/src/args.h
--rw-r--r--   0 vsts      (1001) docker     (122)    13879 2023-05-09 06:21:09.000000 floret-0.10.3/src/autotune.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2266 2023-05-09 06:21:09.000000 floret-0.10.3/src/autotune.h
--rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-05-09 06:21:09.000000 floret-0.10.3/src/densematrix.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2155 2023-05-09 06:21:09.000000 floret-0.10.3/src/densematrix.h
--rw-r--r--   0 vsts      (1001) docker     (122)    15049 2023-05-09 06:21:09.000000 floret-0.10.3/src/dictionary.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3219 2023-05-09 06:21:09.000000 floret-0.10.3/src/dictionary.h
--rw-r--r--   0 vsts      (1001) docker     (122)    25809 2023-05-09 06:21:09.000000 floret-0.10.3/src/fasttext.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     4819 2023-05-09 06:21:09.000000 floret-0.10.3/src/fasttext.h
--rw-r--r--   0 vsts      (1001) docker     (122)     9124 2023-05-09 06:21:09.000000 floret-0.10.3/src/loss.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     3879 2023-05-09 06:21:09.000000 floret-0.10.3/src/loss.h
--rw-r--r--   0 vsts      (1001) docker     (122)    12928 2023-05-09 06:21:09.000000 floret-0.10.3/src/main.cc
--rw-r--r--   0 vsts      (1001) docker     (122)      494 2023-05-09 06:21:09.000000 floret-0.10.3/src/matrix.cc
--rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-05-09 06:21:09.000000 floret-0.10.3/src/matrix.h
--rw-r--r--   0 vsts      (1001) docker     (122)     6129 2023-05-09 06:21:09.000000 floret-0.10.3/src/meter.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     2510 2023-05-09 06:21:09.000000 floret-0.10.3/src/meter.h
--rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-05-09 06:21:09.000000 floret-0.10.3/src/model.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1720 2023-05-09 06:21:09.000000 floret-0.10.3/src/model.h
--rw-r--r--   0 vsts      (1001) docker     (122)     6234 2023-05-09 06:21:09.000000 floret-0.10.3/src/productquantizer.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1607 2023-05-09 06:21:09.000000 floret-0.10.3/src/productquantizer.h
--rw-r--r--   0 vsts      (1001) docker     (122)     3370 2023-05-09 06:21:09.000000 floret-0.10.3/src/quantmatrix.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1474 2023-05-09 06:21:09.000000 floret-0.10.3/src/quantmatrix.h
--rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-05-09 06:21:09.000000 floret-0.10.3/src/real.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-05-09 06:21:09.000000 floret-0.10.3/src/utils.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1722 2023-05-09 06:21:09.000000 floret-0.10.3/src/utils.h
--rw-r--r--   0 vsts      (1001) docker     (122)     1961 2023-05-09 06:21:09.000000 floret-0.10.3/src/vector.cc
--rw-r--r--   0 vsts      (1001) docker     (122)     1273 2023-05-09 06:21:09.000000 floret-0.10.3/src/vector.h
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.651761 floret-0.10.4/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1111 2023-08-02 12:14:27.000000 floret-0.10.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-08-02 12:14:27.000000 floret-0.10.4/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)     3070 2023-08-02 12:14:43.651761 floret-0.10.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)    20392 2023-08-02 12:14:27.000000 floret-0.10.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      111 2023-08-02 12:14:27.000000 floret-0.10.4/pyproject.toml
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.647761 floret-0.10.4/python/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2068 2023-08-02 12:14:27.000000 floret-0.10.4/python/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.643760 floret-0.10.4/python/floret_module/
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.647761 floret-0.10.4/python/floret_module/floret/
+-rw-r--r--   0 vsts      (1001) docker     (122)      639 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    20106 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/floret.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.647761 floret-0.10.4/python/floret_module/floret/pybind/
+-rw-r--r--   0 vsts      (1001) docker     (122)    20431 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/pybind/floret_pybind.cc
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.647761 floret-0.10.4/python/floret_module/floret/tests/
+-rw-r--r--   0 vsts      (1001) docker     (122)      102 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/tests/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      475 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10914 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/tests/data.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)     7060 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/tests/test_configurations.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21765 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/tests/test_script.py
+-rw-r--r--   0 vsts      (1001) docker     (122)       96 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/tests/test_tokenize.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2111 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/tests/test_train.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.647761 floret-0.10.4/python/floret_module/floret/util/
+-rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7490 2023-08-02 12:14:27.000000 floret-0.10.4/python/floret_module/floret/util/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.647761 floret-0.10.4/python/floret_module/floret.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3070 2023-08-02 12:14:43.000000 floret-0.10.4/python/floret_module/floret.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1392 2023-08-02 12:14:43.000000 floret-0.10.4/python/floret_module/floret.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-02 12:14:43.000000 floret-0.10.4/python/floret_module/floret.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-08-02 12:14:43.000000 floret-0.10.4/python/floret_module/floret.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (122)        6 2023-08-02 12:14:43.000000 floret-0.10.4/python/floret_module/floret.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       21 2023-08-02 12:14:43.000000 floret-0.10.4/python/floret_module/floret.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       79 2023-08-02 12:14:43.651761 floret-0.10.4/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     6075 2023-08-02 12:14:27.000000 floret-0.10.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-08-02 12:14:43.651761 floret-0.10.4/src/
+-rw-r--r--   0 vsts      (1001) docker     (122)     8609 2023-08-02 12:14:27.000000 floret-0.10.4/src/MurmurHash3.cpp
+-rw-r--r--   0 vsts      (1001) docker     (122)      804 2023-08-02 12:14:27.000000 floret-0.10.4/src/MurmurHash3.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    17847 2023-08-02 12:14:27.000000 floret-0.10.4/src/args.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2309 2023-08-02 12:14:27.000000 floret-0.10.4/src/args.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    13879 2023-08-02 12:14:27.000000 floret-0.10.4/src/autotune.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2266 2023-08-02 12:14:27.000000 floret-0.10.4/src/autotune.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     4230 2023-08-02 12:14:27.000000 floret-0.10.4/src/densematrix.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2155 2023-08-02 12:14:27.000000 floret-0.10.4/src/densematrix.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    15049 2023-08-02 12:14:27.000000 floret-0.10.4/src/dictionary.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3219 2023-08-02 12:14:27.000000 floret-0.10.4/src/dictionary.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    25809 2023-08-02 12:14:27.000000 floret-0.10.4/src/fasttext.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     4819 2023-08-02 12:14:27.000000 floret-0.10.4/src/fasttext.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     9124 2023-08-02 12:14:27.000000 floret-0.10.4/src/loss.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     3879 2023-08-02 12:14:27.000000 floret-0.10.4/src/loss.h
+-rw-r--r--   0 vsts      (1001) docker     (122)    12928 2023-08-02 12:14:27.000000 floret-0.10.4/src/main.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)      494 2023-08-02 12:14:27.000000 floret-0.10.4/src/matrix.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)      972 2023-08-02 12:14:27.000000 floret-0.10.4/src/matrix.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6129 2023-08-02 12:14:27.000000 floret-0.10.4/src/meter.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     2510 2023-08-02 12:14:27.000000 floret-0.10.4/src/meter.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     2271 2023-08-02 12:14:27.000000 floret-0.10.4/src/model.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1720 2023-08-02 12:14:27.000000 floret-0.10.4/src/model.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     6234 2023-08-02 12:14:27.000000 floret-0.10.4/src/productquantizer.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1607 2023-08-02 12:14:27.000000 floret-0.10.4/src/productquantizer.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     3370 2023-08-02 12:14:27.000000 floret-0.10.4/src/quantmatrix.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1474 2023-08-02 12:14:27.000000 floret-0.10.4/src/quantmatrix.h
+-rw-r--r--   0 vsts      (1001) docker     (122)      266 2023-08-02 12:14:27.000000 floret-0.10.4/src/real.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1275 2023-08-02 12:14:27.000000 floret-0.10.4/src/utils.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1722 2023-08-02 12:14:27.000000 floret-0.10.4/src/utils.h
+-rw-r--r--   0 vsts      (1001) docker     (122)     1961 2023-08-02 12:14:27.000000 floret-0.10.4/src/vector.cc
+-rw-r--r--   0 vsts      (1001) docker     (122)     1273 2023-08-02 12:14:27.000000 floret-0.10.4/src/vector.h
```

### Comparing `floret-0.10.3/LICENSE` & `floret-0.10.4/LICENSE`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/PKG-INFO` & `floret-0.10.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: floret
-Version: 0.10.3
+Version: 0.10.4
 Summary: floret Python bindings
 Home-page: https://github.com/explosion/floret
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: floret Version: 0.10.3 Summary: floret Python
+Metadata-Version: 2.1 Name: floret Version: 0.10.4 Summary: floret Python
 bindings Home-page: https://github.com/explosion/floret Author: Explosion
 Author-email: contact@explosion.ai License: MIT Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
-Development Classifier: Topic :: Scientific/Engineering Classifier: Operating
-System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
-Description-Content-Type: text/markdown License-File: LICENSE [https://
-explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom embeddings for
-compact, full-coverage vectors with spaCy floret is an extended version of
-[fastText](https://fasttext.cc) that can produce word representations for any
-word from a compact vector table. It combines: - fastText's subwords to provide
-embeddings for any word - Bloom embeddings ("hashing trick") for a compact
-vector table ## Installation ```bash pip install floret ``` ## Usage Train
-floret vectors using the options: - `mode`: `"floret"`, storing both words and
-subwords in the same compact hash table - `hashCount`: store each entry in 1-
-4 rows in the hash table (recommended: `2`) - `bucket`: in combination with
-`hashCount>1`, the size of the hash table can be greatly reduced (recommended:
-`25000`--`100000`, reduced from the fastText default of `2000000`) - `minn`:
-min length of char ngram (default: `3`) - `maxn`: max length of char ngram
-(default: `6`) ```python import floret # train vectors model =
-floret.train_unsupervised( "data.txt", model="cbow", mode="floret",
-hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
+Engineering Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX Classifier: Operating System :: Unix Classifier:
+Operating System :: MacOS Description-Content-Type: text/markdown License-File:
+LICENSE [https://explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom
+embeddings for compact, full-coverage vectors with spaCy floret is an extended
+version of [fastText](https://fasttext.cc) that can produce word
+representations for any word from a compact vector table. It combines: -
+fastText's subwords to provide embeddings for any word - Bloom embeddings
+("hashing trick") for a compact vector table ## Installation ```bash pip
+install floret ``` ## Usage Train floret vectors using the options: - `mode`:
+`"floret"`, storing both words and subwords in the same compact hash table -
+`hashCount`: store each entry in 1-4 rows in the hash table (recommended: `2`)
+- `bucket`: in combination with `hashCount>1`, the size of the hash table can
+be greatly reduced (recommended: `25000`--`100000`, reduced from the fastText
+default of `2000000`) - `minn`: min length of char ngram (default: `3`) -
+`maxn`: max length of char ngram (default: `6`) ```python import floret # train
+vectors model = floret.train_unsupervised( "data.txt", model="cbow",
+mode="floret", hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
 model.get_word_vector("broccoli") # save full model model.save_model
 ("vectors.bin") # export standard word-only vector table model.save_vectors
 ("vectors.vec") # export floret vector table model.save_floret_vectors
 ("vectors.floret") ``` **Note:** with the default setting `mode="fasttext"`,
 `floret` trains original fastText vectors. ## Use floret vectors in spaCy
 Import floret vectors into spaCy v3.2+: ```bash spacy init vectors LANG
 vectors.floret spacy_vectors_model --mode floret ``` ## Notes `floret` contains
```

### Comparing `floret-0.10.3/README.md` & `floret-0.10.4/README.md`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/README.md` & `floret-0.10.4/python/README.md`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/floret_module/floret/__init__.py` & `floret-0.10.4/python/floret_module/floret/__init__.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/floret_module/floret/floret.py` & `floret-0.10.4/python/floret_module/floret/floret.py`

 * *Files 1% similar despite different names*

```diff
@@ -540,15 +540,16 @@
         'model': "supervised"
     })
 
     arg_names = ['input', 'lr', 'dim', 'ws', 'epoch', 'minCount',
                  'minCountLabel', 'minn', 'maxn', 'neg', 'wordNgrams', 'loss', 'bucket',
                  'thread', 'lrUpdateRate', 't', 'label', 'verbose', 'pretrainedVectors',
                  'seed', 'autotuneValidationFile', 'autotuneMetric',
-                 'autotunePredictions', 'autotuneDuration', 'autotuneModelSize']
+                 'autotunePredictions', 'autotuneDuration', 'autotuneModelSize',
+                 'hashCount', 'mode']
     args, manually_set_args = read_args(kargs, kwargs, arg_names,
                                         supervised_default)
     a = _build_args(args, manually_set_args)
     ft = _floret(args=a)
     floret.train(ft.f, a)
     ft.set_args(ft.f.getArgs())
     return ft
```

### Comparing `floret-0.10.3/python/floret_module/floret/pybind/floret_pybind.cc` & `floret-0.10.4/python/floret_module/floret/pybind/floret_pybind.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/floret_module/floret/tests/data.txt` & `floret-0.10.4/python/floret_module/floret/tests/data.txt`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/floret_module/floret/tests/test_configurations.py` & `floret-0.10.4/python/floret_module/floret/tests/test_configurations.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/floret_module/floret/tests/test_script.py` & `floret-0.10.4/python/floret_module/floret/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/floret_module/floret/tests/test_train.py` & `floret-0.10.4/python/floret_module/floret/tests/test_train.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/floret_module/floret/util/util.py` & `floret-0.10.4/python/floret_module/floret/util/util.py`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/python/floret_module/floret.egg-info/PKG-INFO` & `floret-0.10.4/python/floret_module/floret.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 Metadata-Version: 2.1
 Name: floret
-Version: 0.10.3
+Version: 0.10.4
 Summary: floret Python bindings
 Home-page: https://github.com/explosion/floret
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,34 +1,35 @@
-Metadata-Version: 2.1 Name: floret Version: 0.10.3 Summary: floret Python
+Metadata-Version: 2.1 Name: floret Version: 0.10.4 Summary: floret Python
 bindings Home-page: https://github.com/explosion/floret Author: Explosion
 Author-email: contact@explosion.ai License: MIT Classifier: Development Status
 :: 3 - Alpha Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: Science/Research Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9 Classifier: Topic :: Software
-Development Classifier: Topic :: Scientific/Engineering Classifier: Operating
-System :: Microsoft :: Windows Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix Classifier: Operating System :: MacOS
-Description-Content-Type: text/markdown License-File: LICENSE [https://
-explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom embeddings for
-compact, full-coverage vectors with spaCy floret is an extended version of
-[fastText](https://fasttext.cc) that can produce word representations for any
-word from a compact vector table. It combines: - fastText's subwords to provide
-embeddings for any word - Bloom embeddings ("hashing trick") for a compact
-vector table ## Installation ```bash pip install floret ``` ## Usage Train
-floret vectors using the options: - `mode`: `"floret"`, storing both words and
-subwords in the same compact hash table - `hashCount`: store each entry in 1-
-4 rows in the hash table (recommended: `2`) - `bucket`: in combination with
-`hashCount>1`, the size of the hash table can be greatly reduced (recommended:
-`25000`--`100000`, reduced from the fastText default of `2000000`) - `minn`:
-min length of char ngram (default: `3`) - `maxn`: max length of char ngram
-(default: `6`) ```python import floret # train vectors model =
-floret.train_unsupervised( "data.txt", model="cbow", mode="floret",
-hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
+Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
+Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development Classifier: Topic :: Scientific/
+Engineering Classifier: Operating System :: Microsoft :: Windows Classifier:
+Operating System :: POSIX Classifier: Operating System :: Unix Classifier:
+Operating System :: MacOS Description-Content-Type: text/markdown License-File:
+LICENSE [https://explosion.ai/assets/img/logo.svg] # floret: fastText + Bloom
+embeddings for compact, full-coverage vectors with spaCy floret is an extended
+version of [fastText](https://fasttext.cc) that can produce word
+representations for any word from a compact vector table. It combines: -
+fastText's subwords to provide embeddings for any word - Bloom embeddings
+("hashing trick") for a compact vector table ## Installation ```bash pip
+install floret ``` ## Usage Train floret vectors using the options: - `mode`:
+`"floret"`, storing both words and subwords in the same compact hash table -
+`hashCount`: store each entry in 1-4 rows in the hash table (recommended: `2`)
+- `bucket`: in combination with `hashCount>1`, the size of the hash table can
+be greatly reduced (recommended: `25000`--`100000`, reduced from the fastText
+default of `2000000`) - `minn`: min length of char ngram (default: `3`) -
+`maxn`: max length of char ngram (default: `6`) ```python import floret # train
+vectors model = floret.train_unsupervised( "data.txt", model="cbow",
+mode="floret", hashCount=2, bucket=50000, minn=3, maxn=6, ) # query vector
 model.get_word_vector("broccoli") # save full model model.save_model
 ("vectors.bin") # export standard word-only vector table model.save_vectors
 ("vectors.vec") # export floret vector table model.save_floret_vectors
 ("vectors.floret") ``` **Note:** with the default setting `mode="fasttext"`,
 `floret` trains original fastText vectors. ## Use floret vectors in spaCy
 Import floret vectors into spaCy v3.2+: ```bash spacy init vectors LANG
 vectors.floret spacy_vectors_model --mode floret ``` ## Notes `floret` contains
```

### Comparing `floret-0.10.3/python/floret_module/floret.egg-info/SOURCES.txt` & `floret-0.10.4/python/floret_module/floret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/setup.py` & `floret-0.10.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import setuptools
 import os
 import subprocess
 import platform
 import io
 import pybind11
 
-__version__ = '0.10.3'
+__version__ = '0.10.4'
 FASTTEXT_SRC = "src"
 
 # Based on https://github.com/pybind/python_example
 
 class get_pybind_include(object):
     """Helper class to determine the pybind11 include path"""
 
@@ -167,14 +167,16 @@
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Topic :: Software Development',
         'Topic :: Scientific/Engineering',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: POSIX',
         'Operating System :: Unix',
         'Operating System :: MacOS',
     ],
```

### Comparing `floret-0.10.3/src/MurmurHash3.cpp` & `floret-0.10.4/src/MurmurHash3.cpp`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/MurmurHash3.h` & `floret-0.10.4/src/MurmurHash3.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/args.cc` & `floret-0.10.4/src/args.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/args.h` & `floret-0.10.4/src/args.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/autotune.cc` & `floret-0.10.4/src/autotune.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/autotune.h` & `floret-0.10.4/src/autotune.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/densematrix.cc` & `floret-0.10.4/src/densematrix.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/densematrix.h` & `floret-0.10.4/src/densematrix.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/dictionary.cc` & `floret-0.10.4/src/dictionary.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/dictionary.h` & `floret-0.10.4/src/dictionary.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/fasttext.cc` & `floret-0.10.4/src/fasttext.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/fasttext.h` & `floret-0.10.4/src/fasttext.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/loss.cc` & `floret-0.10.4/src/loss.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/loss.h` & `floret-0.10.4/src/loss.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/main.cc` & `floret-0.10.4/src/main.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/matrix.h` & `floret-0.10.4/src/matrix.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/meter.cc` & `floret-0.10.4/src/meter.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/meter.h` & `floret-0.10.4/src/meter.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/model.cc` & `floret-0.10.4/src/model.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/model.h` & `floret-0.10.4/src/model.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/productquantizer.cc` & `floret-0.10.4/src/productquantizer.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/productquantizer.h` & `floret-0.10.4/src/productquantizer.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/quantmatrix.cc` & `floret-0.10.4/src/quantmatrix.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/quantmatrix.h` & `floret-0.10.4/src/quantmatrix.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/utils.cc` & `floret-0.10.4/src/utils.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/utils.h` & `floret-0.10.4/src/utils.h`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/vector.cc` & `floret-0.10.4/src/vector.cc`

 * *Files identical despite different names*

### Comparing `floret-0.10.3/src/vector.h` & `floret-0.10.4/src/vector.h`

 * *Files identical despite different names*

