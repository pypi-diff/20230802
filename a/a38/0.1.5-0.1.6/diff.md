# Comparing `tmp/a38-0.1.5.tar.gz` & `tmp/a38-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a38-0.1.5.tar", last modified: Fri Apr  1 11:34:51 2022, max compression
+gzip compressed data, was "a38-0.1.6.tar", last modified: Wed Aug  2 08:24:57 2023, max compression
```

## Comparing `a38-0.1.5.tar` & `a38-0.1.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.512065 a38-0.1.5/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.468063 a38-0.1.5/.github/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.480064 a38-0.1.5/.github/workflows/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      544 2022-03-21 09:42:15.000000 a38-0.1.5/.github/workflows/py.yml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       82 2022-02-24 09:54:05.000000 a38-0.1.5/.gitignore
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      904 2022-04-01 11:31:32.000000 a38-0.1.5/CHANGELOG.md
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    11357 2019-02-20 11:40:04.000000 a38-0.1.5/LICENSE
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      230 2022-03-21 10:13:07.000000 a38-0.1.5/MANIFEST.in
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1130 2022-03-21 09:42:15.000000 a38-0.1.5/Makefile
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     7246 2022-04-01 11:34:51.512065 a38-0.1.5/PKG-INFO
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6797 2022-03-21 09:42:15.000000 a38-0.1.5/README.md
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.500064 a38-0.1.5/a38/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       31 2022-03-21 09:42:15.000000 a38-0.1.5/a38/__init__.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2657 2022-03-21 09:42:15.000000 a38-0.1.5/a38/builder.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    10102 2022-04-01 11:05:48.000000 a38-0.1.5/a38/codec.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     8148 2022-03-21 09:42:15.000000 a38-0.1.5/a38/consts.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     3941 2022-03-21 09:42:15.000000 a38-0.1.5/a38/crypto.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2301 2022-03-21 09:42:15.000000 a38-0.1.5/a38/diff.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    33455 2022-03-21 09:42:15.000000 a38-0.1.5/a38/fattura.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6387 2022-03-21 09:42:15.000000 a38-0.1.5/a38/fattura_semplificata.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    22505 2022-03-21 09:42:15.000000 a38-0.1.5/a38/fields.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     9962 2022-03-21 09:42:15.000000 a38-0.1.5/a38/models.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2674 2022-03-21 09:42:15.000000 a38-0.1.5/a38/render.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      948 2022-03-21 09:42:15.000000 a38-0.1.5/a38/traversal.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     9678 2022-03-21 09:42:15.000000 a38-0.1.5/a38/trustedlist.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1942 2022-03-21 09:42:15.000000 a38-0.1.5/a38/validation.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.500064 a38-0.1.5/a38.egg-info/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     7246 2022-04-01 11:34:50.000000 a38-0.1.5/a38.egg-info/PKG-INFO
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      844 2022-04-01 11:34:51.000000 a38-0.1.5/a38.egg-info/SOURCES.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        1 2022-04-01 11:34:50.000000 a38-0.1.5/a38.egg-info/dependency_links.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      101 2022-04-01 11:34:50.000000 a38-0.1.5/a38.egg-info/requires.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        4 2022-04-01 11:34:50.000000 a38-0.1.5/a38.egg-info/top_level.txt
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)    12321 2022-04-01 11:05:48.000000 a38-0.1.5/a38tool
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6133 2019-03-07 13:13:01.000000 a38-0.1.5/a38tool.md
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.504064 a38-0.1.5/doc/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       51 2019-02-20 11:40:04.000000 a38-0.1.5/doc/.gitignore
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      822 2022-02-24 09:21:12.000000 a38-0.1.5/doc/README.md
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     3268 2019-02-20 11:40:04.000000 a38-0.1.5/document-a38
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     3035 2022-02-24 09:21:12.000000 a38-0.1.5/download-docs
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1898 2022-04-01 11:13:26.000000 a38-0.1.5/publiccode.yml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       30 2022-03-21 09:42:15.000000 a38-0.1.5/requirements-devops.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       43 2022-03-21 09:42:15.000000 a38-0.1.5/requirements-lib.txt
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)      126 2022-04-01 11:34:51.516065 a38-0.1.5/setup.cfg
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      975 2022-04-01 11:10:57.000000 a38-0.1.5/setup.py
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.504064 a38-0.1.5/stubs/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2019-02-20 11:40:04.000000 a38-0.1.5/stubs/__init__.pyi
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.504064 a38-0.1.5/stubs/dateutil/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2019-02-20 11:40:04.000000 a38-0.1.5/stubs/dateutil/__init__.pyi
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)       67 2019-02-20 11:40:04.000000 a38-0.1.5/stubs/dateutil/parser.pyi
--rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      133 2022-02-24 09:34:08.000000 a38-0.1.5/test-coverage
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.508064 a38-0.1.5/tests/
-drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2022-04-01 11:34:51.512065 a38-0.1.5/tests/data/
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     5675 2019-03-07 13:13:01.000000 a38-0.1.5/tests/data/dati_trasporto.xml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2381 2021-07-30 08:50:51.000000 a38-0.1.5/tests/data/test.txt.p7m
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1646 2022-03-21 09:42:15.000000 a38-0.1.5/tests/data/unicode.xml
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    11966 2022-03-21 09:42:15.000000 a38-0.1.5/tests/test_fattura.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)    27312 2022-03-21 09:42:15.000000 a38-0.1.5/tests/test_fields.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2092 2022-03-21 09:42:15.000000 a38-0.1.5/tests/test_models.py
--rw-r--r--   0 valhalla  (1023) valhalla  (1023)     5186 2022-03-21 09:42:15.000000 a38-0.1.5/tests/test_p7m.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.670337 a38-0.1.6/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.666337 a38-0.1.6/.github/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.666337 a38-0.1.6/.github/workflows/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      614 2023-02-16 09:32:46.000000 a38-0.1.6/.github/workflows/py.yml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       82 2023-02-16 09:32:46.000000 a38-0.1.6/.gitignore
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1333 2023-08-02 08:20:15.000000 a38-0.1.6/CHANGELOG.md
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    11357 2023-02-16 09:32:46.000000 a38-0.1.6/LICENSE
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      258 2023-02-16 10:18:51.000000 a38-0.1.6/MANIFEST.in
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1130 2023-02-16 09:32:46.000000 a38-0.1.6/Makefile
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     7226 2023-08-02 08:24:57.670337 a38-0.1.6/PKG-INFO
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6797 2023-02-16 09:32:46.000000 a38-0.1.6/README.md
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.670337 a38-0.1.6/a38/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       31 2023-02-16 09:32:46.000000 a38-0.1.6/a38/__init__.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2657 2023-02-16 09:32:46.000000 a38-0.1.6/a38/builder.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    10102 2023-02-16 09:32:46.000000 a38-0.1.6/a38/codec.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     8148 2023-02-16 09:32:46.000000 a38-0.1.6/a38/consts.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     3941 2023-02-16 09:32:46.000000 a38-0.1.6/a38/crypto.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2301 2023-02-16 09:32:46.000000 a38-0.1.6/a38/diff.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    33508 2023-02-16 09:32:46.000000 a38-0.1.6/a38/fattura.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6387 2023-02-16 09:32:46.000000 a38-0.1.6/a38/fattura_semplificata.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    23264 2023-08-02 08:12:18.000000 a38-0.1.6/a38/fields.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     9962 2023-08-02 08:12:18.000000 a38-0.1.6/a38/models.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2674 2023-02-16 09:32:46.000000 a38-0.1.6/a38/render.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      948 2023-02-16 09:32:46.000000 a38-0.1.6/a38/traversal.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     9678 2023-02-16 09:32:46.000000 a38-0.1.6/a38/trustedlist.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1942 2023-02-16 09:32:46.000000 a38-0.1.6/a38/validation.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.670337 a38-0.1.6/a38.egg-info/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     7226 2023-08-02 08:24:57.000000 a38-0.1.6/a38.egg-info/PKG-INFO
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      844 2023-08-02 08:24:57.000000 a38-0.1.6/a38.egg-info/SOURCES.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        1 2023-08-02 08:24:57.000000 a38-0.1.6/a38.egg-info/dependency_links.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      101 2023-08-02 08:24:57.000000 a38-0.1.6/a38.egg-info/requires.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        4 2023-08-02 08:24:57.000000 a38-0.1.6/a38.egg-info/top_level.txt
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)    12333 2023-02-16 09:32:46.000000 a38-0.1.6/a38tool
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     6133 2023-02-16 09:32:46.000000 a38-0.1.6/a38tool.md
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.670337 a38-0.1.6/doc/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       51 2023-02-16 09:32:46.000000 a38-0.1.6/doc/.gitignore
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      822 2023-02-16 09:32:46.000000 a38-0.1.6/doc/README.md
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     3268 2023-02-16 09:32:46.000000 a38-0.1.6/document-a38
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)     3035 2023-02-16 09:32:46.000000 a38-0.1.6/download-docs
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1898 2023-08-02 08:18:49.000000 a38-0.1.6/publiccode.yml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       30 2023-02-16 09:32:46.000000 a38-0.1.6/requirements-devops.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       43 2023-02-16 09:32:46.000000 a38-0.1.6/requirements-lib.txt
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)      158 2023-08-02 08:24:57.670337 a38-0.1.6/setup.cfg
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      975 2023-08-02 08:18:27.000000 a38-0.1.6/setup.py
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.670337 a38-0.1.6/stubs/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2023-02-16 09:32:46.000000 a38-0.1.6/stubs/__init__.pyi
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.670337 a38-0.1.6/stubs/dateutil/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)        0 2023-02-16 09:32:46.000000 a38-0.1.6/stubs/dateutil/__init__.pyi
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)       67 2023-02-16 09:32:46.000000 a38-0.1.6/stubs/dateutil/parser.pyi
+-rwxr-xr-x   0 valhalla  (1023) valhalla  (1023)      133 2023-02-16 09:32:46.000000 a38-0.1.6/test-coverage
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.670337 a38-0.1.6/tests/
+drwxr-xr-x   0 valhalla  (1023) valhalla  (1023)        0 2023-08-02 08:24:57.670337 a38-0.1.6/tests/data/
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     5675 2023-02-16 09:32:46.000000 a38-0.1.6/tests/data/dati_trasporto.xml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2381 2023-08-02 08:12:18.000000 a38-0.1.6/tests/data/test.txt.p7m
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     1646 2023-02-16 09:32:46.000000 a38-0.1.6/tests/data/unicode.xml
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    15156 2023-08-02 08:12:18.000000 a38-0.1.6/tests/test_fattura.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)    27360 2023-08-02 08:12:18.000000 a38-0.1.6/tests/test_fields.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     2092 2023-02-16 09:32:46.000000 a38-0.1.6/tests/test_models.py
+-rw-r--r--   0 valhalla  (1023) valhalla  (1023)     5210 2023-08-02 08:12:18.000000 a38-0.1.6/tests/test_p7m.py
```

### Comparing `a38-0.1.5/CHANGELOG.md` & `a38-0.1.6/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+# New in version UNRELEASED
+
+# New in version 0.1.6
+
+* Generate `dati_riepilogo` with properly set `natura` (#27)
+* Ignore non-significant digits when computing differences between Decimal fields
+* a38tool diff: return exit code 0 if there are no differences
+* Change Prezzo Unitario decimals precision to 3 digits, thanks @matteorizzello
+* Fixed a rounding issue (#35), thanks @tschager
+* Updated signature in test certificate
+
 # New in version 0.1.5
 
 * Added to `a38.codec` has a basic implementation of interactive editing in a
   text editor
 
 # New in version 0.1.4
```

### Comparing `a38-0.1.5/LICENSE` & `a38-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/Makefile` & `a38-0.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/PKG-INFO` & `a38-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: a38
-Version: 0.1.5
+Version: 0.1.6
 Summary: parse and generate Italian Fattura Elettronica
 Home-page: https://github.com/Truelite/python-a38/
 Author: Enrico Zini
 Author-email: enrico@truelite.it
 License: https://www.apache.org/licenses/LICENSE-2.0.html
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: cacerts
 Provides-Extra: formatted_python
 Provides-Extra: html
 License-File: LICENSE
 
@@ -209,9 +208,7 @@
 
 
 # Copyright
 
 Copyright 2019-2022 Truelite S.r.l.
 
 This software is released under the Apache License 2.0
-
-
```

### Comparing `a38-0.1.5/README.md` & `a38-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/builder.py` & `a38-0.1.6/a38/builder.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/codec.py` & `a38-0.1.6/a38/codec.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/consts.py` & `a38-0.1.6/a38/consts.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/crypto.py` & `a38-0.1.6/a38/crypto.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/diff.py` & `a38-0.1.6/a38/diff.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/fattura.py` & `a38-0.1.6/a38/fattura.py`

 * *Files 1% similar despite different names*

```diff
@@ -391,15 +391,15 @@
     tipo_cessione_prestazione = fields.StringField(length=2, choices=("SC", "PR", "AB", "AC"), null=True)
     codice_articolo = fields.ModelListField(CodiceArticolo, null=True)
     descrizione = fields.StringField(max_length=1000)
     quantita = fields.DecimalField(max_length=21, decimals=2, null=True)
     unita_misura = fields.StringField(max_length=10, null=True)
     data_inizio_periodo = fields.DateField(null=True)
     data_fine_periodo = fields.DateField(null=True)
-    prezzo_unitario = fields.DecimalField(max_length=21)
+    prezzo_unitario = fields.DecimalField(max_length=21, decimals=3)
     sconto_maggiorazione = fields.ModelListField(ScontoMaggiorazione, null=True)
     prezzo_totale = fields.DecimalField(max_length=21)
     aliquota_iva = fields.DecimalField(xmltag="AliquotaIVA", max_length=6)
     ritenuta = fields.StringField(length=2, choices=("SI",), null=True)
     natura = fields.StringField(min_length=2, max_length=4, null=True, choices=consts.NATURA_IVA)
     riferimento_amministrazione = fields.StringField(max_length=20, null=True)
     altri_dati_gestionali = fields.ModelListField(AltriDatiGestionali, null=True)
@@ -487,24 +487,24 @@
         yourself, or better, extend this function and submit a pull request.
         """
         from collections import defaultdict
 
         # Group by aliquota
         by_aliquota = defaultdict(list)
         for linea in self.dettaglio_linee:
-            by_aliquota[linea.aliquota_iva].append(linea)
+            by_aliquota[(linea.aliquota_iva, linea.natura)].append(linea)
 
         self.dati_riepilogo = []
-        for aliquota, linee in sorted(by_aliquota.items()):
+        for (aliquota, natura), linee in sorted(by_aliquota.items()):
             imponibile = sum(linea.prezzo_totale for linea in linee)
             imposta = imponibile * aliquota / 100
             self.dati_riepilogo.append(
                     DatiRiepilogo(
                         aliquota_iva=aliquota, imponibile_importo=imponibile,
-                        imposta=imposta, esigibilita_iva="I"))
+                        imposta=imposta, esigibilita_iva="I", natura=natura))
 
 
 @export
 class DatiDocumentiCorrelati(models.Model):
     riferimento_numero_linea = fields.ListField(fields.IntegerField(max_length=4), null=True)
     id_documento = fields.StringField(max_length=20)
     data = fields.DateField(null=True)
```

### Comparing `a38-0.1.5/a38/fattura_semplificata.py` & `a38-0.1.6/a38/fattura_semplificata.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/fields.py` & `a38-0.1.6/a38/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,15 +325,15 @@
             return Decimal(value)
         except decimal.InvalidOperation:
             raise TypeError("{} cannot be converted to Decimal".format(repr(value)))
 
     def to_str(self, value):
         if not self.has_value(value):
             return "None"
-        return str(self.clean_value(value).quantize(self.quantize_sample))
+        return str(self.clean_value(value).quantize(self.quantize_sample, rounding=decimal.ROUND_HALF_UP))
 
     def to_jsonable(self, value):
         """
         Return a json-able value for this field
         """
         value = self.clean_value(value)
         if not self.has_value(value):
@@ -348,14 +348,31 @@
             xml_value = self.to_str(value)
             if len(xml_value) > self.max_length:
                 validation.add_error(
                         self,
                         "'{}' should be no more than {} digits long".format(xml_value, self.max_length))
         return value
 
+    def diff(self, res: Diff, first: Optional[T], second: Optional[T]):
+        """
+        Report to res if there are differences between values first and second
+        """
+        first = self.clean_value(first)
+        second = self.clean_value(second)
+        has_first = self.has_value(first)
+        has_second = self.has_value(second)
+        if not has_first and not has_second:
+            return
+        elif has_first and not has_second:
+            res.add_only_first(self, first)
+        elif not has_first and has_second:
+            res.add_only_second(self, second)
+        elif first.quantize(self.quantize_sample) != second.quantize(self.quantize_sample):
+            res.add_different(self, first, second)
+
 
 class StringField(ChoicesField[str]):
     def __init__(self, length=None, min_length=None, max_length=None, **kw):
         super().__init__(**kw)
         if length is not None:
             if min_length is not None or max_length is not None:
                 raise ValueError("length cannot be used with min_length or max_length")
```

### Comparing `a38-0.1.5/a38/models.py` & `a38-0.1.6/a38/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
                 _meta[field_name] = val
                 val.set_name(field_name)
             else:
                 # Leave untouched
                 continue
 
             # Remove field_name from class variables
-            dct.pop(field_name)
+            del dct[field_name]
             # Add it as a slot in the instance
             slots.append(field_name)
 
         dct["__slots__"] = slots
         res = super().__new__(cls, name, bases, dct)
         res._meta = _meta
         return res
```

### Comparing `a38-0.1.5/a38/render.py` & `a38-0.1.6/a38/render.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/traversal.py` & `a38-0.1.6/a38/traversal.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/trustedlist.py` & `a38-0.1.6/a38/trustedlist.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38/validation.py` & `a38-0.1.6/a38/validation.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38.egg-info/PKG-INFO` & `a38-0.1.6/a38.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: a38
-Version: 0.1.5
+Version: 0.1.6
 Summary: parse and generate Italian Fattura Elettronica
 Home-page: https://github.com/Truelite/python-a38/
 Author: Enrico Zini
 Author-email: enrico@truelite.it
 License: https://www.apache.org/licenses/LICENSE-2.0.html
-Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: cacerts
 Provides-Extra: formatted_python
 Provides-Extra: html
 License-File: LICENSE
 
@@ -209,9 +208,7 @@
 
 
 # Copyright
 
 Copyright 2019-2022 Truelite S.r.l.
 
 This software is released under the Apache License 2.0
-
-
```

### Comparing `a38-0.1.5/a38.egg-info/SOURCES.txt` & `a38-0.1.6/a38.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/a38tool` & `a38-0.1.6/a38tool`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
     def run(self):
         first = self.load_fattura(self.first)
         second = self.load_fattura(self.second)
         from a38.diff import Diff
         res = Diff()
         first.diff(res, second)
-        if res:
+        if res.differences:
             for d in res.differences:
                 print(d)
             return 1
 
 
 class Validate(App):
     """
```

### Comparing `a38-0.1.5/a38tool.md` & `a38-0.1.6/a38tool.md`

 * *Files 0% similar despite different names*

```diff
@@ -171,15 +171,15 @@
             progressivo_invio='00001',
 …
 ```
 
 
 ### Render to HTML or PDF
 
-You can use a .xslt file to render e fattura to HTML or PDF.
+You can use a .xslt file to render a fattura to HTML or PDF.
 
 ```text
 $ a38tool html --help
 usage: a38tool html [-h] [-f] [-o OUTPUT] stylesheet files [files ...]
 
 positional arguments:
   stylesheet            .xsl/.xslt stylesheet file to use for rendering
```

### Comparing `a38-0.1.5/doc/README.md` & `a38-0.1.6/doc/README.md`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/document-a38` & `a38-0.1.6/document-a38`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/download-docs` & `a38-0.1.6/download-docs`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/publiccode.yml` & `a38-0.1.6/publiccode.yml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This repository adheres to the publiccode.yml standard by including this
 # metadata file that makes public software easily discoverable.
 # More info at https://github.com/italia/publiccode.yml
 
 publiccodeYmlVersion: '0.2'
 name: A38
 url: 'https://github.com/Truelite/python-a38.git'
-softwareVersion: 0.1.5
+softwareVersion: 0.1.6
 releaseDate: '2022-04-01'
 inputTypes:
   - text/xml
 outputTypes:
   - text/html
   - text/xml
   - text/x-python
```

### Comparing `a38-0.1.5/setup.py` & `a38-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 def parse_requirements(filename):
     line_iter = (line.strip() for line in open(filename))
     return [line for line in line_iter if line and not line.startswith("#")]
 
 
 setup(
     name="a38",
-    version="0.1.5",
+    version="0.1.6",
     description="parse and generate Italian Fattura Elettronica",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Enrico Zini",
     author_email="enrico@truelite.it",
     url="https://github.com/Truelite/python-a38/",
     license="https://www.apache.org/licenses/LICENSE-2.0.html",
```

### Comparing `a38-0.1.5/tests/data/dati_trasporto.xml` & `a38-0.1.6/tests/data/dati_trasporto.xml`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/tests/data/unicode.xml` & `a38-0.1.6/tests/data/unicode.xml`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/tests/test_fattura.py` & `a38-0.1.6/tests/test_fattura.py`

 * *Files 19% similar despite different names*

```diff
@@ -90,78 +90,153 @@
         dt.codice_destinatario = None
         self.assert_validates(dt)
 
 
 class TestDatiBeniServizi(TestFatturaMixin, TestCase):
     def test_add_dettaglio_linee(self):
         o = a38.DatiBeniServizi()
-        o.add_dettaglio_linee(descrizione="Line 1", quantita=2, unita_misura="m²", prezzo_unitario=7, aliquota_iva=22)
-        o.add_dettaglio_linee(descrizione="Line 2", quantita=1, unita_misura="A", prezzo_unitario="0.4", aliquota_iva=22)
+        o.add_dettaglio_linee(
+                descrizione="Line 1", quantita=2, unita_misura="m²", prezzo_unitario=7, aliquota_iva=22)
+        o.add_dettaglio_linee(
+                descrizione="Line 2", quantita=1, unita_misura="A", prezzo_unitario="0.4", aliquota_iva=22)
         self.assertEqual(len(o.dettaglio_linee), 2)
         self.assertEqual(o.dettaglio_linee[0], a38.DettaglioLinee(
             numero_linea=1, descrizione="Line 1", quantita=2, unita_misura="m²",
             prezzo_unitario=7, prezzo_totale=14, aliquota_iva=22))
         self.assertEqual(o.dettaglio_linee[1], a38.DettaglioLinee(
             numero_linea=2, descrizione="Line 2", quantita=1, unita_misura="A",
             prezzo_unitario="0.4", prezzo_totale="0.4", aliquota_iva=22))
 
     def test_add_dettaglio_linee_without_quantita(self):
         o = a38.DatiBeniServizi()
         o.add_dettaglio_linee(descrizione="Line 1", prezzo_unitario=7, aliquota_iva=22)
         self.assertEqual(len(o.dettaglio_linee), 1)
-        self.assertEqual(o.dettaglio_linee[0], a38.DettaglioLinee(1, descrizione="Line 1", prezzo_unitario=7, prezzo_totale=7, aliquota_iva=22))
+        self.assertEqual(
+                o.dettaglio_linee[0],
+                a38.DettaglioLinee(1, descrizione="Line 1", prezzo_unitario=7, prezzo_totale=7, aliquota_iva=22))
 
     def test_build_dati_riepilogo(self):
         o = a38.DatiBeniServizi()
         o.add_dettaglio_linee(descrizione="Line 1", quantita=2, unita_misura="m²", prezzo_unitario=7, aliquota_iva=22)
-        o.add_dettaglio_linee(descrizione="Line 2", quantita=1, unita_misura="A", prezzo_unitario="0.4", aliquota_iva=22)
-        o.add_dettaglio_linee(descrizione="Line 3", quantita="3.5", unita_misura="A", prezzo_unitario="0.5", aliquota_iva=10)
+        o.add_dettaglio_linee(
+                descrizione="Line 2", quantita=1, unita_misura="A", prezzo_unitario="0.4", aliquota_iva=22)
+        o.add_dettaglio_linee(
+                descrizione="Line 3", quantita="3.5", unita_misura="A", prezzo_unitario="0.5", aliquota_iva=10)
         o.build_dati_riepilogo()
 
         self.assertEqual(len(o.dati_riepilogo), 2)
-        self.assertEqual(o.dati_riepilogo[0], a38.DatiRiepilogo(aliquota_iva="10", imponibile_importo="1.75", imposta="0.175", esigibilita_iva="I"))
-        self.assertEqual(o.dati_riepilogo[1], a38.DatiRiepilogo(aliquota_iva="22", imponibile_importo="14.40", imposta="3.168", esigibilita_iva="I"))
+        self.assertEqual(
+                o.dati_riepilogo[0],
+                a38.DatiRiepilogo(aliquota_iva="10", imponibile_importo="1.75", imposta="0.175", esigibilita_iva="I"))
+        self.assertEqual(
+                o.dati_riepilogo[1],
+                a38.DatiRiepilogo(aliquota_iva="22", imponibile_importo="14.40", imposta="3.168", esigibilita_iva="I"))
+
+    def test_build_dati_riepilogo_natura(self):
+        self.maxDiff = None
+
+        common_args = {"descrizione": "Line", "quantita": 1, "unita_misura": "N"}
+
+        o = a38.DatiBeniServizi()
+        o.add_dettaglio_linee(prezzo_unitario=7, aliquota_iva=22, natura="N1", **common_args)
+        o.add_dettaglio_linee(prezzo_unitario="1", aliquota_iva=22, natura="N1", **common_args)
+        o.add_dettaglio_linee(prezzo_unitario="3.5", aliquota_iva=10, natura="N6", **common_args)
+        o.add_dettaglio_linee(prezzo_unitario="3.5", aliquota_iva=0, natura="N2.1", **common_args)
+        o.add_dettaglio_linee(prezzo_unitario="7.5", aliquota_iva=0, natura="N2.1", **common_args)
+        o.add_dettaglio_linee(prezzo_unitario="5", aliquota_iva=0, natura="N3.1", **common_args)
+        o.build_dati_riepilogo()
+
+        self.assertEqual(len(o.dati_riepilogo), 4)
+        self.assertEqual(
+                o.dati_riepilogo[0],
+                a38.DatiRiepilogo(
+                    aliquota_iva="0", imponibile_importo="11", imposta="0", esigibilita_iva="I", natura="N2.1"))
+        self.assertEqual(
+                o.dati_riepilogo[1],
+                a38.DatiRiepilogo(
+                    aliquota_iva="0", imponibile_importo="5", imposta="0", esigibilita_iva="I", natura="N3.1"))
+        self.assertEqual(
+                o.dati_riepilogo[2],
+                a38.DatiRiepilogo(
+                    aliquota_iva="10", imponibile_importo="3.5", imposta="0.35", esigibilita_iva="I", natura="N6"))
+        self.assertEqual(
+                o.dati_riepilogo[3],
+                a38.DatiRiepilogo(
+                    aliquota_iva="22", imponibile_importo="8", imposta="1.76", esigibilita_iva="I", natura="N1"))
+
+    def test_build_dati_riepilogo_natura_issue33(self):
+        self.maxDiff = None
+
+        o = a38.DatiBeniServizi()
+        o.add_dettaglio_linee(
+                descrizione="Bollo", quantita=1, unita_misura="EUR",
+                prezzo_unitario="2", aliquota_iva="0.00", natura="N1")
+        o.build_dati_riepilogo()
+
+        self.assertEqual(o.dati_riepilogo[0].natura, "N1")
+
+        from a38.validation import Validation
+        res = Validation()
+        o.validate(res)
+        self.assertEqual(res.warnings, [])
+        self.assertEqual(res.errors, [])
 
 
 class TestFatturaElettronicaBody(TestFatturaMixin, TestCase):
     def test_build_importo_totale_documento(self):
         o = a38.FatturaElettronicaBody()
-        o.dati_beni_servizi.add_dettaglio_linee(descrizione="Line 1", quantita=2, unita_misura="m²", prezzo_unitario=7, aliquota_iva=22)
-        o.dati_beni_servizi.add_dettaglio_linee(descrizione="Line 2", quantita=1, unita_misura="A", prezzo_unitario="0.4", aliquota_iva=22)
-        o.dati_beni_servizi.add_dettaglio_linee(descrizione="Line 3", quantita="3.5", unita_misura="A", prezzo_unitario="0.5", aliquota_iva=10)
+        o.dati_beni_servizi.add_dettaglio_linee(
+                descrizione="Line 1", quantita=2, unita_misura="m²", prezzo_unitario=7, aliquota_iva=22)
+        o.dati_beni_servizi.add_dettaglio_linee(
+                descrizione="Line 2", quantita=1, unita_misura="A", prezzo_unitario="0.4", aliquota_iva=22)
+        o.dati_beni_servizi.add_dettaglio_linee(
+                descrizione="Line 3", quantita="3.5", unita_misura="A", prezzo_unitario="0.5", aliquota_iva=10)
         o.dati_beni_servizi.build_dati_riepilogo()
         o.build_importo_totale_documento()
 
         self.assertEqual(o.dati_generali.dati_generali_documento.importo_totale_documento, Decimal("19.493"))
 
+    def test_rounding_xml(self):
+        f = a38.FatturaPrivati12()
+        o = f.fattura_elettronica_body[0]
+        o.dati_beni_servizi.add_dettaglio_linee(
+            descrizione="Line 1", prezzo_unitario="0.35", aliquota_iva=10, unita_misura='pz', quantita=1)
+        o.dati_beni_servizi.build_dati_riepilogo()
+        o.build_importo_totale_documento()
+
+        self.assertEqual(f.fattura_elettronica_body[0].dati_generali.dati_generali_documento.importo_totale_documento, Decimal("0.385"))
+        self.assertEqual(f.build_etree().getroot().find('.//ImportoTotaleDocumento').text, "0.39")
+
 
 class TestFatturaPrivati12(TestFatturaMixin, TestCase):
     def build_sample(self):
         cedente_prestatore = a38.CedentePrestatore(
             a38.DatiAnagraficiCedentePrestatore(
                 a38.IdFiscaleIVA("IT", "01234567890"),
                 codice_fiscale="NTNBLN22C23A123U",
                 anagrafica=a38.Anagrafica(denominazione="Test User"),
                 regime_fiscale="RF01",
             ),
-            a38.Sede(indirizzo="via Monferrato", numero_civico="1", cap="50100", comune="Firenze", provincia="FI", nazione="IT"),
+            a38.Sede(indirizzo="via Monferrato", numero_civico="1",
+                     cap="50100", comune="Firenze", provincia="FI", nazione="IT"),
             iscrizione_rea=a38.IscrizioneREA(
                 ufficio="FI",
                 numero_rea="123456",
                 stato_liquidazione="LN",
             ),
             contatti=a38.Contatti(email="local_part@pec_domain.it"),
         )
 
         cessionario_committente = a38.CessionarioCommittente(
             a38.DatiAnagraficiCessionarioCommittente(
                 a38.IdFiscaleIVA("IT", "76543210987"),
                 anagrafica=a38.Anagrafica(denominazione="A Company SRL"),
             ),
-            a38.Sede(indirizzo="via Langhe", numero_civico="1", cap="50142", comune="Firenze", provincia="FI", nazione="IT"),
+            a38.Sede(indirizzo="via Langhe", numero_civico="1", cap="50142",
+                     comune="Firenze", provincia="FI", nazione="IT"),
         )
 
         f = a38.FatturaPrivati12()
         f.fattura_elettronica_header.dati_trasmissione.update(
             a38.IdTrasmittente("IT", "10293847561"),
             codice_destinatario="FUFUFUF",
         )
@@ -206,29 +281,33 @@
         f = self.build_sample()
         self.assertEqual(f.fattura_elettronica_header.dati_trasmissione.formato_trasmissione, "FPR12")
         tree = f.build_etree()
         with io.StringIO() as out:
             tree.write(out, encoding="unicode")
             xml = out.getvalue()
 
-        self.assertIn('<ns0:FatturaElettronica xmlns:ns0="http://ivaservizi.agenziaentrate.gov.it/docs/xsd/fatture/v1.2" versione="FPR12">', xml)
+        self.assertIn(
+            '<ns0:FatturaElettronica xmlns:ns0="http://ivaservizi.agenziaentrate.gov.it/docs/xsd/fatture/v1.2"'
+            ' versione="FPR12">', xml)
         self.assertIn('<FormatoTrasmissione>FPR12</FormatoTrasmissione>', xml)
 
     def test_serialize_lxml(self):
         from a38 import builder
         if not builder.HAVE_LXML:
             raise SkipTest("lxml is not available")
 
         f = self.build_sample()
         tree = f.build_etree(lxml=True)
         with io.BytesIO() as out:
             tree.write(out)
             xml = out.getvalue()
 
-        self.assertIn(b'<ns0:FatturaElettronica xmlns:ns0="http://ivaservizi.agenziaentrate.gov.it/docs/xsd/fatture/v1.2" versione="FPR12">', xml)
+        self.assertIn(
+            b'<ns0:FatturaElettronica xmlns:ns0="http://ivaservizi.agenziaentrate.gov.it/docs/xsd/fatture/v1.2"'
+            b' versione="FPR12">', xml)
         self.assertIn(b'<FormatoTrasmissione>FPR12</FormatoTrasmissione>', xml)
 
     def test_to_python(self):
         f = self.build_sample()
         py = f.to_python(namespace="a38")
         parsed = eval(py)
         self.assertEqual(f, parsed)
```

### Comparing `a38-0.1.5/tests/test_fields.py` & `a38-0.1.6/tests/test_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -350,19 +350,20 @@
         f = self.get_field()
         self.assert_to_python_works(f, "1.2")
         self.assert_to_python_works(f, Decimal("1.20"))
 
     def test_diff(self):
         f = self.get_field()
         self.assert_diff_empty(f, Decimal("1.0"), "1.0")
-        self.assert_field_diff(f, "1.0001", "1.0002")
+        self.assert_diff_empty(f, "1.0001", "1.0002")
+        self.assert_field_diff(f, "1.1", "1.2")
 
     def test_xml(self):
         f = self.get_field(null=True)
-        self.assertEqual(self.to_xml(f, "12.345"), "<T><Sample>12.34</Sample></T>")
+        self.assertEqual(self.to_xml(f, "12.345"), "<T><Sample>12.35</Sample></T>")
         self.assertEqual(self.to_xml(f, "34.567"), "<T><Sample>34.57</Sample></T>")
 
 
 class TestDateField(FieldTestMixin, TestCase):
     field_class = fields.DateField
 
     def test_value(self):
```

### Comparing `a38-0.1.5/tests/test_models.py` & `a38-0.1.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `a38-0.1.5/tests/test_p7m.py` & `a38-0.1.6/tests/test_p7m.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,9 +107,10 @@
                 p7m.verify_signature(capath)
 
     def test_verify_noca(self):
         p7m = P7M("tests/data/test.txt.p7m")
         if p7m.is_expired():
             self.skipTest("test signature has expired and needs to be regenerated")
         with tempfile.TemporaryDirectory() as capath:
-            with self.assertRaisesRegexp(InvalidSignatureError, r"Verify error:unable to get local issuer certificate"):
+            with self.assertRaisesRegexp(
+                    InvalidSignatureError, r"Verify error:\s*unable to get local issuer certificate"):
                 p7m.verify_signature(capath)
```

